---
title: PageSetup.PrintHeadings
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Represents if row and column headings are printed with this page
type: docs
url: /net/aspose.cells/pagesetup/printheadings/
---
## PageSetup.PrintHeadings property

Represents if row and column headings are printed with this page.

```csharp
public bool PrintHeadings { get; set; }
```

### Examples

```csharp
// Called: worksheet.PageSetup.PrintHeadings = true;
private void Property_PrintHeadings(string filePath, Worksheet worksheet, int pageNumber, string printArea)
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

            string outputFilePath = filePath + &quot;out_&quot; + pageNumber + &quot;.html&quot;;

            worksheet.Workbook.Save(outputFilePath, saveOptions);
        }
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


