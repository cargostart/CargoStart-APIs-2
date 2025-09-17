---
categories: ["API"]
tags: ["api", "routemap"] 
title: "Triggering"
linkTitle: "Triggering"
date: 2025-09-17
type: docs
weight: 30
description: >
  Triggering a Route Map
---
## Routemap
StarTracking always strives to provide a Route Map as quickly as possible.  
However, in some cases, manually triggering a Route Map is required or highly recommended.

### Triggering a CiQ shipment
You can trigger a CiQ shipment only if:
- You are the legal owner of the Shipment Air Waybill (AWB) number.
- The Carrier’s AWB number is in the CargoStart CiQ participating carriers list.

The request body requires the **full AWB number** and the **full IATA Agent Code**:

```http
POST /ffw/startracking/routemap/sendsme HTTP/1.1
Host: api.startracking.aero
Authorization: Bearer {{BEARER TOKEN}}
Content-Type: application/json
Content-Length: 109

{
  "AirlinePrefix": "999",
  "AwbNumber": "12345675",
  "AgentCode": "3847361",
  "AgentCass": "0011"
}
```

In almost realtime, the AWB is sent to the Carrier, and a Route Map is returned.


{{% alert title="Recommendation" color="warning" %}}
To ensure you receive an updated Cargo iQ Route Map as soon as an operator finalizes a booking and enters the information in their TMS application, it is recommended to call the **/sendsme** endpoint.
{{% /alert %}}

### Triggering a XTD shipment
You can trigger an XTD shipment request only if:
- The Carrier's AWB # is in the CargoStart XTD participating carriers list.

he request is similar to CiQ, but requires the IsXTD flag:

```http
POST /ffw/startracking/routemap/sendsme HTTP/1.1
Host: api.startracking.aero
Authorization: Bearer {{BEARER TOKEN}}
Content-Type: application/json
Content-Length: 109

{
  "AirlinePrefix": "000",
  "AwbNumber": "12345675",
  "AgentCode": "3847361",
  "AgentCass": "0011",
  "IsXTD": true
}
```

{{% alert title="Note" color="warning" %}}
- It is advisable to receive updates of an XTD Routemap only if you **are not the owner** of the Shipment Air Waybill #, e.g. you want to have visibility of an import routemap
- Additional costs 
{{% /alert %}}

{{% alert title="Important" color="danger" %}}
Triggering XTD Route Maps may incur additional charges depending on your service plan.
Make sure to verify your commercial agreement before enabling XTD requests.
{{% /alert %}}