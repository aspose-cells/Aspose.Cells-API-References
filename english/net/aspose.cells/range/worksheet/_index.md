---
title: Range.Worksheet
second_title: Aspose.Cells for .NET API Reference
description: Range property. Gets the Worksheetobject which contains this range
type: docs
url: /net/aspose.cells/range/worksheet/
---
## Range.Worksheet property

Gets the `Worksheet`object which contains this range.

```csharp
public Worksheet Worksheet { get; }
```

### Examples

```csharp
// Called: range.Worksheet.Cells.DeleteRange(range.FirstRow, range.FirstColumn, range.FirstRow + range.RowCount - 1, range.FirstColumn + range.ColumnCount - 1, ShiftType.Up);
public void Range_Property_Worksheet()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    Shape shape = workbook.Worksheets[0].Shapes["Image 44"];
    int e = shape.LowerRightRow;
    Aspose.Cells.Range range = workbook.Worksheets.GetRangeByName("GRAPHE_RULER");
    range.Worksheet.Cells.DeleteRange(range.FirstRow, range.FirstColumn, range.FirstRow + range.RowCount - 1, range.FirstColumn + range.ColumnCount - 1, ShiftType.Up);
    Assert.AreEqual(shape.LowerRightRow, e);
}
```

### See Also

* class [Worksheet](../../worksheet/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


