---
title: "HtmlSaveOptions"
linktitle: "HtmlSaveOptions"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents the options for saving html file."
type: docs
weight: 1810
url: /nodejs/aspose.cells/htmlsaveoptions/
---

## HtmlSaveOptions class

Represents the options for saving html file.

```js
new HtmlSaveOptions()
```

Creates options for saving html file.

## Methods

| Name | Description |
| --- | --- |
| [constructor_overload$1(saveFormat)](#constructor-overload1) | Creates options for saving htm file. |
| [getAddGenericFont()](#getaddgenericfont) | Indicates whether to add a generic font to CSS font-family. The default value is true |
| [getAddTooltipText()](#getaddtooltiptext) | Indicates whether adding tooltip text when the data can't be fully displayed. The default value is false. |
| [getAttachedFilesDirectory()](#getattachedfilesdirectory) | The directory that the attached files will be saved to. Only for saving to html stream. |
| [getAttachedFilesUrlPrefix()](#getattachedfilesurlprefix) | Specify the Url prefix of attached files such as image in the html file. Only for saving to html stream. |
| [getCachedFileFolder()](#getcachedfilefolder) | The cached file folder is used to store some large data. |
| [getCalculateFormula()](#getcalculateformula) | Indicates whether to calculate formulas before saving html file. The default value is false. |
| [getCellCssPrefix()](#getcellcssprefix) | Gets and sets the prefix of the css name,the default value is "". |
| [getCellNameAttribute()](#getcellnameattribute) |  |
| [getCheckExcelRestriction()](#getcheckexcelrestriction) |  |
| [getClearData()](#getcleardata) | Make the workbook empty after saving the file. |
| [getCreateDirectory()](#getcreatedirectory) | If true and the directory does not exist, the directory will be automatically created before saving the file. The defaul |
| [getCssStyles()](#getcssstyles) | Gets or sets the additional css styles for the formatter. Only works when SaveAsSingleFile is True. Example: CssStyles=" |
| [getDataBarRenderMode()](#getdatabarrendermode) | The value of the property is DataBarRenderMode integer constant. |
| [getDefaultFontName()](#getdefaultfontname) | Specify the default font name for exporting html, the default font will be used when the font of style is not existing,  |
| [getDisableCss()](#getdisablecss) |  |
| [getDisableDownlevelRevealedComments()](#getdisabledownlevelrevealedcomments) | Indicates if disable Downlevel-revealed conditional comments when exporting file to html, the default value is false. |
| [getEmbeddedFontType()](#getembeddedfonttype) | The value of the property is HtmlEmbeddedFontType integer constant. |
| [getEnableCssCustomProperties()](#getenablecsscustomproperties) |  |
| [getEncodeEntityAsCode()](#getencodeentityascode) |  |
| [getEncoding()](#getencoding) | If not set,use Encoding.UTF8 as default enconding type. |
| [getEncryptDocumentProperties()](#getencryptdocumentproperties) |  |
| [getExcludeUnusedStyles()](#getexcludeunusedstyles) | Indicating whether excludes unused styles. For the generated html files, excluding unused styles can make the file size  |
| [getExportActiveWorksheetOnly()](#getexportactiveworksheetonly) | Indicates if only exporting the active worksheet to html file. If true then only the active worksheet will be exported t |
| [getExportArea()](#getexportarea) | Gets or Sets the exporting CellArea of current active Worksheet. If you set this attribute, the print area of current ac |
| [getExportBogusRowData()](#getexportbogusrowdata) | Indicating whether exporting bogus bottom row data. The default value is true.If you want to import the html or mht file |
| [getExportCellCoordinate()](#getexportcellcoordinate) | Indicates whether exporting excel coordinate of nonblank cells when saving file to html. The default value is false. If  |
| [getExportCommentsType()](#getexportcommentstype) | Represents type of exporting comments to html files. The value of the property is PrintCommentsType integer constant. |
| [getExportDataOptions()](#getexportdataoptions) | Indicating the rule of exporting html file data.The default value is All. The value of the property is HtmlExportDataOpt |
| [getExportDocumentProperties()](#getexportdocumentproperties) | Indicating whether exporting document properties.The default value is true.If you want to import the html or mht file to |
| [getExportExtraHeadings()](#getexportextraheadings) | Indicates whether exporting extra headings when the length of text is longer than max display column. The default value  |
| [getExportFormula()](#getexportformula) | Indicates whether exporting formula when saving file to html. The default value is true. If you want to import the outpu |
| [getExportFrameScriptsAndProperties()](#getexportframescriptsandproperties) | Indicating whether exporting frame scripts and document properties. The default value is true.If you want to import the  |
| [getExportGridLines()](#getexportgridlines) | Indicating whether exporting the gridlines.The default value is false. |
| [getExportHeadings()](#getexportheadings) | Indicates whether exports sheet's row and column headings when saving to HTML files. NOTE: This member is now obsolete.  |
| [getExportHiddenWorksheet()](#getexporthiddenworksheet) | Indicating if exporting the hidden worksheet content.The default value is true. |
| [getExportImagesAsBase64()](#getexportimagesasbase64) | Specifies whether images are saved in Base64 format to HTML, MHTML or EPUB. When this property is set to true image data |
| [getExportNamedRangeAnchors()](#getexportnamedrangeanchors) |  |
| [getExportObjectListener()](#getexportobjectlistener) | Gets or sets the ExportObjectListener for exporting objects. NOTE: This property is now obsolete. Instead, please use Ht |
| [getExportPageFooters()](#getexportpagefooters) | Indicates whether exporting page headers. Only works when SaveAsSingleFile is True. |
| [getExportPageHeaders()](#getexportpageheaders) | Indicates whether exporting page headers. Only works when SaveAsSingleFile is True. |
| [getExportPrintAreaOnly()](#getexportprintareaonly) | Indicates if only exporting the print area to html file. The default value is false. |
| [getExportRowColumnHeadings()](#getexportrowcolumnheadings) | Indicates whether exports sheet's row and column headings when saving to HTML files. The default value is false. |
| [getExportSimilarBorderStyle()](#getexportsimilarborderstyle) | Indicating whether exporting the similar border style when the border style is not supported by browsers. If you want to |
| [getExportSingleTab()](#getexportsingletab) | Indicates whether exporting the single tab when the file only has one worksheet. The default value is false. |
| [getExportWorkbookProperties()](#getexportworkbookproperties) | Indicating whether exporting workbook properties.The default value is true.If you want to import the html or mht file to |
| [getExportWorksheetCSSSeparately()](#getexportworksheetcssseparately) | Indicating whether export the worksheet css separately.The default value is false. |
| [getExportWorksheetProperties()](#getexportworksheetproperties) | Indicating whether exporting worksheet properties.The default value is true.If you want to import the html or mht file t |
| [getFilePathProvider()](#getfilepathprovider) | Gets or sets the IFilePathProvider for exporting Worksheet to html separately. |
| [getFormatDataIgnoreColumnWidth()](#getformatdataignorecolumnwidth) | Indicating whether show the whole formatted data of cell when overflowing the column. If true then ignore the column wid |
| [getHiddenColDisplayType()](#gethiddencoldisplaytype) | Hidden column(the width of this column is 0) in excel,before save this into html format, if HtmlHiddenColDisplayType is  |
| [getHiddenRowDisplayType()](#gethiddenrowdisplaytype) | Hidden row(the height of this row is 0) in excel,before save this into html format, if HtmlHiddenRowDisplayType is "Remo |
| [getHideOverflowWrappedText()](#gethideoverflowwrappedtext) | Indicates whether to hide overflow text when the cell format is set to wrap text. The default value is false |
| [getHtmlCrossStringType()](#gethtmlcrossstringtype) | Indicates if a cross-cell string will be displayed in the same way as MS Excel when saving an Excel file in html format. |
| [getHtmlVersion()](#gethtmlversion) | The value of the property is HtmlVersion integer constant. |
| [getIgnoreInvisibleShapes()](#getignoreinvisibleshapes) | Indicate whether exporting those not visible shapes The default values is false. |
| [getImageOptions()](#getimageoptions) | Get the ImageOrPrintOptions object before exporting |
| [getImageScalable()](#getimagescalable) | Indicates whether using scalable unit to describe the image width when using scalable unit to describe the column width. |
| [getLayoutMode()](#getlayoutmode) | The value of the property is HtmlLayoutMode integer constant. |
| [getLinkTargetType()](#getlinktargettype) | Indicating the type of target attribute in link. The default value is HtmlLinkTargetType.Parent. The value of the proper |
| [getMergeAreas()](#getmergeareas) | Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is  |
| [getMergeEmptyTdForcely()](#getmergeemptytdforcely) | Indicates whether merging empty TD element forcedly when exporting file to html. The size of html file will be reduced s |
| [getMergeEmptyTdType()](#getmergeemptytdtype) | The option to merge contiguous empty cells(empty td elements) The default value is MergeEmptyTdType.Default. The value o |
| [getOfficeMathOutputMode()](#getofficemathoutputmode) | The value of the property is HtmlOfficeMathOutputType integer constant. |
| [getPageTitle()](#getpagetitle) | The title of the html page. Only for saving to html stream. |
| [getParseHtmlTagInCell()](#getparsehtmltagincell) | Indicates whether html tag(such as ) in cell should be parsed as cell value or preserved as it is. The default value is  |
| [getPresentationPreference()](#getpresentationpreference) | Indicating if html or mht file is presentation preference. The default value is false. if you want to get more beautiful |
| [getRefreshChartCache()](#getrefreshchartcache) | Indicates whether refreshing chart cache data |
| [getSaveAsSingleFile()](#getsaveassinglefile) | Indicates whether save the html as single file. The default value is false. If there are multiple worksheets or other re |
| [getSaveFormat()](#getsaveformat) | Gets the save file format. The value of the property is SaveFormat integer constant. |
| [getSheetSet()](#getsheetset) |  |
| [getShowAllSheets()](#getshowallsheets) | Indicates whether showing all sheets when saving as a single html file. Only works when SaveAsSingleFile is True. |
| [getSortExternalNames()](#getsortexternalnames) | Indicates whether sorting external defined names before saving file. |
| [getSortNames()](#getsortnames) | Indicates whether sorting defined names before saving file. |
| [getSpaceMode()](#getspacemode) | The value of the property is HtmlSpaceMode integer constant. |
| [getTableCssId()](#gettablecssid) | Gets and sets the prefix of the type css name such as tr,col,td and so on, they are contained in the table element which |
| [getUpdateSmartArt()](#getupdatesmartart) | Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSm |
| [getValidateMergedAreas()](#getvalidatemergedareas) | Indicates whether validate merged cells before saving the file. The default value is false. |
| [getWarningCallback()](#getwarningcallback) | Gets or sets warning callback. |
| [getWidthScalable()](#getwidthscalable) | Indicates whether exporting column width in unit of scale to html. The default value is false. |
| [getWorksheetScalable()](#getworksheetscalable) | Indicates if zooming in or out the html via worksheet zoom level when saving file to html, the default value is false. |
| [isBorderCollapsed()](#isbordercollapsed) | Indicates whether the table borders are collapsed. The default value is true. |
| [isExpImageToTempDir()](#isexpimagetotempdir) | Indicates whether exporting image files to temp directory. Only for saving to html stream. |
| [isExportComments()](#isexportcomments) | Indicates if exporting comments when saving file to html, the default value is false. |
| [isFullPathLink()](#isfullpathlink) | Indicating whether using full path link in sheet00x.htm,filelist.xml and tabstrip.htm. The default value is false. |
| [isIECompatible()](#isiecompatible) | Indicating whether the output HTML is compatible with IE browser. The defalut value is false |
| [isJsBrowserCompatible()](#isjsbrowsercompatible) | Indicates whether JavaScript is compatible with browsers that do not support JavaScript. The default value is true. |
| [isMobileCompatible()](#ismobilecompatible) | Indicates whether the output HTML is compatible with mobile devices. The default value is false. |
| [setAddGenericFont()](#setaddgenericfont) | Indicates whether to add a generic font to CSS font-family. The default value is true |
| [setAddTooltipText()](#setaddtooltiptext) | Indicates whether adding tooltip text when the data can't be fully displayed. The default value is false. |
| [setAttachedFilesDirectory()](#setattachedfilesdirectory) | The directory that the attached files will be saved to. Only for saving to html stream. |
| [setAttachedFilesUrlPrefix()](#setattachedfilesurlprefix) | Specify the Url prefix of attached files such as image in the html file. Only for saving to html stream. |
| [setBorderCollapsed()](#setbordercollapsed) | Indicates whether the table borders are collapsed. The default value is true. |
| [setCachedFileFolder()](#setcachedfilefolder) | The cached file folder is used to store some large data. |
| [setCalculateFormula()](#setcalculateformula) | Indicates whether to calculate formulas before saving html file. The default value is false. |
| [setCellCssPrefix()](#setcellcssprefix) | Gets and sets the prefix of the css name,the default value is "". |
| [setCellNameAttribute()](#setcellnameattribute) |  |
| [setCheckExcelRestriction()](#setcheckexcelrestriction) |  |
| [setClearData()](#setcleardata) | Make the workbook empty after saving the file. |
| [setCreateDirectory()](#setcreatedirectory) | If true and the directory does not exist, the directory will be automatically created before saving the file. The defaul |
| [setCssStyles()](#setcssstyles) | Gets or sets the additional css styles for the formatter. Only works when SaveAsSingleFile is True. Example: CssStyles=" |
| [setDataBarRenderMode()](#setdatabarrendermode) | The value of the property is DataBarRenderMode integer constant. |
| [setDefaultFontName()](#setdefaultfontname) | Specify the default font name for exporting html, the default font will be used when the font of style is not existing,  |
| [setDisableCss()](#setdisablecss) |  |
| [setDisableDownlevelRevealedComments()](#setdisabledownlevelrevealedcomments) | Indicates if disable Downlevel-revealed conditional comments when exporting file to html, the default value is false. |
| [setEmbeddedFontType()](#setembeddedfonttype) | The value of the property is HtmlEmbeddedFontType integer constant. |
| [setEnableCssCustomProperties()](#setenablecsscustomproperties) |  |
| [setEncodeEntityAsCode()](#setencodeentityascode) |  |
| [setEncoding()](#setencoding) | If not set,use Encoding.UTF8 as default enconding type. |
| [setEncryptDocumentProperties()](#setencryptdocumentproperties) |  |
| [setExcludeUnusedStyles()](#setexcludeunusedstyles) | Indicating whether excludes unused styles. For the generated html files, excluding unused styles can make the file size  |
| [setExpImageToTempDir()](#setexpimagetotempdir) | Indicates whether exporting image files to temp directory. Only for saving to html stream. |
| [setExportActiveWorksheetOnly()](#setexportactiveworksheetonly) | Indicates if only exporting the active worksheet to html file. If true then only the active worksheet will be exported t |
| [setExportArea()](#setexportarea) | Gets or Sets the exporting CellArea of current active Worksheet. If you set this attribute, the print area of current ac |
| [setExportBogusRowData()](#setexportbogusrowdata) | Indicating whether exporting bogus bottom row data. The default value is true.If you want to import the html or mht file |
| [setExportCellCoordinate()](#setexportcellcoordinate) | Indicates whether exporting excel coordinate of nonblank cells when saving file to html. The default value is false. If  |
| [setExportComments()](#setexportcomments) | Indicates if exporting comments when saving file to html, the default value is false. |
| [setExportCommentsType()](#setexportcommentstype) | Represents type of exporting comments to html files. The value of the property is PrintCommentsType integer constant. |
| [setExportDataOptions()](#setexportdataoptions) | Indicating the rule of exporting html file data.The default value is All. The value of the property is HtmlExportDataOpt |
| [setExportDocumentProperties()](#setexportdocumentproperties) | Indicating whether exporting document properties.The default value is true.If you want to import the html or mht file to |
| [setExportExtraHeadings()](#setexportextraheadings) | Indicates whether exporting extra headings when the length of text is longer than max display column. The default value  |
| [setExportFormula()](#setexportformula) | Indicates whether exporting formula when saving file to html. The default value is true. If you want to import the outpu |
| [setExportFrameScriptsAndProperties()](#setexportframescriptsandproperties) | Indicating whether exporting frame scripts and document properties. The default value is true.If you want to import the  |
| [setExportGridLines()](#setexportgridlines) | Indicating whether exporting the gridlines.The default value is false. |
| [setExportHeadings()](#setexportheadings) | Indicates whether exports sheet's row and column headings when saving to HTML files. NOTE: This member is now obsolete.  |
| [setExportHiddenWorksheet()](#setexporthiddenworksheet) | Indicating if exporting the hidden worksheet content.The default value is true. |
| [setExportImagesAsBase64()](#setexportimagesasbase64) | Specifies whether images are saved in Base64 format to HTML, MHTML or EPUB. When this property is set to true image data |
| [setExportNamedRangeAnchors()](#setexportnamedrangeanchors) |  |
| [setExportObjectListener()](#setexportobjectlistener) | Gets or sets the ExportObjectListener for exporting objects. NOTE: This property is now obsolete. Instead, please use Ht |
| [setExportPageFooters()](#setexportpagefooters) | Indicates whether exporting page headers. Only works when SaveAsSingleFile is True. |
| [setExportPageHeaders()](#setexportpageheaders) | Indicates whether exporting page headers. Only works when SaveAsSingleFile is True. |
| [setExportPrintAreaOnly()](#setexportprintareaonly) | Indicates if only exporting the print area to html file. The default value is false. |
| [setExportRowColumnHeadings()](#setexportrowcolumnheadings) | Indicates whether exports sheet's row and column headings when saving to HTML files. The default value is false. |
| [setExportSimilarBorderStyle()](#setexportsimilarborderstyle) | Indicating whether exporting the similar border style when the border style is not supported by browsers. If you want to |
| [setExportSingleTab()](#setexportsingletab) | Indicates whether exporting the single tab when the file only has one worksheet. The default value is false. |
| [setExportWorkbookProperties()](#setexportworkbookproperties) | Indicating whether exporting workbook properties.The default value is true.If you want to import the html or mht file to |
| [setExportWorksheetCSSSeparately()](#setexportworksheetcssseparately) | Indicating whether export the worksheet css separately.The default value is false. |
| [setExportWorksheetProperties()](#setexportworksheetproperties) | Indicating whether exporting worksheet properties.The default value is true.If you want to import the html or mht file t |
| [setFilePathProvider()](#setfilepathprovider) | Gets or sets the IFilePathProvider for exporting Worksheet to html separately. |
| [setFormatDataIgnoreColumnWidth()](#setformatdataignorecolumnwidth) | Indicating whether show the whole formatted data of cell when overflowing the column. If true then ignore the column wid |
| [setFullPathLink()](#setfullpathlink) | Indicating whether using full path link in sheet00x.htm,filelist.xml and tabstrip.htm. The default value is false. |
| [setHiddenColDisplayType()](#sethiddencoldisplaytype) | Hidden column(the width of this column is 0) in excel,before save this into html format, if HtmlHiddenColDisplayType is  |
| [setHiddenRowDisplayType()](#sethiddenrowdisplaytype) | Hidden row(the height of this row is 0) in excel,before save this into html format, if HtmlHiddenRowDisplayType is "Remo |
| [setHideOverflowWrappedText()](#sethideoverflowwrappedtext) | Indicates whether to hide overflow text when the cell format is set to wrap text. The default value is false |
| [setHtmlCrossStringType()](#sethtmlcrossstringtype) | Indicates if a cross-cell string will be displayed in the same way as MS Excel when saving an Excel file in html format. |
| [setHtmlVersion()](#sethtmlversion) | The value of the property is HtmlVersion integer constant. |
| [setIECompatible()](#setiecompatible) | Indicating whether the output HTML is compatible with IE browser. The defalut value is false |
| [setIgnoreInvisibleShapes()](#setignoreinvisibleshapes) | Indicate whether exporting those not visible shapes The default values is false. |
| [setImageScalable()](#setimagescalable) | Indicates whether using scalable unit to describe the image width when using scalable unit to describe the column width. |
| [setJsBrowserCompatible()](#setjsbrowsercompatible) | Indicates whether JavaScript is compatible with browsers that do not support JavaScript. The default value is true. |
| [setLayoutMode()](#setlayoutmode) | The value of the property is HtmlLayoutMode integer constant. |
| [setLinkTargetType()](#setlinktargettype) | Indicating the type of target attribute in link. The default value is HtmlLinkTargetType.Parent. The value of the proper |
| [setMergeAreas()](#setmergeareas) | Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is  |
| [setMergeEmptyTdForcely()](#setmergeemptytdforcely) | Indicates whether merging empty TD element forcedly when exporting file to html. The size of html file will be reduced s |
| [setMergeEmptyTdType()](#setmergeemptytdtype) | The option to merge contiguous empty cells(empty td elements) The default value is MergeEmptyTdType.Default. The value o |
| [setMobileCompatible()](#setmobilecompatible) | Indicates whether the output HTML is compatible with mobile devices. The default value is false. |
| [setOfficeMathOutputMode()](#setofficemathoutputmode) | The value of the property is HtmlOfficeMathOutputType integer constant. |
| [setPageTitle()](#setpagetitle) | The title of the html page. Only for saving to html stream. |
| [setParseHtmlTagInCell()](#setparsehtmltagincell) | Indicates whether html tag(such as ) in cell should be parsed as cell value or preserved as it is. The default value is  |
| [setPresentationPreference()](#setpresentationpreference) | Indicating if html or mht file is presentation preference. The default value is false. if you want to get more beautiful |
| [setRefreshChartCache()](#setrefreshchartcache) | Indicates whether refreshing chart cache data |
| [setSaveAsSingleFile()](#setsaveassinglefile) | Indicates whether save the html as single file. The default value is false. If there are multiple worksheets or other re |
| [setSheetSet()](#setsheetset) |  |
| [setShowAllSheets()](#setshowallsheets) | Indicates whether showing all sheets when saving as a single html file. Only works when SaveAsSingleFile is True. |
| [setSortExternalNames()](#setsortexternalnames) | Indicates whether sorting external defined names before saving file. |
| [setSortNames()](#setsortnames) | Indicates whether sorting defined names before saving file. |
| [setSpaceMode()](#setspacemode) | The value of the property is HtmlSpaceMode integer constant. |
| [setTableCssId()](#settablecssid) | Gets and sets the prefix of the type css name such as tr,col,td and so on, they are contained in the table element which |
| [setUpdateSmartArt()](#setupdatesmartart) | Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSm |
| [setValidateMergedAreas()](#setvalidatemergedareas) | Indicates whether validate merged cells before saving the file. The default value is false. |
| [setWarningCallback()](#setwarningcallback) | Gets or sets warning callback. |
| [setWidthScalable()](#setwidthscalable) | Indicates whether exporting column width in unit of scale to html. The default value is false. |
| [setWorksheetScalable()](#setworksheetscalable) | Indicates if zooming in or out the html via worksheet zoom level when saving file to html, the default value is false. |

### constructor_overload$1(saveFormat) {#constructor-overload1}

Creates options for saving htm file.

| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | Number | SaveFormat |

### getAddGenericFont() {#getaddgenericfont}

Indicates whether to add a generic font to CSS font-family. The default value is true

### getAddTooltipText() {#getaddtooltiptext}

Indicates whether adding tooltip text when the data can't be fully displayed. The default value is false.

### getAttachedFilesDirectory() {#getattachedfilesdirectory}

The directory that the attached files will be saved to. Only for saving to html stream.

### getAttachedFilesUrlPrefix() {#getattachedfilesurlprefix}

Specify the Url prefix of attached files such as image in the html file. Only for saving to html stream.

### getCachedFileFolder() {#getcachedfilefolder}

The cached file folder is used to store some large data.

### getCalculateFormula() {#getcalculateformula}

Indicates whether to calculate formulas before saving html file. The default value is false.

### getCellCssPrefix() {#getcellcssprefix}

Gets and sets the prefix of the css name,the default value is "".

### getCellNameAttribute() {#getcellnameattribute}

### getCheckExcelRestriction() {#getcheckexcelrestriction}

### getClearData() {#getcleardata}

Make the workbook empty after saving the file.

### getCreateDirectory() {#getcreatedirectory}

If true and the directory does not exist, the directory will be automatically created before saving the file. The default value is false.

### getCssStyles() {#getcssstyles}

Gets or sets the additional css styles for the formatter. Only works when SaveAsSingleFile is True. Example: CssStyles="body { padding: 5px }";

### getDataBarRenderMode() {#getdatabarrendermode}

The value of the property is DataBarRenderMode integer constant.

### getDefaultFontName() {#getdefaultfontname}

Specify the default font name for exporting html, the default font will be used when the font of style is not existing, If this property is null, Aspose.Cells will use universal font which have the same family with the original font, the default value is null.

### getDisableCss() {#getdisablecss}

### getDisableDownlevelRevealedComments() {#getdisabledownlevelrevealedcomments}

Indicates if disable Downlevel-revealed conditional comments when exporting file to html, the default value is false.

### getEmbeddedFontType() {#getembeddedfonttype}

The value of the property is HtmlEmbeddedFontType integer constant.

### getEnableCssCustomProperties() {#getenablecsscustomproperties}

### getEncodeEntityAsCode() {#getencodeentityascode}

### getEncoding() {#getencoding}

If not set,use Encoding.UTF8 as default enconding type.

### getEncryptDocumentProperties() {#getencryptdocumentproperties}

### getExcludeUnusedStyles() {#getexcludeunusedstyles}

Indicating whether excludes unused styles. For the generated html files, excluding unused styles can make the file size smaller without affecting the visual effects. So the default value of this property is true. If user needs to keep all styles in the workbook for the generated html(such as the scenario that user needs to restore the workbook from the generated html later), please set this property as false.

### getExportActiveWorksheetOnly() {#getexportactiveworksheetonly}

Indicates if only exporting the active worksheet to html file. If true then only the active worksheet will be exported to html file; If false then the whole workbook will be exported to html file. The default value is false.

### getExportArea() {#getexportarea}

Gets or Sets the exporting CellArea of current active Worksheet. If you set this attribute, the print area of current active Worksheet will be omitted. Only the specified area will be exported when saving the file to html.

### getExportBogusRowData() {#getexportbogusrowdata}

Indicating whether exporting bogus bottom row data. The default value is true.If you want to import the html or mht file to excel, please keep the default value.

### getExportCellCoordinate() {#getexportcellcoordinate}

Indicates whether exporting excel coordinate of nonblank cells when saving file to html. The default value is false. If you want to import the output html to excel, please keep the default value.

### getExportCommentsType() {#getexportcommentstype}

Represents type of exporting comments to html files. The value of the property is PrintCommentsType integer constant.

### getExportDataOptions() {#getexportdataoptions}

Indicating the rule of exporting html file data.The default value is All. The value of the property is HtmlExportDataOptions integer constant.

### getExportDocumentProperties() {#getexportdocumentproperties}

Indicating whether exporting document properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value.

### getExportExtraHeadings() {#getexportextraheadings}

Indicates whether exporting extra headings when the length of text is longer than max display column. The default value is false. If you want to import the html file to excel, please keep the default value.

### getExportFormula() {#getexportformula}

Indicates whether exporting formula when saving file to html. The default value is true. If you want to import the output html to excel, please keep the default value.

### getExportFrameScriptsAndProperties() {#getexportframescriptsandproperties}

Indicating whether exporting frame scripts and document properties. The default value is true.If you want to import the html or mht file to excel, please keep the default value.

### getExportGridLines() {#getexportgridlines}

Indicating whether exporting the gridlines.The default value is false.

### getExportHeadings() {#getexportheadings}

Indicates whether exports sheet's row and column headings when saving to HTML files. NOTE: This member is now obsolete. Instead, please use HtmlSaveOptions.ExportRowColumnHeadings property. This property will be removed 12 months later since June 2022. Aspose apologizes for any inconvenience you may have experienced.

### getExportHiddenWorksheet() {#getexporthiddenworksheet}

Indicating if exporting the hidden worksheet content.The default value is true.

### getExportImagesAsBase64() {#getexportimagesasbase64}

Specifies whether images are saved in Base64 format to HTML, MHTML or EPUB. When this property is set to true image data is exported directly on the img elements and separate files are not created.

### getExportNamedRangeAnchors() {#getexportnamedrangeanchors}

### getExportObjectListener() {#getexportobjectlistener}

Gets or sets the ExportObjectListener for exporting objects. NOTE: This property is now obsolete. Instead, please use HtmlSaveOptions.IStreamProvider property. This property will be removed 12 months later since August 2015. Aspose apologizes for any inconvenience you may have experienced.

### getExportPageFooters() {#getexportpagefooters}

Indicates whether exporting page headers. Only works when SaveAsSingleFile is True.

### getExportPageHeaders() {#getexportpageheaders}

Indicates whether exporting page headers. Only works when SaveAsSingleFile is True.

### getExportPrintAreaOnly() {#getexportprintareaonly}

Indicates if only exporting the print area to html file. The default value is false.

### getExportRowColumnHeadings() {#getexportrowcolumnheadings}

Indicates whether exports sheet's row and column headings when saving to HTML files. The default value is false.

### getExportSimilarBorderStyle() {#getexportsimilarborderstyle}

Indicating whether exporting the similar border style when the border style is not supported by browsers. If you want to import the html or mht file to excel, please keep the default value. The default value is false.

### getExportSingleTab() {#getexportsingletab}

Indicates whether exporting the single tab when the file only has one worksheet. The default value is false.

### getExportWorkbookProperties() {#getexportworkbookproperties}

Indicating whether exporting workbook properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value.

### getExportWorksheetCSSSeparately() {#getexportworksheetcssseparately}

Indicating whether export the worksheet css separately.The default value is false.

### getExportWorksheetProperties() {#getexportworksheetproperties}

Indicating whether exporting worksheet properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value.

### getFilePathProvider() {#getfilepathprovider}

Gets or sets the IFilePathProvider for exporting Worksheet to html separately.

### getFormatDataIgnoreColumnWidth() {#getformatdataignorecolumnwidth}

Indicating whether show the whole formatted data of cell when overflowing the column. If true then ignore the column width and the whole data of cell will be exported. If false then the data will be exported same as Excel. The default value is false.

### getHiddenColDisplayType() {#gethiddencoldisplaytype}

Hidden column(the width of this column is 0) in excel,before save this into html format, if HtmlHiddenColDisplayType is "Remove",the hidden column would not been output, if the value is "Hidden", the column would been output,but was hidden,the default value is "Hidden" The value of the property is HtmlHiddenColDisplayType integer constant.

### getHiddenRowDisplayType() {#gethiddenrowdisplaytype}

Hidden row(the height of this row is 0) in excel,before save this into html format, if HtmlHiddenRowDisplayType is "Remove",the hidden row would not been output, if the value is "Hidden", the row would been output,but was hidden,the default value is "Hidden" The value of the property is HtmlHiddenRowDisplayType integer constant.

### getHideOverflowWrappedText() {#gethideoverflowwrappedtext}

Indicates whether to hide overflow text when the cell format is set to wrap text. The default value is false

### getHtmlCrossStringType() {#gethtmlcrossstringtype}

Indicates if a cross-cell string will be displayed in the same way as MS Excel when saving an Excel file in html format. By default the value is Default, so, for cross-cell strings, there is little difference between the html files created by Aspose.Cells and MS Excel. But the performance for creating large html files,setting the value to Cross would be several times faster than setting it to Default or Fit2Cell. The value of the property is HtmlCrossType integer constant.

### getHtmlVersion() {#gethtmlversion}

The value of the property is HtmlVersion integer constant.

### getIgnoreInvisibleShapes() {#getignoreinvisibleshapes}

Indicate whether exporting those not visible shapes The default values is false.

### getImageOptions() {#getimageoptions}

Get the ImageOrPrintOptions object before exporting

### getImageScalable() {#getimagescalable}

Indicates whether using scalable unit to describe the image width when using scalable unit to describe the column width. The default value is true.

### getLayoutMode() {#getlayoutmode}

The value of the property is HtmlLayoutMode integer constant.

### getLinkTargetType() {#getlinktargettype}

Indicating the type of target attribute in link. The default value is HtmlLinkTargetType.Parent. The value of the property is HtmlLinkTargetType integer constant.

### getMergeAreas() {#getmergeareas}

Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is false.

### getMergeEmptyTdForcely() {#getmergeemptytdforcely}

Indicates whether merging empty TD element forcedly when exporting file to html. The size of html file will be reduced significantly after setting value to true. The default value is false. If you want to import the html file to excel or export perfect grid lines when saving file to html, please keep the default value.

### getMergeEmptyTdType() {#getmergeemptytdtype}

The option to merge contiguous empty cells(empty td elements) The default value is MergeEmptyTdType.Default. The value of the property is MergeEmptyTdType integer constant.

### getOfficeMathOutputMode() {#getofficemathoutputmode}

The value of the property is HtmlOfficeMathOutputType integer constant.

### getPageTitle() {#getpagetitle}

The title of the html page. Only for saving to html stream.

### getParseHtmlTagInCell() {#getparsehtmltagincell}

Indicates whether html tag(such as ) in cell should be parsed as cell value or preserved as it is. The default value is true.

### getPresentationPreference() {#getpresentationpreference}

Indicating if html or mht file is presentation preference. The default value is false. if you want to get more beautiful presentation,please set the value to true.

### getRefreshChartCache() {#getrefreshchartcache}

Indicates whether refreshing chart cache data

### getSaveAsSingleFile() {#getsaveassinglefile}

Indicates whether save the html as single file. The default value is false. If there are multiple worksheets or other required resources such as pictures in the workbook, commonly those worksheets and other resources need to be saved into separate files. For some scenarios, user maybe need to get only one resultant file such as for the convenience of transferring. If so, user may set this property as true.

### getSaveFormat() {#getsaveformat}

Gets the save file format. The value of the property is SaveFormat integer constant.

### getSheetSet() {#getsheetset}

### getShowAllSheets() {#getshowallsheets}

Indicates whether showing all sheets when saving as a single html file. Only works when SaveAsSingleFile is True.

### getSortExternalNames() {#getsortexternalnames}

Indicates whether sorting external defined names before saving file.

### getSortNames() {#getsortnames}

Indicates whether sorting defined names before saving file.

### getSpaceMode() {#getspacemode}

The value of the property is HtmlSpaceMode integer constant.

### getTableCssId() {#gettablecssid}

Gets and sets the prefix of the type css name such as tr,col,td and so on, they are contained in the table element which has the specific TableCssId attribute. The default value is "".

### getUpdateSmartArt() {#getupdatesmartart}

Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

### getValidateMergedAreas() {#getvalidatemergedareas}

Indicates whether validate merged cells before saving the file. The default value is false.

### getWarningCallback() {#getwarningcallback}

Gets or sets warning callback.

### getWidthScalable() {#getwidthscalable}

Indicates whether exporting column width in unit of scale to html. The default value is false.

### getWorksheetScalable() {#getworksheetscalable}

Indicates if zooming in or out the html via worksheet zoom level when saving file to html, the default value is false.

### isBorderCollapsed() {#isbordercollapsed}

Indicates whether the table borders are collapsed. The default value is true.

### isExpImageToTempDir() {#isexpimagetotempdir}

Indicates whether exporting image files to temp directory. Only for saving to html stream.

### isExportComments() {#isexportcomments}

Indicates if exporting comments when saving file to html, the default value is false.

### isFullPathLink() {#isfullpathlink}

Indicating whether using full path link in sheet00x.htm,filelist.xml and tabstrip.htm. The default value is false.

### isIECompatible() {#isiecompatible}

Indicating whether the output HTML is compatible with IE browser. The defalut value is false

### isJsBrowserCompatible() {#isjsbrowsercompatible}

Indicates whether JavaScript is compatible with browsers that do not support JavaScript. The default value is true.

### isMobileCompatible() {#ismobilecompatible}

Indicates whether the output HTML is compatible with mobile devices. The default value is false.

### setAddGenericFont() {#setaddgenericfont}

Indicates whether to add a generic font to CSS font-family. The default value is true

### setAddTooltipText() {#setaddtooltiptext}

Indicates whether adding tooltip text when the data can't be fully displayed. The default value is false.

### setAttachedFilesDirectory() {#setattachedfilesdirectory}

The directory that the attached files will be saved to. Only for saving to html stream.

### setAttachedFilesUrlPrefix() {#setattachedfilesurlprefix}

Specify the Url prefix of attached files such as image in the html file. Only for saving to html stream.

### setBorderCollapsed() {#setbordercollapsed}

Indicates whether the table borders are collapsed. The default value is true.

### setCachedFileFolder() {#setcachedfilefolder}

The cached file folder is used to store some large data.

### setCalculateFormula() {#setcalculateformula}

Indicates whether to calculate formulas before saving html file. The default value is false.

### setCellCssPrefix() {#setcellcssprefix}

Gets and sets the prefix of the css name,the default value is "".

### setCellNameAttribute() {#setcellnameattribute}

### setCheckExcelRestriction() {#setcheckexcelrestriction}

### setClearData() {#setcleardata}

Make the workbook empty after saving the file.

### setCreateDirectory() {#setcreatedirectory}

If true and the directory does not exist, the directory will be automatically created before saving the file. The default value is false.

### setCssStyles() {#setcssstyles}

Gets or sets the additional css styles for the formatter. Only works when SaveAsSingleFile is True. Example: CssStyles="body { padding: 5px }";

### setDataBarRenderMode() {#setdatabarrendermode}

The value of the property is DataBarRenderMode integer constant.

### setDefaultFontName() {#setdefaultfontname}

Specify the default font name for exporting html, the default font will be used when the font of style is not existing, If this property is null, Aspose.Cells will use universal font which have the same family with the original font, the default value is null.

### setDisableCss() {#setdisablecss}

### setDisableDownlevelRevealedComments() {#setdisabledownlevelrevealedcomments}

Indicates if disable Downlevel-revealed conditional comments when exporting file to html, the default value is false.

### setEmbeddedFontType() {#setembeddedfonttype}

The value of the property is HtmlEmbeddedFontType integer constant.

### setEnableCssCustomProperties() {#setenablecsscustomproperties}

### setEncodeEntityAsCode() {#setencodeentityascode}

### setEncoding() {#setencoding}

If not set,use Encoding.UTF8 as default enconding type.

### setEncryptDocumentProperties() {#setencryptdocumentproperties}

### setExcludeUnusedStyles() {#setexcludeunusedstyles}

Indicating whether excludes unused styles. For the generated html files, excluding unused styles can make the file size smaller without affecting the visual effects. So the default value of this property is true. If user needs to keep all styles in the workbook for the generated html(such as the scenario that user needs to restore the workbook from the generated html later), please set this property as false.

### setExpImageToTempDir() {#setexpimagetotempdir}

Indicates whether exporting image files to temp directory. Only for saving to html stream.

### setExportActiveWorksheetOnly() {#setexportactiveworksheetonly}

Indicates if only exporting the active worksheet to html file. If true then only the active worksheet will be exported to html file; If false then the whole workbook will be exported to html file. The default value is false.

### setExportArea() {#setexportarea}

Gets or Sets the exporting CellArea of current active Worksheet. If you set this attribute, the print area of current active Worksheet will be omitted. Only the specified area will be exported when saving the file to html.

### setExportBogusRowData() {#setexportbogusrowdata}

Indicating whether exporting bogus bottom row data. The default value is true.If you want to import the html or mht file to excel, please keep the default value.

### setExportCellCoordinate() {#setexportcellcoordinate}

Indicates whether exporting excel coordinate of nonblank cells when saving file to html. The default value is false. If you want to import the output html to excel, please keep the default value.

### setExportComments() {#setexportcomments}

Indicates if exporting comments when saving file to html, the default value is false.

### setExportCommentsType() {#setexportcommentstype}

Represents type of exporting comments to html files. The value of the property is PrintCommentsType integer constant.

### setExportDataOptions() {#setexportdataoptions}

Indicating the rule of exporting html file data.The default value is All. The value of the property is HtmlExportDataOptions integer constant.

### setExportDocumentProperties() {#setexportdocumentproperties}

Indicating whether exporting document properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value.

### setExportExtraHeadings() {#setexportextraheadings}

Indicates whether exporting extra headings when the length of text is longer than max display column. The default value is false. If you want to import the html file to excel, please keep the default value.

### setExportFormula() {#setexportformula}

Indicates whether exporting formula when saving file to html. The default value is true. If you want to import the output html to excel, please keep the default value.

### setExportFrameScriptsAndProperties() {#setexportframescriptsandproperties}

Indicating whether exporting frame scripts and document properties. The default value is true.If you want to import the html or mht file to excel, please keep the default value.

### setExportGridLines() {#setexportgridlines}

Indicating whether exporting the gridlines.The default value is false.

### setExportHeadings() {#setexportheadings}

Indicates whether exports sheet's row and column headings when saving to HTML files. NOTE: This member is now obsolete. Instead, please use HtmlSaveOptions.ExportRowColumnHeadings property. This property will be removed 12 months later since June 2022. Aspose apologizes for any inconvenience you may have experienced.

### setExportHiddenWorksheet() {#setexporthiddenworksheet}

Indicating if exporting the hidden worksheet content.The default value is true.

### setExportImagesAsBase64() {#setexportimagesasbase64}

Specifies whether images are saved in Base64 format to HTML, MHTML or EPUB. When this property is set to true image data is exported directly on the img elements and separate files are not created.

### setExportNamedRangeAnchors() {#setexportnamedrangeanchors}

### setExportObjectListener() {#setexportobjectlistener}

Gets or sets the ExportObjectListener for exporting objects. NOTE: This property is now obsolete. Instead, please use HtmlSaveOptions.IStreamProvider property. This property will be removed 12 months later since August 2015. Aspose apologizes for any inconvenience you may have experienced.

### setExportPageFooters() {#setexportpagefooters}

Indicates whether exporting page headers. Only works when SaveAsSingleFile is True.

### setExportPageHeaders() {#setexportpageheaders}

Indicates whether exporting page headers. Only works when SaveAsSingleFile is True.

### setExportPrintAreaOnly() {#setexportprintareaonly}

Indicates if only exporting the print area to html file. The default value is false.

### setExportRowColumnHeadings() {#setexportrowcolumnheadings}

Indicates whether exports sheet's row and column headings when saving to HTML files. The default value is false.

### setExportSimilarBorderStyle() {#setexportsimilarborderstyle}

Indicating whether exporting the similar border style when the border style is not supported by browsers. If you want to import the html or mht file to excel, please keep the default value. The default value is false.

### setExportSingleTab() {#setexportsingletab}

Indicates whether exporting the single tab when the file only has one worksheet. The default value is false.

### setExportWorkbookProperties() {#setexportworkbookproperties}

Indicating whether exporting workbook properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value.

### setExportWorksheetCSSSeparately() {#setexportworksheetcssseparately}

Indicating whether export the worksheet css separately.The default value is false.

### setExportWorksheetProperties() {#setexportworksheetproperties}

Indicating whether exporting worksheet properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value.

### setFilePathProvider() {#setfilepathprovider}

Gets or sets the IFilePathProvider for exporting Worksheet to html separately.

### setFormatDataIgnoreColumnWidth() {#setformatdataignorecolumnwidth}

Indicating whether show the whole formatted data of cell when overflowing the column. If true then ignore the column width and the whole data of cell will be exported. If false then the data will be exported same as Excel. The default value is false.

### setFullPathLink() {#setfullpathlink}

Indicating whether using full path link in sheet00x.htm,filelist.xml and tabstrip.htm. The default value is false.

### setHiddenColDisplayType() {#sethiddencoldisplaytype}

Hidden column(the width of this column is 0) in excel,before save this into html format, if HtmlHiddenColDisplayType is "Remove",the hidden column would not been output, if the value is "Hidden", the column would been output,but was hidden,the default value is "Hidden" The value of the property is HtmlHiddenColDisplayType integer constant.

### setHiddenRowDisplayType() {#sethiddenrowdisplaytype}

Hidden row(the height of this row is 0) in excel,before save this into html format, if HtmlHiddenRowDisplayType is "Remove",the hidden row would not been output, if the value is "Hidden", the row would been output,but was hidden,the default value is "Hidden" The value of the property is HtmlHiddenRowDisplayType integer constant.

### setHideOverflowWrappedText() {#sethideoverflowwrappedtext}

Indicates whether to hide overflow text when the cell format is set to wrap text. The default value is false

### setHtmlCrossStringType() {#sethtmlcrossstringtype}

Indicates if a cross-cell string will be displayed in the same way as MS Excel when saving an Excel file in html format. By default the value is Default, so, for cross-cell strings, there is little difference between the html files created by Aspose.Cells and MS Excel. But the performance for creating large html files,setting the value to Cross would be several times faster than setting it to Default or Fit2Cell. The value of the property is HtmlCrossType integer constant.

### setHtmlVersion() {#sethtmlversion}

The value of the property is HtmlVersion integer constant.

### setIECompatible() {#setiecompatible}

Indicating whether the output HTML is compatible with IE browser. The defalut value is false

### setIgnoreInvisibleShapes() {#setignoreinvisibleshapes}

Indicate whether exporting those not visible shapes The default values is false.

### setImageScalable() {#setimagescalable}

Indicates whether using scalable unit to describe the image width when using scalable unit to describe the column width. The default value is true.

### setJsBrowserCompatible() {#setjsbrowsercompatible}

Indicates whether JavaScript is compatible with browsers that do not support JavaScript. The default value is true.

### setLayoutMode() {#setlayoutmode}

The value of the property is HtmlLayoutMode integer constant.

### setLinkTargetType() {#setlinktargettype}

Indicating the type of target attribute in link. The default value is HtmlLinkTargetType.Parent. The value of the property is HtmlLinkTargetType integer constant.

### setMergeAreas() {#setmergeareas}

Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is false.

### setMergeEmptyTdForcely() {#setmergeemptytdforcely}

Indicates whether merging empty TD element forcedly when exporting file to html. The size of html file will be reduced significantly after setting value to true. The default value is false. If you want to import the html file to excel or export perfect grid lines when saving file to html, please keep the default value.

### setMergeEmptyTdType() {#setmergeemptytdtype}

The option to merge contiguous empty cells(empty td elements) The default value is MergeEmptyTdType.Default. The value of the property is MergeEmptyTdType integer constant.

### setMobileCompatible() {#setmobilecompatible}

Indicates whether the output HTML is compatible with mobile devices. The default value is false.

### setOfficeMathOutputMode() {#setofficemathoutputmode}

The value of the property is HtmlOfficeMathOutputType integer constant.

### setPageTitle() {#setpagetitle}

The title of the html page. Only for saving to html stream.

### setParseHtmlTagInCell() {#setparsehtmltagincell}

Indicates whether html tag(such as ) in cell should be parsed as cell value or preserved as it is. The default value is true.

### setPresentationPreference() {#setpresentationpreference}

Indicating if html or mht file is presentation preference. The default value is false. if you want to get more beautiful presentation,please set the value to true.

### setRefreshChartCache() {#setrefreshchartcache}

Indicates whether refreshing chart cache data

### setSaveAsSingleFile() {#setsaveassinglefile}

Indicates whether save the html as single file. The default value is false. If there are multiple worksheets or other required resources such as pictures in the workbook, commonly those worksheets and other resources need to be saved into separate files. For some scenarios, user maybe need to get only one resultant file such as for the convenience of transferring. If so, user may set this property as true.

### setSheetSet() {#setsheetset}

### setShowAllSheets() {#setshowallsheets}

Indicates whether showing all sheets when saving as a single html file. Only works when SaveAsSingleFile is True.

### setSortExternalNames() {#setsortexternalnames}

Indicates whether sorting external defined names before saving file.

### setSortNames() {#setsortnames}

Indicates whether sorting defined names before saving file.

### setSpaceMode() {#setspacemode}

The value of the property is HtmlSpaceMode integer constant.

### setTableCssId() {#settablecssid}

Gets and sets the prefix of the type css name such as tr,col,td and so on, they are contained in the table element which has the specific TableCssId attribute. The default value is "".

### setUpdateSmartArt() {#setupdatesmartart}

Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

### setValidateMergedAreas() {#setvalidatemergedareas}

Indicates whether validate merged cells before saving the file. The default value is false.

### setWarningCallback() {#setwarningcallback}

Gets or sets warning callback.

### setWidthScalable() {#setwidthscalable}

Indicates whether exporting column width in unit of scale to html. The default value is false.

### setWorksheetScalable() {#setworksheetscalable}

Indicates if zooming in or out the html via worksheet zoom level when saving file to html, the default value is false.
