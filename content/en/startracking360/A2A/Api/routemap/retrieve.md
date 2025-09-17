---
categories: ["API"]
tags: ["api", "routemap"] 
title: "Retrieve"
linkTitle: "Retrieve"
date: 2022-07-19
type: docs
weight: 20
description: >
  Retrieve a single Routemap
---
Once you know which AWB # you want to retrieve you can do that merely adding the awb# to the route map endpoint,

## Request

```http
GET /ffw/startracking/routemap/17607818425 HTTP/1.1
Authorization: Bearer {{BEARER TOKEN}}
Content-Type: application/json
Host: api.startracking.aero
```
##  Response


```json
{
  "MilestonePlan": {
    "OriginCycle": {
      "Milestone": [
        {
          "Status": "Ko",
          "ArchivedStatus": "Ko",
          "Name": "FWB",
          "Station": "SWK",
          "PlannedDateTime": {
            "Utc": "2025-02-25T12:00:00Z",
            "Local": "2025-02-25T13:00:00"
          },
          "ActualDateTime": {
            "Utc": "2025-02-25T13:10:26Z",
            "Local": "2025-02-25T14:10:26"
          },
          "IsReplanned": false,
          "ActualNoOfPieces": 12
        },
        {
          "Status": "Missing",
          "ArchivedStatus": "Missing",
          "Name": "LAT",
          "Station": "SWK",
          "PlannedDateTime": {
            "Utc": "2025-02-25T12:05:00Z",
            "Local": "2025-02-25T13:05:00"
          },
          "ActualDateTime": null,
          "IsReplanned": false,
          "ActualNoOfPieces": 0
        },
        {
          "Status": "Ko",
          "ArchivedStatus": "Ko",
          "Name": "RCS",
          "Station": "SWK",
          "PlannedDateTime": {
            "Utc": "2025-02-25T16:05:00Z",
            "Local": "2025-02-25T17:05:00"
          },
          "ActualDateTime": {
            "Utc": "2025-02-25T18:24:41Z",
            "Local": "2025-02-25T19:24:41"
          },
          "IsReplanned": false,
          "ActualNoOfPieces": 12
        }
      ],
      "Status": "Partial",
      "isReplanned": false
    },
    "RoutingCycle": {
      "Flight": [
        {
          "FlightInfo": {
            "CarrierCode": "EK",
            "Number": "9806T",
            "Date": "25FEB",
            "Scheduled": {
              "DepartureDateTime": {
                "Utc": "2025-02-25T18:05:00Z",
                "Local": "2025-02-25T19:05:00"
              },
              "ArrivalDateTime": {
                "Utc": "2025-02-26T07:00:00Z",
                "Local": "2025-02-26T08:00:00"
              }
            },
            "Actual": null,
            "Routing": {
              "Origin": "SWK",
              "Destination": "BLQ"
            },
            "isRoadFeederService": true
          },
          "Total": {
            "NoOfPieces": 12,
            "WeightCode": "K",
            "Weight": 2480,
            "VolumeCode": "CM",
            "Volume": 6.74
          },
          "PlannedTotal": null,
          "Milestone": [
            {
              "Status": "Missing",
              "ArchivedStatus": "Missing",
              "Name": "DEP",
              "Station": "SWK",
              "PlannedDateTime": {
                "Utc": "2025-02-25T19:05:00Z",
                "Local": "2025-02-25T20:05:00"
              },
              "ActualDateTime": null,
              "IsReplanned": false,
              "ActualNoOfPieces": 0
            },
            {
              "Status": "Missing",
              "ArchivedStatus": "Missing",
              "Name": "ARR",
              "Station": "BLQ",
              "PlannedDateTime": {
                "Utc": "2025-02-26T07:40:00Z",
                "Local": "2025-02-26T08:40:00"
              },
              "ActualDateTime": null,
              "IsReplanned": false,
              "ActualNoOfPieces": 0
            },
            {
              "Status": "Ko",
              "ArchivedStatus": "Ko",
              "Name": "RCF",
              "Station": "BLQ",
              "PlannedDateTime": {
                "Utc": "2025-02-26T07:45:00Z",
                "Local": "2025-02-26T08:45:00"
              },
              "ActualDateTime": {
                "Utc": "2025-02-26T10:55:51Z",
                "Local": "2025-02-26T11:55:51"
              },
              "IsReplanned": false,
              "ActualNoOfPieces": 12
            }
          ]
        },
        {
          "FlightInfo": {
            "CarrierCode": "EK",
            "Number": "94",
            "Date": "26FEB",
            "Scheduled": {
              "DepartureDateTime": {
                "Utc": "2025-02-26T13:30:00Z",
                "Local": "2025-02-26T14:30:00"
              },
              "ArrivalDateTime": {
                "Utc": "2025-02-26T19:20:00Z",
                "Local": "2025-02-26T23:20:00"
              }
            },
            "Actual": {
              "DepartureDateTime": {
                "Utc": "2025-02-26T13:19:00Z",
                "Local": "2025-02-26T14:19:00"
              },
              "ArrivalDateTime": {
                "Utc": "2025-02-26T19:01:00Z",
                "Local": "2025-02-26T23:01:00"
              }
            },
            "Routing": {
              "Origin": "BLQ",
              "Destination": "DXB"
            },
            "isRoadFeederService": false
          },
          "Total": {
            "NoOfPieces": 12,
            "WeightCode": "K",
            "Weight": 2480,
            "VolumeCode": "CM",
            "Volume": 6.74
          },
          "PlannedTotal": null,
          "Milestone": [
            {
              "Status": "Ok",
              "ArchivedStatus": "Ok",
              "Name": "DEP",
              "Station": "BLQ",
              "PlannedDateTime": {
                "Utc": "2025-02-26T14:30:00Z",
                "Local": "2025-02-26T15:30:00"
              },
              "ActualDateTime": {
                "Utc": "2025-02-26T13:19:00Z",
                "Local": "2025-02-26T14:19:00"
              },
              "IsReplanned": false,
              "ActualNoOfPieces": 12
            },
            {
              "Status": "Ok",
              "ArchivedStatus": "Ok",
              "Name": "ARR",
              "Station": "DXB",
              "PlannedDateTime": {
                "Utc": "2025-02-26T20:20:00Z",
                "Local": "2025-02-27T00:20:00"
              },
              "ActualDateTime": {
                "Utc": "2025-02-26T19:01:00Z",
                "Local": "2025-02-26T23:01:00"
              },
              "IsReplanned": false,
              "ActualNoOfPieces": 12
            },
            {
              "Status": "Ok",
              "ArchivedStatus": "Ok",
              "Name": "RCF",
              "Station": "DXB",
              "PlannedDateTime": {
                "Utc": "2025-02-27T00:20:00Z",
                "Local": "2025-02-27T04:20:00"
              },
              "ActualDateTime": {
                "Utc": "2025-02-26T23:22:06Z",
                "Local": "2025-02-27T03:22:06"
              },
              "IsReplanned": false,
              "ActualNoOfPieces": 12
            }
          ]
        }
      ],
      "Status": "Partial",
      "isReplanned": false
    },
    "DestinationCycle": {
      "Milestone": [
        {
          "Status": "Ok",
          "ArchivedStatus": "Ok",
          "Name": "NFD",
          "Station": "DXB",
          "PlannedDateTime": {
            "Utc": "2025-02-27T01:20:00Z",
            "Local": "2025-02-27T05:20:00"
          },
          "ActualDateTime": {
            "Utc": "2025-02-26T22:04:12Z",
            "Local": "2025-02-27T02:04:12"
          },
          "IsReplanned": false,
          "ActualNoOfPieces": 12
        },
        {
          "Status": "Ko",
          "ArchivedStatus": "Ko",
          "Name": "AWD",
          "Station": "DXB",
          "PlannedDateTime": {
            "Utc": "2025-02-27T03:20:00Z",
            "Local": "2025-02-27T07:20:00"
          },
          "ActualDateTime": {
            "Utc": "2025-02-27T07:02:52Z",
            "Local": "2025-02-27T11:02:52"
          },
          "IsReplanned": false,
          "ActualNoOfPieces": 12
        },
        {
          "Status": "Ok",
          "ArchivedStatus": "Ok",
          "Name": "DLV",
          "Station": "DXB",
          "PlannedDateTime": {
            "Utc": "2025-03-01T19:20:00Z",
            "Local": "2025-03-01T23:20:00"
          },
          "ActualDateTime": {
            "Utc": "2025-02-27T08:01:31Z",
            "Local": "2025-02-27T12:01:31"
          },
          "IsReplanned": false,
          "ActualNoOfPieces": 12
        }
      ],
      "Status": "Completed",
      "isReplanned": false
    }
  },
  "LastUpdate": "2025-02-27T15:25:25Z",
  "Shipment": {
    "AirlinePrefix": "176",
    "AwbNumber": "07818425",
    "Routing": {
      "Origin": "SWK",
      "Destination": "DXB"
    },
    "Total": {
      "NoOfPieces": 12,
      "WeightCode": "K",
      "Weight": 2480,
      "VolumeCode": "CM",
      "Volume": 6.74
    }
  },
  "DeliveryDate": {
    "Utc": "2025-02-26T22:04:12Z",
    "Local": "2025-02-27T02:04:12"
  },
  "ReceiptDate": {
    "Utc": "2025-02-25T18:24:41Z",
    "Local": "2025-02-25T19:24:41"
  },
  "ProductCode": "GCR",
  "IsRoadFeederService": false,
  "Status": "AtDestination",
  "IsReplanned": false,
  "RoutingIsReplanned": false,
  "OriginState": 0,
  "RoutingState": 0,
  "DestinationState": 0,
  "Origin": null,
  "Routing": null,
  "Destination": null,
  "CreationDate": {
    "Utc": "2025-02-26T19:27:10Z",
    "Local": "2025-02-26T20:27:10"
  }
}
```
### Anatomy of the Response

