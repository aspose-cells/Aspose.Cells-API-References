---
title: SetRefreshOnChange Method 
linktitle: SetRefreshOnChange
second_title: Aspose.Cells for Go API Reference
description: 'SetRefreshOnChange method. Encapsulates the function that represents setrefreshonchange in Go.'
type: docs
weight: 200
url: /go-cpp/connectionparameter/setrefreshonchange/
---

## SetRefreshOnChange function

Flag indicating whether the query should automatically refresh when the contents of acell that provides the parameter value changes. If true, then external data is refreshedusing the new parameter value every time there's a change. If false, then external datais only refreshed when requested by the user, or some other event triggers refresh (e.g., workbook opened).

```go

func (instance *ConnectionParameter) SetRefreshOnChange(value bool)  error

```

## Remarks


## See Also

* Class [ConnectionParameter](../)
* Namespace [Aspose.Cells.ExternalConnections](../../)
* Library [Aspose.Cells for Go](../../../)
