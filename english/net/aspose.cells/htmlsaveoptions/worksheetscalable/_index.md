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
[Test]
        public void Property_WorksheetScalable()
        {
            
            // Creating a Workbook object
            Workbook workbook = new Workbook(Constants.sourcePath + "NET48312.xlsx");
            workbook.Worksheets.ActiveSheetIndex = 4;
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.WorksheetScalable = true;
            options.ExportActiveWorksheetOnly = true;
            workbook.Save(_destFilesPath + "NET48711.html", options);

            string text = File.ReadAllText(_destFilesPath + "NET48711.html");
            Assert.IsTrue(text.IndexOf("transform: scale(0.6)") != -1);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


