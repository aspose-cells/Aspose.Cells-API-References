---
title: Delegate CellErrorHandler
second_title: Aspose.Cells for .NET API Reference
description: Represents the interface that intend to handle cell error events
type: docs
url: /net/aspose.cells.gridweb.data/cellerrorhandler/
---
## CellErrorHandler delegate

Represents the interface that intend to handle cell error events.

void **handleCellEvent**(Object sender, GridCellException ex, OnErrorActionQuery query);

```csharp
public delegate void CellErrorHandler(object sender, WebCellException ex, 
    OnErrorActionQuery action);
```

| Parameter | Type | Description |
| --- | --- | --- |
| sender | Object | The source of the event. |
| ex | WebCellException | The cell operation error. |
| action | OnErrorActionQuery | can get onerror action type information. |

### See Also

* class [WebCellException](../webcellexception/)
* class [OnErrorActionQuery](../onerroractionquery/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


