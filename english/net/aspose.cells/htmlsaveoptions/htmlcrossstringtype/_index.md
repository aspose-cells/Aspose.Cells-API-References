---
title: HtmlSaveOptions.HtmlCrossStringType
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates if a crosscell string will be displayed in the same way as MS Excel when saving an Excel file in html format. By default the value is Default so for crosscell strings there is little difference between the html files created by Aspose.Cells and MS Excel. But the performance for creating large html filessetting the value to Cross would be several times faster than setting it to Default or Fit2Cell
type: docs
url: /net/aspose.cells/htmlsaveoptions/htmlcrossstringtype/
---
## HtmlSaveOptions.HtmlCrossStringType property

Indicates if a cross-cell string will be displayed in the same way as MS Excel when saving an Excel file in html format. By default the value is Default, so, for cross-cell strings, there is little difference between the html files created by Aspose.Cells and MS Excel. But the performance for creating large html files,setting the value to Cross would be several times faster than setting it to Default or Fit2Cell.

```csharp
public HtmlCrossType HtmlCrossStringType { get; set; }
```

### Examples

```csharp
// Called: options.HtmlCrossStringType = HtmlCrossType.CrossHideRight;
public void HtmlSaveOptions_Property_HtmlCrossStringType()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"JAVA42856/";

    //Load the sample Excel file
    Workbook workbook = new Workbook(filePath + "wpsCAP4触发CAP3.xlsx");
    //workbook.Worksheets[1].Shapes[0].ToImage(CreateFolder(filePath) + "shape1.png", new ImageOrPrintOptions());

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

* enum [HtmlCrossType](../../htmlcrosstype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


