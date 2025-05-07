---
title: SheetRender.GetPageSizeInch
second_title: Aspose.Cells for .NET API Reference
description: SheetRender method. Get page size in inch of output image
type: docs
url: /net/aspose.cells.rendering/sheetrender/getpagesizeinch/
---
## SheetRender.GetPageSizeInch method

Get page size in inch of output image.

```csharp
public float[] GetPageSizeInch(int pageIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | The page index is based on zero. |

### Return Value

Page size of image, [0] for width and [1] for height

### Examples

```csharp
// Called: float[] pageSize = sr.GetPageSizeInch(0);
[Test]
        public void Method_Int32_()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            sheet.Cells["A1"].PutValue("Test page size");
            sheet.PageSetup.PaperSize = PaperSizeType.PaperLetter;

            ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();

            SheetRender sr = new SheetRender(sheet, imgOpt);
            float[] pageSize = sr.GetPageSizeInch(0);
            Assert.AreEqual(8.5, pageSize[0]);
            Assert.AreEqual(11, pageSize[1]);

            WorkbookRender wr = new WorkbookRender(wb, imgOpt);
            pageSize = wr.GetPageSizeInch(0);
            Assert.AreEqual(8.5, pageSize[0]);
            Assert.AreEqual(11, pageSize[1]);
        }
```

### See Also

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


