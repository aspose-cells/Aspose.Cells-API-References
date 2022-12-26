---
title: ReConnectionMethodType enumeration
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 130
url: /python-net/aspose.cells.externalconnections/reconnectionmethodtype/
is_root: false
---

## ReConnectionMethodType enumeration

Specifies what the spreadsheet application should do when a connection fails.



The ReConnectionMethodType type exposes the following members:

### Fields
| Field | Description |
| :- | :- |
| REQUIRED | On refresh use the existing connection information and if it ends up being invalid <br/>then get updated connection information, if available from the external connection file. |
| ALWAYS | On every refresh get updated connection information from the external connection file, <br/>if available, and use that instead of the existing connection information. <br/>In this case the data refresh will fail if the external connection file is unavailable. |
| NEVER | Never get updated connection information from the external connection file <br/>even if it is available and even if the existing connection information is invalid |


### See Also

* module [aspose.cells.externalconnections](../)
