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
// Called: range.MoveTo(range.FirstRow + 10, range.FirstColumn);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet45544.xlsx");
            Aspose.Cells.Range range = workbook.Worksheets.GetRangeByName("range");
            range.MoveTo(range.FirstRow + 10, range.FirstColumn);
            workbook.Save(Constants.destPath + "CellsNet45544.xlsx");
        }
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


