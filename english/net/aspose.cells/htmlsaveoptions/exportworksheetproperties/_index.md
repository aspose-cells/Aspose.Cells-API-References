---
title: HtmlSaveOptions.ExportWorksheetProperties
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicating whether exporting worksheet properties.The default value is true.If you want to import the html or mht file to excel please keep the default value
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportworksheetproperties/
---
## HtmlSaveOptions.ExportWorksheetProperties property

Indicating whether exporting worksheet properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value.

```csharp
public bool ExportWorksheetProperties { get; set; }
```

### Examples

```csharp
// Called: options.ExportWorksheetProperties = false;
[Test]
        public void Property_ExportWorksheetProperties()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @"JAVA43377/";
            string savePath = CreateFolder(filePath);

            Workbook workbook = new Workbook(filePath + "11月5S检查通报(1).xlsx");
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportDocumentProperties = false;
            options.ExportWorkbookProperties = false;
            options.ExportWorksheetProperties = false;
            options.ExportSimilarBorderStyle = true;
            options.ExportImagesAsBase64 = false;
            options.ExcludeUnusedStyles = true;
            options.ExportHiddenWorksheet = false;
            options.WidthScalable = false;
            options.PresentationPreference = true;
            options.HtmlCrossStringType = HtmlCrossType.CrossHideRight;
            workbook.Save(savePath + "11月5S检查通报(1)_20.12.html", options);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


