---
title: HtmlSaveOptions
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the options for saving html file.
type: docs
url: /nodejs-cpp/htmlsaveoptions/
---

## HtmlSaveOptions class

Represents the options for saving html file.

```javascript
class HtmlSaveOptions extends SaveOptions;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Creates options for saving html file. |
| [constructor(SaveOptions)](#constructor-saveoptions-)| Constructs from a parent object convertible to this. |
| [constructor(SaveFormat)](#constructor-saveformat-)| Creates options for saving htm file. |

## Methods

| Method | Description |
| --- | --- |
| [getIgnoreInvisibleShapes()](#getIgnoreInvisibleShapes--)| Indicate whether exporting those not visible shapes |
| [setIgnoreInvisibleShapes(boolean)](#setIgnoreInvisibleShapes-boolean-)| Indicate whether exporting those not visible shapes |
| [getPageTitle()](#getPageTitle--)| The title of the html page. Only for saving to html stream. |
| [setPageTitle(string)](#setPageTitle-string-)| The title of the html page. Only for saving to html stream. |
| [getAttachedFilesDirectory()](#getAttachedFilesDirectory--)| The directory that the attached files will be saved to. Only for saving to html stream. |
| [setAttachedFilesDirectory(string)](#setAttachedFilesDirectory-string-)| The directory that the attached files will be saved to. Only for saving to html stream. |
| [getAttachedFilesUrlPrefix()](#getAttachedFilesUrlPrefix--)| Specify the Url prefix of attached files such as image in the html file. Only for saving to html stream. |
| [setAttachedFilesUrlPrefix(string)](#setAttachedFilesUrlPrefix-string-)| Specify the Url prefix of attached files such as image in the html file. Only for saving to html stream. |
| [getDefaultFontName()](#getDefaultFontName--)| Specify the default font name for exporting html, the default font will be used  when the font of style is not existing, If this property is null, Aspose.Cells will use universal font which have the same family with the original font, the default value is null. |
| [setDefaultFontName(string)](#setDefaultFontName-string-)| Specify the default font name for exporting html, the default font will be used  when the font of style is not existing, If this property is null, Aspose.Cells will use universal font which have the same family with the original font, the default value is null. |
| [getAddGenericFont()](#getAddGenericFont--)| Indicates whether to add a generic font to CSS font-family. The default value is true |
| [setAddGenericFont(boolean)](#setAddGenericFont-boolean-)| Indicates whether to add a generic font to CSS font-family. The default value is true |
| [getWorksheetScalable()](#getWorksheetScalable--)| Indicates if zooming in or out the html via worksheet zoom level when saving file to html, the default value is false. |
| [setWorksheetScalable(boolean)](#setWorksheetScalable-boolean-)| Indicates if zooming in or out the html via worksheet zoom level when saving file to html, the default value is false. |
| [isExportComments()](#isExportComments--)| Indicates if exporting comments when saving file to html, the default value is false. |
| [setIsExportComments(boolean)](#setIsExportComments-boolean-)| Indicates if exporting comments when saving file to html, the default value is false. |
| [getExportCommentsType()](#getExportCommentsType--)| Represents type of exporting comments to html files. |
| [setExportCommentsType(PrintCommentsType)](#setExportCommentsType-printcommentstype-)| Represents type of exporting comments to html files. |
| [getDisableDownlevelRevealedComments()](#getDisableDownlevelRevealedComments--)| Indicates if disable Downlevel-revealed conditional comments when exporting file to html, the default value is false. |
| [setDisableDownlevelRevealedComments(boolean)](#setDisableDownlevelRevealedComments-boolean-)| Indicates if disable Downlevel-revealed conditional comments when exporting file to html, the default value is false. |
| [isExpImageToTempDir()](#isExpImageToTempDir--)| Indicates whether exporting image files to temp directory. Only for saving to html stream. |
| [setIsExpImageToTempDir(boolean)](#setIsExpImageToTempDir-boolean-)| Indicates whether exporting image files to temp directory. Only for saving to html stream. |
| [getImageScalable()](#getImageScalable--)| Indicates whether using scalable unit to describe the image width when using scalable unit to describe the column width. The default value is true. |
| [setImageScalable(boolean)](#setImageScalable-boolean-)| Indicates whether using scalable unit to describe the image width when using scalable unit to describe the column width. The default value is true. |
| [getWidthScalable()](#getWidthScalable--)| Indicates whether exporting column width in unit of scale to html. The default value is false. |
| [setWidthScalable(boolean)](#setWidthScalable-boolean-)| Indicates whether exporting column width in unit of scale to html. The default value is false. |
| [getExportSingleTab()](#getExportSingleTab--)| Indicates whether exporting the single tab when the file only has one worksheet. The default value is false. |
| [setExportSingleTab(boolean)](#setExportSingleTab-boolean-)| Indicates whether exporting the single tab when the file only has one worksheet. The default value is false. |
| [getExportImagesAsBase64()](#getExportImagesAsBase64--)| Specifies whether images are saved in Base64 format to HTML, MHTML or EPUB. |
| [setExportImagesAsBase64(boolean)](#setExportImagesAsBase64-boolean-)| Specifies whether images are saved in Base64 format to HTML, MHTML or EPUB. |
| [getExportActiveWorksheetOnly()](#getExportActiveWorksheetOnly--)| Indicates if only exporting the active worksheet to html file. If true then only the active worksheet will be exported to html file; If false then the whole workbook will be exported to html file. The default value is false. |
| [setExportActiveWorksheetOnly(boolean)](#setExportActiveWorksheetOnly-boolean-)| Indicates if only exporting the active worksheet to html file. If true then only the active worksheet will be exported to html file; If false then the whole workbook will be exported to html file. The default value is false. |
| [getExportPrintAreaOnly()](#getExportPrintAreaOnly--)| Indicates if only exporting the print area to html file. The default value is false. |
| [setExportPrintAreaOnly(boolean)](#setExportPrintAreaOnly-boolean-)| Indicates if only exporting the print area to html file. The default value is false. |
| [getExportArea()](#getExportArea--)| Gets or Sets the exporting CellArea of current active Worksheet. If you set this attribute, the print area of current active Worksheet will be omitted. Only the specified area will be exported when saving the file to html. |
| [setExportArea(CellArea)](#setExportArea-cellarea-)| Gets or Sets the exporting CellArea of current active Worksheet. If you set this attribute, the print area of current active Worksheet will be omitted. Only the specified area will be exported when saving the file to html. |
| [getParseHtmlTagInCell()](#getParseHtmlTagInCell--)| Indicates whether html tag(such as <c>&lt;div&gt;&lt;/div&gt;</c>) in cell should be parsed as cell value or preserved as it is. The default value is true. |
| [setParseHtmlTagInCell(boolean)](#setParseHtmlTagInCell-boolean-)| Indicates whether html tag(such as <c>&lt;div&gt;&lt;/div&gt;</c>) in cell should be parsed as cell value or preserved as it is. The default value is true. |
| [getHtmlCrossStringType()](#getHtmlCrossStringType--)| Indicates if a cross-cell string will be displayed in the same way as MS Excel when saving an Excel file in html format. By default the value is Default, so, for cross-cell strings, there is little difference between the html files created by Aspose.Cells and MS Excel. But the performance for creating large html files,setting the value to Cross would be several times faster than setting it to Default or Fit2Cell. |
| [setHtmlCrossStringType(HtmlCrossType)](#setHtmlCrossStringType-htmlcrosstype-)| Indicates if a cross-cell string will be displayed in the same way as MS Excel when saving an Excel file in html format. By default the value is Default, so, for cross-cell strings, there is little difference between the html files created by Aspose.Cells and MS Excel. But the performance for creating large html files,setting the value to Cross would be several times faster than setting it to Default or Fit2Cell. |
| [getHiddenColDisplayType()](#getHiddenColDisplayType--)| Hidden column(the width of this column is 0) in excel,before save this into html format, if HtmlHiddenColDisplayType is "Remove",the hidden column would not been output, if the value is "Hidden", the column would been output,but was hidden,the default value is "Hidden" |
| [setHiddenColDisplayType(HtmlHiddenColDisplayType)](#setHiddenColDisplayType-htmlhiddencoldisplaytype-)| Hidden column(the width of this column is 0) in excel,before save this into html format, if HtmlHiddenColDisplayType is "Remove",the hidden column would not been output, if the value is "Hidden", the column would been output,but was hidden,the default value is "Hidden" |
| [getHiddenRowDisplayType()](#getHiddenRowDisplayType--)| Hidden row(the height of this row is 0) in excel,before save this into html format, if HtmlHiddenRowDisplayType is "Remove",the hidden row would not been output, if the value is "Hidden", the row would been output,but was hidden,the default value is "Hidden" |
| [setHiddenRowDisplayType(HtmlHiddenRowDisplayType)](#setHiddenRowDisplayType-htmlhiddenrowdisplaytype-)| Hidden row(the height of this row is 0) in excel,before save this into html format, if HtmlHiddenRowDisplayType is "Remove",the hidden row would not been output, if the value is "Hidden", the row would been output,but was hidden,the default value is "Hidden" |
| [getEncoding()](#getEncoding--)| If not set,use Encoding.UTF8 as default enconding type. |
| [setEncoding(EncodingType)](#setEncoding-encodingtype-)| If not set,use Encoding.UTF8 as default enconding type. |
| [getFilePathProvider()](#getFilePathProvider--)| Gets or sets the IFilePathProvider for exporting Worksheet to html separately. |
| [setFilePathProvider(IFilePathProvider)](#setFilePathProvider-ifilepathprovider-)| Gets or sets the IFilePathProvider for exporting Worksheet to html separately. |
| [getImageOptions()](#getImageOptions--)| Get the ImageOrPrintOptions object before exporting |
| [getSaveAsSingleFile()](#getSaveAsSingleFile--)| Indicates whether save the html as single file. The default value is false. |
| [setSaveAsSingleFile(boolean)](#setSaveAsSingleFile-boolean-)| Indicates whether save the html as single file. The default value is false. |
| [getShowAllSheets()](#getShowAllSheets--)| Indicates whether showing all sheets when saving  as a single html file. |
| [setShowAllSheets(boolean)](#setShowAllSheets-boolean-)| Indicates whether showing all sheets when saving  as a single html file. |
| [getExportPageHeaders()](#getExportPageHeaders--)| Indicates whether exporting page headers. |
| [setExportPageHeaders(boolean)](#setExportPageHeaders-boolean-)| Indicates whether exporting page headers. |
| [getExportPageFooters()](#getExportPageFooters--)| Indicates whether exporting page headers. |
| [setExportPageFooters(boolean)](#setExportPageFooters-boolean-)| Indicates whether exporting page headers. |
| [getExportHiddenWorksheet()](#getExportHiddenWorksheet--)| Indicating if exporting the hidden worksheet content.The default value is true. |
| [setExportHiddenWorksheet(boolean)](#setExportHiddenWorksheet-boolean-)| Indicating if exporting the hidden worksheet content.The default value is true. |
| [getPresentationPreference()](#getPresentationPreference--)| Indicating if html or mht file is presentation preference. The default value is false. if you want to get more beautiful presentation,please set the value to true. |
| [setPresentationPreference(boolean)](#setPresentationPreference-boolean-)| Indicating if html or mht file is presentation preference. The default value is false. if you want to get more beautiful presentation,please set the value to true. |
| [getCellCssPrefix()](#getCellCssPrefix--)| Gets and sets the prefix of the css name,the default value is "". |
| [setCellCssPrefix(string)](#setCellCssPrefix-string-)| Gets and sets the prefix of the css name,the default value is "". |
| [getTableCssId()](#getTableCssId--)| Gets and sets the prefix of the type css name such as tr,col,td and so on, they are contained in the table element which has the specific TableCssId attribute. The default value is "". |
| [setTableCssId(string)](#setTableCssId-string-)| Gets and sets the prefix of the type css name such as tr,col,td and so on, they are contained in the table element which has the specific TableCssId attribute. The default value is "". |
| [isFullPathLink()](#isFullPathLink--)| Indicating whether using full path link in sheet00x.htm,filelist.xml and tabstrip.htm. The default value is false. |
| [setIsFullPathLink(boolean)](#setIsFullPathLink-boolean-)| Indicating whether using full path link in sheet00x.htm,filelist.xml and tabstrip.htm. The default value is false. |
| [getExportWorksheetCSSSeparately()](#getExportWorksheetCSSSeparately--)| Indicating whether export the worksheet css separately.The default value is false. |
| [setExportWorksheetCSSSeparately(boolean)](#setExportWorksheetCSSSeparately-boolean-)| Indicating whether export the worksheet css separately.The default value is false. |
| [getExportSimilarBorderStyle()](#getExportSimilarBorderStyle--)| Indicating whether exporting the similar border style when the border style is not supported by browsers. If you want to import the html or mht file to excel, please keep the default value. The default value is false. |
| [setExportSimilarBorderStyle(boolean)](#setExportSimilarBorderStyle-boolean-)| Indicating whether exporting the similar border style when the border style is not supported by browsers. If you want to import the html or mht file to excel, please keep the default value. The default value is false. |
| [getMergeEmptyTdForcely()](#getMergeEmptyTdForcely--)| Indicates whether merging empty TD element forcedly when exporting file to html. The size of html file will be reduced significantly after setting value to true. The default value is false. If you want to import the html file to excel or export perfect grid lines when saving file to html, please keep the default value. |
| [setMergeEmptyTdForcely(boolean)](#setMergeEmptyTdForcely-boolean-)| Indicates whether merging empty TD element forcedly when exporting file to html. The size of html file will be reduced significantly after setting value to true. The default value is false. If you want to import the html file to excel or export perfect grid lines when saving file to html, please keep the default value. |
| [getMergeEmptyTdType()](#getMergeEmptyTdType--)| The option to merge contiguous empty cells(empty td elements) The default value is MergeEmptyTdType.Default. |
| [setMergeEmptyTdType(MergeEmptyTdType)](#setMergeEmptyTdType-mergeemptytdtype-)| The option to merge contiguous empty cells(empty td elements) The default value is MergeEmptyTdType.Default. |
| [getExportCellCoordinate()](#getExportCellCoordinate--)| Indicates whether exporting excel coordinate of nonblank cells when saving file to html. The default value is false. If you want to import the output html to excel, please keep the default value. |
| [setExportCellCoordinate(boolean)](#setExportCellCoordinate-boolean-)| Indicates whether exporting excel coordinate of nonblank cells when saving file to html. The default value is false. If you want to import the output html to excel, please keep the default value. |
| [getExportExtraHeadings()](#getExportExtraHeadings--)| Indicates whether exporting extra headings when the length of text is longer than max display column. The default value is false. If you want to import the html file to excel, please keep the default value. |
| [setExportExtraHeadings(boolean)](#setExportExtraHeadings-boolean-)| Indicates whether exporting extra headings when the length of text is longer than max display column. The default value is false. If you want to import the html file to excel, please keep the default value. |
| [getExportRowColumnHeadings()](#getExportRowColumnHeadings--)| Indicates whether exports sheet's row and column headings when saving to HTML files. |
| [setExportRowColumnHeadings(boolean)](#setExportRowColumnHeadings-boolean-)| Indicates whether exports sheet's row and column headings when saving to HTML files. |
| [getExportFormula()](#getExportFormula--)| Indicates whether exporting formula when saving file to html. The default value is true. If you want to import the output html to excel, please keep the default value. |
| [setExportFormula(boolean)](#setExportFormula-boolean-)| Indicates whether exporting formula when saving file to html. The default value is true. If you want to import the output html to excel, please keep the default value. |
| [getAddTooltipText()](#getAddTooltipText--)| Indicates whether adding tooltip text when the data can't be fully displayed. The default value is false. |
| [setAddTooltipText(boolean)](#setAddTooltipText-boolean-)| Indicates whether adding tooltip text when the data can't be fully displayed. The default value is false. |
| [getExportGridLines()](#getExportGridLines--)| Indicating whether exporting the gridlines.The default value is false. |
| [setExportGridLines(boolean)](#setExportGridLines-boolean-)| Indicating whether exporting the gridlines.The default value is false. |
| [getExportBogusRowData()](#getExportBogusRowData--)| Indicating whether exporting bogus bottom row data. The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [setExportBogusRowData(boolean)](#setExportBogusRowData-boolean-)| Indicating whether exporting bogus bottom row data. The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [getExcludeUnusedStyles()](#getExcludeUnusedStyles--)| Indicating whether excludes unused styles. For the generated html files, excluding unused styles can make the file size smaller without affecting the visual effects. So the default value of this property is true. If user needs to keep all styles in the workbook for the generated html(such as the scenario that user needs to restore the workbook from the generated html later), please set this property as false. |
| [setExcludeUnusedStyles(boolean)](#setExcludeUnusedStyles-boolean-)| Indicating whether excludes unused styles. For the generated html files, excluding unused styles can make the file size smaller without affecting the visual effects. So the default value of this property is true. If user needs to keep all styles in the workbook for the generated html(such as the scenario that user needs to restore the workbook from the generated html later), please set this property as false. |
| [getExportDocumentProperties()](#getExportDocumentProperties--)| Indicating whether exporting document properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [setExportDocumentProperties(boolean)](#setExportDocumentProperties-boolean-)| Indicating whether exporting document properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [getExportWorksheetProperties()](#getExportWorksheetProperties--)| Indicating whether exporting worksheet properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [setExportWorksheetProperties(boolean)](#setExportWorksheetProperties-boolean-)| Indicating whether exporting worksheet properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [getExportWorkbookProperties()](#getExportWorkbookProperties--)| Indicating whether exporting workbook properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [setExportWorkbookProperties(boolean)](#setExportWorkbookProperties-boolean-)| Indicating whether exporting workbook properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [getExportFrameScriptsAndProperties()](#getExportFrameScriptsAndProperties--)| Indicating whether exporting frame scripts and document properties. The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [setExportFrameScriptsAndProperties(boolean)](#setExportFrameScriptsAndProperties-boolean-)| Indicating whether exporting frame scripts and document properties. The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [getExportDataOptions()](#getExportDataOptions--)| Indicating the rule of exporting html file data.The default value is All. |
| [setExportDataOptions(HtmlExportDataOptions)](#setExportDataOptions-htmlexportdataoptions-)| Indicating the rule of exporting html file data.The default value is All. |
| [getLinkTargetType()](#getLinkTargetType--)| Indicating the type of target attribute in <c>&lt;a&gt;</c> link. The default value is HtmlLinkTargetType.Parent. |
| [setLinkTargetType(HtmlLinkTargetType)](#setLinkTargetType-htmllinktargettype-)| Indicating the type of target attribute in <c>&lt;a&gt;</c> link. The default value is HtmlLinkTargetType.Parent. |
| [isIECompatible()](#isIECompatible--)| Indicating whether the output HTML is compatible with IE browser. The defalut value is false |
| [setIsIECompatible(boolean)](#setIsIECompatible-boolean-)| Indicating whether the output HTML is compatible with IE browser. The defalut value is false |
| [getFormatDataIgnoreColumnWidth()](#getFormatDataIgnoreColumnWidth--)| Indicating whether show the whole formatted data of cell when overflowing the column. If true then ignore the column width and the whole data of cell will be exported. If false then the data will be exported same as Excel. The default value is false. |
| [setFormatDataIgnoreColumnWidth(boolean)](#setFormatDataIgnoreColumnWidth-boolean-)| Indicating whether show the whole formatted data of cell when overflowing the column. If true then ignore the column width and the whole data of cell will be exported. If false then the data will be exported same as Excel. The default value is false. |
| [getCalculateFormula()](#getCalculateFormula--)| Indicates whether to calculate formulas before saving html file. |
| [setCalculateFormula(boolean)](#setCalculateFormula-boolean-)| Indicates whether to calculate formulas before saving html file. |
| [isJsBrowserCompatible()](#isJsBrowserCompatible--)| Indicates whether JavaScript is compatible with browsers that do not support JavaScript. The default value is true. |
| [setIsJsBrowserCompatible(boolean)](#setIsJsBrowserCompatible-boolean-)| Indicates whether JavaScript is compatible with browsers that do not support JavaScript. The default value is true. |
| [isMobileCompatible()](#isMobileCompatible--)| Indicates whether the output HTML is compatible with mobile devices. The default value is false. |
| [setIsMobileCompatible(boolean)](#setIsMobileCompatible-boolean-)| Indicates whether the output HTML is compatible with mobile devices. The default value is false. |
| [getCssStyles()](#getCssStyles--)| Gets or sets the additional css styles for the formatter. Only works when [SaveAsSingleFile](../saveassinglefile/) is True. <example> CssStyles="body { padding: 5px }"; </example> |
| [setCssStyles(string)](#setCssStyles-string-)| Gets or sets the additional css styles for the formatter. Only works when [SaveAsSingleFile](../saveassinglefile/) is True. <example> CssStyles="body { padding: 5px }"; </example> |
| [getHideOverflowWrappedText()](#getHideOverflowWrappedText--)| Indicates whether to hide overflow text when the cell format is set to wrap text. The default value is false |
| [setHideOverflowWrappedText(boolean)](#setHideOverflowWrappedText-boolean-)| Indicates whether to hide overflow text when the cell format is set to wrap text. The default value is false |
| [isBorderCollapsed()](#isBorderCollapsed--)| Indicates whether the table borders are collapsed. The default value is true. |
| [setIsBorderCollapsed(boolean)](#setIsBorderCollapsed-boolean-)| Indicates whether the table borders are collapsed. The default value is true. |
| [getEncodeEntityAsCode()](#getEncodeEntityAsCode--)| Indicates whether the html character entities are replaced with decimal code. (e.g. "&amp;nbsp;" is replaced with "&amp;#160;"). The default value is false. |
| [setEncodeEntityAsCode(boolean)](#setEncodeEntityAsCode-boolean-)| Indicates whether the html character entities are replaced with decimal code. (e.g. "&amp;nbsp;" is replaced with "&amp;#160;"). The default value is false. |
| [getOfficeMathOutputMode()](#getOfficeMathOutputMode--)| Indicates how export OfficeMath objects to HTML, Default value is Image. |
| [setOfficeMathOutputMode(HtmlOfficeMathOutputType)](#setOfficeMathOutputMode-htmlofficemathoutputtype-)| Indicates how export OfficeMath objects to HTML, Default value is Image. |
| [getCellNameAttribute()](#getCellNameAttribute--)| Specifies the attribute that indicates the CellName to be written. (e.g. If the value is "id", then for cell "A1", the output will be:&lt;td id='A1'&gt;). The default value is null. |
| [setCellNameAttribute(string)](#setCellNameAttribute-string-)| Specifies the attribute that indicates the CellName to be written. (e.g. If the value is "id", then for cell "A1", the output will be:&lt;td id='A1'&gt;). The default value is null. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getSaveFormat()](#getSaveFormat--)| Gets the save file format. |
| [getClearData()](#getClearData--)| Make the workbook empty after saving the file. |
| [setClearData(boolean)](#setClearData-boolean-)| Make the workbook empty after saving the file. |
| [getCachedFileFolder()](#getCachedFileFolder--)| The cached file folder is used to store some large data. |
| [setCachedFileFolder(string)](#setCachedFileFolder-string-)| The cached file folder is used to store some large data. |
| [getValidateMergedAreas()](#getValidateMergedAreas--)| Indicates whether validate merged cells before saving the file. |
| [setValidateMergedAreas(boolean)](#setValidateMergedAreas-boolean-)| Indicates whether validate merged cells before saving the file. |
| [getMergeAreas()](#getMergeAreas--)| Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [setMergeAreas(boolean)](#setMergeAreas-boolean-)| Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [getCreateDirectory()](#getCreateDirectory--)| If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [setCreateDirectory(boolean)](#setCreateDirectory-boolean-)| If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [getSortNames()](#getSortNames--)| Indicates whether sorting defined names before saving file. |
| [setSortNames(boolean)](#setSortNames-boolean-)| Indicates whether sorting defined names before saving file. |
| [getSortExternalNames()](#getSortExternalNames--)| Indicates whether sorting external defined names before saving file. |
| [setSortExternalNames(boolean)](#setSortExternalNames-boolean-)| Indicates whether sorting external defined names before saving file. |
| [getRefreshChartCache()](#getRefreshChartCache--)| Indicates whether refreshing chart cache data |
| [setRefreshChartCache(boolean)](#setRefreshChartCache-boolean-)| Indicates whether refreshing chart cache data |
| [setWarningCallback(IWarningCallback)](#setWarningCallback-iwarningcallback-)| Gets or sets warning callback. |
| [getWarningCallback()](#getWarningCallback--)| Gets or sets warning callback. |
| [getUpdateSmartArt()](#getUpdateSmartArt--)| Indicates whether updating smart art setting. The default value is false. |
| [setUpdateSmartArt(boolean)](#setUpdateSmartArt-boolean-)| Indicates whether updating smart art setting. The default value is false. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--)| Indicates whether encrypt document properties when saving as .xls file. The default value is true. |
| [setEncryptDocumentProperties(boolean)](#setEncryptDocumentProperties-boolean-)| Indicates whether encrypt document properties when saving as .xls file. The default value is true. |


### constructor() {#constructor--}

Creates options for saving html file.

```javascript
constructor();
```


### constructor(SaveOptions) {#constructor-saveoptions-}

Constructs from a parent object convertible to this.

```javascript
constructor(obj: SaveOptions);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | SaveOptions | The parent object. |

