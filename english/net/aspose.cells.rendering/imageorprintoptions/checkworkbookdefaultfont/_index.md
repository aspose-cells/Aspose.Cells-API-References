---
title: ImageOrPrintOptions.CheckWorkbookDefaultFont
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. When characters in the Excel are Unicode and not be set with correct font in cell style They may appear as block in pdfimage. Set this to true to try to use workbooks default font to show these characters first
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/checkworkbookdefaultfont/
---
## ImageOrPrintOptions.CheckWorkbookDefaultFont property

When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first.

```csharp
public bool CheckWorkbookDefaultFont { get; set; }
```

### Remarks

Default is true.

### Examples

```csharp
// Called: options.CheckWorkbookDefaultFont = true;
[Test]
        public void Property_CheckWorkbookDefaultFont()
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


