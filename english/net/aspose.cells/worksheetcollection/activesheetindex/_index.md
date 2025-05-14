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
public void WorksheetCollection_Property_ActiveSheetIndex()
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

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


