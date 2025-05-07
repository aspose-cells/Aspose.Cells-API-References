---
title: ImageOrPrintOptions.PageCount
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. Gets or sets the number of pages to save
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/pagecount/
---
## ImageOrPrintOptions.PageCount property

Gets or sets the number of pages to save.

```csharp
public int PageCount { get; set; }
```

### Remarks

Default is System.Int32.MaxValue which means all pages will be rendered.

### Examples

```csharp
// Called: options.PageCount = 1;
[Test]
        public void Property_PageCount()
        {
            Workbook wb = new Workbook(Constants.TemplatePath + "CELLSNET-51476.xlsx");
            int activeIndex = wb.Worksheets.ActiveSheetIndex;

            CalculationOptions opts = new CalculationOptions();
            opts.Recursive = true;
            opts.IgnoreError = false;
            wb.CalculateFormula(opts);
            Worksheet sheet = wb.Worksheets[activeIndex];
            sheet.CalculateFormula(opts, true);
            sheet.Shapes.UpdateSelectedValue();

            sheet.PageSetup.PrintArea = "A1:C1";
            sheet.PageSetup.LeftMargin = 0;
            sheet.PageSetup.RightMargin = 0;
            sheet.PageSetup.TopMargin = 0;
            sheet.PageSetup.BottomMargin = 0;

            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.PageCount = 1;
            options.Transparent = true;
            options.CheckWorkbookDefaultFont = true;
            options.HorizontalResolution = 200;
            options.VerticalResolution = 200;
            options.TextRenderingHint = System.Drawing.Text.TextRenderingHint.AntiAliasGridFit;
            options.SmoothingMode = System.Drawing.Drawing2D.SmoothingMode.HighQuality;
            SheetRender sr = new SheetRender(sheet, options);
            MemoryStream ms = new MemoryStream();
            sr.ToImage(0, ms);
            using (Bitmap img = (Bitmap)Image.FromStream(ms))
            {
                Assert.IsTrue(img.GetPixel(1076, 32).B > 100);
            }
        }
```

### See Also

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


