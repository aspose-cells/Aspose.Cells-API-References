---
title: ImageOrPrintOptions.IsOptimized
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. Indicates whether to optimize the output elements
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/isoptimized/
---
## ImageOrPrintOptions.IsOptimized property

Indicates whether to optimize the output elements.

```csharp
public bool IsOptimized { get; set; }
```

### Remarks

Default value is false. Currently when this property is set to true, the following optimizations will be done: 1. optimize the border lines. 2. optimize the file size while rendering to Svg image.

### Examples

```csharp
// Called: options.IsOptimized = true;
[Test]
        public void Property_IsOptimized()
        {
            Workbook wb = new Workbook(Constants.TemplatePath + "CELLSNET-49049.xlsx");
            var sheet = wb.Worksheets["Rendering"];
            var range = sheet.Workbook.Worksheets.GetRangeByName("ImageRange");

            var pgSetup = sheet.PageSetup;
            pgSetup.PrintArea = range.Address;
            pgSetup.LeftMargin = 0.04;
            pgSetup.TopMargin = 0.04;
            pgSetup.RightMargin = 0.04;
            pgSetup.BottomMargin = 0.04;
            var options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Emf;
            options.OnlyArea = true;
            options.OnePagePerSheet = true;
            options.IsOptimized = true;
            options.EmfType = System.Drawing.Imaging.EmfType.EmfOnly;
            SheetRender sr = new SheetRender(sheet, options);

            MemoryStream ms = new MemoryStream();
            sr.ToImage(0, ms);
            ms.Position = 0xcc;

            byte[] buffer = new byte[4];
            ms.Read(buffer, 0, buffer.Length);

            int val = BitConverter.ToInt32(buffer, 0);

            Assert.IsTrue(val > 1);
        }
```

### See Also

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