You can see many parts are similar to the Routemap Search response; we will concentrate only to the new properties.

The Routemap milestone is separated into three different cycles:
* [OriginCycle](#origincycle) 
* [RoutingCycle](#routingcycle) 
* [DestinationCycle](#destinationcycle) 

Every Cycle has a collection of specific Milestones:

#### OriginCycle
Here you can find all the origin milestones, every with its information on the Status, the Station of Origin, the Planned and the Actual time 
*	FWB 
*	LAT
*	RCS


#### RoutingCycle
Essentially a collection of all the flight numbers, from origin to destination; for every flight there are the following milestones:
*	DEP
* ARR
* RCF

#### DestinationCycle
* NFD
* DLV

Any Cycle has the Status property that can be:

*	Planned
*	Partial
*	Completed

Milestone Status property can be
*	Missing, Scheduled Time occurred, but no Milestone message received
*	Ko, Milestone message sent late
*	Ok, Milestone message arrived in time 

They summarize all the milestones inside the specific Cycle.

## Routemap with its History

In case you need all the life cycle of a Routemap, you can add the "/history" word to the call: 

GET  /ffw/startracking/routemap/{AWB}/history

This call returns the selected route map and all its snapshots. 

> Keep in mind that the history data are available only for 30 days from the route map creation. 
