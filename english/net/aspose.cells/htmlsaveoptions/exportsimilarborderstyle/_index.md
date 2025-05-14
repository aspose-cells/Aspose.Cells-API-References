---
title: HtmlSaveOptions.ExportSimilarBorderStyle
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicating whether exporting the similar border style when the border style is not supported by browsers. If you want to import the html or mht file to excel please keep the default value. The default value is false
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportsimilarborderstyle/
---
## HtmlSaveOptions.ExportSimilarBorderStyle property

Indicating whether exporting the similar border style when the border style is not supported by browsers. If you want to import the html or mht file to excel, please keep the default value. The default value is false.

```csharp
public bool ExportSimilarBorderStyle { get; set; }
```

### Examples

```csharp
// Called: htmlSaveOptions.ExportSimilarBorderStyle = true;
public void HtmlSaveOptions_Property_ExportSimilarBorderStyle()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"JAVA42853/";

    Workbook workbook = new Workbook(filePath + "view_qldtl_Admin.xlsx");
    HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions(SaveFormat.Html);
    htmlSaveOptions.DisableDownlevelRevealedComments = true;
    htmlSaveOptions.ExcludeUnusedStyles = true;
    htmlSaveOptions.ExportActiveWorksheetOnly = true;
    htmlSaveOptions.ExportDocumentProperties = false;
    htmlSaveOptions.ExportFrameScriptsAndProperties = false;
    htmlSaveOptions.ExportImagesAsBase64 = false;
    htmlSaveOptions.ExportPrintAreaOnly = true;
    htmlSaveOptions.ExportSimilarBorderStyle = true;
    htmlSaveOptions.ExportWorkbookProperties = false;
    htmlSaveOptions.ExportWorksheetCSSSeparately = false;
    htmlSaveOptions.ExportWorksheetProperties = false;
    htmlSaveOptions.ParseHtmlTagInCell = true;
    htmlSaveOptions.HtmlCrossStringType = HtmlCrossType.FitToCell;

    DateTime start = DateTime.Now;

    workbook.Save(CreateFolder(filePath) + "out.html", htmlSaveOptions);

    Assert.Less(DateTime.Now.Subtract(start).Seconds, 30);
}
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


