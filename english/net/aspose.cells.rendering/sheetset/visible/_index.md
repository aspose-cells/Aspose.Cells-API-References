---
title: SheetSet.Visible
second_title: Aspose.Cells for .NET API Reference
description: SheetSet property. Gets a set with visible sheets of the workbook in their original order
type: docs
url: /net/aspose.cells.rendering/sheetset/visible/
---
## SheetSet.Visible property

Gets a set with visible sheets of the workbook in their original order.

```csharp
public static SheetSet Visible { get; }
```

### Examples

```csharp
// Called: SheetSet = SheetSet.Visible,
public static void Property_Visible()
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

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


