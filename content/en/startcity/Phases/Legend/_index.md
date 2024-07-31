
---
title: "Legend"
linkTitle: "Legend"
type: docs
weight: 40
---

**LEGEND OF CODES AND FIELDS SPECIFICATION**:

> The English meaning of Bordero is **DELIVERY NOTE**

| Code | Mandatory | Name                      | Notes                                                        |
| :--: | :-------: | :------------------------ | :----------------------------------------------------------- |
|  C  |     N     |  Airport Customs Agent     | The Agent Code will do custom declaration inside the Airport  |
|  CI  |     N     | Customer ID               | Numeric Customer Identification Code (for internal purposes) |
|  S   |     Y     | Bordero is SECURED         | 0 corresponds to FALSE and 1 to TRUE[^1]                       |
| BDX  |     N     | Bordero ID              | Customer Identification for Bordero		              |
|  H   |     C 	   | Handler                   | SmartCity Handler (es. MLE. ALH). Mandatory for Phase 2. For Phase 1, if not indicated, Ecosystem Cargo MXP assigns it automatically |
|  AG  |     Y     | Agent Code                |                                                              |
|  DN  |     N     | Driver Name               |                                                              |
|  DT  |     N     | Document Type             |                                                              |
|  DA  |     N     | Document Issuer Authority |                                                              |
|  DI  |     N     | Document Number           |                                                              |
|  PN  |     N     | PLATE #                   | Can be Repeated                                              |
|  SN  |     N     | SEAL #                    | Can be Repeated                                              |
|  CN  |     Y     | DRIVER COMPANY NAME       | Name of the company for which the driver works.              |
|  TN  |     N     | TRUCK COMPANY NAME        | Name of the company to which the truck belongs.              |
| DN2  |     N     | DRIVER NAME               | 2nd DRIVER                                                   |
| DT2  |     N     | DOCUMENT TYPE             | 2nd DRIVER                                                   |
| DA2  |     N     | DOCUMENT AUTHORITY        | 2nd DRIVER                                                   |
| DI2  |     N     | DOCUMENT NUMBER           | 2nd DRIVER                                                   |
| CN2  |     N     | COMPANY NAME              | 2nd DRIVER    
| DTI  |    N	   | Code of subject delegated to Transport Information | 	
| DSI  | N			| Code of subject delegated to Security Information| 
| DCD  |    N			| Code of subject delegated to Custom Declaration| 

[^1]: if Bordero is secured, Regulated Agent must be indicated| 
