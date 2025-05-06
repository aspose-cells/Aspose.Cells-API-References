---
title: Cells.GetViewRowHeight
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Gets the height of a specified row
type: docs
url: /net/aspose.cells/cells/getviewrowheight/
---
## Cells.GetViewRowHeight method

Gets the height of a specified row.

```csharp
public double GetViewRowHeight(int row)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index. |

### Return Value

Height of row.

### Examples

```csharp
// Called: Assert.AreEqual(12.75, workbook.Worksheets[0].Cells.GetViewRowHeight(3));
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet47454.xls&quot;);
            Assert.AreEqual(13.15, workbook.Worksheets[0].Cells.GetRowHeight(3));
            Assert.AreEqual(12.75, workbook.Worksheets[0].Cells.GetViewRowHeight(3));
           // Assert.AreEqual(12.75, workbook.Worksheets[0].Cells.GetRowHeight(3,WidthViewMode.View, CellsUnitType.Point));
            workbook.Save(Constants.destPath + &quot;CellsNet47454.xlsx&quot;);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


