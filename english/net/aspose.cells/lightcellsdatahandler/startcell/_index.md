---
title: LightCellsDataHandler.StartCell
second_title: Aspose.Cells for .NET API Reference
description: LightCellsDataHandler method. Prepares to process a cell
type: docs
url: /net/aspose.cells/lightcellsdatahandler/startcell/
---
## LightCellsDataHandler.StartCell method

Prepares to process a cell.

```csharp
public bool StartCell(int columnIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | column index of the cell to be processed |

### Return Value

whether this cell needs to be processed. false to ignore the cell and check the next one until reach the end of cells data of current row

### Remarks

It will be called when reaching an existing cell in current row. Current row is the row of last call of [`ProcessRow`](../processrow/).

### See Also

* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


