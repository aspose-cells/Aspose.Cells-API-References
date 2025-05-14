---
title: PaginatedSaveOptions.IgnoreError
second_title: Aspose.Cells for .NET API Reference
description: PaginatedSaveOptions property. Indicates if you need to hide the error while rendering. The error can be error in shape image chart rendering etc
type: docs
url: /net/aspose.cells/paginatedsaveoptions/ignoreerror/
---
## PaginatedSaveOptions.IgnoreError property

Indicates if you need to hide the error while rendering. The error can be error in shape, image, chart rendering, etc.

```csharp
public bool IgnoreError { get; set; }
```

### Examples

```csharp
// Called: options.IgnoreError = true;
public static void PaginatedSaveOptions_Property_IgnoreError()
        {
            // Open an Excel file
            Workbook workbook = new Workbook("PaginatedSaveOptionsExample_original.xlsx");

            // Create an instance of PaginatedSaveOptions
            PdfSaveOptions options = new PdfSaveOptions();

            // Setting properties
            options.DefaultFont = "Arial";
            options.CheckWorkbookDefaultFont = true;
            options.CheckFontCompatibility = true;
            options.IsFontSubstitutionCharGranularity = true;
            options.OnePagePerSheet = false;
            options.AllColumnsInOnePagePerSheet = false;
            options.IgnoreError = true;
            options.OutputBlankPageWhenNothingToPrint = false;
            options.PageIndex = 3; // Starting page index (0-based index)
            options.PageCount = 2; // Number of pages to be printed
            options.PrintingPageType = PrintingPageType.IgnoreBlank;
            options.GridlineType = GridlineType.Dotted;
            options.TextCrossType = TextCrossType.CrossKeep;
            options.DefaultEditLanguage = DefaultEditLanguage.English;
            options.SheetSet = new SheetSet(new int[] { workbook.Worksheets.ActiveSheetIndex });
            options.ClearData = false;
            options.CachedFileFolder = "C:\\Temp";
            options.ValidateMergedAreas = true;
            options.MergeAreas = true;
            options.SortNames = true;
            options.SortExternalNames = true;
            options.RefreshChartCache = true;
            options.UpdateSmartArt = false;

            // Save the PDF file
            workbook.Save("PaginatedSaveOptionsExample.pdf", options);

            return;
        }
```

### See Also

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


