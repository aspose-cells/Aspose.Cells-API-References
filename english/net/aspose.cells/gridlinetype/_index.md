---
title: Enum GridlineType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.GridlineType enum. Enumerates grid line Type
type: docs
url: /net/aspose.cells/gridlinetype/
---
## GridlineType enumeration

Enumerates grid line Type.

```csharp
public enum GridlineType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Dotted | `0` | Represents dotted line. |
| Hair | `1` | Represents hair line. |

### Examples

```csharp
// Called: saveOptions.GridlineType = GridlineType.Dotted;
public static void Cells_Type_GridlineType()
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

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


