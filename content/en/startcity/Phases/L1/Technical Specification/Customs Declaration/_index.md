
---
title: "Customs Declaration"
linkTitle: "Customs Declaration"
type: docs
weight: 10
---

```
OCI/IT/EXP/M/15ITQ1V1T0240456E9
//COR//X
```
**15ITQ1V1T0240456E9** is the _MRN_; **X** is the customs status (eg. X, T1, T2, TBD).

> Note: in case the customs status is **TBD** (To Be Declared), the _Custom operator_ will carry out the customs operation at the airport;

Customs Declaration data must be reported indicating the SmartCity Code of Custom operator with the following syntax:

```
OCI/IT/COR//TBD
///ST/..C..XYZ..C..
```

In the case where the airport customs operator is not registered in Smart City Ecosystem, the name of the operator must be inserted with the following syntax:

```
OCI//IT/COR//TBD
///ST/..C..MARIO ROSSI..C..
```

> **Delegation**

Sending Custom Declaration data can be delegated at a third ecosystem user with the following syntax:

```
OCI///ST/..DCD..YYY..DCD..
```
**YYY** is the SmartCity code of delegated user.
