---
title: HtmlSaveOptions.WorksheetScalable
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates if zooming in or out the html via worksheet zoom level when saving file to html the default value is false
type: docs
url: /net/aspose.cells/htmlsaveoptions/worksheetscalable/
---
## HtmlSaveOptions.WorksheetScalable property

Indicates if zooming in or out the html via worksheet zoom level when saving file to html, the default value is false.

```csharp
public bool WorksheetScalable { get; set; }
```

### Examples

```csharp
// Called: options.WorksheetScalable = true;
public void HtmlSaveOptions_Property_WorksheetScalable()
{
            
    // Creating a Workbook object
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    workbook.Worksheets.ActiveSheetIndex = 4;
    HtmlSaveOptions options = new HtmlSaveOptions();
    options.WorksheetScalable = true;
    options.ExportActiveWorksheetOnly = true;
    workbook.Save(_destFilesPath + "example.html", options);

    string text = File.ReadAllText(_destFilesPath + "example.html");
    Assert.IsTrue(text.IndexOf("transform: scale(0.6)") != -1);
}
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


