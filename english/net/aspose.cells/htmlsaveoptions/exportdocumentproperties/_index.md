---
title: HtmlSaveOptions.ExportDocumentProperties
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicating whether exporting document properties.The default value is true.If you want to import the html or mht file to excel please keep the default value
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportdocumentproperties/
---
## HtmlSaveOptions.ExportDocumentProperties property

Indicating whether exporting document properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value.

```csharp
public bool ExportDocumentProperties { get; set; }
```

### Examples

```csharp
// Called: options.ExportDocumentProperties = false;
[Test]
        public void Property_ExportDocumentProperties()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @"JAVA42899/";

            String fontFolder = filePath + "font";
            FontConfigs.SetFontFolder(fontFolder, true);

            //Load the sample Excel file
            Workbook workbook = new Workbook(filePath + "test.xlsx");
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

            workbook.Save(CreateFolder(filePath) + "out.html", options);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


