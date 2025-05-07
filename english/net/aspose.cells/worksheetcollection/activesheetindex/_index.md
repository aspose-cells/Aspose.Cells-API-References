---
title: WorksheetCollection.ActiveSheetIndex
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection property. Represents the index of active worksheet when the spreadsheet is opened
type: docs
url: /net/aspose.cells/worksheetcollection/activesheetindex/
---
## WorksheetCollection.ActiveSheetIndex property

Represents the index of active worksheet when the spreadsheet is opened.

```csharp
public int ActiveSheetIndex { get; set; }
```

### Remarks

Sheet index is zero based.

### Examples

```csharp
// Called: wb.Worksheets.ActiveSheetIndex = 0;
public void Property_ActiveSheetIndex(string filePath)
            {
                Console.WriteLine("Convert to HTML with embedded resources.");

                Workbook wb = new Workbook(filePath);
                Worksheet ws = wb.Worksheets[0];

                wb.Worksheets.ActiveSheetIndex = 0;

                HtmlSaveOptions options = new HtmlSaveOptions();
                options.ExportHiddenWorksheet = false;
                options.ExportActiveWorksheetOnly = true;
                options.HtmlCrossStringType = HtmlCrossType.Cross;
                options.ExportDataOptions = HtmlExportDataOptions.All;
                options.CellCssPrefix = "prefix";
                options.ExportImagesAsBase64 = true;

                string outputFile = _outputDirectory + "page1.html";
                FileStream fileStream = File.Create(outputFile);
                wb.Save(fileStream, options);
            }
```

### See Also

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


