---
title: PaginatedSaveOptions.CheckFontCompatibility
second_title: Aspose.Cells for .NET API Reference
description: PaginatedSaveOptions property. Indicates whether to check font compatibility for every character in text
type: docs
url: /net/aspose.cells/paginatedsaveoptions/checkfontcompatibility/
---
## PaginatedSaveOptions.CheckFontCompatibility property

Indicates whether to check font compatibility for every character in text.

```csharp
public bool CheckFontCompatibility { get; set; }
```

### Remarks

The default value is true. Disable this property may give better performance. But when the default or specified font of text/character cannot be used to render it, unreadable characters(such as block) maybe occur in the generated pdf. For such situation user should keep this property as true so that alternative font can be searched and used to render the text instead;

### Examples

```csharp
// Called: options.CheckFontCompatibility = true;
public static void Property_CheckFontCompatibility()
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

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


