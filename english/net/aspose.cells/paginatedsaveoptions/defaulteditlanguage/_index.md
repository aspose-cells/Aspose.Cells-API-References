---
title: PaginatedSaveOptions.DefaultEditLanguage
second_title: Aspose.Cells for .NET API Reference
description: PaginatedSaveOptions property. Gets or sets default edit language
type: docs
url: /net/aspose.cells/paginatedsaveoptions/defaulteditlanguage/
---
## PaginatedSaveOptions.DefaultEditLanguage property

Gets or sets default edit language.

```csharp
public DefaultEditLanguage DefaultEditLanguage { get; set; }
```

### Remarks

It may display/render different layouts for text paragraph when different edit languages is set. Default is Auto.

### Examples

```csharp
// Called: saveOptions.DefaultEditLanguage = DefaultEditLanguage.CJK;
public static void Property_DefaultEditLanguage()
        {
            // Open an Excel file
            Workbook workbook = new Workbook("DocxSaveOptions_original.xlsx");

            // Create an instance of DocxSaveOptions
            DocxSaveOptions saveOptions = new DocxSaveOptions();

            // Setting properties
            saveOptions.DefaultFont = "MS Gothic";
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
            saveOptions.CachedFileFolder = @"C:\Cache";
            saveOptions.ValidateMergedAreas = true;
            saveOptions.MergeAreas = false;
            saveOptions.SortNames = false;
            saveOptions.SortExternalNames = true;
            saveOptions.RefreshChartCache = true;
            saveOptions.UpdateSmartArt = false;

            // Save the document in DOCX format
            workbook.Save("DocxSaveOptionsExample.docx", saveOptions);

            return;
        }
```

### See Also

* enum [DefaultEditLanguage](../../defaulteditlanguage/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


