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
// Called: IgnoreError = true,
public static void Property_IgnoreError()
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

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


