---
title: Aspose::Cells::HtmlSaveOptions class
linktitle: HtmlSaveOptions
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::HtmlSaveOptions class. Represents the options for saving html file in C++.'
type: docs
weight: 8100
url: /cpp/aspose.cells/htmlsaveoptions/
---
## HtmlSaveOptions class


Represents the options for saving html file.

```cpp
class HtmlSaveOptions : public Aspose::Cells::SaveOptions
```

## Methods

| Method | Description |
| --- | --- |
| [GetAddGenericFont()](./getaddgenericfont/) | Indicates whether to add a generic font to CSS font-family. The default value is true. |
| [GetAddTooltipText()](./getaddtooltiptext/) | Indicates whether adding tooltip text when the data can't be fully displayed. The default value is false. |
| [GetAttachedFilesDirectory()](./getattachedfilesdirectory/) | The directory that the attached files will be saved to. Only for saving to html stream. |
| [GetAttachedFilesUrlPrefix()](./getattachedfilesurlprefix/) | Specify the Url prefix of attached files such as image in the html file. Only for saving to html stream. |
| [GetCachedFileFolder()](../saveoptions/getcachedfilefolder/) | The folder for temporary files that may be used as data cache. |
| [GetCalculateFormula()](./getcalculateformula/) | Indicates whether to calculate formulas before saving html file. |
| [GetCellCssPrefix()](./getcellcssprefix/) | Gets and sets the prefix of the css name,the default value is "". |
| [GetCellNameAttribute()](./getcellnameattribute/) | Specifies the attribute that indicates the CellName to be written. (e.g. If the value is "id", then for cell "A1", the output will be:<td id='A1'>). The default value is null. |
| [GetCheckExcelRestriction()](../saveoptions/getcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated. |
| [GetClearData()](../saveoptions/getcleardata/) | Make the workbook empty after saving the file. |
| [GetCreateDirectory()](../saveoptions/getcreatedirectory/) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [GetCssStyles()](./getcssstyles/) | Gets or sets the additional css styles for the formatter. Only works when SaveAsSingleFile is True. |
| [GetDataBarRenderMode()](./getdatabarrendermode/) | Represents the mode of how to render [DataBar](../databar/) when converting Excel files to html files. Default value is DataBarRenderMode.BackgroundColor. |
| [GetDefaultFontName()](./getdefaultfontname/) | Specify the default font name for exporting html, the default font will be used when the font of style is not existing, If this property is null, [Aspose.Cells](../) will use universal font which have the same family with the original font, the default value is null. |
| [GetDisableCss()](./getdisablecss/) | Indicates whether only inline styles are applied, without relying on CSS. The default value is false. |
| [GetDisableDownlevelRevealedComments()](./getdisabledownlevelrevealedcomments/) | Indicates if disable Downlevel-revealed conditional comments when exporting file to html, the default value is false. |
| [GetEmbeddedFontType()](./getembeddedfonttype/) | Gets or sets the type of embedding font file into html file. Default value is HtmlEmbeddedFontType.None which indicates that no font will be embedded in html. |
| [GetEnableCssCustomProperties()](./getenablecsscustomproperties/) | Optimize the output of html by using CSS custom properties. For example, for the scenario that there are multiple occurences for one base64 image, with custom property the image data only needs to be saved once so the performance of the resultant html can be improved. The default value is false. |
| [GetEncodeEntityAsCode()](./getencodeentityascode/) | Indicates whether the html character entities are replaced with decimal code. (e.g. "&amp;nbsp;" is replaced with "&amp;#160;"). The default value is false. |
| [GetEncoding()](./getencoding/) | If not set,use Encoding.UTF8 as default enconding type. |
| [GetEncryptDocumentProperties()](../saveoptions/getencryptdocumentproperties/) | Indicates whether encrypt document properties when saving as .xls file. The default value is true. |
| [GetExcludeUnusedStyles()](./getexcludeunusedstyles/) | Indicating whether excludes unused styles. For the generated html files, excluding unused styles can make the file size smaller without affecting the visual effects. So the default value of this property is true. If user needs to keep all styles in the workbook for the generated html(such as the scenario that user needs to restore the workbook from the generated html later), please set this property as false. |
| [GetExportActiveWorksheetOnly()](./getexportactiveworksheetonly/) | Indicates if only exporting the active worksheet to html file. If true then only the active worksheet will be exported to html file; If false then the whole workbook will be exported to html file. The default value is false. |
| [GetExportArea()](./getexportarea/) | Gets or Sets the exporting [CellArea](../cellarea/) of current active [Worksheet](../worksheet/). If you set this attribute, the print area of current active [Worksheet](../worksheet/) will be omitted. Only the specified area will be exported when saving the file to html. |
| [GetExportBogusRowData()](./getexportbogusrowdata/) | Indicating whether exporting bogus bottom row data. The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [GetExportCellCoordinate()](./getexportcellcoordinate/) | Indicates whether exporting excel coordinate of nonblank cells when saving file to html. The default value is false. If you want to import the output html to excel, please keep the default value. |
| [GetExportCommentsType()](./getexportcommentstype/) | Represents type of exporting comments to html files. |
| [GetExportDataOptions()](./getexportdataoptions/) | Indicating the rule of exporting html file data.The default value is All. |
| [GetExportDocumentProperties()](./getexportdocumentproperties/) | Indicating whether exporting document properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [GetExportExtraHeadings()](./getexportextraheadings/) | Indicates whether exporting extra headings when the length of text is longer than max display column. The default value is false. If you want to import the html file to excel, please keep the default value. |
| [GetExportFormula()](./getexportformula/) | Indicates whether exporting formula when saving file to html. The default value is true. If you want to import the output html to excel, please keep the default value. |
| [GetExportFrameScriptsAndProperties()](./getexportframescriptsandproperties/) | Indicating whether exporting frame scripts and document properties. The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [GetExportGridLines()](./getexportgridlines/) | Indicating whether exporting the gridlines.The default value is false. |
| [GetExportHiddenWorksheet()](./getexporthiddenworksheet/) | Indicating if exporting the hidden worksheet content.The default value is true. |
| [GetExportImagesAsBase64()](./getexportimagesasbase64/) | Specifies whether images are saved in Base64 format to HTML, MHTML or EPUB. |
| [GetExportNamedRangeAnchors()](./getexportnamedrangeanchors/) | Indicates whether to export anchor elements for named ranges when saving as HTML. Default value is true. |
| [GetExportPageFooters()](./getexportpagefooters/) | Indicates whether exporting page headers. |
| [GetExportPageHeaders()](./getexportpageheaders/) | Indicates whether exporting page headers. |
| [GetExportPrintAreaOnly()](./getexportprintareaonly/) | Indicates if only exporting the print area to html file. The default value is false. |
| [GetExportRowColumnHeadings()](./getexportrowcolumnheadings/) | Indicates whether exports sheet's row and column headings when saving to HTML files. |
| [GetExportSimilarBorderStyle()](./getexportsimilarborderstyle/) | Indicating whether exporting the similar border style when the border style is not supported by browsers. If you want to import the html or mht file to excel, please keep the default value. The default value is false. |
| [GetExportSingleTab()](./getexportsingletab/) | Indicates whether exporting the single tab when the file only has one worksheet. The default value is false. |
| [GetExportWorkbookProperties()](./getexportworkbookproperties/) | Indicating whether exporting workbook properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [GetExportWorksheetCSSSeparately()](./getexportworksheetcssseparately/) | Indicating whether export the worksheet css separately.The default value is false. |
| [GetExportWorksheetProperties()](./getexportworksheetproperties/) | Indicating whether exporting worksheet properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [GetFilePathProvider()](./getfilepathprovider/) | Gets or sets the [IFilePathProvider](../ifilepathprovider/) for exporting [Worksheet](../worksheet/) to html separately. |
| [GetFormatDataIgnoreColumnWidth()](./getformatdataignorecolumnwidth/) | Indicating whether show the whole formatted data of cell when overflowing the column. If true then ignore the column width and the whole data of cell will be exported. If false then the data will be exported same as Excel. The default value is false. |
| [GetHiddenColDisplayType()](./gethiddencoldisplaytype/) | Hidden column(the width of this column is 0) in excel,before save this into html format, if HtmlHiddenColDisplayType is "Remove",the hidden column would not been output, if the value is "Hidden", the column would been output,but was hidden,the default value is "Hidden". |
| [GetHiddenRowDisplayType()](./gethiddenrowdisplaytype/) | Hidden row(the height of this row is 0) in excel,before save this into html format, if HtmlHiddenRowDisplayType is "Remove",the hidden row would not been output, if the value is "Hidden", the row would been output,but was hidden,the default value is "Hidden". |
| [GetHideOverflowWrappedText()](./gethideoverflowwrappedtext/) | Indicates whether to hide overflow text when the cell format is set to wrap text. The default value is false. |
| [GetHtmlCrossStringType()](./gethtmlcrossstringtype/) | Indicates if a cross-cell string will be displayed in the same way as MS Excel when saving an Excel file in html format. By default the value is Default, so, for cross-cell strings, there is little difference between the html files created by [Aspose.Cells](../) and MS Excel. But the performance for creating large html files,setting the value to Cross would be several times faster than setting it to Default or Fit2Cell. |
| [GetHtmlVersion()](./gethtmlversion/) | Specifies version of HTML standard that should be used when saving the HTML format. Default value is [HtmlVersion.Default](../htmlversion/). |
| [GetIgnoreInvisibleShapes()](./getignoreinvisibleshapes/) | Indicate whether exporting those not visible shapes. |
| [GetImageOptions()](./getimageoptions/) | Get the ImageOrPrintOptions object before exporting. |
| [GetImageScalable()](./getimagescalable/) | Indicates whether using scalable unit to describe the image width when using scalable unit to describe the column width. The default value is true. |
| [GetLayoutMode()](./getlayoutmode/) | Gets or sets the layout mode when saving to HTML. The default value is HtmlLayoutMode.Normal |
| [GetLinkTargetType()](./getlinktargettype/) | Indicating the type of target attribute in **<a>** link. The default value is [HtmlLinkTargetType.Parent](../htmllinktargettype/). |
| [GetMergeAreas()](../saveoptions/getmergeareas/) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [GetMergeEmptyTdForcely()](./getmergeemptytdforcely/) |  **(Deprecated)** Indicates whether merging empty TD element forcedly when exporting file to html. The size of html file will be reduced significantly after setting value to true. The default value is false. If you want to import the html file to excel or export perfect grid lines when saving file to html, please keep the default value. |
| [GetMergeEmptyTdType()](./getmergeemptytdtype/) | The option to merge contiguous empty cells(empty td elements) The default value is [MergeEmptyTdType.Default](../mergeemptytdtype/). |
| [GetOfficeMathOutputMode()](./getofficemathoutputmode/) | Indicates how OfficeMath objects are exported to HTML, Default value is Image. |
| [GetPageTitle()](./getpagetitle/) | The title of the html page. Only for saving to html stream. |
| [GetParseHtmlTagInCell()](./getparsehtmltagincell/) | Indicates whether html tag(such as **<div></div>**) in cell should be parsed as cell value or preserved as it is. The default value is true. |
| [GetPresentationPreference()](./getpresentationpreference/) | Indicating if html or mht file is presentation preference. The default value is false. if you want to get more beautiful presentation,please set the value to true. |
| [GetRefreshChartCache()](../saveoptions/getrefreshchartcache/) | Indicates whether refreshing chart cache data. |
| [GetSaveAsSingleFile()](./getsaveassinglefile/) | Indicates whether save the html as single file. The default value is false. |
| [GetSaveFormat()](../saveoptions/getsaveformat/) | Gets the save file format. |
| [GetSheetSet()](./getsheetset/) | Gets or sets the sheets to render. Default is all visible sheets in the workbook: Aspose.Cells.Rendering.SheetSet.Visible. |
| [GetShowAllSheets()](./getshowallsheets/) | Indicates whether showing all sheets when saving as a single html file. |
| [GetSortExternalNames()](../saveoptions/getsortexternalnames/) | Indicates whether sorting external defined names before saving file. |
| [GetSortNames()](../saveoptions/getsortnames/) | Indicates whether sorting defined names before saving file. |
| [GetTableCssId()](./gettablecssid/) | Gets and sets the prefix of the type css name such as tr,col,td and so on, they are contained in the table element which has the specific TableCssId attribute. The default value is "". |
| [GetUpdateSmartArt()](../saveoptions/getupdatesmartart/) | Indicates whether updating smart art setting. The default value is false. |
| [GetValidateMergedAreas()](../saveoptions/getvalidatemergedareas/) | Indicates whether validate merged cells before saving the file. |
| [GetWarningCallback()](../saveoptions/getwarningcallback/) | Gets or sets warning callback. |
| [GetWidthScalable()](./getwidthscalable/) | Indicates whether exporting column width in unit of scale to html. The default value is false. |
| [GetWorksheetScalable()](./getworksheetscalable/) | Indicates if zooming in or out the html via worksheet zoom level when saving file to html, the default value is false. |
| [HtmlSaveOptions()](./htmlsaveoptions/) | Creates options for saving html file. |
| explicit [HtmlSaveOptions(SaveFormat saveFormat)](./htmlsaveoptions/) | Creates options for saving htm file. |
| [HtmlSaveOptions(HtmlSaveOptions_Impl* impl)](./htmlsaveoptions/) | Constructs from an implementation object. |
| [HtmlSaveOptions(const HtmlSaveOptions\& src)](./htmlsaveoptions/) | Copy constructor. |
| [HtmlSaveOptions(const SaveOptions\& src)](./htmlsaveoptions/) | Constructs from a parent object. |
| [IsBorderCollapsed()](./isbordercollapsed/) | Indicates whether the table borders are collapsed. The default value is true. |
| [IsExpImageToTempDir()](./isexpimagetotempdir/) | Indicates whether exporting image files to temp directory. Only for saving to html stream. |
| [IsExportComments()](./isexportcomments/) | Indicates if exporting comments when saving file to html, the default value is false. |
| [IsFullPathLink()](./isfullpathlink/) | Indicating whether using full path link in sheet00x.htm,filelist.xml and tabstrip.htm. The default value is false. |
| [IsIECompatible()](./isiecompatible/) | Indicating whether the output HTML is compatible with IE browser. The defalut value is false. |
| [IsJsBrowserCompatible()](./isjsbrowsercompatible/) | Indicates whether JavaScript is compatible with browsers that do not support JavaScript. The default value is true. |
| [IsMobileCompatible()](./ismobilecompatible/) | Indicates whether the output HTML is compatible with mobile devices. The default value is false. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const HtmlSaveOptions\& src)](./operator_asm/) | operator= |
| [operator=(const SaveOptions\& src)](../saveoptions/operator_asm/) | operator= |
| [SaveOptions(SaveOptions_Impl* impl)](../saveoptions/saveoptions/) | Constructs from an implementation object. |
| [SaveOptions(const SaveOptions\& src)](../saveoptions/saveoptions/) | Copy constructor. |
| [SetAddGenericFont(bool value)](./setaddgenericfont/) | Indicates whether to add a generic font to CSS font-family. The default value is true. |
| [SetAddTooltipText(bool value)](./setaddtooltiptext/) | Indicates whether adding tooltip text when the data can't be fully displayed. The default value is false. |
| [SetAttachedFilesDirectory(const U16String\& value)](./setattachedfilesdirectory/) | The directory that the attached files will be saved to. Only for saving to html stream. |
| [SetAttachedFilesDirectory(const char16_t* value)](./setattachedfilesdirectory/) | The directory that the attached files will be saved to. Only for saving to html stream. |
| [SetAttachedFilesUrlPrefix(const U16String\& value)](./setattachedfilesurlprefix/) | Specify the Url prefix of attached files such as image in the html file. Only for saving to html stream. |
| [SetAttachedFilesUrlPrefix(const char16_t* value)](./setattachedfilesurlprefix/) | Specify the Url prefix of attached files such as image in the html file. Only for saving to html stream. |
| [SetCachedFileFolder(const U16String\& value)](../saveoptions/setcachedfilefolder/) | The folder for temporary files that may be used as data cache. |
| [SetCachedFileFolder(const char16_t* value)](../saveoptions/setcachedfilefolder/) | The folder for temporary files that may be used as data cache. |
| [SetCalculateFormula(bool value)](./setcalculateformula/) | Indicates whether to calculate formulas before saving html file. |
| [SetCellCssPrefix(const U16String\& value)](./setcellcssprefix/) | Gets and sets the prefix of the css name,the default value is "". |
| [SetCellCssPrefix(const char16_t* value)](./setcellcssprefix/) | Gets and sets the prefix of the css name,the default value is "". |
| [SetCellNameAttribute(const U16String\& value)](./setcellnameattribute/) | Specifies the attribute that indicates the CellName to be written. (e.g. If the value is "id", then for cell "A1", the output will be:<td id='A1'>). The default value is null. |
| [SetCellNameAttribute(const char16_t* value)](./setcellnameattribute/) | Specifies the attribute that indicates the CellName to be written. (e.g. If the value is "id", then for cell "A1", the output will be:<td id='A1'>). The default value is null. |
| [SetCheckExcelRestriction(bool value)](../saveoptions/setcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated. |
| [SetClearData(bool value)](../saveoptions/setcleardata/) | Make the workbook empty after saving the file. |
| [SetCreateDirectory(bool value)](../saveoptions/setcreatedirectory/) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [SetCssStyles(const U16String\& value)](./setcssstyles/) | Gets or sets the additional css styles for the formatter. Only works when SaveAsSingleFile is True. |
| [SetCssStyles(const char16_t* value)](./setcssstyles/) | Gets or sets the additional css styles for the formatter. Only works when SaveAsSingleFile is True. |
| [SetDataBarRenderMode(DataBarRenderMode value)](./setdatabarrendermode/) | Represents the mode of how to render [DataBar](../databar/) when converting Excel files to html files. Default value is DataBarRenderMode.BackgroundColor. |
| [SetDefaultFontName(const U16String\& value)](./setdefaultfontname/) | Specify the default font name for exporting html, the default font will be used when the font of style is not existing, If this property is null, [Aspose.Cells](../) will use universal font which have the same family with the original font, the default value is null. |
| [SetDefaultFontName(const char16_t* value)](./setdefaultfontname/) | Specify the default font name for exporting html, the default font will be used when the font of style is not existing, If this property is null, [Aspose.Cells](../) will use universal font which have the same family with the original font, the default value is null. |
| [SetDisableCss(bool value)](./setdisablecss/) | Indicates whether only inline styles are applied, without relying on CSS. The default value is false. |
| [SetDisableDownlevelRevealedComments(bool value)](./setdisabledownlevelrevealedcomments/) | Indicates if disable Downlevel-revealed conditional comments when exporting file to html, the default value is false. |
| [SetEmbeddedFontType(HtmlEmbeddedFontType value)](./setembeddedfonttype/) | Gets or sets the type of embedding font file into html file. Default value is HtmlEmbeddedFontType.None which indicates that no font will be embedded in html. |
| [SetEnableCssCustomProperties(bool value)](./setenablecsscustomproperties/) | Optimize the output of html by using CSS custom properties. For example, for the scenario that there are multiple occurences for one base64 image, with custom property the image data only needs to be saved once so the performance of the resultant html can be improved. The default value is false. |
| [SetEncodeEntityAsCode(bool value)](./setencodeentityascode/) | Indicates whether the html character entities are replaced with decimal code. (e.g. "&amp;nbsp;" is replaced with "&amp;#160;"). The default value is false. |
| [SetEncoding(EncodingType value)](./setencoding/) | If not set,use Encoding.UTF8 as default enconding type. |
| [SetEncryptDocumentProperties(bool value)](../saveoptions/setencryptdocumentproperties/) | Indicates whether encrypt document properties when saving as .xls file. The default value is true. |
| [SetExcludeUnusedStyles(bool value)](./setexcludeunusedstyles/) | Indicating whether excludes unused styles. For the generated html files, excluding unused styles can make the file size smaller without affecting the visual effects. So the default value of this property is true. If user needs to keep all styles in the workbook for the generated html(such as the scenario that user needs to restore the workbook from the generated html later), please set this property as false. |
| [SetExportActiveWorksheetOnly(bool value)](./setexportactiveworksheetonly/) | Indicates if only exporting the active worksheet to html file. If true then only the active worksheet will be exported to html file; If false then the whole workbook will be exported to html file. The default value is false. |
| [SetExportArea(const CellArea\& value)](./setexportarea/) | Gets or Sets the exporting [CellArea](../cellarea/) of current active [Worksheet](../worksheet/). If you set this attribute, the print area of current active [Worksheet](../worksheet/) will be omitted. Only the specified area will be exported when saving the file to html. |
| [SetExportBogusRowData(bool value)](./setexportbogusrowdata/) | Indicating whether exporting bogus bottom row data. The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [SetExportCellCoordinate(bool value)](./setexportcellcoordinate/) | Indicates whether exporting excel coordinate of nonblank cells when saving file to html. The default value is false. If you want to import the output html to excel, please keep the default value. |
| [SetExportCommentsType(PrintCommentsType value)](./setexportcommentstype/) | Represents type of exporting comments to html files. |
| [SetExportDataOptions(HtmlExportDataOptions value)](./setexportdataoptions/) | Indicating the rule of exporting html file data.The default value is All. |
| [SetExportDocumentProperties(bool value)](./setexportdocumentproperties/) | Indicating whether exporting document properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [SetExportExtraHeadings(bool value)](./setexportextraheadings/) | Indicates whether exporting extra headings when the length of text is longer than max display column. The default value is false. If you want to import the html file to excel, please keep the default value. |
| [SetExportFormula(bool value)](./setexportformula/) | Indicates whether exporting formula when saving file to html. The default value is true. If you want to import the output html to excel, please keep the default value. |
| [SetExportFrameScriptsAndProperties(bool value)](./setexportframescriptsandproperties/) | Indicating whether exporting frame scripts and document properties. The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [SetExportGridLines(bool value)](./setexportgridlines/) | Indicating whether exporting the gridlines.The default value is false. |
| [SetExportHiddenWorksheet(bool value)](./setexporthiddenworksheet/) | Indicating if exporting the hidden worksheet content.The default value is true. |
| [SetExportImagesAsBase64(bool value)](./setexportimagesasbase64/) | Specifies whether images are saved in Base64 format to HTML, MHTML or EPUB. |
| [SetExportNamedRangeAnchors(bool value)](./setexportnamedrangeanchors/) | Indicates whether to export anchor elements for named ranges when saving as HTML. Default value is true. |
| [SetExportPageFooters(bool value)](./setexportpagefooters/) | Indicates whether exporting page headers. |
| [SetExportPageHeaders(bool value)](./setexportpageheaders/) | Indicates whether exporting page headers. |
| [SetExportPrintAreaOnly(bool value)](./setexportprintareaonly/) | Indicates if only exporting the print area to html file. The default value is false. |
| [SetExportRowColumnHeadings(bool value)](./setexportrowcolumnheadings/) | Indicates whether exports sheet's row and column headings when saving to HTML files. |
| [SetExportSimilarBorderStyle(bool value)](./setexportsimilarborderstyle/) | Indicating whether exporting the similar border style when the border style is not supported by browsers. If you want to import the html or mht file to excel, please keep the default value. The default value is false. |
| [SetExportSingleTab(bool value)](./setexportsingletab/) | Indicates whether exporting the single tab when the file only has one worksheet. The default value is false. |
| [SetExportWorkbookProperties(bool value)](./setexportworkbookproperties/) | Indicating whether exporting workbook properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [SetExportWorksheetCSSSeparately(bool value)](./setexportworksheetcssseparately/) | Indicating whether export the worksheet css separately.The default value is false. |
| [SetExportWorksheetProperties(bool value)](./setexportworksheetproperties/) | Indicating whether exporting worksheet properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [SetFilePathProvider(IFilePathProvider* value)](./setfilepathprovider/) | Gets or sets the [IFilePathProvider](../ifilepathprovider/) for exporting [Worksheet](../worksheet/) to html separately. |
| [SetFormatDataIgnoreColumnWidth(bool value)](./setformatdataignorecolumnwidth/) | Indicating whether show the whole formatted data of cell when overflowing the column. If true then ignore the column width and the whole data of cell will be exported. If false then the data will be exported same as Excel. The default value is false. |
| [SetHiddenColDisplayType(HtmlHiddenColDisplayType value)](./sethiddencoldisplaytype/) | Hidden column(the width of this column is 0) in excel,before save this into html format, if HtmlHiddenColDisplayType is "Remove",the hidden column would not been output, if the value is "Hidden", the column would been output,but was hidden,the default value is "Hidden". |
| [SetHiddenRowDisplayType(HtmlHiddenRowDisplayType value)](./sethiddenrowdisplaytype/) | Hidden row(the height of this row is 0) in excel,before save this into html format, if HtmlHiddenRowDisplayType is "Remove",the hidden row would not been output, if the value is "Hidden", the row would been output,but was hidden,the default value is "Hidden". |
| [SetHideOverflowWrappedText(bool value)](./sethideoverflowwrappedtext/) | Indicates whether to hide overflow text when the cell format is set to wrap text. The default value is false. |
| [SetHtmlCrossStringType(HtmlCrossType value)](./sethtmlcrossstringtype/) | Indicates if a cross-cell string will be displayed in the same way as MS Excel when saving an Excel file in html format. By default the value is Default, so, for cross-cell strings, there is little difference between the html files created by [Aspose.Cells](../) and MS Excel. But the performance for creating large html files,setting the value to Cross would be several times faster than setting it to Default or Fit2Cell. |
| [SetHtmlVersion(HtmlVersion value)](./sethtmlversion/) | Specifies version of HTML standard that should be used when saving the HTML format. Default value is [HtmlVersion.Default](../htmlversion/). |
| [SetIgnoreInvisibleShapes(bool value)](./setignoreinvisibleshapes/) | Indicate whether exporting those not visible shapes. |
| [SetImageScalable(bool value)](./setimagescalable/) | Indicates whether using scalable unit to describe the image width when using scalable unit to describe the column width. The default value is true. |
| [SetIsBorderCollapsed(bool value)](./setisbordercollapsed/) | Indicates whether the table borders are collapsed. The default value is true. |
| [SetIsExpImageToTempDir(bool value)](./setisexpimagetotempdir/) | Indicates whether exporting image files to temp directory. Only for saving to html stream. |
| [SetIsExportComments(bool value)](./setisexportcomments/) | Indicates if exporting comments when saving file to html, the default value is false. |
| [SetIsFullPathLink(bool value)](./setisfullpathlink/) | Indicating whether using full path link in sheet00x.htm,filelist.xml and tabstrip.htm. The default value is false. |
| [SetIsIECompatible(bool value)](./setisiecompatible/) | Indicating whether the output HTML is compatible with IE browser. The defalut value is false. |
| [SetIsJsBrowserCompatible(bool value)](./setisjsbrowsercompatible/) | Indicates whether JavaScript is compatible with browsers that do not support JavaScript. The default value is true. |
| [SetIsMobileCompatible(bool value)](./setismobilecompatible/) | Indicates whether the output HTML is compatible with mobile devices. The default value is false. |
| [SetLayoutMode(HtmlLayoutMode value)](./setlayoutmode/) | Gets or sets the layout mode when saving to HTML. The default value is HtmlLayoutMode.Normal |
| [SetLinkTargetType(HtmlLinkTargetType value)](./setlinktargettype/) | Indicating the type of target attribute in **<a>** link. The default value is [HtmlLinkTargetType.Parent](../htmllinktargettype/). |
| [SetMergeAreas(bool value)](../saveoptions/setmergeareas/) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [SetMergeEmptyTdForcely(bool value)](./setmergeemptytdforcely/) |  **(Deprecated)** Indicates whether merging empty TD element forcedly when exporting file to html. The size of html file will be reduced significantly after setting value to true. The default value is false. If you want to import the html file to excel or export perfect grid lines when saving file to html, please keep the default value. |
| [SetMergeEmptyTdType(MergeEmptyTdType value)](./setmergeemptytdtype/) | The option to merge contiguous empty cells(empty td elements) The default value is [MergeEmptyTdType.Default](../mergeemptytdtype/). |
| [SetOfficeMathOutputMode(HtmlOfficeMathOutputType value)](./setofficemathoutputmode/) | Indicates how OfficeMath objects are exported to HTML, Default value is Image. |
| [SetPageTitle(const U16String\& value)](./setpagetitle/) | The title of the html page. Only for saving to html stream. |
| [SetPageTitle(const char16_t* value)](./setpagetitle/) | The title of the html page. Only for saving to html stream. |
| [SetParseHtmlTagInCell(bool value)](./setparsehtmltagincell/) | Indicates whether html tag(such as **<div></div>**) in cell should be parsed as cell value or preserved as it is. The default value is true. |
| [SetPresentationPreference(bool value)](./setpresentationpreference/) | Indicating if html or mht file is presentation preference. The default value is false. if you want to get more beautiful presentation,please set the value to true. |
| [SetRefreshChartCache(bool value)](../saveoptions/setrefreshchartcache/) | Indicates whether refreshing chart cache data. |
| [SetSaveAsSingleFile(bool value)](./setsaveassinglefile/) | Indicates whether save the html as single file. The default value is false. |
| [SetSheetSet(const SheetSet\& value)](./setsheetset/) | Gets or sets the sheets to render. Default is all visible sheets in the workbook: Aspose.Cells.Rendering.SheetSet.Visible. |
| [SetShowAllSheets(bool value)](./setshowallsheets/) | Indicates whether showing all sheets when saving as a single html file. |
| [SetSortExternalNames(bool value)](../saveoptions/setsortexternalnames/) | Indicates whether sorting external defined names before saving file. |
| [SetSortNames(bool value)](../saveoptions/setsortnames/) | Indicates whether sorting defined names before saving file. |
| [SetTableCssId(const U16String\& value)](./settablecssid/) | Gets and sets the prefix of the type css name such as tr,col,td and so on, they are contained in the table element which has the specific TableCssId attribute. The default value is "". |
| [SetTableCssId(const char16_t* value)](./settablecssid/) | Gets and sets the prefix of the type css name such as tr,col,td and so on, they are contained in the table element which has the specific TableCssId attribute. The default value is "". |
| [SetUpdateSmartArt(bool value)](../saveoptions/setupdatesmartart/) | Indicates whether updating smart art setting. The default value is false. |
| [SetValidateMergedAreas(bool value)](../saveoptions/setvalidatemergedareas/) | Indicates whether validate merged cells before saving the file. |
| [SetWarningCallback(IWarningCallback* value)](../saveoptions/setwarningcallback/) | Gets or sets warning callback. |
| [SetWidthScalable(bool value)](./setwidthscalable/) | Indicates whether exporting column width in unit of scale to html. The default value is false. |
| [SetWorksheetScalable(bool value)](./setworksheetscalable/) | Indicates if zooming in or out the html via worksheet zoom level when saving file to html, the default value is false. |
| [~HtmlSaveOptions()](./~htmlsaveoptions/) | Destructor. |
| [~SaveOptions()](../saveoptions/~saveoptions/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also

* Class [SaveOptions](../saveoptions/)
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
