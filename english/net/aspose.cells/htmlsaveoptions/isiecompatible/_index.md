---
title: HtmlSaveOptions.IsIECompatible
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicating whether the output HTML is compatible with IE browser. The defalut value is false
type: docs
url: /net/aspose.cells/htmlsaveoptions/isiecompatible/
---
## HtmlSaveOptions.IsIECompatible property

Indicating whether the output HTML is compatible with IE browser. The defalut value is false

```csharp
public bool IsIECompatible { get; set; }
```

### Examples

```csharp
// Called: saveOptions.IsIECompatible = false;
public static void Property_IsIECompatible()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].PutValue(&quot;Hello World&quot;);

            // Create an instance of EbookSaveOptions
            EbookSaveOptions saveOptions = new EbookSaveOptions();

            // Setting properties
            saveOptions.IgnoreInvisibleShapes = true;
            saveOptions.PageTitle = &quot;Sample Page Title&quot;;
            saveOptions.AttachedFilesDirectory = &quot;attached_files&quot;;
            saveOptions.AttachedFilesUrlPrefix = &quot;http://example.com/files/&quot;;
            saveOptions.DefaultFontName = &quot;Arial&quot;;
            saveOptions.AddGenericFont = true;
            saveOptions.WorksheetScalable = false;
            saveOptions.IsExportComments = false;
            saveOptions.ExportCommentsType = PrintCommentsType.PrintNoComments;
            saveOptions.DisableDownlevelRevealedComments = false;
            saveOptions.IsExpImageToTempDir = false;
            saveOptions.ImageScalable = true;
            saveOptions.WidthScalable = false;
            saveOptions.ExportSingleTab = false;
            saveOptions.ExportImagesAsBase64 = false;
            saveOptions.ExportActiveWorksheetOnly = false;
            saveOptions.ExportPrintAreaOnly = false;
            saveOptions.ExportArea = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            saveOptions.ParseHtmlTagInCell = true;
            saveOptions.HtmlCrossStringType = HtmlCrossType.Default;
            saveOptions.HiddenColDisplayType = HtmlHiddenColDisplayType.Hidden;
            saveOptions.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden;
            saveOptions.Encoding = System.Text.Encoding.UTF8;
            saveOptions.SaveAsSingleFile = false;
            saveOptions.ShowAllSheets = true;
            saveOptions.ExportPageHeaders = true;
            saveOptions.ExportPageFooters = true;
            saveOptions.ExportHiddenWorksheet = true;
            saveOptions.PresentationPreference = false;
            saveOptions.CellCssPrefix = &quot;cell_&quot;;
            saveOptions.TableCssId = &quot;table_&quot;;
            saveOptions.IsFullPathLink = false;
            saveOptions.ExportWorksheetCSSSeparately = false;
            saveOptions.ExportSimilarBorderStyle = false;
            saveOptions.MergeEmptyTdForcely = false;
            saveOptions.MergeEmptyTdType = MergeEmptyTdType.Default;
            saveOptions.ExportCellCoordinate = false;
            saveOptions.ExportExtraHeadings = false;
            saveOptions.ExportHeadings = true;
            saveOptions.ExportRowColumnHeadings = true;
            saveOptions.ExportFormula = true;
            saveOptions.AddTooltipText = false;
            saveOptions.ExportGridLines = false;
            saveOptions.ExportBogusRowData = true;
            saveOptions.ExcludeUnusedStyles = true;
            saveOptions.ExportDocumentProperties = true;
            saveOptions.ExportWorksheetProperties = true;
            saveOptions.ExportWorkbookProperties = true;
            saveOptions.ExportFrameScriptsAndProperties = true;
            saveOptions.ExportDataOptions = HtmlExportDataOptions.All;
            saveOptions.LinkTargetType = HtmlLinkTargetType.Parent;
            saveOptions.IsIECompatible = false;
            saveOptions.FormatDataIgnoreColumnWidth = false;
            saveOptions.CalculateFormula = true;
            saveOptions.IsJsBrowserCompatible = true;
            saveOptions.IsMobileCompatible = false;
            saveOptions.CssStyles = &quot;body { padding: 5px }&quot;;
            saveOptions.HideOverflowWrappedText = false;
            saveOptions.IsBorderCollapsed = true;
            saveOptions.ClearData = true;
            saveOptions.CachedFileFolder = &quot;cache&quot;;
            saveOptions.ValidateMergedAreas = true;
            saveOptions.MergeAreas = true;
            saveOptions.SortNames = true;
            saveOptions.SortExternalNames = true;
            saveOptions.RefreshChartCache = true;
            saveOptions.WarningCallback = null;
            saveOptions.UpdateSmartArt = true;

            // Save the workbook to an HTML file with the specified options
            workbook.Save(&quot;EbookSaveOptionsExample.html&quot;, saveOptions);

            return;
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


