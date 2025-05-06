---
title: PaginatedSaveOptions.TextCrossType
second_title: Aspose.Cells for .NET API Reference
description: PaginatedSaveOptions property. Gets or sets displaying text type when the text width is larger than cell width
type: docs
url: /net/aspose.cells/paginatedsaveoptions/textcrosstype/
---
## PaginatedSaveOptions.TextCrossType property

Gets or sets displaying text type when the text width is larger than cell width.

```csharp
public TextCrossType TextCrossType { get; set; }
```

### Examples

```csharp
// Called: options.TextCrossType = TextCrossType.CrossKeep;
public static void Property_TextCrossType()
        {
            // Open an Excel file
            Workbook workbook = new Workbook(&quot;PaginatedSaveOptionsExample_original.xlsx&quot;);

            // Create an instance of PaginatedSaveOptions
            PdfSaveOptions options = new PdfSaveOptions();

            // Setting properties
            options.DefaultFont = &quot;Arial&quot;;
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
            options.CachedFileFolder = &quot;C:\\Temp&quot;;
            options.ValidateMergedAreas = true;
            options.MergeAreas = true;
            options.SortNames = true;
            options.SortExternalNames = true;
            options.RefreshChartCache = true;
            options.UpdateSmartArt = false;

            // Save the PDF file
            workbook.Save(&quot;PaginatedSaveOptionsExample.pdf&quot;, options);

            return;
        }
```

### See Also

* enum [TextCrossType](../../textcrosstype/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


