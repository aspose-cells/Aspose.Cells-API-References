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
// Called: GridlineType = GridlineType.Dotted,
public static void Type_GridlineType()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fill some data into the worksheet
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Hello&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;World&quot;);

            // Create an instance of PptxSaveOptions
            PptxSaveOptions saveOptions = new PptxSaveOptions
            {
                IgnoreHiddenRows = true,
                AdjustFontSizeForRowType = AdjustFontSizeForRowType.EmptyRows,
                ExportViewType = SlideViewType.Print,
                DefaultFont = &quot;Arial&quot;,
                CheckWorkbookDefaultFont = true,
                CheckFontCompatibility = true,
                IsFontSubstitutionCharGranularity = true,
                OnePagePerSheet = true,
                AllColumnsInOnePagePerSheet = true,
                IgnoreError = true,
                OutputBlankPageWhenNothingToPrint = true,
                PageIndex = 0,
                PageCount = 1,
                PrintingPageType = PrintingPageType.IgnoreBlank,
                GridlineType = GridlineType.Dotted,
                TextCrossType = TextCrossType.CrossKeep,
                DefaultEditLanguage = DefaultEditLanguage.English,
                SheetSet = SheetSet.Visible,
                EmfRenderSetting = EmfRenderSetting.EmfOnly,
                ClearData = true,
                CachedFileFolder = &quot;C:\\Temp&quot;,
                ValidateMergedAreas = true,
                MergeAreas = true,
                SortNames = true,
                SortExternalNames = true,
                RefreshChartCache = true,
                UpdateSmartArt = true
            };

            // Save the workbook as a PPTX file
            workbook.Save(&quot;PptxSaveOptionsExample.pptx&quot;, saveOptions);
        }
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


