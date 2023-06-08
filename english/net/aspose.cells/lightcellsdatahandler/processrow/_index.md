---
title: LightCellsDataHandler.ProcessRow
second_title: Aspose.Cells for .NET API Reference
description: LightCellsDataHandler method. Starts to process one row
type: docs
url: /net/aspose.cells/lightcellsdatahandler/processrow/
---
## LightCellsDataHandler.ProcessRow method

Starts to process one row.

```csharp
public bool ProcessRow(Row row)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Row | Row object which is being processed currently. |

### Return Value

whether this row's cells need to be processed. false to ignore all cells in this row.

### Remarks

It will be called after row's properties such as height, style, ...etc. have been read. However, cells in this row has not been read yet.

### See Also

* class [Row](../../row/)
* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


