---
title: Enum SlideViewType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Slides.SlideViewType enum. Represents the type when exporting to slides
type: docs
url: /net/aspose.cells.slides/slideviewtype/
---
## SlideViewType enumeration

Represents the type when exporting to slides.

```csharp
public enum SlideViewType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| View | `0` | Exporting as view in MS Excel. |
| Print | `1` | Exporting as printing. |

### Examples

```csharp
// Called: ExportViewType = SlideViewType.Print,
public static void Type_SlideViewType()
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

* namespace [Aspose.Cells.Slides](../../aspose.cells.slides/)
* assembly [Aspose.Cells](../../)


