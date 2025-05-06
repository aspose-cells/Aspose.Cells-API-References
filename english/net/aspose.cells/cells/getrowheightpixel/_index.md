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
// Called: Assert.AreEqual(247, wb.Worksheets[0].Cells.GetRowHeightPixel(0));
[Test]
        public void Method_Int32_()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSNET-53267.xlsx&quot;);
            AutoFitterOptions autoFitterOptions = new AutoFitterOptions();
            autoFitterOptions.ForRendering= true;
            wb.Worksheets[0].AutoFitRows(autoFitterOptions);

            Assert.AreEqual(247, wb.Worksheets[0].Cells.GetRowHeightPixel(0));
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


