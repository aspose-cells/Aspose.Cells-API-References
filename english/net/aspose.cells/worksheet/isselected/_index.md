---
title: Worksheet.IsSelected
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Indicates whether this worksheet is selected when the workbook is opened
type: docs
url: /net/aspose.cells/worksheet/isselected/
---
## Worksheet.IsSelected property

Indicates whether this worksheet is selected when the workbook is opened.

```csharp
public bool IsSelected { get; set; }
```

### Examples

```csharp
// Called: worksheet.IsSelected = true;
private void Worksheet_Property_IsSelected(string filePath, Worksheet worksheet, int pageNumber, string printArea)
        {
            //this code only selects the specified worksheet tab
            worksheet.IsSelected = true;

            //you should set active worksheet index again.
            worksheet.Workbook.Worksheets.ActiveSheetIndex = worksheet.Index;

            worksheet.PageSetup.PrintHeadings = true;
            worksheet.PageSetup.PrintArea = printArea;

            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportActiveWorksheetOnly = true;
            saveOptions.ExportPrintAreaOnly = true;
            saveOptions.ExportGridLines = true;
            saveOptions.ExportHeadings = true;

            string outputFilePath = filePath + "out_" + pageNumber + ".html";

            worksheet.Workbook.Save(outputFilePath, saveOptions);
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


