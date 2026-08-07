---
categories: ["API"]
tags: ["api", "routemap", "magiclink"]
title: "Magic Link"
linkTitle: "Magic Link"
date: 2026-08-07
type: docs
weight: 20
description: >
  Generate and retrieve a public Magic Link for a Route Map
---

The API endpoint generates and returns a public Magic Link associated with a Route Map.

```http
GET /ffw/startracking/routemap/{AWB}/magiclink?day=10 HTTP/1.1
Host: api.startracking.aero
Accept: application/json
Authorization: Bearer {{BEARER TOKEN}}
```

## Parameters

| Parameter | Type | Required | Description |
|------------|------|----------|-------------|
| AWB | string | Yes | Air Waybill number composed of exactly 11 digits. |
| day | integer | No | Number of days the Magic Link remains valid. Values greater than 10 are automatically set to 10. Values below 0 are used to disable any previosly generated link. |

## Response

```json
{
  "Guid": "8d7c44c6-18b6-4b35-8b98-8b4f679418fb",
  "WebSiteUrl": "https://routemap.example.com/12345678901/8d7c44c6-18b6-4b35-8b98-8b4f679418fb"
}
```

## Returned Properties

| Property | Description |
|------------|-------------|
| Guid | Unique identifier generated for the Link. |
| WebSiteUrl | Ready to use public URL. |

## Behaviour

The endpoint:

1. Verifies that the Magic Link feature is enabled.
2. Validates the AWB format.
3. Generates or retrieves the Magic Link.
4. Populates the `WebSiteUrl` property.
5. Returns the `MagicLink` object.

## Responses

| HTTP Code | Description |
|------------|-------------|
| 200 | Magic Link successfully generated or retrieved. |
| 400 | Invalid request parameters. |
| 500 | Internal server error. |

> **Note**
>
> When no Route Map is found for the specified AWB, the API returns an empty JSON object (`{}`).
