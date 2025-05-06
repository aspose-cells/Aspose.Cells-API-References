---
title: SheetRender.SheetRender
second_title: Aspose.Cells for .NET API Reference
description: SheetRender constructor. the construct of SheetRender need worksheet and ImageOrPrintOptions as params
type: docs
url: /net/aspose.cells.rendering/sheetrender/sheetrender/
---
## SheetRender constructor

the construct of SheetRender, need worksheet and ImageOrPrintOptions as params

```csharp
public SheetRender(Worksheet worksheet, ImageOrPrintOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| worksheet | Worksheet | Indicate which spreadsheet to be rendered. |
| options | ImageOrPrintOptions | ImageOrPrintOptions contains some property of output image |

### Examples

```csharp
// Called: SheetRender sr = new SheetRender(worksheet, options);
[Test]
        public void SheetRender_Constructor()
        {
            string path = Constants.TemplatePath + &quot;NetCoreTests/CELLSNETCORE20/&quot;;
            string path2 = Constants.destPath + &quot;NetCoreTests/&quot;;
            string excelPath = path + &quot;chart-of-anothersheet.xlsx&quot;;
            using (var ms = new FileStream(excelPath, FileMode.OpenOrCreate, FileAccess.Read))
            {
                using (var workbook = new Workbook(ms))
                {
                    Worksheet worksheet = workbook.Worksheets[0];
                    worksheet.PageSetup.PrintArea = &quot;A1: W62&quot;;// &quot;A1: N50&quot;;

                    // Set all margins as 0
                    worksheet.PageSetup.LeftMargin = 0;
                    worksheet.PageSetup.RightMargin = 0;
                    worksheet.PageSetup.TopMargin = 0;
                    worksheet.PageSetup.BottomMargin = 0;

                    // Set OnePagePerSheet option as true
                    ImageOrPrintOptions options = new ImageOrPrintOptions();
                    options.OnePagePerSheet = true;
                    options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
                    options.OnlyArea = true;
                    options.HorizontalResolution = 90;
                    options.VerticalResolution = 90;
                    SheetRender sr = new SheetRender(worksheet, options);
                    sr.ToImage(0, path2 + Guid.NewGuid() + &quot;.png&quot;);
                }
            }

            excelPath = path + &quot;NPS Monthly Report 2018-Sept.xlsx&quot;;//&quot;chart-of-anothersheet.xlsx&quot;;
            using (var ms = new FileStream(excelPath, FileMode.OpenOrCreate, FileAccess.Read))
            {
                using (var workbook = new Workbook(ms))
                {
                    Worksheet worksheet = workbook.Worksheets[0];
                    worksheet.PageSetup.PrintArea = &quot;A1: W62&quot;;// &quot;A1: N50&quot;;

                    // Set all margins as 0
                    worksheet.PageSetup.LeftMargin = 0;
                    worksheet.PageSetup.RightMargin = 0;
                    worksheet.PageSetup.TopMargin = 0;
                    worksheet.PageSetup.BottomMargin = 0;

                    // Set OnePagePerSheet option as true
                    ImageOrPrintOptions options = new ImageOrPrintOptions();
                    options.OnePagePerSheet = true;
                    options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
                    options.OnlyArea = true;
                    options.HorizontalResolution = 90;
                    options.VerticalResolution = 90;
                    SheetRender sr = new SheetRender(worksheet, options);
                    sr.ToImage(0, path2 + Guid.NewGuid() + &quot;.png&quot;);
                }
            }
        }
```

### See Also

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


