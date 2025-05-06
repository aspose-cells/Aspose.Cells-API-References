---
title: ImageOrPrintOptions.TextRenderingHint
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. Specifies the quality of text rendering. The default value is TextRenderingHint.SystemDefault
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/textrenderinghint/
---
## ImageOrPrintOptions.TextRenderingHint property

Specifies the quality of text rendering. The default value is TextRenderingHint.SystemDefault

```csharp
public TextRenderingHint TextRenderingHint { get; set; }
```

### Examples

```csharp
// Called: options.TextRenderingHint = System.Drawing.Text.TextRenderingHint.AntiAliasGridFit;
[Test]
        public void Property_TextRenderingHint()
        {
            Workbook wb = new Workbook(Constants.TemplatePath + &quot;CELLSNET-51476.xlsx&quot;);
            int activeIndex = wb.Worksheets.ActiveSheetIndex;

            CalculationOptions opts = new CalculationOptions();
            opts.Recursive = true;
            opts.IgnoreError = false;
            wb.CalculateFormula(opts);
            Worksheet sheet = wb.Worksheets[activeIndex];
            sheet.CalculateFormula(opts, true);
            sheet.Shapes.UpdateSelectedValue();

            sheet.PageSetup.PrintArea = &quot;A1:C1&quot;;
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
                Assert.IsTrue(img.GetPixel(1076, 32).B &gt; 100);
            }
        }
```

### See Also

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


