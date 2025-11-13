---
title: Class HtmlSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.HtmlSaveOptions class. Represents the options for saving html file
type: docs
url: /net/aspose.cells/htmlsaveoptions/
---
## HtmlSaveOptions class

Represents the options for saving html file.

```csharp
public class HtmlSaveOptions : SaveOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions/#constructor)() | Creates options for saving html file. |
| [HtmlSaveOptions](htmlsaveoptions/#constructor_1)(SaveFormat) | Creates options for saving htm file. |

## Properties

| Name | Description |
| --- | --- |
| [AddGenericFont](../../aspose.cells/htmlsaveoptions/addgenericfont/) { get; set; } | Indicates whether to add a generic font to CSS font-family. The default value is true |
| [AddTooltipText](../../aspose.cells/htmlsaveoptions/addtooltiptext/) { get; set; } | Indicates whether adding tooltip text when the data can't be fully displayed. The default value is false. |
| [AttachedFilesDirectory](../../aspose.cells/htmlsaveoptions/attachedfilesdirectory/) { get; set; } | The directory that the attached files will be saved to. Only for saving to html stream. |
| [AttachedFilesUrlPrefix](../../aspose.cells/htmlsaveoptions/attachedfilesurlprefix/) { get; set; } | Specify the Url prefix of attached files such as image in the html file. Only for saving to html stream. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | The folder for temporary files that may be used as data cache.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [CalculateFormula](../../aspose.cells/htmlsaveoptions/calculateformula/) { get; set; } | Indicates whether to calculate formulas before saving html file. |
| [CellCssPrefix](../../aspose.cells/htmlsaveoptions/cellcssprefix/) { get; set; } | Gets and sets the prefix of the css name,the default value is "". |
| [CellNameAttribute](../../aspose.cells/htmlsaveoptions/cellnameattribute/) { get; set; } | Specifies the attribute that indicates the CellName to be written. (e.g. If the value is "id", then for cell "A1", the output will be:&lt;td id='A1'&gt;). The default value is null. |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Make the workbook empty after saving the file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | If true and the directory does not exist, the directory will be automatically created before saving the file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [CssStyles](../../aspose.cells/htmlsaveoptions/cssstyles/) { get; set; } | Gets or sets the additional css styles for the formatter. Only works when [`SaveAsSingleFile`](./saveassinglefile/) is True.  CssStyles="body { padding: 5px }"; |
| [DefaultFontName](../../aspose.cells/htmlsaveoptions/defaultfontname/) { get; set; } | Specify the default font name for exporting html, the default font will be used when the font of style is not existing, If this property is null, Aspose.Cells will use universal font which have the same family with the original font, the default value is null. |
| [DisableCss](../../aspose.cells/htmlsaveoptions/disablecss/) { get; set; } | Indicates whether only inline styles are applied, without relying on CSS. The default value is false. |
| [DisableDownlevelRevealedComments](../../aspose.cells/htmlsaveoptions/disabledownlevelrevealedcomments/) { get; set; } | Indicates if disable Downlevel-revealed conditional comments when exporting file to html, the default value is false. |
| [EmbeddedFontType](../../aspose.cells/htmlsaveoptions/embeddedfonttype/) { get; set; } | Gets or sets the type of embedding font file into html file. Default value is None which indicates that no font will be embedded in html. |
| [EnableCssCustomProperties](../../aspose.cells/htmlsaveoptions/enablecsscustomproperties/) { get; set; } | Optimize the output of html by using CSS custom properties. For example, for the scenario that there are multiple occurences for one base64 image, with custom property the image data only needs to be saved once so the performance of the resultant html can be improved. The default value is false. |
| [EncodeEntityAsCode](../../aspose.cells/htmlsaveoptions/encodeentityascode/) { get; set; } | Indicates whether the html character entities are replaced with decimal code. (e.g. "&amp;nbsp;" is replaced with "&amp;#160;"). The default value is false. |
| [Encoding](../../aspose.cells/htmlsaveoptions/encoding/) { get; set; } | If not set,use Encoding.UTF8 as default enconding type. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indicates whether encrypt document properties when saving as .xls file. The default value is true.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [ExcludeUnusedStyles](../../aspose.cells/htmlsaveoptions/excludeunusedstyles/) { get; set; } | Indicating whether excludes unused styles. For the generated html files, excluding unused styles can make the file size smaller without affecting the visual effects. So the default value of this property is true. If user needs to keep all styles in the workbook for the generated html(such as the scenario that user needs to restore the workbook from the generated html later), please set this property as false. |
| [ExportActiveWorksheetOnly](../../aspose.cells/htmlsaveoptions/exportactiveworksheetonly/) { get; set; } | Indicates if only exporting the active worksheet to html file. If true then only the active worksheet will be exported to html file; If false then the whole workbook will be exported to html file. The default value is false. |
| [ExportArea](../../aspose.cells/htmlsaveoptions/exportarea/) { get; set; } | Gets or Sets the exporting CellArea of current active Worksheet. If you set this attribute, the print area of current active Worksheet will be omitted. Only the specified area will be exported when saving the file to html. |
| [ExportBogusRowData](../../aspose.cells/htmlsaveoptions/exportbogusrowdata/) { get; set; } | Indicating whether exporting bogus bottom row data. The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [ExportCellCoordinate](../../aspose.cells/htmlsaveoptions/exportcellcoordinate/) { get; set; } | Indicates whether exporting excel coordinate of nonblank cells when saving file to html. The default value is false. If you want to import the output html to excel, please keep the default value. |
| [ExportCommentsType](../../aspose.cells/htmlsaveoptions/exportcommentstype/) { get; set; } | Represents type of exporting comments to html files. |
| [ExportDataOptions](../../aspose.cells/htmlsaveoptions/exportdataoptions/) { get; set; } | Indicating the rule of exporting html file data.The default value is All. |
| [ExportDocumentProperties](../../aspose.cells/htmlsaveoptions/exportdocumentproperties/) { get; set; } | Indicating whether exporting document properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [ExportExtraHeadings](../../aspose.cells/htmlsaveoptions/exportextraheadings/) { get; set; } | Indicates whether exporting extra headings when the length of text is longer than max display column. The default value is false. If you want to import the html file to excel, please keep the default value. |
| [ExportFormula](../../aspose.cells/htmlsaveoptions/exportformula/) { get; set; } | Indicates whether exporting formula when saving file to html. The default value is true. If you want to import the output html to excel, please keep the default value. |
| [ExportFrameScriptsAndProperties](../../aspose.cells/htmlsaveoptions/exportframescriptsandproperties/) { get; set; } | Indicating whether exporting frame scripts and document properties. The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [ExportGridLines](../../aspose.cells/htmlsaveoptions/exportgridlines/) { get; set; } | Indicating whether exporting the gridlines.The default value is false. |
| [ExportHeadings](../../aspose.cells/htmlsaveoptions/exportheadings/) { get; set; } | (**Obsolete.**) Indicates whether exports sheet's row and column headings when saving to HTML files. |
| [ExportHiddenWorksheet](../../aspose.cells/htmlsaveoptions/exporthiddenworksheet/) { get; set; } | Indicating if exporting the hidden worksheet content.The default value is true. |
| [ExportImagesAsBase64](../../aspose.cells/htmlsaveoptions/exportimagesasbase64/) { get; set; } | Specifies whether images are saved in Base64 format to HTML, MHTML or EPUB. |
| [ExportObjectListener](../../aspose.cells/htmlsaveoptions/exportobjectlistener/) { get; set; } | (**Obsolete.**) Gets or sets the ExportObjectListener for exporting objects. |
| [ExportPageFooters](../../aspose.cells/htmlsaveoptions/exportpagefooters/) { get; set; } | Indicates whether exporting page headers. |
| [ExportPageHeaders](../../aspose.cells/htmlsaveoptions/exportpageheaders/) { get; set; } | Indicates whether exporting page headers. |
| [ExportPrintAreaOnly](../../aspose.cells/htmlsaveoptions/exportprintareaonly/) { get; set; } | Indicates if only exporting the print area to html file. The default value is false. |
| [ExportRowColumnHeadings](../../aspose.cells/htmlsaveoptions/exportrowcolumnheadings/) { get; set; } | Indicates whether exports sheet's row and column headings when saving to HTML files. |
| [ExportSimilarBorderStyle](../../aspose.cells/htmlsaveoptions/exportsimilarborderstyle/) { get; set; } | Indicating whether exporting the similar border style when the border style is not supported by browsers. If you want to import the html or mht file to excel, please keep the default value. The default value is false. |
| [ExportSingleTab](../../aspose.cells/htmlsaveoptions/exportsingletab/) { get; set; } | Indicates whether exporting the single tab when the file only has one worksheet. The default value is false. |
| [ExportWorkbookProperties](../../aspose.cells/htmlsaveoptions/exportworkbookproperties/) { get; set; } | Indicating whether exporting workbook properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [ExportWorksheetCSSSeparately](../../aspose.cells/htmlsaveoptions/exportworksheetcssseparately/) { get; set; } | Indicating whether export the worksheet css separately.The default value is false. |
| [ExportWorksheetProperties](../../aspose.cells/htmlsaveoptions/exportworksheetproperties/) { get; set; } | Indicating whether exporting worksheet properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [FilePathProvider](../../aspose.cells/htmlsaveoptions/filepathprovider/) { get; set; } | Gets or sets the IFilePathProvider for exporting Worksheet to html separately. |
| [FormatDataIgnoreColumnWidth](../../aspose.cells/htmlsaveoptions/formatdataignorecolumnwidth/) { get; set; } | Indicating whether show the whole formatted data of cell when overflowing the column. If true then ignore the column width and the whole data of cell will be exported. If false then the data will be exported same as Excel. The default value is false. |
| [HiddenColDisplayType](../../aspose.cells/htmlsaveoptions/hiddencoldisplaytype/) { get; set; } | Hidden column(the width of this column is 0) in excel,before save this into html format, if HtmlHiddenColDisplayType is "Remove",the hidden column would not been output, if the value is "Hidden", the column would been output,but was hidden,the default value is "Hidden" |
| [HiddenRowDisplayType](../../aspose.cells/htmlsaveoptions/hiddenrowdisplaytype/) { get; set; } | Hidden row(the height of this row is 0) in excel,before save this into html format, if HtmlHiddenRowDisplayType is "Remove",the hidden row would not been output, if the value is "Hidden", the row would been output,but was hidden,the default value is "Hidden" |
| [HideOverflowWrappedText](../../aspose.cells/htmlsaveoptions/hideoverflowwrappedtext/) { get; set; } | Indicates whether to hide overflow text when the cell format is set to wrap text. The default value is false |
| [HtmlCrossStringType](../../aspose.cells/htmlsaveoptions/htmlcrossstringtype/) { get; set; } | Indicates if a cross-cell string will be displayed in the same way as MS Excel when saving an Excel file in html format. By default the value is Default, so, for cross-cell strings, there is little difference between the html files created by Aspose.Cells and MS Excel. But the performance for creating large html files,setting the value to Cross would be several times faster than setting it to Default or Fit2Cell. |
| [HtmlVersion](../../aspose.cells/htmlsaveoptions/htmlversion/) { get; set; } | Specifies version of HTML standard that should be used when saving the HTML format. Default value is HtmlVersion.Default. |
| [IgnoreInvisibleShapes](../../aspose.cells/htmlsaveoptions/ignoreinvisibleshapes/) { get; set; } | Indicate whether exporting those not visible shapes |
| [ImageOptions](../../aspose.cells/htmlsaveoptions/imageoptions/) { get; } | Get the ImageOrPrintOptions object before exporting |
| [ImageScalable](../../aspose.cells/htmlsaveoptions/imagescalable/) { get; set; } | Indicates whether using scalable unit to describe the image width when using scalable unit to describe the column width. The default value is true. |
| [IsBorderCollapsed](../../aspose.cells/htmlsaveoptions/isbordercollapsed/) { get; set; } | Indicates whether the table borders are collapsed. The default value is true. |
| [IsExpImageToTempDir](../../aspose.cells/htmlsaveoptions/isexpimagetotempdir/) { get; set; } | Indicates whether exporting image files to temp directory. Only for saving to html stream. |
| [IsExportComments](../../aspose.cells/htmlsaveoptions/isexportcomments/) { get; set; } | Indicates if exporting comments when saving file to html, the default value is false. |
| [IsFullPathLink](../../aspose.cells/htmlsaveoptions/isfullpathlink/) { get; set; } | Indicating whether using full path link in sheet00x.htm,filelist.xml and tabstrip.htm. The default value is false. |
| [IsIECompatible](../../aspose.cells/htmlsaveoptions/isiecompatible/) { get; set; } | Indicating whether the output HTML is compatible with IE browser. The defalut value is false |
| [IsJsBrowserCompatible](../../aspose.cells/htmlsaveoptions/isjsbrowsercompatible/) { get; set; } | Indicates whether JavaScript is compatible with browsers that do not support JavaScript. The default value is true. |
| [IsMobileCompatible](../../aspose.cells/htmlsaveoptions/ismobilecompatible/) { get; set; } | Indicates whether the output HTML is compatible with mobile devices. The default value is false. |
| [LayoutMode](../../aspose.cells/htmlsaveoptions/layoutmode/) { get; set; } | Gets or sets the layout mode when saving to HTML. The default value is Normal |
| [LinkTargetType](../../aspose.cells/htmlsaveoptions/linktargettype/) { get; set; } | Indicating the type of target attribute in `<a>` link. The default value is HtmlLinkTargetType.Parent. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indicates whether merge the areas of conditional formatting and validation before saving the file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [MergeEmptyTdForcely](../../aspose.cells/htmlsaveoptions/mergeemptytdforcely/) { get; set; } | (**Obsolete.**) Indicates whether merging empty TD element forcedly when exporting file to html. The size of html file will be reduced significantly after setting value to true. The default value is false. If you want to import the html file to excel or export perfect grid lines when saving file to html, please keep the default value. |
| [MergeEmptyTdType](../../aspose.cells/htmlsaveoptions/mergeemptytdtype/) { get; set; } | The option to merge contiguous empty cells(empty td elements) The default value is MergeEmptyTdType.Default. |
| [OfficeMathOutputMode](../../aspose.cells/htmlsaveoptions/officemathoutputmode/) { get; set; } | Indicates how export OfficeMath objects to HTML, Default value is Image. |
| [PageTitle](../../aspose.cells/htmlsaveoptions/pagetitle/) { get; set; } | The title of the html page. Only for saving to html stream. |
| [ParseHtmlTagInCell](../../aspose.cells/htmlsaveoptions/parsehtmltagincell/) { get; set; } | Indicates whether html tag(such as `<div></div>`) in cell should be parsed as cell value or preserved as it is. The default value is true. |
| [PresentationPreference](../../aspose.cells/htmlsaveoptions/presentationpreference/) { get; set; } | Indicating if html or mht file is presentation preference. The default value is false. if you want to get more beautiful presentation,please set the value to true. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indicates whether refreshing chart cache data(Inherited from [`SaveOptions`](../saveoptions/).) |
| [SaveAsSingleFile](../../aspose.cells/htmlsaveoptions/saveassinglefile/) { get; set; } | Indicates whether save the html as single file. The default value is false. |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Gets the save file format.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [SheetSet](../../aspose.cells/htmlsaveoptions/sheetset/) { get; set; } | Gets or sets the sheets to render. Default is all visible sheets in the workbook: [`Visible`](../../aspose.cells.rendering/sheetset/visible/). |
| [ShowAllSheets](../../aspose.cells/htmlsaveoptions/showallsheets/) { get; set; } | Indicates whether showing all sheets when saving as a single html file. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indicates whether sorting external defined names before saving file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indicates whether sorting defined names before saving file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [StreamProvider](../../aspose.cells/htmlsaveoptions/streamprovider/) { get; set; } | Gets or sets the IStreamProvider for exporting objects. |
| [TableCssId](../../aspose.cells/htmlsaveoptions/tablecssid/) { get; set; } | Gets and sets the prefix of the type css name such as tr,col,td and so on, they are contained in the table element which has the specific TableCssId attribute. The default value is "". |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Indicates whether updating smart art setting. The default value is false.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Indicates whether validate merged cells before saving the file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Gets or sets warning callback.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [WidthScalable](../../aspose.cells/htmlsaveoptions/widthscalable/) { get; set; } | Indicates whether exporting column width in unit of scale to html. The default value is false. |
| [WorksheetScalable](../../aspose.cells/htmlsaveoptions/worksheetscalable/) { get; set; } | Indicates if zooming in or out the html via worksheet zoom level when saving file to html, the default value is false. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlSaveOptionsDemo
    {
        public static void HtmlSaveOptionsExample()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // Create an instance of HtmlSaveOptions
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                IgnoreInvisibleShapes = true,
                PageTitle = "Sample HTML Page",
                AttachedFilesDirectory = "attached_files",
                AttachedFilesUrlPrefix = "http://example.com/files/",
                DefaultFontName = "Arial",
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
                CellCssPrefix = "",
                TableCssId = "",
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
                CssStyles = "body { padding: 5px }",
                HideOverflowWrappedText = false,
                IsBorderCollapsed = true,
                ClearData = false,
                CachedFileFolder = "cache",
                ValidateMergedAreas = true,
                MergeAreas = true,
                SortNames = true,
                SortExternalNames = true,
                RefreshChartCache = true,
                UpdateSmartArt = false
            };

            // Save the workbook as HTML
            workbook.Save("HtmlSaveOptionsExample.html", saveOptions);

            return;
        }
    }
}
```

### See Also

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


