---
title: Enum EmfRenderSetting
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.EmfRenderSetting enum. Setting for rendering Emf metafile
type: docs
url: /net/aspose.cells/emfrendersetting/
---
## EmfRenderSetting enumeration

Setting for rendering Emf metafile.

```csharp
public enum EmfRenderSetting
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| EmfOnly | `0` | Only rendering Emf records. |
| EmfPlusPrefer | `1` | Prefer rendering EmfPlus records. |

### Examples

```csharp
// Called: EmfRenderSetting = EmfRenderSetting.EmfOnly,
public static void Type_EmfRenderSetting()
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

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


