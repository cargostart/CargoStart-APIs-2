
---
title: "Legend"
linkTitle: "Legend"
type: docs
weight: 40
---

**LEGEND OF CODES AND FIELDS SPECIFICATION**:

{{% alert title="Note" color="warning" %}}
 The English meaning of Bordero is **DELIVERY NOTE**
{{% /alert %}}



| Code | Mandatory | Name                      | Notes                                                        |
| :--: | :-------: | :------------------------ | :----------------------------------------------------------- |
|  C  |     N     |  Airport Customs Agent     | The Agent Code will do custom declaration inside the Airport  |
|  CI  |     N     | Customer ID               | Numeric Customer Identification Code (for internal purposes) |
|  S   |     Y     | Bordero is SECURED         | 0 corresponds to FALSE and 1 to TRUE[^1]                       |
| BDX  |     N     | Bordero ID              | Customer Identification for Bordero		              |
|  H   |     C 	   | Handler                   | SmartCity Handler (es. MLE. ALH). Mandatory for Phase 2. For Phase 1, if not indicated, Ecosystem Cargo MXP assigns it automatically |
|  AG  |     Y     | Agent Code                |                                                              |
|  DN  |     C     | Driver Name               |[^2]                                                              |
|  DT  |     C     | Document Type             |[^2]                                                              |
|  DA  |     C     | Document Issuer Authority |[^2]                                                              |
|  DI  |     C     | Document Number           |[^2]                                                              |
|  PN  |     C     | PLATE #                   | Can be Repeated [^2]                                              |
|  SN  |     C     | SEAL #                    | Can be Repeated [^2]                                             |
|  CN  |     C     | DRIVER COMPANY NAME       | Name of the company for which the driver works. [^2]              |
|  TN  |     C     | TRUCK COMPANY NAME        | Name of the company to which the truck belongs. [^2]             |
| DN2  |     C     | DRIVER NAME               | 2nd DRIVER [^2]                                                  |
| DT2  |     C     | DOCUMENT TYPE             | 2nd DRIVER [^2]                                                  |
| DA2  |     C     | DOCUMENT AUTHORITY        | 2nd DRIVER [^2]                                                  |
| DI2  |     C     | DOCUMENT NUMBER           | 2nd DRIVER [^2]                                                  |
| CN2  |     C     | COMPANY NAME              | 2nd DRIVER [^2]   
| DTI  |    N	   | Code of subject delegated to Transport Information | 	
| DSI  | N			| Code of subject delegated to Security Information| 
| DCD  |    N			| Code of subject delegated to Custom Declaration| 

[^1]: if Bordero is secured, Regulated Agent must be indicated| 
[^2]: Under the latest SEA SmartCityMXP rules, these fields are optional. If you choose to provide one, you must also provide all the others.