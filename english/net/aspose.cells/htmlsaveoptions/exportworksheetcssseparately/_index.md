---
title: HtmlSaveOptions.ExportWorksheetCSSSeparately
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicating whether export the worksheet css separately.The default value is false
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportworksheetcssseparately/
---
## HtmlSaveOptions.ExportWorksheetCSSSeparately property

Indicating whether export the worksheet css separately.The default value is false.

```csharp
public bool ExportWorksheetCSSSeparately { get; set; }
```

### Examples

```csharp
// Called: options.ExportWorksheetCSSSeparately = true;
[Test]
        public void Property_ExportWorksheetCSSSeparately()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @"NET46818/";

            Workbook wb = new Workbook(filePath + "input.xlsx");

            wb.Worksheets.ActiveSheetIndex = 0;

            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportActiveWorksheetOnly = true;
            options.ExportDataOptions = HtmlExportDataOptions.All;
            options.ExportWorksheetCSSSeparately = true;
            options.ExcludeUnusedStyles = true;

            wb.Save(CreateFolder(filePath) + "out.html", options);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


