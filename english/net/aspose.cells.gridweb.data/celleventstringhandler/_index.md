---
title: Delegate CellEventStringHandler
second_title: Aspose.Cells for .NET API Reference
description: Represents the method that intend to handle cell events. same as CellEventHandler interfacebut return string result
type: docs
url: /net/aspose.cells.gridweb.data/celleventstringhandler/
---
## CellEventStringHandler delegate

Represents the method that intend to handle cell events. same as CellEventHandler interface,but return string result

String **handleCellEvent**(Object sender, CellEventArgs e);

```csharp
public delegate string CellEventStringHandler(object sender, CellEventArgs e);
```

| Parameter | Type | Description |
| --- | --- | --- |
| sender | Object | The source grid of the event. |
| e | CellEventArgs | The event argument. The e.Cell is the cell who fires the event. The e.Argument contains the argument of the event. |

### Return Value

string value

### See Also

* class [CellEventArgs](../../aspose.cells.gridweb/celleventargs/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


