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
public void HtmlSaveOptions_Property_WidthScalable()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"JAVA43377/";
    string savePath = CreateFolder(filePath);

    Workbook workbook = new Workbook(filePath + "example.xlsx");
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
    workbook.Save(savePath + "example.html", options);
}
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


