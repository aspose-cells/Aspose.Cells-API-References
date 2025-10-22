##Aspose::Cells::Saving::EbookSaveOptions class
'Aspose::Cells::Saving::EbookSaveOptions class. Represents the options for saving ebook file in C++.'
## EbookSaveOptions class
Represents the options for saving ebook file.
```cpp
class EbookSaveOptions : public Aspose::Cells::HtmlSaveOptions
```
## Methods
| Method | Description |
| --- | --- |
| [EbookSaveOptions()](./ebooksaveoptions/) | Creates options for saving ebook file. |
| explicit [EbookSaveOptions(SaveFormat saveFormat)](./ebooksaveoptions/) | Creates options for saving ebook file. |
| [EbookSaveOptions(EbookSaveOptions_Impl* impl)](./ebooksaveoptions/) | Constructs from an implementation object. |
| [EbookSaveOptions(const EbookSaveOptions\& src)](./ebooksaveoptions/) | Copy constructor. |
| [EbookSaveOptions(const HtmlSaveOptions\& src)](./ebooksaveoptions/) | Constructs from a parent object. |
| [GetAddGenericFont()](../../aspose.cells/htmlsaveoptions/getaddgenericfont/) | Indicates whether to add a generic font to CSS font-family. The default value is true. |
| [GetAddTooltipText()](../../aspose.cells/htmlsaveoptions/getaddtooltiptext/) | Indicates whether adding tooltip text when the data can't be fully displayed. The default value is false. |
| [GetAttachedFilesDirectory()](../../aspose.cells/htmlsaveoptions/getattachedfilesdirectory/) | The directory that the attached files will be saved to. Only for saving to html stream. |
| [GetAttachedFilesUrlPrefix()](../../aspose.cells/htmlsaveoptions/getattachedfilesurlprefix/) | Specify the Url prefix of attached files such as image in the html file. Only for saving to html stream. |
| [GetCachedFileFolder()](../../aspose.cells/saveoptions/getcachedfilefolder/) | The folder for temporary files that may be used as data cache. |
| [GetCalculateFormula()](../../aspose.cells/htmlsaveoptions/getcalculateformula/) | Indicates whether to calculate formulas before saving html file. |
| [GetCellCssPrefix()](../../aspose.cells/htmlsaveoptions/getcellcssprefix/) | Gets and sets the prefix of the css name,the default value is "". |
| [GetCellNameAttribute()](../../aspose.cells/htmlsaveoptions/getcellnameattribute/) | Specifies the attribute that indicates the CellName to be written. (e.g. If the value is "id", then for cell "A1", the output will be:<td id='A1'>). The default value is null. |
| [GetCheckExcelRestriction()](../../aspose.cells/saveoptions/getcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated. |
| [GetClearData()](../../aspose.cells/saveoptions/getcleardata/) | Make the workbook empty after saving the file. |
| [GetCreateDirectory()](../../aspose.cells/saveoptions/getcreatedirectory/) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [GetCssStyles()](../../aspose.cells/htmlsaveoptions/getcssstyles/) | Gets or sets the additional css styles for the formatter. Only works when SaveAsSingleFile is True. |
| [GetDefaultFontName()](../../aspose.cells/htmlsaveoptions/getdefaultfontname/) | Specify the default font name for exporting html, the default font will be used when the font of style is not existing, If this property is null, [Aspose.Cells](../../aspose.cells/) will use universal font which have the same family with the original font, the default value is null. |
| [GetDisableCss()](../../aspose.cells/htmlsaveoptions/getdisablecss/) | Indicates whether only inline styles are applied, without relying on CSS. The default value is false. |
| [GetDisableDownlevelRevealedComments()](../../aspose.cells/htmlsaveoptions/getdisabledownlevelrevealedcomments/) | Indicates if disable Downlevel-revealed conditional comments when exporting file to html, the default value is false. |
| [GetEmbeddedFontType()](../../aspose.cells/htmlsaveoptions/getembeddedfonttype/) | Gets or sets the type of font that embedded in html. Default value is HtmlEmbeddedFontType.None which indicates that it will not embed font in html. |
| [GetEnableCssCustomProperties()](../../aspose.cells/htmlsaveoptions/getenablecsscustomproperties/) | Optimize the output of html by using CSS custom properties. For example, for the scenario that there are multiple occurences for one base64 image, with custom property the image data only needs to be saved once so the performance of the resultant html can be improved. The default value is false. |
| [GetEncodeEntityAsCode()](../../aspose.cells/htmlsaveoptions/getencodeentityascode/) | Indicates whether the html character entities are replaced with decimal code. (e.g. "&amp;nbsp;" is replaced with "&amp;#160;"). The default value is false. |
| [GetEncoding()](../../aspose.cells/htmlsaveoptions/getencoding/) | If not set,use Encoding.UTF8 as default enconding type. |
| [GetEncryptDocumentProperties()](../../aspose.cells/saveoptions/getencryptdocumentproperties/) | Indicates whether encrypt document properties when saving as .xls file. The default value is true. |
| [GetExcludeUnusedStyles()](../../aspose.cells/htmlsaveoptions/getexcludeunusedstyles/) | Indicating whether excludes unused styles. For the generated html files, excluding unused styles can make the file size smaller without affecting the visual effects. So the default value of this property is true. If user needs to keep all styles in the workbook for the generated html(such as the scenario that user needs to restore the workbook from the generated html later), please set this property as false. |
| [GetExportActiveWorksheetOnly()](../../aspose.cells/htmlsaveoptions/getexportactiveworksheetonly/) | Indicates if only exporting the active worksheet to html file. If true then only the active worksheet will be exported to html file; If false then the whole workbook will be exported to html file. The default value is false. |
| [GetExportArea()](../../aspose.cells/htmlsaveoptions/getexportarea/) | Gets or Sets the exporting [CellArea](../../aspose.cells/cellarea/) of current active [Worksheet](../../aspose.cells/worksheet/). If you set this attribute, the print area of current active [Worksheet](../../aspose.cells/worksheet/) will be omitted. Only the specified area will be exported when saving the file to html. |
| [GetExportBogusRowData()](../../aspose.cells/htmlsaveoptions/getexportbogusrowdata/) | Indicating whether exporting bogus bottom row data. The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [GetExportCellCoordinate()](../../aspose.cells/htmlsaveoptions/getexportcellcoordinate/) | Indicates whether exporting excel coordinate of nonblank cells when saving file to html. The default value is false. If you want to import the output html to excel, please keep the default value. |
| [GetExportCommentsType()](../../aspose.cells/htmlsaveoptions/getexportcommentstype/) | Represents type of exporting comments to html files. |
| [GetExportDataOptions()](../../aspose.cells/htmlsaveoptions/getexportdataoptions/) | Indicating the rule of exporting html file data.The default value is All. |
| [GetExportDocumentProperties()](../../aspose.cells/htmlsaveoptions/getexportdocumentproperties/) | Indicating whether exporting document properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [GetExportExtraHeadings()](../../aspose.cells/htmlsaveoptions/getexportextraheadings/) | Indicates whether exporting extra headings when the length of text is longer than max display column. The default value is false. If you want to import the html file to excel, please keep the default value. |
| [GetExportFormula()](../../aspose.cells/htmlsaveoptions/getexportformula/) | Indicates whether exporting formula when saving file to html. The default value is true. If you want to import the output html to excel, please keep the default value. |
| [GetExportFrameScriptsAndProperties()](../../aspose.cells/htmlsaveoptions/getexportframescriptsandproperties/) | Indicating whether exporting frame scripts and document properties. The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [GetExportGridLines()](../../aspose.cells/htmlsaveoptions/getexportgridlines/) | Indicating whether exporting the gridlines.The default value is false. |
| [GetExportHiddenWorksheet()](../../aspose.cells/htmlsaveoptions/getexporthiddenworksheet/) | Indicating if exporting the hidden worksheet content.The default value is true. |
| [GetExportImagesAsBase64()](../../aspose.cells/htmlsaveoptions/getexportimagesasbase64/) | Specifies whether images are saved in Base64 format to HTML, MHTML or EPUB. |
| [GetExportPageFooters()](../../aspose.cells/htmlsaveoptions/getexportpagefooters/) | Indicates whether exporting page headers. |
| [GetExportPageHeaders()](../../aspose.cells/htmlsaveoptions/getexportpageheaders/) | Indicates whether exporting page headers. |
| [GetExportPrintAreaOnly()](../../aspose.cells/htmlsaveoptions/getexportprintareaonly/) | Indicates if only exporting the print area to html file. The default value is false. |
| [GetExportRowColumnHeadings()](../../aspose.cells/htmlsaveoptions/getexportrowcolumnheadings/) | Indicates whether exports sheet's row and column headings when saving to HTML files. |
| [GetExportSimilarBorderStyle()](../../aspose.cells/htmlsaveoptions/getexportsimilarborderstyle/) | Indicating whether exporting the similar border style when the border style is not supported by browsers. If you want to import the html or mht file to excel, please keep the default value. The default value is false. |
| [GetExportSingleTab()](../../aspose.cells/htmlsaveoptions/getexportsingletab/) | Indicates whether exporting the single tab when the file only has one worksheet. The default value is false. |
| [GetExportWorkbookProperties()](../../aspose.cells/htmlsaveoptions/getexportworkbookproperties/) | Indicating whether exporting workbook properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [GetExportWorksheetCSSSeparately()](../../aspose.cells/htmlsaveoptions/getexportworksheetcssseparately/) | Indicating whether export the worksheet css separately.The default value is false. |
| [GetExportWorksheetProperties()](../../aspose.cells/htmlsaveoptions/getexportworksheetproperties/) | Indicating whether exporting worksheet properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [GetFilePathProvider()](../../aspose.cells/htmlsaveoptions/getfilepathprovider/) | Gets or sets the [IFilePathProvider](../../aspose.cells/ifilepathprovider/) for exporting [Worksheet](../../aspose.cells/worksheet/) to html separately. |
| [GetFormatDataIgnoreColumnWidth()](../../aspose.cells/htmlsaveoptions/getformatdataignorecolumnwidth/) | Indicating whether show the whole formatted data of cell when overflowing the column. If true then ignore the column width and the whole data of cell will be exported. If false then the data will be exported same as Excel. The default value is false. |
| [GetHiddenColDisplayType()](../../aspose.cells/htmlsaveoptions/gethiddencoldisplaytype/) | Hidden column(the width of this column is 0) in excel,before save this into html format, if HtmlHiddenColDisplayType is "Remove",the hidden column would not been output, if the value is "Hidden", the column would been output,but was hidden,the default value is "Hidden". |
| [GetHiddenRowDisplayType()](../../aspose.cells/htmlsaveoptions/gethiddenrowdisplaytype/) | Hidden row(the height of this row is 0) in excel,before save this into html format, if HtmlHiddenRowDisplayType is "Remove",the hidden row would not been output, if the value is "Hidden", the row would been output,but was hidden,the default value is "Hidden". |
| [GetHideOverflowWrappedText()](../../aspose.cells/htmlsaveoptions/gethideoverflowwrappedtext/) | Indicates whether to hide overflow text when the cell format is set to wrap text. The default value is false. |
| [GetHtmlCrossStringType()](../../aspose.cells/htmlsaveoptions/gethtmlcrossstringtype/) | Indicates if a cross-cell string will be displayed in the same way as MS Excel when saving an Excel file in html format. By default the value is Default, so, for cross-cell strings, there is little difference between the html files created by [Aspose.Cells](../../aspose.cells/) and MS Excel. But the performance for creating large html files,setting the value to Cross would be several times faster than setting it to Default or Fit2Cell. |
| [GetHtmlVersion()](../../aspose.cells/htmlsaveoptions/gethtmlversion/) | Specifies version of HTML standard that should be used when saving the HTML format. Default value is [HtmlVersion.Default](../../aspose.cells/htmlversion/). |
| [GetIgnoreInvisibleShapes()](../../aspose.cells/htmlsaveoptions/getignoreinvisibleshapes/) | Indicate whether exporting those not visible shapes. |
| [GetImageOptions()](../../aspose.cells/htmlsaveoptions/getimageoptions/) | Get the ImageOrPrintOptions object before exporting. |
| [GetImageScalable()](../../aspose.cells/htmlsaveoptions/getimagescalable/) | Indicates whether using scalable unit to describe the image width when using scalable unit to describe the column width. The default value is true. |
| [GetLinkTargetType()](../../aspose.cells/htmlsaveoptions/getlinktargettype/) | Indicating the type of target attribute in **<a>** link. The default value is [HtmlLinkTargetType.Parent](../../aspose.cells/htmllinktargettype/). |
| [GetMergeAreas()](../../aspose.cells/saveoptions/getmergeareas/) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [GetMergeEmptyTdForcely()](../../aspose.cells/htmlsaveoptions/getmergeemptytdforcely/) |  **(Deprecated)** Indicates whether merging empty TD element forcedly when exporting file to html. The size of html file will be reduced significantly after setting value to true. The default value is false. If you want to import the html file to excel or export perfect grid lines when saving file to html, please keep the default value. |
| [GetMergeEmptyTdType()](../../aspose.cells/htmlsaveoptions/getmergeemptytdtype/) | The option to merge contiguous empty cells(empty td elements) The default value is [MergeEmptyTdType.Default](../../aspose.cells/mergeemptytdtype/). |
| [GetOfficeMathOutputMode()](../../aspose.cells/htmlsaveoptions/getofficemathoutputmode/) | Indicates how export OfficeMath objects to HTML, Default value is Image. |
| [GetPageTitle()](../../aspose.cells/htmlsaveoptions/getpagetitle/) | The title of the html page. Only for saving to html stream. |
| [GetParseHtmlTagInCell()](../../aspose.cells/htmlsaveoptions/getparsehtmltagincell/) | Indicates whether html tag(such as **<div></div>**) in cell should be parsed as cell value or preserved as it is. The default value is true. |
| [GetPresentationPreference()](../../aspose.cells/htmlsaveoptions/getpresentationpreference/) | Indicating if html or mht file is presentation preference. The default value is false. if you want to get more beautiful presentation,please set the value to true. |
| [GetRefreshChartCache()](../../aspose.cells/saveoptions/getrefreshchartcache/) | Indicates whether refreshing chart cache data. |
| [GetSaveAsSingleFile()](../../aspose.cells/htmlsaveoptions/getsaveassinglefile/) | Indicates whether save the html as single file. The default value is false. |
| [GetSaveFormat()](../../aspose.cells/saveoptions/getsaveformat/) | Gets the save file format. |
| [GetSheetSet()](../../aspose.cells/htmlsaveoptions/getsheetset/) | Gets or sets the sheets to render. Default is all visible sheets in the workbook: Aspose.Cells.Rendering.SheetSet.Visible. |
| [GetShowAllSheets()](../../aspose.cells/htmlsaveoptions/getshowallsheets/) | Indicates whether showing all sheets when saving as a single html file. |
| [GetSortExternalNames()](../../aspose.cells/saveoptions/getsortexternalnames/) | Indicates whether sorting external defined names before saving file. |
| [GetSortNames()](../../aspose.cells/saveoptions/getsortnames/) | Indicates whether sorting defined names before saving file. |
| [GetTableCssId()](../../aspose.cells/htmlsaveoptions/gettablecssid/) | Gets and sets the prefix of the type css name such as tr,col,td and so on, they are contained in the table element which has the specific TableCssId attribute. The default value is "". |
| [GetUpdateSmartArt()](../../aspose.cells/saveoptions/getupdatesmartart/) | Indicates whether updating smart art setting. The default value is false. |
| [GetValidateMergedAreas()](../../aspose.cells/saveoptions/getvalidatemergedareas/) | Indicates whether validate merged cells before saving the file. |
| [GetWarningCallback()](../../aspose.cells/saveoptions/getwarningcallback/) | Gets or sets warning callback. |
| [GetWidthScalable()](../../aspose.cells/htmlsaveoptions/getwidthscalable/) | Indicates whether exporting column width in unit of scale to html. The default value is false. |
| [GetWorksheetScalable()](../../aspose.cells/htmlsaveoptions/getworksheetscalable/) | Indicates if zooming in or out the html via worksheet zoom level when saving file to html, the default value is false. |
| [HtmlSaveOptions()](../../aspose.cells/htmlsaveoptions/htmlsaveoptions/) | Creates options for saving html file. |
| explicit [HtmlSaveOptions(SaveFormat saveFormat)](../../aspose.cells/htmlsaveoptions/htmlsaveoptions/) | Creates options for saving htm file. |
| [HtmlSaveOptions(HtmlSaveOptions_Impl* impl)](../../aspose.cells/htmlsaveoptions/htmlsaveoptions/) | Constructs from an implementation object. |
| [HtmlSaveOptions(const HtmlSaveOptions\& src)](../../aspose.cells/htmlsaveoptions/htmlsaveoptions/) | Copy constructor. |
| [HtmlSaveOptions(const SaveOptions\& src)](../../aspose.cells/htmlsaveoptions/htmlsaveoptions/) | Constructs from a parent object. |
| [IsBorderCollapsed()](../../aspose.cells/htmlsaveoptions/isbordercollapsed/) | Indicates whether the table borders are collapsed. The default value is true. |
| [IsExpImageToTempDir()](../../aspose.cells/htmlsaveoptions/isexpimagetotempdir/) | Indicates whether exporting image files to temp directory. Only for saving to html stream. |
| [IsExportComments()](../../aspose.cells/htmlsaveoptions/isexportcomments/) | Indicates if exporting comments when saving file to html, the default value is false. |
| [IsFullPathLink()](../../aspose.cells/htmlsaveoptions/isfullpathlink/) | Indicating whether using full path link in sheet00x.htm,filelist.xml and tabstrip.htm. The default value is false. |
| [IsIECompatible()](../../aspose.cells/htmlsaveoptions/isiecompatible/) | Indicating whether the output HTML is compatible with IE browser. The defalut value is false. |
| [IsJsBrowserCompatible()](../../aspose.cells/htmlsaveoptions/isjsbrowsercompatible/) | Indicates whether JavaScript is compatible with browsers that do not support JavaScript. The default value is true. |
| [IsMobileCompatible()](../../aspose.cells/htmlsaveoptions/ismobilecompatible/) | Indicates whether the output HTML is compatible with mobile devices. The default value is false. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const EbookSaveOptions\& src)](./operator_asm/) | operator= |
| [operator=(const HtmlSaveOptions\& src)](../../aspose.cells/htmlsaveoptions/operator_asm/) | operator= |
| [operator=(const SaveOptions\& src)](../../aspose.cells/saveoptions/operator_asm/) | operator= |
| [SaveOptions(SaveOptions_Impl* impl)](../../aspose.cells/saveoptions/saveoptions/) | Constructs from an implementation object. |
| [SaveOptions(const SaveOptions\& src)](../../aspose.cells/saveoptions/saveoptions/) | Copy constructor. |
| [SetAddGenericFont(bool value)](../../aspose.cells/htmlsaveoptions/setaddgenericfont/) | Indicates whether to add a generic font to CSS font-family. The default value is true. |
| [SetAddTooltipText(bool value)](../../aspose.cells/htmlsaveoptions/setaddtooltiptext/) | Indicates whether adding tooltip text when the data can't be fully displayed. The default value is false. |
| [SetAttachedFilesDirectory(const U16String\& value)](../../aspose.cells/htmlsaveoptions/setattachedfilesdirectory/) | The directory that the attached files will be saved to. Only for saving to html stream. |
| [SetAttachedFilesDirectory(const char16_t* value)](../../aspose.cells/htmlsaveoptions/setattachedfilesdirectory/) | The directory that the attached files will be saved to. Only for saving to html stream. |
| [SetAttachedFilesUrlPrefix(const U16String\& value)](../../aspose.cells/htmlsaveoptions/setattachedfilesurlprefix/) | Specify the Url prefix of attached files such as image in the html file. Only for saving to html stream. |
| [SetAttachedFilesUrlPrefix(const char16_t* value)](../../aspose.cells/htmlsaveoptions/setattachedfilesurlprefix/) | Specify the Url prefix of attached files such as image in the html file. Only for saving to html stream. |
| [SetCachedFileFolder(const U16String\& value)](../../aspose.cells/saveoptions/setcachedfilefolder/) | The folder for temporary files that may be used as data cache. |
| [SetCachedFileFolder(const char16_t* value)](../../aspose.cells/saveoptions/setcachedfilefolder/) | The folder for temporary files that may be used as data cache. |
| [SetCalculateFormula(bool value)](../../aspose.cells/htmlsaveoptions/setcalculateformula/) | Indicates whether to calculate formulas before saving html file. |
| [SetCellCssPrefix(const U16String\& value)](../../aspose.cells/htmlsaveoptions/setcellcssprefix/) | Gets and sets the prefix of the css name,the default value is "". |
| [SetCellCssPrefix(const char16_t* value)](../../aspose.cells/htmlsaveoptions/setcellcssprefix/) | Gets and sets the prefix of the css name,the default value is "". |
| [SetCellNameAttribute(const U16String\& value)](../../aspose.cells/htmlsaveoptions/setcellnameattribute/) | Specifies the attribute that indicates the CellName to be written. (e.g. If the value is "id", then for cell "A1", the output will be:<td id='A1'>). The default value is null. |
| [SetCellNameAttribute(const char16_t* value)](../../aspose.cells/htmlsaveoptions/setcellnameattribute/) | Specifies the attribute that indicates the CellName to be written. (e.g. If the value is "id", then for cell "A1", the output will be:<td id='A1'>). The default value is null. |
| [SetCheckExcelRestriction(bool value)](../../aspose.cells/saveoptions/setcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated. |
| [SetClearData(bool value)](../../aspose.cells/saveoptions/setcleardata/) | Make the workbook empty after saving the file. |
| [SetCreateDirectory(bool value)](../../aspose.cells/saveoptions/setcreatedirectory/) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [SetCssStyles(const U16String\& value)](../../aspose.cells/htmlsaveoptions/setcssstyles/) | Gets or sets the additional css styles for the formatter. Only works when SaveAsSingleFile is True. |
| [SetCssStyles(const char16_t* value)](../../aspose.cells/htmlsaveoptions/setcssstyles/) | Gets or sets the additional css styles for the formatter. Only works when SaveAsSingleFile is True. |
| [SetDefaultFontName(const U16String\& value)](../../aspose.cells/htmlsaveoptions/setdefaultfontname/) | Specify the default font name for exporting html, the default font will be used when the font of style is not existing, If this property is null, [Aspose.Cells](../../aspose.cells/) will use universal font which have the same family with the original font, the default value is null. |
| [SetDefaultFontName(const char16_t* value)](../../aspose.cells/htmlsaveoptions/setdefaultfontname/) | Specify the default font name for exporting html, the default font will be used when the font of style is not existing, If this property is null, [Aspose.Cells](../../aspose.cells/) will use universal font which have the same family with the original font, the default value is null. |
| [SetDisableCss(bool value)](../../aspose.cells/htmlsaveoptions/setdisablecss/) | Indicates whether only inline styles are applied, without relying on CSS. The default value is false. |
| [SetDisableDownlevelRevealedComments(bool value)](../../aspose.cells/htmlsaveoptions/setdisabledownlevelrevealedcomments/) | Indicates if disable Downlevel-revealed conditional comments when exporting file to html, the default value is false. |
| [SetEmbeddedFontType(HtmlEmbeddedFontType value)](../../aspose.cells/htmlsaveoptions/setembeddedfonttype/) | Gets or sets the type of font that embedded in html. Default value is HtmlEmbeddedFontType.None which indicates that it will not embed font in html. |
| [SetEnableCssCustomProperties(bool value)](../../aspose.cells/htmlsaveoptions/setenablecsscustomproperties/) | Optimize the output of html by using CSS custom properties. For example, for the scenario that there are multiple occurences for one base64 image, with custom property the image data only needs to be saved once so the performance of the resultant html can be improved. The default value is false. |
| [SetEncodeEntityAsCode(bool value)](../../aspose.cells/htmlsaveoptions/setencodeentityascode/) | Indicates whether the html character entities are replaced with decimal code. (e.g. "&amp;nbsp;" is replaced with "&amp;#160;"). The default value is false. |
| [SetEncoding(EncodingType value)](../../aspose.cells/htmlsaveoptions/setencoding/) | If not set,use Encoding.UTF8 as default enconding type. |
| [SetEncryptDocumentProperties(bool value)](../../aspose.cells/saveoptions/setencryptdocumentproperties/) | Indicates whether encrypt document properties when saving as .xls file. The default value is true. |
| [SetExcludeUnusedStyles(bool value)](../../aspose.cells/htmlsaveoptions/setexcludeunusedstyles/) | Indicating whether excludes unused styles. For the generated html files, excluding unused styles can make the file size smaller without affecting the visual effects. So the default value of this property is true. If user needs to keep all styles in the workbook for the generated html(such as the scenario that user needs to restore the workbook from the generated html later), please set this property as false. |
| [SetExportActiveWorksheetOnly(bool value)](../../aspose.cells/htmlsaveoptions/setexportactiveworksheetonly/) | Indicates if only exporting the active worksheet to html file. If true then only the active worksheet will be exported to html file; If false then the whole workbook will be exported to html file. The default value is false. |
| [SetExportArea(const CellArea\& value)](../../aspose.cells/htmlsaveoptions/setexportarea/) | Gets or Sets the exporting [CellArea](../../aspose.cells/cellarea/) of current active [Worksheet](../../aspose.cells/worksheet/). If you set this attribute, the print area of current active [Worksheet](../../aspose.cells/worksheet/) will be omitted. Only the specified area will be exported when saving the file to html. |
| [SetExportBogusRowData(bool value)](../../aspose.cells/htmlsaveoptions/setexportbogusrowdata/) | Indicating whether exporting bogus bottom row data. The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [SetExportCellCoordinate(bool value)](../../aspose.cells/htmlsaveoptions/setexportcellcoordinate/) | Indicates whether exporting excel coordinate of nonblank cells when saving file to html. The default value is false. If you want to import the output html to excel, please keep the default value. |
| [SetExportCommentsType(PrintCommentsType value)](../../aspose.cells/htmlsaveoptions/setexportcommentstype/) | Represents type of exporting comments to html files. |
| [SetExportDataOptions(HtmlExportDataOptions value)](../../aspose.cells/htmlsaveoptions/setexportdataoptions/) | Indicating the rule of exporting html file data.The default value is All. |
| [SetExportDocumentProperties(bool value)](../../aspose.cells/htmlsaveoptions/setexportdocumentproperties/) | Indicating whether exporting document properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [SetExportExtraHeadings(bool value)](../../aspose.cells/htmlsaveoptions/setexportextraheadings/) | Indicates whether exporting extra headings when the length of text is longer than max display column. The default value is false. If you want to import the html file to excel, please keep the default value. |
| [SetExportFormula(bool value)](../../aspose.cells/htmlsaveoptions/setexportformula/) | Indicates whether exporting formula when saving file to html. The default value is true. If you want to import the output html to excel, please keep the default value. |
| [SetExportFrameScriptsAndProperties(bool value)](../../aspose.cells/htmlsaveoptions/setexportframescriptsandproperties/) | Indicating whether exporting frame scripts and document properties. The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [SetExportGridLines(bool value)](../../aspose.cells/htmlsaveoptions/setexportgridlines/) | Indicating whether exporting the gridlines.The default value is false. |
| [SetExportHiddenWorksheet(bool value)](../../aspose.cells/htmlsaveoptions/setexporthiddenworksheet/) | Indicating if exporting the hidden worksheet content.The default value is true. |
| [SetExportImagesAsBase64(bool value)](../../aspose.cells/htmlsaveoptions/setexportimagesasbase64/) | Specifies whether images are saved in Base64 format to HTML, MHTML or EPUB. |
| [SetExportPageFooters(bool value)](../../aspose.cells/htmlsaveoptions/setexportpagefooters/) | Indicates whether exporting page headers. |
| [SetExportPageHeaders(bool value)](../../aspose.cells/htmlsaveoptions/setexportpageheaders/) | Indicates whether exporting page headers. |
| [SetExportPrintAreaOnly(bool value)](../../aspose.cells/htmlsaveoptions/setexportprintareaonly/) | Indicates if only exporting the print area to html file. The default value is false. |
| [SetExportRowColumnHeadings(bool value)](../../aspose.cells/htmlsaveoptions/setexportrowcolumnheadings/) | Indicates whether exports sheet's row and column headings when saving to HTML files. |
| [SetExportSimilarBorderStyle(bool value)](../../aspose.cells/htmlsaveoptions/setexportsimilarborderstyle/) | Indicating whether exporting the similar border style when the border style is not supported by browsers. If you want to import the html or mht file to excel, please keep the default value. The default value is false. |
| [SetExportSingleTab(bool value)](../../aspose.cells/htmlsaveoptions/setexportsingletab/) | Indicates whether exporting the single tab when the file only has one worksheet. The default value is false. |
| [SetExportWorkbookProperties(bool value)](../../aspose.cells/htmlsaveoptions/setexportworkbookproperties/) | Indicating whether exporting workbook properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [SetExportWorksheetCSSSeparately(bool value)](../../aspose.cells/htmlsaveoptions/setexportworksheetcssseparately/) | Indicating whether export the worksheet css separately.The default value is false. |
| [SetExportWorksheetProperties(bool value)](../../aspose.cells/htmlsaveoptions/setexportworksheetproperties/) | Indicating whether exporting worksheet properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [SetFilePathProvider(IFilePathProvider* value)](../../aspose.cells/htmlsaveoptions/setfilepathprovider/) | Gets or sets the [IFilePathProvider](../../aspose.cells/ifilepathprovider/) for exporting [Worksheet](../../aspose.cells/worksheet/) to html separately. |
| [SetFormatDataIgnoreColumnWidth(bool value)](../../aspose.cells/htmlsaveoptions/setformatdataignorecolumnwidth/) | Indicating whether show the whole formatted data of cell when overflowing the column. If true then ignore the column width and the whole data of cell will be exported. If false then the data will be exported same as Excel. The default value is false. |
| [SetHiddenColDisplayType(HtmlHiddenColDisplayType value)](../../aspose.cells/htmlsaveoptions/sethiddencoldisplaytype/) | Hidden column(the width of this column is 0) in excel,before save this into html format, if HtmlHiddenColDisplayType is "Remove",the hidden column would not been output, if the value is "Hidden", the column would been output,but was hidden,the default value is "Hidden". |
| [SetHiddenRowDisplayType(HtmlHiddenRowDisplayType value)](../../aspose.cells/htmlsaveoptions/sethiddenrowdisplaytype/) | Hidden row(the height of this row is 0) in excel,before save this into html format, if HtmlHiddenRowDisplayType is "Remove",the hidden row would not been output, if the value is "Hidden", the row would been output,but was hidden,the default value is "Hidden". |
| [SetHideOverflowWrappedText(bool value)](../../aspose.cells/htmlsaveoptions/sethideoverflowwrappedtext/) | Indicates whether to hide overflow text when the cell format is set to wrap text. The default value is false. |
| [SetHtmlCrossStringType(HtmlCrossType value)](../../aspose.cells/htmlsaveoptions/sethtmlcrossstringtype/) | Indicates if a cross-cell string will be displayed in the same way as MS Excel when saving an Excel file in html format. By default the value is Default, so, for cross-cell strings, there is little difference between the html files created by [Aspose.Cells](../../aspose.cells/) and MS Excel. But the performance for creating large html files,setting the value to Cross would be several times faster than setting it to Default or Fit2Cell. |
| [SetHtmlVersion(HtmlVersion value)](../../aspose.cells/htmlsaveoptions/sethtmlversion/) | Specifies version of HTML standard that should be used when saving the HTML format. Default value is [HtmlVersion.Default](../../aspose.cells/htmlversion/). |
| [SetIgnoreInvisibleShapes(bool value)](../../aspose.cells/htmlsaveoptions/setignoreinvisibleshapes/) | Indicate whether exporting those not visible shapes. |
| [SetImageScalable(bool value)](../../aspose.cells/htmlsaveoptions/setimagescalable/) | Indicates whether using scalable unit to describe the image width when using scalable unit to describe the column width. The default value is true. |
| [SetIsBorderCollapsed(bool value)](../../aspose.cells/htmlsaveoptions/setisbordercollapsed/) | Indicates whether the table borders are collapsed. The default value is true. |
| [SetIsExpImageToTempDir(bool value)](../../aspose.cells/htmlsaveoptions/setisexpimagetotempdir/) | Indicates whether exporting image files to temp directory. Only for saving to html stream. |
| [SetIsExportComments(bool value)](../../aspose.cells/htmlsaveoptions/setisexportcomments/) | Indicates if exporting comments when saving file to html, the default value is false. |
| [SetIsFullPathLink(bool value)](../../aspose.cells/htmlsaveoptions/setisfullpathlink/) | Indicating whether using full path link in sheet00x.htm,filelist.xml and tabstrip.htm. The default value is false. |
| [SetIsIECompatible(bool value)](../../aspose.cells/htmlsaveoptions/setisiecompatible/) | Indicating whether the output HTML is compatible with IE browser. The defalut value is false. |
| [SetIsJsBrowserCompatible(bool value)](../../aspose.cells/htmlsaveoptions/setisjsbrowsercompatible/) | Indicates whether JavaScript is compatible with browsers that do not support JavaScript. The default value is true. |
| [SetIsMobileCompatible(bool value)](../../aspose.cells/htmlsaveoptions/setismobilecompatible/) | Indicates whether the output HTML is compatible with mobile devices. The default value is false. |
| [SetLinkTargetType(HtmlLinkTargetType value)](../../aspose.cells/htmlsaveoptions/setlinktargettype/) | Indicating the type of target attribute in **<a>** link. The default value is [HtmlLinkTargetType.Parent](../../aspose.cells/htmllinktargettype/). |
| [SetMergeAreas(bool value)](../../aspose.cells/saveoptions/setmergeareas/) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [SetMergeEmptyTdForcely(bool value)](../../aspose.cells/htmlsaveoptions/setmergeemptytdforcely/) |  **(Deprecated)** Indicates whether merging empty TD element forcedly when exporting file to html. The size of html file will be reduced significantly after setting value to true. The default value is false. If you want to import the html file to excel or export perfect grid lines when saving file to html, please keep the default value. |
| [SetMergeEmptyTdType(MergeEmptyTdType value)](../../aspose.cells/htmlsaveoptions/setmergeemptytdtype/) | The option to merge contiguous empty cells(empty td elements) The default value is [MergeEmptyTdType.Default](../../aspose.cells/mergeemptytdtype/). |
| [SetOfficeMathOutputMode(HtmlOfficeMathOutputType value)](../../aspose.cells/htmlsaveoptions/setofficemathoutputmode/) | Indicates how export OfficeMath objects to HTML, Default value is Image. |
| [SetPageTitle(const U16String\& value)](../../aspose.cells/htmlsaveoptions/setpagetitle/) | The title of the html page. Only for saving to html stream. |
| [SetPageTitle(const char16_t* value)](../../aspose.cells/htmlsaveoptions/setpagetitle/) | The title of the html page. Only for saving to html stream. |
| [SetParseHtmlTagInCell(bool value)](../../aspose.cells/htmlsaveoptions/setparsehtmltagincell/) | Indicates whether html tag(such as **<div></div>**) in cell should be parsed as cell value or preserved as it is. The default value is true. |
| [SetPresentationPreference(bool value)](../../aspose.cells/htmlsaveoptions/setpresentationpreference/) | Indicating if html or mht file is presentation preference. The default value is false. if you want to get more beautiful presentation,please set the value to true. |
| [SetRefreshChartCache(bool value)](../../aspose.cells/saveoptions/setrefreshchartcache/) | Indicates whether refreshing chart cache data. |
| [SetSaveAsSingleFile(bool value)](../../aspose.cells/htmlsaveoptions/setsaveassinglefile/) | Indicates whether save the html as single file. The default value is false. |
| [SetSheetSet(const SheetSet\& value)](../../aspose.cells/htmlsaveoptions/setsheetset/) | Gets or sets the sheets to render. Default is all visible sheets in the workbook: Aspose.Cells.Rendering.SheetSet.Visible. |
| [SetShowAllSheets(bool value)](../../aspose.cells/htmlsaveoptions/setshowallsheets/) | Indicates whether showing all sheets when saving as a single html file. |
| [SetSortExternalNames(bool value)](../../aspose.cells/saveoptions/setsortexternalnames/) | Indicates whether sorting external defined names before saving file. |
| [SetSortNames(bool value)](../../aspose.cells/saveoptions/setsortnames/) | Indicates whether sorting defined names before saving file. |
| [SetTableCssId(const U16String\& value)](../../aspose.cells/htmlsaveoptions/settablecssid/) | Gets and sets the prefix of the type css name such as tr,col,td and so on, they are contained in the table element which has the specific TableCssId attribute. The default value is "". |
| [SetTableCssId(const char16_t* value)](../../aspose.cells/htmlsaveoptions/settablecssid/) | Gets and sets the prefix of the type css name such as tr,col,td and so on, they are contained in the table element which has the specific TableCssId attribute. The default value is "". |
| [SetUpdateSmartArt(bool value)](../../aspose.cells/saveoptions/setupdatesmartart/) | Indicates whether updating smart art setting. The default value is false. |
| [SetValidateMergedAreas(bool value)](../../aspose.cells/saveoptions/setvalidatemergedareas/) | Indicates whether validate merged cells before saving the file. |
| [SetWarningCallback(IWarningCallback* value)](../../aspose.cells/saveoptions/setwarningcallback/) | Gets or sets warning callback. |
| [SetWidthScalable(bool value)](../../aspose.cells/htmlsaveoptions/setwidthscalable/) | Indicates whether exporting column width in unit of scale to html. The default value is false. |
| [SetWorksheetScalable(bool value)](../../aspose.cells/htmlsaveoptions/setworksheetscalable/) | Indicates if zooming in or out the html via worksheet zoom level when saving file to html, the default value is false. |
| [~EbookSaveOptions()](./~ebooksaveoptions/) | Destructor. |
| [~HtmlSaveOptions()](../../aspose.cells/htmlsaveoptions/~htmlsaveoptions/) | Destructor. |
| [~SaveOptions()](../../aspose.cells/saveoptions/~saveoptions/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Class [HtmlSaveOptions](../../aspose.cells/htmlsaveoptions/)
* Namespace [Aspose::Cells::Saving](../)
* Library [Aspose.Cells for C++](../../)