### constructor(SaveFormat) {#constructor-saveformat-}

Creates options for saving htm file.

```javascript
constructor(saveFormat: SaveFormat);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | [SaveFormat](../saveformat/) | The file format.         /// It should be one of following types: [SaveFormat.Html](../saveformat.html/), [SaveFormat.MHtml](../saveformat.mhtml/),         /// or [SaveFormat.XHtml](../saveformat.xhtml/),         /// otherwise the saved format will be set as [SaveFormat.Html](../saveformat.html/) automatically. |

### getIgnoreInvisibleShapes() {#getIgnoreInvisibleShapes--}

Indicate whether exporting those not visible shapes

```javascript
getIgnoreInvisibleShapes() : boolean;
```


**Remarks**

The default values is false.

### setIgnoreInvisibleShapes(boolean) {#setIgnoreInvisibleShapes-boolean-}

Indicate whether exporting those not visible shapes

```javascript
setIgnoreInvisibleShapes(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

The default values is false.

### getPageTitle() {#getPageTitle--}

The title of the html page. Only for saving to html stream.

```javascript
getPageTitle() : string;
```


### setPageTitle(string) {#setPageTitle-string-}

The title of the html page. Only for saving to html stream.

```javascript
setPageTitle(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getAttachedFilesDirectory() {#getAttachedFilesDirectory--}

The directory that the attached files will be saved to. Only for saving to html stream.

```javascript
getAttachedFilesDirectory() : string;
```


### setAttachedFilesDirectory(string) {#setAttachedFilesDirectory-string-}

The directory that the attached files will be saved to. Only for saving to html stream.

```javascript
setAttachedFilesDirectory(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getAttachedFilesUrlPrefix() {#getAttachedFilesUrlPrefix--}

Specify the Url prefix of attached files such as image in the html file. Only for saving to html stream.

```javascript
getAttachedFilesUrlPrefix() : string;
```


### setAttachedFilesUrlPrefix(string) {#setAttachedFilesUrlPrefix-string-}

Specify the Url prefix of attached files such as image in the html file. Only for saving to html stream.

```javascript
setAttachedFilesUrlPrefix(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getDefaultFontName() {#getDefaultFontName--}

Specify the default font name for exporting html, the default font will be used  when the font of style is not existing, If this property is null, Aspose.Cells will use universal font which have the same family with the original font, the default value is null.

```javascript
getDefaultFontName() : string;
```


### setDefaultFontName(string) {#setDefaultFontName-string-}

Specify the default font name for exporting html, the default font will be used  when the font of style is not existing, If this property is null, Aspose.Cells will use universal font which have the same family with the original font, the default value is null.

```javascript
setDefaultFontName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getAddGenericFont() {#getAddGenericFont--}

Indicates whether to add a generic font to CSS font-family. The default value is true

```javascript
getAddGenericFont() : boolean;
```


### setAddGenericFont(boolean) {#setAddGenericFont-boolean-}

Indicates whether to add a generic font to CSS font-family. The default value is true

```javascript
setAddGenericFont(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getWorksheetScalable() {#getWorksheetScalable--}

Indicates if zooming in or out the html via worksheet zoom level when saving file to html, the default value is false.

```javascript
getWorksheetScalable() : boolean;
```


### setWorksheetScalable(boolean) {#setWorksheetScalable-boolean-}

Indicates if zooming in or out the html via worksheet zoom level when saving file to html, the default value is false.

```javascript
setWorksheetScalable(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isExportComments() {#isExportComments--}

Indicates if exporting comments when saving file to html, the default value is false.

```javascript
isExportComments() : boolean;
```


### setIsExportComments(boolean) {#setIsExportComments-boolean-}

Indicates if exporting comments when saving file to html, the default value is false.

```javascript
setIsExportComments(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExportCommentsType() {#getExportCommentsType--}

Represents type of exporting comments to html files.

```javascript
getExportCommentsType() : PrintCommentsType;
```


**Returns**

[PrintCommentsType](../printcommentstype/)

### setExportCommentsType(PrintCommentsType) {#setExportCommentsType-printcommentstype-}

Represents type of exporting comments to html files.

```javascript
setExportCommentsType(value: PrintCommentsType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PrintCommentsType](../printcommentstype/) | The value to set. |

### getDisableDownlevelRevealedComments() {#getDisableDownlevelRevealedComments--}

Indicates if disable Downlevel-revealed conditional comments when exporting file to html, the default value is false.

```javascript
getDisableDownlevelRevealedComments() : boolean;
```


### setDisableDownlevelRevealedComments(boolean) {#setDisableDownlevelRevealedComments-boolean-}

Indicates if disable Downlevel-revealed conditional comments when exporting file to html, the default value is false.

```javascript
setDisableDownlevelRevealedComments(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isExpImageToTempDir() {#isExpImageToTempDir--}

Indicates whether exporting image files to temp directory. Only for saving to html stream.

```javascript
isExpImageToTempDir() : boolean;
```


### setIsExpImageToTempDir(boolean) {#setIsExpImageToTempDir-boolean-}

Indicates whether exporting image files to temp directory. Only for saving to html stream.

```javascript
setIsExpImageToTempDir(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getImageScalable() {#getImageScalable--}

Indicates whether using scalable unit to describe the image width when using scalable unit to describe the column width. The default value is true.

```javascript
getImageScalable() : boolean;
```


### setImageScalable(boolean) {#setImageScalable-boolean-}

Indicates whether using scalable unit to describe the image width when using scalable unit to describe the column width. The default value is true.

```javascript
setImageScalable(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getWidthScalable() {#getWidthScalable--}

Indicates whether exporting column width in unit of scale to html. The default value is false.

```javascript
getWidthScalable() : boolean;
```


### setWidthScalable(boolean) {#setWidthScalable-boolean-}

Indicates whether exporting column width in unit of scale to html. The default value is false.

```javascript
setWidthScalable(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExportSingleTab() {#getExportSingleTab--}

Indicates whether exporting the single tab when the file only has one worksheet. The default value is false.

```javascript
getExportSingleTab() : boolean;
```


### setExportSingleTab(boolean) {#setExportSingleTab-boolean-}

Indicates whether exporting the single tab when the file only has one worksheet. The default value is false.

```javascript
setExportSingleTab(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExportImagesAsBase64() {#getExportImagesAsBase64--}

Specifies whether images are saved in Base64 format to HTML, MHTML or EPUB.

```javascript
getExportImagesAsBase64() : boolean;
```


**Remarks**

When this property is set to true image data is exported directly on the img elements and separate files are not created.

### setExportImagesAsBase64(boolean) {#setExportImagesAsBase64-boolean-}

Specifies whether images are saved in Base64 format to HTML, MHTML or EPUB.

```javascript
setExportImagesAsBase64(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

When this property is set to true image data is exported directly on the img elements and separate files are not created.

### getExportActiveWorksheetOnly() {#getExportActiveWorksheetOnly--}

Indicates if only exporting the active worksheet to html file. If true then only the active worksheet will be exported to html file; If false then the whole workbook will be exported to html file. The default value is false.

```javascript
getExportActiveWorksheetOnly() : boolean;
```


### setExportActiveWorksheetOnly(boolean) {#setExportActiveWorksheetOnly-boolean-}

Indicates if only exporting the active worksheet to html file. If true then only the active worksheet will be exported to html file; If false then the whole workbook will be exported to html file. The default value is false.

```javascript
setExportActiveWorksheetOnly(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExportPrintAreaOnly() {#getExportPrintAreaOnly--}

Indicates if only exporting the print area to html file. The default value is false.

```javascript
getExportPrintAreaOnly() : boolean;
```


### setExportPrintAreaOnly(boolean) {#setExportPrintAreaOnly-boolean-}

Indicates if only exporting the print area to html file. The default value is false.

```javascript
setExportPrintAreaOnly(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExportArea() {#getExportArea--}

Gets or Sets the exporting CellArea of current active Worksheet. If you set this attribute, the print area of current active Worksheet will be omitted. Only the specified area will be exported when saving the file to html.

```javascript
getExportArea() : CellArea;
```


**Returns**

[CellArea](../cellarea/)

### setExportArea(CellArea) {#setExportArea-cellarea-}

Gets or Sets the exporting CellArea of current active Worksheet. If you set this attribute, the print area of current active Worksheet will be omitted. Only the specified area will be exported when saving the file to html.

```javascript
setExportArea(value: CellArea) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellArea](../cellarea/) | The value to set. |

### getParseHtmlTagInCell() {#getParseHtmlTagInCell--}

Indicates whether html tag(such as <c>&lt;div&gt;&lt;/div&gt;</c>) in cell should be parsed as cell value or preserved as it is. The default value is true.

```javascript
getParseHtmlTagInCell() : boolean;
```


### setParseHtmlTagInCell(boolean) {#setParseHtmlTagInCell-boolean-}

Indicates whether html tag(such as <c>&lt;div&gt;&lt;/div&gt;</c>) in cell should be parsed as cell value or preserved as it is. The default value is true.

```javascript
setParseHtmlTagInCell(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getHtmlCrossStringType() {#getHtmlCrossStringType--}

Indicates if a cross-cell string will be displayed in the same way as MS Excel when saving an Excel file in html format. By default the value is Default, so, for cross-cell strings, there is little difference between the html files created by Aspose.Cells and MS Excel. But the performance for creating large html files,setting the value to Cross would be several times faster than setting it to Default or Fit2Cell.

```javascript
getHtmlCrossStringType() : HtmlCrossType;
```


**Returns**

[HtmlCrossType](../htmlcrosstype/)

### setHtmlCrossStringType(HtmlCrossType) {#setHtmlCrossStringType-htmlcrosstype-}

Indicates if a cross-cell string will be displayed in the same way as MS Excel when saving an Excel file in html format. By default the value is Default, so, for cross-cell strings, there is little difference between the html files created by Aspose.Cells and MS Excel. But the performance for creating large html files,setting the value to Cross would be several times faster than setting it to Default or Fit2Cell.

```javascript
setHtmlCrossStringType(value: HtmlCrossType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [HtmlCrossType](../htmlcrosstype/) | The value to set. |

### getHiddenColDisplayType() {#getHiddenColDisplayType--}

Hidden column(the width of this column is 0) in excel,before save this into html format, if HtmlHiddenColDisplayType is "Remove",the hidden column would not been output, if the value is "Hidden", the column would been output,but was hidden,the default value is "Hidden"

```javascript
getHiddenColDisplayType() : HtmlHiddenColDisplayType;
```


**Returns**

[HtmlHiddenColDisplayType](../htmlhiddencoldisplaytype/)

### setHiddenColDisplayType(HtmlHiddenColDisplayType) {#setHiddenColDisplayType-htmlhiddencoldisplaytype-}

Hidden column(the width of this column is 0) in excel,before save this into html format, if HtmlHiddenColDisplayType is "Remove",the hidden column would not been output, if the value is "Hidden", the column would been output,but was hidden,the default value is "Hidden"

```javascript
setHiddenColDisplayType(value: HtmlHiddenColDisplayType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [HtmlHiddenColDisplayType](../htmlhiddencoldisplaytype/) | The value to set. |

### getHiddenRowDisplayType() {#getHiddenRowDisplayType--}

Hidden row(the height of this row is 0) in excel,before save this into html format, if HtmlHiddenRowDisplayType is "Remove",the hidden row would not been output, if the value is "Hidden", the row would been output,but was hidden,the default value is "Hidden"

```javascript
getHiddenRowDisplayType() : HtmlHiddenRowDisplayType;
```


**Returns**

[HtmlHiddenRowDisplayType](../htmlhiddenrowdisplaytype/)

### setHiddenRowDisplayType(HtmlHiddenRowDisplayType) {#setHiddenRowDisplayType-htmlhiddenrowdisplaytype-}

Hidden row(the height of this row is 0) in excel,before save this into html format, if HtmlHiddenRowDisplayType is "Remove",the hidden row would not been output, if the value is "Hidden", the row would been output,but was hidden,the default value is "Hidden"

```javascript
setHiddenRowDisplayType(value: HtmlHiddenRowDisplayType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [HtmlHiddenRowDisplayType](../htmlhiddenrowdisplaytype/) | The value to set. |

### getEncoding() {#getEncoding--}

If not set,use Encoding.UTF8 as default enconding type.

```javascript
getEncoding() : EncodingType;
```


**Returns**

[EncodingType](../encodingtype/)

### setEncoding(EncodingType) {#setEncoding-encodingtype-}

If not set,use Encoding.UTF8 as default enconding type.

```javascript
setEncoding(value: EncodingType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [EncodingType](../encodingtype/) | The value to set. |

### getFilePathProvider() {#getFilePathProvider--}

Gets or sets the IFilePathProvider for exporting Worksheet to html separately.

```javascript
getFilePathProvider() : IFilePathProvider;
```


**Returns**

[IFilePathProvider](../ifilepathprovider/)

### setFilePathProvider(IFilePathProvider) {#setFilePathProvider-ifilepathprovider-}

Gets or sets the IFilePathProvider for exporting Worksheet to html separately.

```javascript
setFilePathProvider(value: IFilePathProvider) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IFilePathProvider](../ifilepathprovider/) | The value to set. |

### getImageOptions() {#getImageOptions--}

Get the ImageOrPrintOptions object before exporting

```javascript
getImageOptions() : ImageOrPrintOptions;
```


**Returns**

[ImageOrPrintOptions](../imageorprintoptions/)

### getSaveAsSingleFile() {#getSaveAsSingleFile--}

Indicates whether save the html as single file. The default value is false.

```javascript
getSaveAsSingleFile() : boolean;
```


**Remarks**

If there are multiple worksheets or other required resources such as pictures in the workbook, commonly those worksheets and other resources need to be saved into separate files. For some scenarios, user maybe need to get only one resultant file such as for the convenience of transferring. If so, user may set this property as true.

### setSaveAsSingleFile(boolean) {#setSaveAsSingleFile-boolean-}

Indicates whether save the html as single file. The default value is false.

```javascript
setSaveAsSingleFile(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

If there are multiple worksheets or other required resources such as pictures in the workbook, commonly those worksheets and other resources need to be saved into separate files. For some scenarios, user maybe need to get only one resultant file such as for the convenience of transferring. If so, user may set this property as true.

### getShowAllSheets() {#getShowAllSheets--}

Indicates whether showing all sheets when saving  as a single html file.

```javascript
getShowAllSheets() : boolean;
```


**Remarks**

Only works when [SaveAsSingleFile](../saveassinglefile/) is True.

### setShowAllSheets(boolean) {#setShowAllSheets-boolean-}

Indicates whether showing all sheets when saving  as a single html file.

```javascript
setShowAllSheets(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Only works when [SaveAsSingleFile](../saveassinglefile/) is True.

### getExportPageHeaders() {#getExportPageHeaders--}

Indicates whether exporting page headers.

```javascript
getExportPageHeaders() : boolean;
```


**Remarks**

Only works when [SaveAsSingleFile](../saveassinglefile/) is True.

### setExportPageHeaders(boolean) {#setExportPageHeaders-boolean-}

Indicates whether exporting page headers.

```javascript
setExportPageHeaders(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Only works when [SaveAsSingleFile](../saveassinglefile/) is True.

### getExportPageFooters() {#getExportPageFooters--}

Indicates whether exporting page headers.

```javascript
getExportPageFooters() : boolean;
```


**Remarks**

Only works when [SaveAsSingleFile](../saveassinglefile/) is True.

### setExportPageFooters(boolean) {#setExportPageFooters-boolean-}

Indicates whether exporting page headers.

```javascript
setExportPageFooters(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Only works when [SaveAsSingleFile](../saveassinglefile/) is True.

### getExportHiddenWorksheet() {#getExportHiddenWorksheet--}

Indicating if exporting the hidden worksheet content.The default value is true.

```javascript
getExportHiddenWorksheet() : boolean;
```


### setExportHiddenWorksheet(boolean) {#setExportHiddenWorksheet-boolean-}

Indicating if exporting the hidden worksheet content.The default value is true.

```javascript
setExportHiddenWorksheet(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getPresentationPreference() {#getPresentationPreference--}

Indicating if html or mht file is presentation preference. The default value is false. if you want to get more beautiful presentation,please set the value to true.

```javascript
getPresentationPreference() : boolean;
```


### setPresentationPreference(boolean) {#setPresentationPreference-boolean-}

Indicating if html or mht file is presentation preference. The default value is false. if you want to get more beautiful presentation,please set the value to true.

```javascript
setPresentationPreference(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getCellCssPrefix() {#getCellCssPrefix--}

Gets and sets the prefix of the css name,the default value is "".

```javascript
getCellCssPrefix() : string;
```


### setCellCssPrefix(string) {#setCellCssPrefix-string-}

Gets and sets the prefix of the css name,the default value is "".

```javascript
setCellCssPrefix(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getTableCssId() {#getTableCssId--}

Gets and sets the prefix of the type css name such as tr,col,td and so on, they are contained in the table element which has the specific TableCssId attribute. The default value is "".

```javascript
getTableCssId() : string;
```


### setTableCssId(string) {#setTableCssId-string-}

Gets and sets the prefix of the type css name such as tr,col,td and so on, they are contained in the table element which has the specific TableCssId attribute. The default value is "".

```javascript
setTableCssId(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### isFullPathLink() {#isFullPathLink--}

Indicating whether using full path link in sheet00x.htm,filelist.xml and tabstrip.htm. The default value is false.

```javascript
isFullPathLink() : boolean;
```


### setIsFullPathLink(boolean) {#setIsFullPathLink-boolean-}

Indicating whether using full path link in sheet00x.htm,filelist.xml and tabstrip.htm. The default value is false.

```javascript
setIsFullPathLink(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExportWorksheetCSSSeparately() {#getExportWorksheetCSSSeparately--}

Indicating whether export the worksheet css separately.The default value is false.

```javascript
getExportWorksheetCSSSeparately() : boolean;
```


### setExportWorksheetCSSSeparately(boolean) {#setExportWorksheetCSSSeparately-boolean-}

Indicating whether export the worksheet css separately.The default value is false.

```javascript
setExportWorksheetCSSSeparately(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExportSimilarBorderStyle() {#getExportSimilarBorderStyle--}

Indicating whether exporting the similar border style when the border style is not supported by browsers. If you want to import the html or mht file to excel, please keep the default value. The default value is false.

```javascript
getExportSimilarBorderStyle() : boolean;
```


### setExportSimilarBorderStyle(boolean) {#setExportSimilarBorderStyle-boolean-}

Indicating whether exporting the similar border style when the border style is not supported by browsers. If you want to import the html or mht file to excel, please keep the default value. The default value is false.

```javascript
setExportSimilarBorderStyle(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getMergeEmptyTdForcely() {#getMergeEmptyTdForcely--}

Indicates whether merging empty TD element forcedly when exporting file to html. The size of html file will be reduced significantly after setting value to true. The default value is false. If you want to import the html file to excel or export perfect grid lines when saving file to html, please keep the default value.

```javascript
getMergeEmptyTdForcely() : boolean;
```


### setMergeEmptyTdForcely(boolean) {#setMergeEmptyTdForcely-boolean-}

Indicates whether merging empty TD element forcedly when exporting file to html. The size of html file will be reduced significantly after setting value to true. The default value is false. If you want to import the html file to excel or export perfect grid lines when saving file to html, please keep the default value.

```javascript
setMergeEmptyTdForcely(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getMergeEmptyTdType() {#getMergeEmptyTdType--}

The option to merge contiguous empty cells(empty td elements) The default value is MergeEmptyTdType.Default.

```javascript
getMergeEmptyTdType() : MergeEmptyTdType;
```


**Returns**

[MergeEmptyTdType](../mergeemptytdtype/)

### setMergeEmptyTdType(MergeEmptyTdType) {#setMergeEmptyTdType-mergeemptytdtype-}

The option to merge contiguous empty cells(empty td elements) The default value is MergeEmptyTdType.Default.

```javascript
setMergeEmptyTdType(value: MergeEmptyTdType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MergeEmptyTdType](../mergeemptytdtype/) | The value to set. |

### getExportCellCoordinate() {#getExportCellCoordinate--}

Indicates whether exporting excel coordinate of nonblank cells when saving file to html. The default value is false. If you want to import the output html to excel, please keep the default value.

```javascript
getExportCellCoordinate() : boolean;
```


### setExportCellCoordinate(boolean) {#setExportCellCoordinate-boolean-}

Indicates whether exporting excel coordinate of nonblank cells when saving file to html. The default value is false. If you want to import the output html to excel, please keep the default value.

```javascript
setExportCellCoordinate(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExportExtraHeadings() {#getExportExtraHeadings--}

Indicates whether exporting extra headings when the length of text is longer than max display column. The default value is false. If you want to import the html file to excel, please keep the default value.

```javascript
getExportExtraHeadings() : boolean;
```


### setExportExtraHeadings(boolean) {#setExportExtraHeadings-boolean-}

Indicates whether exporting extra headings when the length of text is longer than max display column. The default value is false. If you want to import the html file to excel, please keep the default value.

```javascript
setExportExtraHeadings(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExportRowColumnHeadings() {#getExportRowColumnHeadings--}

Indicates whether exports sheet's row and column headings when saving to HTML files.

```javascript
getExportRowColumnHeadings() : boolean;
```


**Remarks**

The default value is false.

### setExportRowColumnHeadings(boolean) {#setExportRowColumnHeadings-boolean-}

Indicates whether exports sheet's row and column headings when saving to HTML files.

```javascript
setExportRowColumnHeadings(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

The default value is false.

### getExportFormula() {#getExportFormula--}

Indicates whether exporting formula when saving file to html. The default value is true. If you want to import the output html to excel, please keep the default value.

```javascript
getExportFormula() : boolean;
```


### setExportFormula(boolean) {#setExportFormula-boolean-}

Indicates whether exporting formula when saving file to html. The default value is true. If you want to import the output html to excel, please keep the default value.

```javascript
setExportFormula(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getAddTooltipText() {#getAddTooltipText--}

Indicates whether adding tooltip text when the data can't be fully displayed. The default value is false.

```javascript
getAddTooltipText() : boolean;
```


### setAddTooltipText(boolean) {#setAddTooltipText-boolean-}

Indicates whether adding tooltip text when the data can't be fully displayed. The default value is false.

```javascript
setAddTooltipText(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExportGridLines() {#getExportGridLines--}

Indicating whether exporting the gridlines.The default value is false.

```javascript
getExportGridLines() : boolean;
```


### setExportGridLines(boolean) {#setExportGridLines-boolean-}

Indicating whether exporting the gridlines.The default value is false.

```javascript
setExportGridLines(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExportBogusRowData() {#getExportBogusRowData--}

Indicating whether exporting bogus bottom row data. The default value is true.If you want to import the html or mht file to excel, please keep the default value.

```javascript
getExportBogusRowData() : boolean;
```


### setExportBogusRowData(boolean) {#setExportBogusRowData-boolean-}

Indicating whether exporting bogus bottom row data. The default value is true.If you want to import the html or mht file to excel, please keep the default value.

```javascript
setExportBogusRowData(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExcludeUnusedStyles() {#getExcludeUnusedStyles--}

Indicating whether excludes unused styles. For the generated html files, excluding unused styles can make the file size smaller without affecting the visual effects. So the default value of this property is true. If user needs to keep all styles in the workbook for the generated html(such as the scenario that user needs to restore the workbook from the generated html later), please set this property as false.

```javascript
getExcludeUnusedStyles() : boolean;
```


### setExcludeUnusedStyles(boolean) {#setExcludeUnusedStyles-boolean-}

Indicating whether excludes unused styles. For the generated html files, excluding unused styles can make the file size smaller without affecting the visual effects. So the default value of this property is true. If user needs to keep all styles in the workbook for the generated html(such as the scenario that user needs to restore the workbook from the generated html later), please set this property as false.

```javascript
setExcludeUnusedStyles(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExportDocumentProperties() {#getExportDocumentProperties--}

Indicating whether exporting document properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value.

```javascript
getExportDocumentProperties() : boolean;
```


### setExportDocumentProperties(boolean) {#setExportDocumentProperties-boolean-}

Indicating whether exporting document properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value.

```javascript
setExportDocumentProperties(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExportWorksheetProperties() {#getExportWorksheetProperties--}

Indicating whether exporting worksheet properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value.

```javascript
getExportWorksheetProperties() : boolean;
```


### setExportWorksheetProperties(boolean) {#setExportWorksheetProperties-boolean-}

Indicating whether exporting worksheet properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value.

```javascript
setExportWorksheetProperties(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExportWorkbookProperties() {#getExportWorkbookProperties--}

Indicating whether exporting workbook properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value.

```javascript
getExportWorkbookProperties() : boolean;
```


### setExportWorkbookProperties(boolean) {#setExportWorkbookProperties-boolean-}

Indicating whether exporting workbook properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value.

```javascript
setExportWorkbookProperties(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExportFrameScriptsAndProperties() {#getExportFrameScriptsAndProperties--}

Indicating whether exporting frame scripts and document properties. The default value is true.If you want to import the html or mht file to excel, please keep the default value.

```javascript
getExportFrameScriptsAndProperties() : boolean;
```


### setExportFrameScriptsAndProperties(boolean) {#setExportFrameScriptsAndProperties-boolean-}

Indicating whether exporting frame scripts and document properties. The default value is true.If you want to import the html or mht file to excel, please keep the default value.

```javascript
setExportFrameScriptsAndProperties(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExportDataOptions() {#getExportDataOptions--}

Indicating the rule of exporting html file data.The default value is All.

```javascript
getExportDataOptions() : HtmlExportDataOptions;
```


**Returns**

[HtmlExportDataOptions](../htmlexportdataoptions/)

### setExportDataOptions(HtmlExportDataOptions) {#setExportDataOptions-htmlexportdataoptions-}

Indicating the rule of exporting html file data.The default value is All.

```javascript
setExportDataOptions(value: HtmlExportDataOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [HtmlExportDataOptions](../htmlexportdataoptions/) | The value to set. |

### getLinkTargetType() {#getLinkTargetType--}

Indicating the type of target attribute in <c>&lt;a&gt;</c> link. The default value is HtmlLinkTargetType.Parent.

```javascript
getLinkTargetType() : HtmlLinkTargetType;
```


**Returns**

[HtmlLinkTargetType](../htmllinktargettype/)

### setLinkTargetType(HtmlLinkTargetType) {#setLinkTargetType-htmllinktargettype-}

Indicating the type of target attribute in <c>&lt;a&gt;</c> link. The default value is HtmlLinkTargetType.Parent.

```javascript
setLinkTargetType(value: HtmlLinkTargetType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [HtmlLinkTargetType](../htmllinktargettype/) | The value to set. |

### isIECompatible() {#isIECompatible--}

Indicating whether the output HTML is compatible with IE browser. The defalut value is false

```javascript
isIECompatible() : boolean;
```


### setIsIECompatible(boolean) {#setIsIECompatible-boolean-}

Indicating whether the output HTML is compatible with IE browser. The defalut value is false

```javascript
setIsIECompatible(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getFormatDataIgnoreColumnWidth() {#getFormatDataIgnoreColumnWidth--}

Indicating whether show the whole formatted data of cell when overflowing the column. If true then ignore the column width and the whole data of cell will be exported. If false then the data will be exported same as Excel. The default value is false.

```javascript
getFormatDataIgnoreColumnWidth() : boolean;
```


### setFormatDataIgnoreColumnWidth(boolean) {#setFormatDataIgnoreColumnWidth-boolean-}

Indicating whether show the whole formatted data of cell when overflowing the column. If true then ignore the column width and the whole data of cell will be exported. If false then the data will be exported same as Excel. The default value is false.

```javascript
setFormatDataIgnoreColumnWidth(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getCalculateFormula() {#getCalculateFormula--}

Indicates whether to calculate formulas before saving html file.

```javascript
getCalculateFormula() : boolean;
```


**Remarks**

The default value is false.

### setCalculateFormula(boolean) {#setCalculateFormula-boolean-}

Indicates whether to calculate formulas before saving html file.

```javascript
setCalculateFormula(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

The default value is false.

### isJsBrowserCompatible() {#isJsBrowserCompatible--}

Indicates whether JavaScript is compatible with browsers that do not support JavaScript. The default value is true.

```javascript
isJsBrowserCompatible() : boolean;
```


### setIsJsBrowserCompatible(boolean) {#setIsJsBrowserCompatible-boolean-}

Indicates whether JavaScript is compatible with browsers that do not support JavaScript. The default value is true.

```javascript
setIsJsBrowserCompatible(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isMobileCompatible() {#isMobileCompatible--}

Indicates whether the output HTML is compatible with mobile devices. The default value is false.

```javascript
isMobileCompatible() : boolean;
```


### setIsMobileCompatible(boolean) {#setIsMobileCompatible-boolean-}

Indicates whether the output HTML is compatible with mobile devices. The default value is false.

```javascript
setIsMobileCompatible(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getCssStyles() {#getCssStyles--}

Gets or sets the additional css styles for the formatter. Only works when [SaveAsSingleFile](../saveassinglefile/) is True. <example> CssStyles="body { padding: 5px }"; </example>

```javascript
getCssStyles() : string;
```


### setCssStyles(string) {#setCssStyles-string-}

Gets or sets the additional css styles for the formatter. Only works when [SaveAsSingleFile](../saveassinglefile/) is True. <example> CssStyles="body { padding: 5px }"; </example>

```javascript
setCssStyles(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getHideOverflowWrappedText() {#getHideOverflowWrappedText--}

Indicates whether to hide overflow text when the cell format is set to wrap text. The default value is false

```javascript
getHideOverflowWrappedText() : boolean;
```


### setHideOverflowWrappedText(boolean) {#setHideOverflowWrappedText-boolean-}

Indicates whether to hide overflow text when the cell format is set to wrap text. The default value is false

```javascript
setHideOverflowWrappedText(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isBorderCollapsed() {#isBorderCollapsed--}

Indicates whether the table borders are collapsed. The default value is true.

```javascript
isBorderCollapsed() : boolean;
```


### setIsBorderCollapsed(boolean) {#setIsBorderCollapsed-boolean-}

Indicates whether the table borders are collapsed. The default value is true.

```javascript
setIsBorderCollapsed(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getEncodeEntityAsCode() {#getEncodeEntityAsCode--}

Indicates whether the html character entities are replaced with decimal code. (e.g. "&amp;nbsp;" is replaced with "&amp;#160;"). The default value is false.

```javascript
getEncodeEntityAsCode() : boolean;
```


### setEncodeEntityAsCode(boolean) {#setEncodeEntityAsCode-boolean-}

Indicates whether the html character entities are replaced with decimal code. (e.g. "&amp;nbsp;" is replaced with "&amp;#160;"). The default value is false.

```javascript
setEncodeEntityAsCode(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getOfficeMathOutputMode() {#getOfficeMathOutputMode--}

Indicates how export OfficeMath objects to HTML, Default value is Image.

```javascript
getOfficeMathOutputMode() : HtmlOfficeMathOutputType;
```


**Returns**

[HtmlOfficeMathOutputType](../htmlofficemathoutputtype/)

### setOfficeMathOutputMode(HtmlOfficeMathOutputType) {#setOfficeMathOutputMode-htmlofficemathoutputtype-}

Indicates how export OfficeMath objects to HTML, Default value is Image.

```javascript
setOfficeMathOutputMode(value: HtmlOfficeMathOutputType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [HtmlOfficeMathOutputType](../htmlofficemathoutputtype/) | The value to set. |

### getCellNameAttribute() {#getCellNameAttribute--}

Specifies the attribute that indicates the CellName to be written. (e.g. If the value is "id", then for cell "A1", the output will be:&lt;td id='A1'&gt;). The default value is null.

```javascript
getCellNameAttribute() : string;
```


### setCellNameAttribute(string) {#setCellNameAttribute-string-}

Specifies the attribute that indicates the CellName to be written. (e.g. If the value is "id", then for cell "A1", the output will be:&lt;td id='A1'&gt;). The default value is null.

```javascript
setCellNameAttribute(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```


### getSaveFormat() {#getSaveFormat--}

Gets the save file format.

```javascript
getSaveFormat() : SaveFormat;
```


**Returns**

[SaveFormat](../saveformat/)

### getClearData() {#getClearData--}

Make the workbook empty after saving the file.

```javascript
getClearData() : boolean;
```


### setClearData(boolean) {#setClearData-boolean-}

Make the workbook empty after saving the file.

```javascript
setClearData(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getCachedFileFolder() {#getCachedFileFolder--}

The cached file folder is used to store some large data.

```javascript
getCachedFileFolder() : string;
```


### setCachedFileFolder(string) {#setCachedFileFolder-string-}

The cached file folder is used to store some large data.

```javascript
setCachedFileFolder(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getValidateMergedAreas() {#getValidateMergedAreas--}

Indicates whether validate merged cells before saving the file.

```javascript
getValidateMergedAreas() : boolean;
```


**Remarks**

The default value is false.

### setValidateMergedAreas(boolean) {#setValidateMergedAreas-boolean-}

Indicates whether validate merged cells before saving the file.

```javascript
setValidateMergedAreas(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

The default value is false.

### getMergeAreas() {#getMergeAreas--}

Indicates whether merge the areas of conditional formatting and validation before saving the file.

```javascript
getMergeAreas() : boolean;
```


**Remarks**

The default value is false.

### setMergeAreas(boolean) {#setMergeAreas-boolean-}

Indicates whether merge the areas of conditional formatting and validation before saving the file.

```javascript
setMergeAreas(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

The default value is false.

### getCreateDirectory() {#getCreateDirectory--}

If true and the directory does not exist, the directory will be automatically created before saving the file.

```javascript
getCreateDirectory() : boolean;
```


**Remarks**

The default value is false.

### setCreateDirectory(boolean) {#setCreateDirectory-boolean-}

If true and the directory does not exist, the directory will be automatically created before saving the file.

```javascript
setCreateDirectory(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

The default value is false.

### getSortNames() {#getSortNames--}

Indicates whether sorting defined names before saving file.

```javascript
getSortNames() : boolean;
```


### setSortNames(boolean) {#setSortNames-boolean-}

Indicates whether sorting defined names before saving file.

```javascript
setSortNames(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getSortExternalNames() {#getSortExternalNames--}

Indicates whether sorting external defined names before saving file.

```javascript
getSortExternalNames() : boolean;
```


### setSortExternalNames(boolean) {#setSortExternalNames-boolean-}

Indicates whether sorting external defined names before saving file.

```javascript
setSortExternalNames(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getRefreshChartCache() {#getRefreshChartCache--}

Indicates whether refreshing chart cache data

```javascript
getRefreshChartCache() : boolean;
```


### setRefreshChartCache(boolean) {#setRefreshChartCache-boolean-}

Indicates whether refreshing chart cache data

```javascript
setRefreshChartCache(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### setWarningCallback(IWarningCallback) {#setWarningCallback-iwarningcallback-}

Gets or sets warning callback.

```javascript
setWarningCallback(value: IWarningCallback) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IWarningCallback](../iwarningcallback/) | The value to set. |

### getWarningCallback() {#getWarningCallback--}

Gets or sets warning callback.

```javascript
getWarningCallback() : IWarningCallback;
```


**Returns**

[IWarningCallback](../iwarningcallback/)

### getUpdateSmartArt() {#getUpdateSmartArt--}

Indicates whether updating smart art setting. The default value is false.

```javascript
getUpdateSmartArt() : boolean;
```


**Remarks**

Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

### setUpdateSmartArt(boolean) {#setUpdateSmartArt-boolean-}

Indicates whether updating smart art setting. The default value is false.

```javascript
setUpdateSmartArt(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}

Indicates whether encrypt document properties when saving as .xls file. The default value is true.

```javascript
getEncryptDocumentProperties() : boolean;
```


**Remarks**

Only for .xls,xlsx,xlsb and xlsm file.

### setEncryptDocumentProperties(boolean) {#setEncryptDocumentProperties-boolean-}

Indicates whether encrypt document properties when saving as .xls file. The default value is true.

```javascript
setEncryptDocumentProperties(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Only for .xls,xlsx,xlsb and xlsm file.


