---
title: HtmlSaveOptions.ExportWorkbookProperties
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicating whether exporting workbook properties.The default value is true.If you want to import the html or mht file to excel please keep the default value
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportworkbookproperties/
---
## HtmlSaveOptions.ExportWorkbookProperties property

Indicating whether exporting workbook properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value.

```csharp
public bool ExportWorkbookProperties { get; set; }
```

### Examples

```csharp
// Called: options.ExportWorkbookProperties = false;
[Test]
        public void Property_ExportWorkbookProperties()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @"JAVA43162/";

            Workbook workbook = new Workbook(filePath + "878914550142091892.xls");
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportDocumentProperties = false;
            options.ExportWorkbookProperties = false;
            options.ExportWorkbookProperties = false;
            options.ExportSimilarBorderStyle = true;
            options.ExportImagesAsBase64 = false;
            options.ExcludeUnusedStyles = true;
            options.ExportHiddenWorksheet = false;
            options.WidthScalable = false;
            options.PresentationPreference = true;
            options.HtmlCrossStringType = HtmlCrossType.CrossHideRight;


            workbook.Save(CreateFolder(filePath) + "out.html");
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


