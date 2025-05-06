---
title: PaginatedSaveOptions.CheckWorkbookDefaultFont
second_title: Aspose.Cells for .NET API Reference
description: PaginatedSaveOptions property. When characters in the Excel are Unicode and not be set with correct font in cell style They may appear as block in pdfimage. Set this to true to try to use workbooks default font to show these characters first
type: docs
url: /net/aspose.cells/paginatedsaveoptions/checkworkbookdefaultfont/
---
## PaginatedSaveOptions.CheckWorkbookDefaultFont property

When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first.

```csharp
public bool CheckWorkbookDefaultFont { get; set; }
```

### Remarks

Default is true.

### Examples

```csharp
// Called: saveOptions.CheckWorkbookDefaultFont = true;
public static void Property_CheckWorkbookDefaultFont()
        {
            // Open an Excel file
            Workbook workbook = new Workbook(&quot;DocxSaveOptions_original.xlsx&quot;);

            // Create an instance of DocxSaveOptions
            DocxSaveOptions saveOptions = new DocxSaveOptions();

            // Setting properties
            saveOptions.DefaultFont = &quot;MS Gothic&quot;;
            saveOptions.CheckWorkbookDefaultFont = true;
            saveOptions.CheckFontCompatibility = false;
            saveOptions.IsFontSubstitutionCharGranularity = true;
            saveOptions.OnePagePerSheet = true;
            saveOptions.AllColumnsInOnePagePerSheet = false;
            saveOptions.IgnoreError = true;
            saveOptions.OutputBlankPageWhenNothingToPrint = false;
            saveOptions.PageIndex = 0;  // Starting page index (0-based index)
            saveOptions.PageCount = 2;  // Number of pages to be printed
            saveOptions.PrintingPageType = PrintingPageType.IgnoreBlank;
            saveOptions.GridlineType = GridlineType.Dotted;
            saveOptions.TextCrossType = TextCrossType.CrossKeep;
            saveOptions.DefaultEditLanguage = DefaultEditLanguage.CJK;
            saveOptions.SheetSet = SheetSet.All;
            saveOptions.ClearData = true;
            saveOptions.CachedFileFolder = @&quot;C:\Cache&quot;;
            saveOptions.ValidateMergedAreas = true;
            saveOptions.MergeAreas = false;
            saveOptions.SortNames = false;
            saveOptions.SortExternalNames = true;
            saveOptions.RefreshChartCache = true;
            saveOptions.UpdateSmartArt = false;

            // Save the document in DOCX format
            workbook.Save(&quot;DocxSaveOptionsExample.docx&quot;, saveOptions);

            return;
        }
```

### See Also

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


