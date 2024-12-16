---
title: GetRefreshOnChange Method 
linktitle: GetRefreshOnChange
second_title: Aspose.Cells for Go via C++ API Reference
description: 'GetRefreshOnChange method. Encapsulates the function that represents getrefreshonchange in Go.'
type: docs
weight: 200
url: /go-cpp/connectionparameter/getrefreshonchange/
---

## GetRefreshOnChange function

Flag indicating whether the query should automatically refresh when the contents of acell that provides the parameter value changes. If true, then external data is refreshedusing the new parameter value every time there's a change. If false, then external datais only refreshed when requested by the user, or some other event triggers refresh (e.g., workbook opened).

```go

func (instance *ConnectionParameter) GetRefreshOnChange()  (bool,  error) 

```

## Remarks


## See Also

* Class [ConnectionParameter](../)
* Namespace [Aspose.Cells.ExternalConnections](../../)
* Library [Aspose.Cells for Go](../../../)
