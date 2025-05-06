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
[Test]
        public void Property_IsSelected()
        {
            var workbook = new Workbook(Constants.sourcePath + &quot;CellsNet48504.xlsx&quot;);
            var worksheet = workbook.Worksheets[workbook.Worksheets.Count - 1];

            var printOptions = new ImageOrPrintOptions();
            printOptions.OnePagePerSheet = false;

            CellArea[] pages = worksheet.GetPrintingPageBreaks(printOptions);
            var lastPage = pages[pages.Length - 1];

            int firstRow = lastPage.StartRow;
            int firstColumn = lastPage.StartColumn;
            int totalRows = lastPage.EndRow - lastPage.StartRow + 1;
            int totalColumns = lastPage.EndColumn - lastPage.StartColumn + 1;

            var lastPageRange = worksheet.Cells.CreateRange(firstRow, firstColumn, totalRows, totalColumns);

            Console.WriteLine($&quot;Last page of address &apos;{lastPageRange.Address}&apos;&quot;);

            worksheet.IsSelected = true;
            worksheet.Workbook.Worksheets.ActiveSheetIndex = worksheet.Index;
            worksheet.PageSetup.PrintArea = lastPageRange.Address;

            var saveOptions = new HtmlSaveOptions();
            saveOptions.ExportPrintAreaOnly = true;
            saveOptions.ExportActiveWorksheetOnly = true;
            saveOptions.ExportImagesAsBase64 = true;
            saveOptions.ExportDataOptions = HtmlExportDataOptions.All;
            saveOptions.ExportExtraHeadings = true;

            workbook.Save(new MemoryStream(), saveOptions);
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


