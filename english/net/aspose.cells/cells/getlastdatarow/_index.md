---
title: Cells.GetLastDataRow
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Gets the last row index of cell which contains data in the specified column
type: docs
url: /net/aspose.cells/cells/getlastdatarow/
---
## Cells.GetLastDataRow method

Gets the last row index of cell which contains data in the specified column.

```csharp
public int GetLastDataRow(int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | Column index. |

### Return Value

last row index.

### Examples

```csharp
// Called: cellarea.EndRow = workbook.Worksheets["Volumes"].Cells.GetLastDataRow(0);
public void Cells_Method_GetLastDataRow()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    CellArea cellarea = new CellArea();
    cellarea.StartColumn = 0;
    cellarea.StartRow = 9;
    cellarea.EndColumn = 6;
    cellarea.EndRow = workbook.Worksheets["Volumes"].Cells.GetLastDataRow(0);
    workbook.Worksheets["Volumes"].Cells.InsertRange(cellarea, 1, ShiftType.Down, true);
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


