---
title: HtmlSaveOptions.CssStyles
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Gets or sets the additional css styles for the formatter. Only works when SaveAsSingleFile is True.  CssStylesbody  padding 5px 
type: docs
url: /net/aspose.cells/htmlsaveoptions/cssstyles/
---
## HtmlSaveOptions.CssStyles property

Gets or sets the additional css styles for the formatter. Only works when [`SaveAsSingleFile`](../saveassinglefile/) is True.  CssStyles="body { padding: 5px }";

```csharp
public string CssStyles { get; set; }
```

### Examples

```csharp
// Called: CssStyles = &amp;quot;body { padding: 5px }&amp;quot;,
public static void Property_CssStyles()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Hello&quot;);
            worksheet.Cells[&quot;B1&quot;].PutValue(&quot;World&quot;);

            // Create an instance of HtmlSaveOptions
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                IgnoreInvisibleShapes = true,
                PageTitle = &quot;Sample HTML Page&quot;,
                AttachedFilesDirectory = &quot;attached_files&quot;,
                AttachedFilesUrlPrefix = &quot;http://example.com/files/&quot;,
                DefaultFontName = &quot;Arial&quot;,
                AddGenericFont = true,
                WorksheetScalable = false,
                IsExportComments = false,
                ExportCommentsType = PrintCommentsType.PrintNoComments,
                DisableDownlevelRevealedComments = false,
                IsExpImageToTempDir = false,
                ImageScalable = true,
                WidthScalable = false,
                ExportSingleTab = false,
                ExportImagesAsBase64 = false,
                ExportActiveWorksheetOnly = false,
                ExportPrintAreaOnly = false,
                ExportArea = new CellArea { StartRow = 0, EndRow = 1, StartColumn = 0, EndColumn = 1 },
                ParseHtmlTagInCell = true,
                HtmlCrossStringType = HtmlCrossType.Default,
                HiddenColDisplayType = HtmlHiddenColDisplayType.Hidden,
                HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden,
                Encoding = System.Text.Encoding.UTF8,
                SaveAsSingleFile = false,
                ShowAllSheets = false,
                ExportPageHeaders = false,
                ExportPageFooters = false,
                ExportHiddenWorksheet = true,
                PresentationPreference = false,
                CellCssPrefix = &quot;&quot;,
                TableCssId = &quot;&quot;,
                IsFullPathLink = false,
                ExportWorksheetCSSSeparately = false,
                ExportSimilarBorderStyle = false,
                MergeEmptyTdForcely = false,
                MergeEmptyTdType = MergeEmptyTdType.Default,
                ExportCellCoordinate = false,
                ExportExtraHeadings = false,
                ExportHeadings = false,
                ExportRowColumnHeadings = false,
                ExportFormula = true,
                AddTooltipText = false,
                ExportGridLines = false,
                ExportBogusRowData = true,
                ExcludeUnusedStyles = true,
                ExportDocumentProperties = true,
                ExportWorksheetProperties = true,
                ExportWorkbookProperties = true,
                ExportFrameScriptsAndProperties = true,
                ExportDataOptions = HtmlExportDataOptions.All,
                LinkTargetType = HtmlLinkTargetType.Parent,
                IsIECompatible = false,
                FormatDataIgnoreColumnWidth = false,
                CalculateFormula = true,
                IsJsBrowserCompatible = true,
                IsMobileCompatible = false,
                CssStyles = &quot;body { padding: 5px }&quot;,
                HideOverflowWrappedText = false,
                IsBorderCollapsed = true,
                ClearData = false,
                CachedFileFolder = &quot;cache&quot;,
                ValidateMergedAreas = true,
                MergeAreas = true,
                SortNames = true,
                SortExternalNames = true,
                RefreshChartCache = true,
                UpdateSmartArt = false
            };

            // Save the workbook as HTML
            workbook.Save(&quot;HtmlSaveOptionsExample.html&quot;, saveOptions);

            return;
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


