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
public void HtmlSaveOptions_Property_ExportWorksheetProperties()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"NET45876/";

    string savePath = CreateFolder(filePath);
    Workbook workbook = new Workbook(filePath + "a.xlsx");
    HtmlSaveOptions options = new HtmlSaveOptions();
    workbook.Save(savePath + "out.html", options);

    options.ExcludeUnusedStyles = true;
    options.ExportDocumentProperties = false;
    options.ExportWorkbookProperties = false;
    options.ExportWorksheetProperties = false;
    workbook.Save(savePath + "out2.html", options);
}
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


