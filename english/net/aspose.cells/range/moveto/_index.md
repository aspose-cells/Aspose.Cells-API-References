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
// Called: blockRange.MoveTo(7, CellsHelper.ColumnNameToIndex(&amp;quot;H&amp;quot;)); //moving to H8
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;ConditionalFormattings/CellsNet45197.xlsx&quot;);
            Aspose.Cells.Range blockRange = workbook.Worksheets.GetRangeByName(&quot;range&quot;);
            blockRange.MoveTo(7, CellsHelper.ColumnNameToIndex(&quot;H&quot;)); //moving to H8 
            Assert.AreEqual(1, workbook.Worksheets[0].ConditionalFormattings.Count);
            Assert.AreEqual(7, workbook.Worksheets[0].ConditionalFormattings[0].GetCellArea(0).StartRow);
            workbook.Save(Constants.destPath + &quot;CellsNet45197.xlsx&quot;);
        }
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


