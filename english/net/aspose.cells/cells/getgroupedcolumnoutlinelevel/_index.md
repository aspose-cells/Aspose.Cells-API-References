---
title: Cells.GetGroupedColumnOutlineLevel
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Gets the outline level zerobased of the column
type: docs
url: /net/aspose.cells/cells/getgroupedcolumnoutlinelevel/
---
## Cells.GetGroupedColumnOutlineLevel method

Gets the outline level (zero-based) of the column.

```csharp
public int GetGroupedColumnOutlineLevel(int columnIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | The column index |

### Return Value

The outline level of the column

### Remarks

If the column is not grouped, returns zero.

### Examples

```csharp
// Called: int m = mWorksheet.Cells.GetGroupedColumnOutlineLevel(0);
public void Cells_Method_GetGroupedColumnOutlineLevel()
{
    Workbook workbook = new Workbook();
    Worksheet mWorksheet = workbook.Worksheets["Sheet1"];

mWorksheet.Cells[0, 0].Formula = "='C:\\book1.xls'!SomeNamedRange";
mWorksheet.Cells[1, 0].Formula = "='[C:\\book1.xls]'!SomeNamedRange";
int m = mWorksheet.Cells.GetGroupedColumnOutlineLevel(0);
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


