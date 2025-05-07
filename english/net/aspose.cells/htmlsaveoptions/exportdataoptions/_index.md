---
title: HtmlSaveOptions.ExportDataOptions
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicating the rule of exporting html file data.The default value is All
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportdataoptions/
---
## HtmlSaveOptions.ExportDataOptions property

Indicating the rule of exporting html file data.The default value is All.

```csharp
public HtmlExportDataOptions ExportDataOptions { get; set; }
```

### Examples

```csharp
// Called: options.ExportDataOptions = HtmlExportDataOptions.All;
public void Property_ExportDataOptions()
            {
                Workbook wb = new Workbook(_outputDir + "graph.xlsx");

                wb.Worksheets.ActiveSheetIndex = 0;

                HtmlSaveOptions options = new HtmlSaveOptions();
                options.ExportActiveWorksheetOnly = true;
                options.ExportDataOptions = HtmlExportDataOptions.All;
                options.StreamProvider = this;
                options.IsExpImageToTempDir = true;

                string outputFilePath = Path.Combine(CreateFolder(Constants.HtmlDestPath + "NET46383"), "output.html");

                using (FileStream fs = new FileStream(outputFilePath, FileMode.Create))
                    wb.Save(fs, options);
            }
```

### See Also

* enum [HtmlExportDataOptions](../../htmlexportdataoptions/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


