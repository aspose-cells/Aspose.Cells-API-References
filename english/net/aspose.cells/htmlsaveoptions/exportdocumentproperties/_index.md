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
public void HtmlSaveOptions_Property_ExportDocumentProperties()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"JAVA42495/";

    Workbook workbook = new Workbook(filePath + "input.xlsx");
    HtmlSaveOptions options = new HtmlSaveOptions();
    Worksheet sheet = workbook.Worksheets["Entry points"];
    workbook.Worksheets.ActiveSheetIndex = sheet.Index;
    options.ExportActiveWorksheetOnly = true;
    options.ExportDocumentProperties = false;
    options.ExportWorkbookProperties = false;
    options.ExportWorksheetProperties = false;
    workbook.Save(Constants.destPath + "example.html", options);

    //simon
    workbook = new Workbook(Constants.destPath + "example.html");
    Style style = workbook.Worksheets[0].Cells["C3"].GetStyle();
    Assert.IsTrue(style.IsTextWrapped);
}
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


