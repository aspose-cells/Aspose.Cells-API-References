---
title: Aspose::Cells::Saving::EbookSaveOptions class
linktitle: EbookSaveOptions
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Saving::EbookSaveOptions class. Represents the options for saving ebook file in C++.'
type: docs
weight: 100
url: /cpp/aspose.cells.saving/ebooksaveoptions/
---
## EbookSaveOptions class


Represents the options for saving ebook file.

```cpp
class EbookSaveOptions : public Aspose::Cells::HtmlSaveOptions
```

## Methods

| Method | Description |
| --- | --- |
| [EbookSaveOptions()](./ebooksaveoptions/) | Creates options for saving ebook file. |
| [EbookSaveOptions(EbookSaveOptions_Impl* impl)](./ebooksaveoptions/) | Constructs from an implementation object. |
| [EbookSaveOptions(const EbookSaveOptions\& src)](./ebooksaveoptions/) | Copy constructor. |
| [EbookSaveOptions(const HtmlSaveOptions\& src)](./ebooksaveoptions/) | Constructs from a parent object. |
| [GetAddTooltipText()](../../aspose.cells/htmlsaveoptions/getaddtooltiptext/) | Indicates whether adding tooltip text when the data can't be fully displayed. The default value is false. |
| [GetAttachedFilesDirectory()](../../aspose.cells/htmlsaveoptions/getattachedfilesdirectory/) | The directory that the attached files will be saved to. Only for saving to html stream. |
| [GetAttachedFilesUrlPrefix()](../../aspose.cells/htmlsaveoptions/getattachedfilesurlprefix/) | Specify the Url prefix of attached files such as image in the html file. Only for saving to html stream. |
| [GetCachedFileFolder()](../../aspose.cells/saveoptions/getcachedfilefolder/) | The cached file folder is used to store some large data. |
| [GetCalculateFormula()](../../aspose.cells/htmlsaveoptions/getcalculateformula/) | Indicates whether to calculate formulas before saving html file. |
| [GetCellCssPrefix()](../../aspose.cells/htmlsaveoptions/getcellcssprefix/) | Gets and sets the prefix of the css name,the default value is "". |
| [GetClearData()](../../aspose.cells/saveoptions/getcleardata/) | Make the workbook empty after saving the file. |
| [GetCreateDirectory()](../../aspose.cells/saveoptions/getcreatedirectory/) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [GetDefaultFontName()](../../aspose.cells/htmlsaveoptions/getdefaultfontname/) | Specify the default font name for exporting html, the default font will be used when the font of style is not existing, If this property is null, [Aspose.Cells](../../aspose.cells/) will use universal font which have the same family with the original font, the default value is null. |
| [GetDisableDownlevelRevealedComments()](../../aspose.cells/htmlsaveoptions/getdisabledownlevelrevealedcomments/) | Indicates if disable Downlevel-revealed conditional comments when exporting file to html, the default value is false. |
| [GetEncoding()](../../aspose.cells/htmlsaveoptions/getencoding/) | If not set,use Encoding.UTF8 as default enconding type. |
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
| [GetHtmlCrossStringType()](../../aspose.cells/htmlsaveoptions/gethtmlcrossstringtype/) | Indicates if a cross-cell string will be displayed in the same way as MS Excel when saving an Excel file in html format. By default the value is Default, so, for cross-cell strings, there is little difference between the html files created by [Aspose.Cells](../../aspose.cells/) and MS Excel. But the performance for creating large html files,setting the value to Cross would be several times faster than setting it to Default or Fit2Cell. |
| [GetIgnoreInvisibleShapes()](../../aspose.cells/htmlsaveoptions/getignoreinvisibleshapes/) | Indicate whether exporting those not visible shapes. |
| [GetImageOptions()](../../aspose.cells/htmlsaveoptions/getimageoptions/) | Get the ImageOrPrintOptions object before exporting. |
| [GetImageScalable()](../../aspose.cells/htmlsaveoptions/getimagescalable/) | Indicates whether using scalable unit to describe the image width when using scalable unit to describe the column width. The default value is true. |
| [GetLinkTargetType()](../../aspose.cells/htmlsaveoptions/getlinktargettype/) | Indicating the type of target attribute in **<a>** link. The default value is [HtmlLinkTargetType.Parent](../../aspose.cells/htmllinktargettype/). |
| [GetMergeAreas()](../../aspose.cells/saveoptions/getmergeareas/) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [GetMergeEmptyTdForcely()](../../aspose.cells/htmlsaveoptions/getmergeemptytdforcely/) | Indicates whether merging empty TD element forcedly when exporting file to html. The size of html file will be reduced significantly after setting value to true. The default value is false. If you want to import the html file to excel or export perfect grid lines when saving file to html, please keep the default value. |
| [GetPageTitle()](../../aspose.cells/htmlsaveoptions/getpagetitle/) | The title of the html page. Only for saving to html stream. |
| [GetParseHtmlTagInCell()](../../aspose.cells/htmlsaveoptions/getparsehtmltagincell/) | Indicates whether html tag(such as **<div></div>**) in cell should be parsed as cell value or preserved as it is. The default value is true. |
| [GetPresentationPreference()](../../aspose.cells/htmlsaveoptions/getpresentationpreference/) | Indicating if html or mht file is presentation preference. The default value is false. if you want to get more beautiful presentation,please set the value to true. |
| [GetRefreshChartCache()](../../aspose.cells/saveoptions/getrefreshchartcache/) | Indicates whether refreshing chart cache data. |
| [GetSaveAsSingleFile()](../../aspose.cells/htmlsaveoptions/getsaveassinglefile/) | Indicates whether save the html as single file. The default value is false. |
| [GetSaveFormat()](../../aspose.cells/saveoptions/getsaveformat/) | Gets the save file format. |
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
| [IsExpImageToTempDir()](../../aspose.cells/htmlsaveoptions/isexpimagetotempdir/) | Indicates whether exporting image files to temp directory. Only for saving to html stream. |
| [IsExportComments()](../../aspose.cells/htmlsaveoptions/isexportcomments/) | Indicates if exporting comments when saving file to html, the default value is false. |
| [IsFullPathLink()](../../aspose.cells/htmlsaveoptions/isfullpathlink/) | Indicating whether using full path link in sheet00x.htm,filelist.xml and tabstrip.htm. The default value is false. |
| [IsIECompatible()](../../aspose.cells/htmlsaveoptions/isiecompatible/) | Indicating whether the output HTML is compatible with IE browser. The defalut value is false. |
| [IsJsBrowserCompatible()](../../aspose.cells/htmlsaveoptions/isjsbrowsercompatible/) | Indicates whether JavaScript is compatible with browsers that do not support JavaScript. The default value is true. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const EbookSaveOptions\& src)](./operator_asm/) | operator= |
| [operator=(const HtmlSaveOptions\& src)](../../aspose.cells/htmlsaveoptions/operator_asm/) | operator= |
| [operator=(const SaveOptions\& src)](../../aspose.cells/saveoptions/operator_asm/) | operator= |
| [SaveOptions(SaveOptions_Impl* impl)](../../aspose.cells/saveoptions/saveoptions/) | Constructs from an implementation object. |
| [SaveOptions(const SaveOptions\& src)](../../aspose.cells/saveoptions/saveoptions/) | Copy constructor. |
| [SetAddTooltipText(bool value)](../../aspose.cells/htmlsaveoptions/setaddtooltiptext/) | Indicates whether adding tooltip text when the data can't be fully displayed. The default value is false. |
| [SetAttachedFilesDirectory(const U16String\& value)](../../aspose.cells/htmlsaveoptions/setattachedfilesdirectory/) | The directory that the attached files will be saved to. Only for saving to html stream. |
| [SetAttachedFilesDirectory(const char16_t* value)](../../aspose.cells/htmlsaveoptions/setattachedfilesdirectory/) | The directory that the attached files will be saved to. Only for saving to html stream. |
| [SetAttachedFilesUrlPrefix(const U16String\& value)](../../aspose.cells/htmlsaveoptions/setattachedfilesurlprefix/) | Specify the Url prefix of attached files such as image in the html file. Only for saving to html stream. |
| [SetAttachedFilesUrlPrefix(const char16_t* value)](../../aspose.cells/htmlsaveoptions/setattachedfilesurlprefix/) | Specify the Url prefix of attached files such as image in the html file. Only for saving to html stream. |
| [SetCachedFileFolder(const U16String\& value)](../../aspose.cells/saveoptions/setcachedfilefolder/) | The cached file folder is used to store some large data. |
| [SetCachedFileFolder(const char16_t* value)](../../aspose.cells/saveoptions/setcachedfilefolder/) | The cached file folder is used to store some large data. |
| [SetCalculateFormula(bool value)](../../aspose.cells/htmlsaveoptions/setcalculateformula/) | Indicates whether to calculate formulas before saving html file. |
| [SetCellCssPrefix(const U16String\& value)](../../aspose.cells/htmlsaveoptions/setcellcssprefix/) | Gets and sets the prefix of the css name,the default value is "". |
| [SetCellCssPrefix(const char16_t* value)](../../aspose.cells/htmlsaveoptions/setcellcssprefix/) | Gets and sets the prefix of the css name,the default value is "". |
| [SetClearData(bool value)](../../aspose.cells/saveoptions/setcleardata/) | Make the workbook empty after saving the file. |
| [SetCreateDirectory(bool value)](../../aspose.cells/saveoptions/setcreatedirectory/) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [SetDefaultFontName(const U16String\& value)](../../aspose.cells/htmlsaveoptions/setdefaultfontname/) | Specify the default font name for exporting html, the default font will be used when the font of style is not existing, If this property is null, [Aspose.Cells](../../aspose.cells/) will use universal font which have the same family with the original font, the default value is null. |
| [SetDefaultFontName(const char16_t* value)](../../aspose.cells/htmlsaveoptions/setdefaultfontname/) | Specify the default font name for exporting html, the default font will be used when the font of style is not existing, If this property is null, [Aspose.Cells](../../aspose.cells/) will use universal font which have the same family with the original font, the default value is null. |
| [SetDisableDownlevelRevealedComments(bool value)](../../aspose.cells/htmlsaveoptions/setdisabledownlevelrevealedcomments/) | Indicates if disable Downlevel-revealed conditional comments when exporting file to html, the default value is false. |
| [SetEncoding(EncodingType value)](../../aspose.cells/htmlsaveoptions/setencoding/) | If not set,use Encoding.UTF8 as default enconding type. |
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
| [SetHtmlCrossStringType(HtmlCrossType value)](../../aspose.cells/htmlsaveoptions/sethtmlcrossstringtype/) | Indicates if a cross-cell string will be displayed in the same way as MS Excel when saving an Excel file in html format. By default the value is Default, so, for cross-cell strings, there is little difference between the html files created by [Aspose.Cells](../../aspose.cells/) and MS Excel. But the performance for creating large html files,setting the value to Cross would be several times faster than setting it to Default or Fit2Cell. |
| [SetIgnoreInvisibleShapes(bool value)](../../aspose.cells/htmlsaveoptions/setignoreinvisibleshapes/) | Indicate whether exporting those not visible shapes. |
| [SetImageScalable(bool value)](../../aspose.cells/htmlsaveoptions/setimagescalable/) | Indicates whether using scalable unit to describe the image width when using scalable unit to describe the column width. The default value is true. |
| [SetIsExpImageToTempDir(bool value)](../../aspose.cells/htmlsaveoptions/setisexpimagetotempdir/) | Indicates whether exporting image files to temp directory. Only for saving to html stream. |
| [SetIsExportComments(bool value)](../../aspose.cells/htmlsaveoptions/setisexportcomments/) | Indicates if exporting comments when saving file to html, the default value is false. |
| [SetIsFullPathLink(bool value)](../../aspose.cells/htmlsaveoptions/setisfullpathlink/) | Indicating whether using full path link in sheet00x.htm,filelist.xml and tabstrip.htm. The default value is false. |
| [SetIsIECompatible(bool value)](../../aspose.cells/htmlsaveoptions/setisiecompatible/) | Indicating whether the output HTML is compatible with IE browser. The defalut value is false. |
| [SetIsJsBrowserCompatible(bool value)](../../aspose.cells/htmlsaveoptions/setisjsbrowsercompatible/) | Indicates whether JavaScript is compatible with browsers that do not support JavaScript. The default value is true. |
| [SetLinkTargetType(HtmlLinkTargetType value)](../../aspose.cells/htmlsaveoptions/setlinktargettype/) | Indicating the type of target attribute in **<a>** link. The default value is [HtmlLinkTargetType.Parent](../../aspose.cells/htmllinktargettype/). |
| [SetMergeAreas(bool value)](../../aspose.cells/saveoptions/setmergeareas/) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [SetMergeEmptyTdForcely(bool value)](../../aspose.cells/htmlsaveoptions/setmergeemptytdforcely/) | Indicates whether merging empty TD element forcedly when exporting file to html. The size of html file will be reduced significantly after setting value to true. The default value is false. If you want to import the html file to excel or export perfect grid lines when saving file to html, please keep the default value. |
| [SetPageTitle(const U16String\& value)](../../aspose.cells/htmlsaveoptions/setpagetitle/) | The title of the html page. Only for saving to html stream. |
| [SetPageTitle(const char16_t* value)](../../aspose.cells/htmlsaveoptions/setpagetitle/) | The title of the html page. Only for saving to html stream. |
| [SetParseHtmlTagInCell(bool value)](../../aspose.cells/htmlsaveoptions/setparsehtmltagincell/) | Indicates whether html tag(such as **<div></div>**) in cell should be parsed as cell value or preserved as it is. The default value is true. |
| [SetPresentationPreference(bool value)](../../aspose.cells/htmlsaveoptions/setpresentationpreference/) | Indicating if html or mht file is presentation preference. The default value is false. if you want to get more beautiful presentation,please set the value to true. |
| [SetRefreshChartCache(bool value)](../../aspose.cells/saveoptions/setrefreshchartcache/) | Indicates whether refreshing chart cache data. |
| [SetSaveAsSingleFile(bool value)](../../aspose.cells/htmlsaveoptions/setsaveassinglefile/) | Indicates whether save the html as single file. The default value is false. |
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
