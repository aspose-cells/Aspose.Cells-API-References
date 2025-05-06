---
title: HtmlSaveOptions.WidthScalable
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates whether exporting column width in unit of scale to html. The default value is false
type: docs
url: /net/aspose.cells/htmlsaveoptions/widthscalable/
---
## HtmlSaveOptions.WidthScalable property

Indicates whether exporting column width in unit of scale to html. The default value is false.

```csharp
public bool WidthScalable { get; set; }
```

### Examples

```csharp
// Called: options.WidthScalable = false;
[Test]
        public void Property_WidthScalable()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;JAVA42890/&quot;;

            Workbook wb = new Workbook(filePath + &quot;4415697226273472958xls.xls&quot;);

            string savePath = CreateFolder(filePath);

            //ImageOrPrintOptions imgOptions = new ImageOrPrintOptions();            
            //wb.Worksheets[0].Shapes[0].ToImage(savePath + &quot;image000.png&quot;, imgOptions);
            //wb.Worksheets[0].Shapes[1].ToImage(savePath + &quot;image001.png&quot;, imgOptions);

            //Specify Html Save Options
            HtmlSaveOptions options = new HtmlSaveOptions();
            //We do not want to export document, workbook and worksheet properties
            options.ExportDocumentProperties = false;
            options.ExportWorkbookProperties = false;
            options.ExportWorksheetProperties = false;
            options.ExportSimilarBorderStyle = true;
            options.ExportImagesAsBase64 = false;
            options.ExcludeUnusedStyles = true;
            options.ExportHiddenWorksheet = false;
            options.WidthScalable = false;
            options.PresentationPreference = true;

            //Specify HtmlSaveOptions - Hide Overlaid Content with CrossHideRight while saving to Html
            options.HtmlCrossStringType = HtmlCrossType.CrossHideRight;
            //Export the Excel file to Html with Html Save Options


            wb.Save(savePath + &quot;out.html&quot;, options);
            wb.Save(savePath + &quot;out.pdf&quot;);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


