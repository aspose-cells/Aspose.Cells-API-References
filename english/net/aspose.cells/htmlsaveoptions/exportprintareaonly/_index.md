---
title: HtmlSaveOptions.ExportPrintAreaOnly
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates if only exporting the print area to html file. The default value is false
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportprintareaonly/
---
## HtmlSaveOptions.ExportPrintAreaOnly property

Indicates if only exporting the print area to html file. The default value is false.

```csharp
public bool ExportPrintAreaOnly { get; set; }
```

### Examples

```csharp
// Called: ExportPrintAreaOnly = false, //was true
[Test]
        public void Property_ExportPrintAreaOnly()
        {
            string path = PathNetCore + &quot;CELLSNETCORE121/&quot;;
            Workbook workbook = new Workbook(path + &quot;EACDef_BAK.xlsx&quot;);

            
            int count1 = 0;
            foreach (Shape sp in workbook.Worksheets[0].Shapes)
            {
                sp.ToImage(String.Format(destPathNetCore + &quot;CELLSNETCORE121_{0}.png&quot;, count1), new ImageOrPrintOptions());
                count1++;
            }
            
            workbook.Save(destPathNetCore + &quot;CELLSNETCORE121.pdf&quot;);
            
            
            var htmlSaveOptions = new HtmlSaveOptions
            {
                Encoding = Encoding.UTF8,
                ExportImagesAsBase64 = true,
                ExportPrintAreaOnly = false, //was true
                ExportActiveWorksheetOnly = true,
                ExportWorksheetCSSSeparately = false,
                ExcludeUnusedStyles = true,
                ExportDocumentProperties = false,
                ExportWorkbookProperties = false,
                HtmlCrossStringType = HtmlCrossType.Default,
                ExportSimilarBorderStyle = true,

                // Set the property for scalable width
                WidthScalable = true,

            };

            htmlSaveOptions.ImageOptions.ImageType = ImageType.Svg;
            htmlSaveOptions.ImageOptions.HorizontalResolution = 150;
            htmlSaveOptions.ImageOptions.VerticalResolution = 150;

            workbook.Save(destPathNetCore + &quot;CELLSNETCORE121.htm&quot;, htmlSaveOptions);
            
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


