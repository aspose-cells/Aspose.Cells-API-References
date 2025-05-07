---
title: Cells.GetRowHeightPixel
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Gets the height of a specified row in unit of pixel
type: docs
url: /net/aspose.cells/cells/getrowheightpixel/
---
## Cells.GetRowHeightPixel method

Gets the height of a specified row in unit of pixel.

```csharp
public int GetRowHeightPixel(int row)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index |

### Return Value

Height of row

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[0].Cells.GetRowHeightPixel(0),34);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet21133.xls");
            workbook.Worksheets[0].AutoFitRows();
            Assert.AreEqual(workbook.Worksheets[0].Cells.GetRowHeightPixel(0),34);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


