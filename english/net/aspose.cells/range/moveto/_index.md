---
title: Range.MoveTo
second_title: Aspose.Cells for .NET API Reference
description: Range method. Move the current range to the dest range
type: docs
url: /net/aspose.cells/range/moveto/
---
## Range.MoveTo method

Move the current range to the dest range.

```csharp
public void MoveTo(int destRow, int destColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| destRow | Int32 | The start row of the dest range. |
| destColumn | Int32 | The start column of the dest range. |

### Examples

```csharp
// Called: range.MoveTo(range.FirstRow - 1, range.FirstColumn);
public void Range_Method_MoveTo()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");

    Aspose.Cells.Range range = workbook.Worksheets.GetRangeByName("range");
    range.MoveTo(range.FirstRow - 1, range.FirstColumn);
    Assert.AreEqual(workbook.Worksheets[0].ConditionalFormattings[0].GetCellArea(0).StartRow, 5);
    Assert.AreEqual(workbook.Worksheets[0].ConditionalFormattings[1].GetCellArea(0).StartRow, 6);
    workbook.Save(Constants.destPath + "dest.xlsx");
}
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


