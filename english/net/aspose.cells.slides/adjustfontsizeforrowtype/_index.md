---
title: Enum AdjustFontSizeForRowType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Slides.AdjustFontSizeForRowType enum. Represents which kind of rows should be ajusted
type: docs
url: /net/aspose.cells.slides/adjustfontsizeforrowtype/
---
## AdjustFontSizeForRowType enumeration

Represents which kind of rows should be ajusted.

```csharp
public enum AdjustFontSizeForRowType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| None | `0` | No adjsut. |
| EmptyRows | `1` | If the row is empty, change font size to fit row height. |

### Examples

```csharp
// Called: AdjustFontSizeForRowType = AdjustFontSizeForRowType.EmptyRows,
public static void Slides_Type_AdjustFontSizeForRowType()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fill some data into the worksheet
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // Create an instance of PptxSaveOptions
            PptxSaveOptions saveOptions = new PptxSaveOptions
            {
                IgnoreHiddenRows = true,
                AdjustFontSizeForRowType = AdjustFontSizeForRowType.EmptyRows,
                ExportViewType = SlideViewType.Print,
                DefaultFont = "Arial",
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
                CachedFileFolder = "C:\\Temp",
                ValidateMergedAreas = true,
                MergeAreas = true,
                SortNames = true,
                SortExternalNames = true,
                RefreshChartCache = true,
                UpdateSmartArt = true
            };

            // Save the workbook as a PPTX file
            workbook.Save("PptxSaveOptionsExample.pptx", saveOptions);
        }
```

### See Also

* namespace [Aspose.Cells.Slides](../../aspose.cells.slides/)
* assembly [Aspose.Cells](../../)


