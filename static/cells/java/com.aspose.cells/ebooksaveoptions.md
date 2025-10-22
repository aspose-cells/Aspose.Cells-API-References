##EbookSaveOptions
Represents the options for saving ebook file.
**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions), [com.aspose.cells.HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions)
```
public class EbookSaveOptions extends HtmlSaveOptions
```
Represents the options for saving ebook file.
## Constructors
| Constructor | Description |
| --- | --- |
| [EbookSaveOptions()](#EbookSaveOptions--) | Creates options for saving ebook file. |
| [EbookSaveOptions(int saveFormat)](#EbookSaveOptions-int-) | Creates options for saving ebook file. |
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAddGenericFont()](#getAddGenericFont--) | Indicates whether to add a generic font to CSS font-family. |
| [getAddTooltipText()](#getAddTooltipText--) | Indicates whether adding tooltip text when the data can't be fully displayed. |
| [getAttachedFilesDirectory()](#getAttachedFilesDirectory--) | The directory that the attached files will be saved to. |
| [getAttachedFilesUrlPrefix()](#getAttachedFilesUrlPrefix--) | Specify the Url prefix of attached files such as image in the html file. |
| [getCachedFileFolder()](#getCachedFileFolder--) | The folder for temporary files that may be used as data cache. |
| [getCalculateFormula()](#getCalculateFormula--) | Indicates whether to calculate formulas before saving html file. |
| [getCellCssPrefix()](#getCellCssPrefix--) | Gets the prefix of the css name,the default value is "". |
| [getCellNameAttribute()](#getCellNameAttribute--) | Specifies the attribute that indicates the CellName to be written. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Whether check restriction of excel file when user modify cells related objects. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Make the workbook empty after saving the file. |
| [getCreateDirectory()](#getCreateDirectory--) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [getCssStyles()](#getCssStyles--) | Gets the additional css styles for the formatter. |
| [getDefaultFontName()](#getDefaultFontName--) | Specify the default font name for exporting html, the default font will be used when the font of style is not existing, If this property is null, Aspose.Cells will use universal font which have the same family with the original font, the default value is null. |
| [getDisableCss()](#getDisableCss--) | Indicates whether only inline styles are applied, without relying on CSS. |
| [getDisableDownlevelRevealedComments()](#getDisableDownlevelRevealedComments--) | Indicates if disable Downlevel-revealed conditional comments when exporting file to html, the default value is false. |
| [getEmbeddedFontType()](#getEmbeddedFontType--) | Gets the type of font that embedded in html. |
| [getEnableCssCustomProperties()](#getEnableCssCustomProperties--) | Optimize the output of html by using CSS custom properties. |
| [getEncodeEntityAsCode()](#getEncodeEntityAsCode--) | Indicates whether the html character entities are replaced with decimal code. |
| [getEncoding()](#getEncoding--) | If not set,use Encoding.UTF8 as default enconding type. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Indicates whether encrypt document properties when saving as .xls file. |
| [getExcludeUnusedStyles()](#getExcludeUnusedStyles--) | Indicating whether excludes unused styles. |
| [getExportActiveWorksheetOnly()](#getExportActiveWorksheetOnly--) | Indicates if only exporting the active worksheet to html file. |
| [getExportArea()](#getExportArea--) | Gets the exporting CellArea of current active Worksheet. |
| [getExportBogusRowData()](#getExportBogusRowData--) | Indicating whether exporting bogus bottom row data. |
| [getExportCellCoordinate()](#getExportCellCoordinate--) | Indicates whether exporting excel coordinate of nonblank cells when saving file to html. |
| [getExportCommentsType()](#getExportCommentsType--) | Represents type of exporting comments to html files. |
| [getExportDataOptions()](#getExportDataOptions--) | Indicating the rule of exporting html file data.The default value is All. |
| [getExportDocumentProperties()](#getExportDocumentProperties--) | Indicating whether exporting document properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [getExportExtraHeadings()](#getExportExtraHeadings--) | Indicates whether exporting extra headings when the length of text is longer than max display column. |
| [getExportFormula()](#getExportFormula--) | Indicates whether exporting formula when saving file to html. |
| [getExportFrameScriptsAndProperties()](#getExportFrameScriptsAndProperties--) | Indicating whether exporting frame scripts and document properties. |
| [getExportGridLines()](#getExportGridLines--) | Indicating whether exporting the gridlines.The default value is false. |
| [getExportHeadings()](#getExportHeadings--) | Indicates whether exports sheet's row and column headings when saving to HTML files. |
| [getExportHiddenWorksheet()](#getExportHiddenWorksheet--) | Indicating if exporting the hidden worksheet content.The default value is true. |
| [getExportImagesAsBase64()](#getExportImagesAsBase64--) | Specifies whether images are saved in Base64 format to HTML, MHTML or EPUB. |
| [getExportObjectListener()](#getExportObjectListener--) | Gets the ExportObjectListener for exporting objects. |
| [getExportPageFooters()](#getExportPageFooters--) | Indicates whether exporting page headers. |
| [getExportPageHeaders()](#getExportPageHeaders--) | Indicates whether exporting page headers. |
| [getExportPrintAreaOnly()](#getExportPrintAreaOnly--) | Indicates if only exporting the print area to html file. |
| [getExportRowColumnHeadings()](#getExportRowColumnHeadings--) | Indicates whether exports sheet's row and column headings when saving to HTML files. |
| [getExportSimilarBorderStyle()](#getExportSimilarBorderStyle--) | Indicating whether exporting the similar border style when the border style is not supported by browsers. |
| [getExportSingleTab()](#getExportSingleTab--) | Indicates whether exporting the single tab when the file only has one worksheet. |
| [getExportWorkbookProperties()](#getExportWorkbookProperties--) | Indicating whether exporting workbook properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [getExportWorksheetCSSSeparately()](#getExportWorksheetCSSSeparately--) | Indicating whether export the worksheet css separately.The default value is false. |
| [getExportWorksheetProperties()](#getExportWorksheetProperties--) | Indicating whether exporting worksheet properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [getFilePathProvider()](#getFilePathProvider--) | Gets the IFilePathProvider for exporting Worksheet to html separately. |
| [getFormatDataIgnoreColumnWidth()](#getFormatDataIgnoreColumnWidth--) | Indicating whether show the whole formatted data of cell when overflowing the column. |
| [getHiddenColDisplayType()](#getHiddenColDisplayType--) | Hidden column(the width of this column is 0) in excel,before save this into html format, if HtmlHiddenColDisplayType is "Remove",the hidden column would not been output, if the value is "Hidden", the column would been output,but was hidden,the default value is "Hidden" |
| [getHiddenRowDisplayType()](#getHiddenRowDisplayType--) | Hidden row(the height of this row is 0) in excel,before save this into html format, if HtmlHiddenRowDisplayType is "Remove",the hidden row would not been output, if the value is "Hidden", the row would been output,but was hidden,the default value is "Hidden" |
| [getHideOverflowWrappedText()](#getHideOverflowWrappedText--) | Indicates whether to hide overflow text when the cell format is set to wrap text. |
| [getHtmlCrossStringType()](#getHtmlCrossStringType--) | Indicates if a cross-cell string will be displayed in the same way as MS Excel when saving an Excel file in html format. |
| [getHtmlVersion()](#getHtmlVersion--) | Specifies version of HTML standard that should be used when saving the HTML format. |
| [getIgnoreInvisibleShapes()](#getIgnoreInvisibleShapes--) | Indicate whether exporting those not visible shapes |
| [getImageOptions()](#getImageOptions--) | Get the ImageOrPrintOptions object before exporting |
| [getImageScalable()](#getImageScalable--) | Indicates whether using scalable unit to describe the image width when using scalable unit to describe the column width. |
| [getLinkTargetType()](#getLinkTargetType--) | Indicating the type of target attribute in `<a>` link. |
| [getMergeAreas()](#getMergeAreas--) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [getMergeEmptyTdForcely()](#getMergeEmptyTdForcely--) | Indicates whether merging empty TD element forcedly when exporting file to html. |
| [getMergeEmptyTdType()](#getMergeEmptyTdType--) | The option to merge contiguous empty cells(empty td elements) The default value is MergeEmptyTdType.Default. |
| [getOfficeMathOutputMode()](#getOfficeMathOutputMode--) | Indicates how export OfficeMath objects to HTML, Default value is Image. |
| [getPageTitle()](#getPageTitle--) | The title of the html page. |
| [getParseHtmlTagInCell()](#getParseHtmlTagInCell--) | Indicates whether html tag(such as `<div></div>`) in cell should be parsed as cell value or preserved as it is. |
| [getPresentationPreference()](#getPresentationPreference--) | Indicating if html or mht file is presentation preference. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Indicates whether refreshing chart cache data |
| [getSaveAsSingleFile()](#getSaveAsSingleFile--) | Indicates whether save the html as single file. |
| [getSaveFormat()](#getSaveFormat--) | Gets the save file format. |
| [getSheetSet()](#getSheetSet--) | Gets the sheets to render. |
| [getShowAllSheets()](#getShowAllSheets--) | Indicates whether showing all sheets when saving as a single html file. |
| [getSortExternalNames()](#getSortExternalNames--) | Indicates whether sorting external defined names before saving file. |
| [getSortNames()](#getSortNames--) | Indicates whether sorting defined names before saving file. |
| [getStreamProvider()](#getStreamProvider--) | Gets the IStreamProvider for exporting objects. |
| [getTableCssId()](#getTableCssId--) | Gets the prefix of the type css name such as tr,col,td and so on, they are contained in the table element which has the specific TableCssId attribute. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Indicates whether updating smart art setting. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Indicates whether validate merged cells before saving the file. |
| [getWarningCallback()](#getWarningCallback--) | Gets warning callback. |
| [getWidthScalable()](#getWidthScalable--) | Indicates whether exporting column width in unit of scale to html. |
| [getWorksheetScalable()](#getWorksheetScalable--) | Indicates if zooming in or out the html via worksheet zoom level when saving file to html, the default value is false. |
| [hashCode()](#hashCode--) |  |
| [isBorderCollapsed()](#isBorderCollapsed--) | Indicates whether the table borders are collapsed. |
| [isExpImageToTempDir()](#isExpImageToTempDir--) | Indicates whether exporting image files to temp directory. |
| [isExportComments()](#isExportComments--) | Indicates if exporting comments when saving file to html, the default value is false. |
| [isFullPathLink()](#isFullPathLink--) | Indicating whether using full path link in sheet00x.htm,filelist.xml and tabstrip.htm. |
| [isIECompatible()](#isIECompatible--) | Indicating whether the output HTML is compatible with IE browser. |
| [isJsBrowserCompatible()](#isJsBrowserCompatible--) | Indicates whether JavaScript is compatible with browsers that do not support JavaScript. |
| [isMobileCompatible()](#isMobileCompatible--) | Indicates whether the output HTML is compatible with mobile devices. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAddGenericFont(boolean value)](#setAddGenericFont-boolean-) | Indicates whether to add a generic font to CSS font-family. |
| [setAddTooltipText(boolean value)](#setAddTooltipText-boolean-) | Indicates whether adding tooltip text when the data can't be fully displayed. |
| [setAttachedFilesDirectory(String value)](#setAttachedFilesDirectory-java.lang.String-) | The directory that the attached files will be saved to. |
| [setAttachedFilesUrlPrefix(String value)](#setAttachedFilesUrlPrefix-java.lang.String-) | Specify the Url prefix of attached files such as image in the html file. |
| [setBorderCollapsed(boolean value)](#setBorderCollapsed-boolean-) | Indicates whether the table borders are collapsed. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | The folder for temporary files that may be used as data cache. |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | Indicates whether to calculate formulas before saving html file. |
| [setCellCssPrefix(String value)](#setCellCssPrefix-java.lang.String-) | Sets the prefix of the css name,the default value is "". |
| [setCellNameAttribute(String value)](#setCellNameAttribute-java.lang.String-) | Specifies the attribute that indicates the CellName to be written. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Whether check restriction of excel file when user modify cells related objects. |
| [setClearData(boolean value)](#setClearData-boolean-) | Make the workbook empty after saving the file. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [setCssStyles(String value)](#setCssStyles-java.lang.String-) | Sets the additional css styles for the formatter. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Specify the default font name for exporting html, the default font will be used when the font of style is not existing, If this property is null, Aspose.Cells will use universal font which have the same family with the original font, the default value is null. |
| [setDisableCss(boolean value)](#setDisableCss-boolean-) | Indicates whether only inline styles are applied, without relying on CSS. |
| [setDisableDownlevelRevealedComments(boolean value)](#setDisableDownlevelRevealedComments-boolean-) | Indicates if disable Downlevel-revealed conditional comments when exporting file to html, the default value is false. |
| [setEmbeddedFontType(int value)](#setEmbeddedFontType-int-) | Sets the type of font that embedded in html. |
| [setEnableCssCustomProperties(boolean value)](#setEnableCssCustomProperties-boolean-) | Optimize the output of html by using CSS custom properties. |
| [setEncodeEntityAsCode(boolean value)](#setEncodeEntityAsCode-boolean-) | Indicates whether the html character entities are replaced with decimal code. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | If not set,use Encoding.UTF8 as default enconding type. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Indicates whether encrypt document properties when saving as .xls file. |
| [setExcludeUnusedStyles(boolean value)](#setExcludeUnusedStyles-boolean-) | Indicating whether excludes unused styles. |
| [setExpImageToTempDir(boolean value)](#setExpImageToTempDir-boolean-) | Indicates whether exporting image files to temp directory. |
| [setExportActiveWorksheetOnly(boolean value)](#setExportActiveWorksheetOnly-boolean-) | Indicates if only exporting the active worksheet to html file. |
| [setExportArea(CellArea value)](#setExportArea-com.aspose.cells.CellArea-) | Sets the exporting CellArea of current active Worksheet. |
| [setExportBogusRowData(boolean value)](#setExportBogusRowData-boolean-) | Indicating whether exporting bogus bottom row data. |
| [setExportCellCoordinate(boolean value)](#setExportCellCoordinate-boolean-) | Indicates whether exporting excel coordinate of nonblank cells when saving file to html. |
| [setExportComments(boolean value)](#setExportComments-boolean-) | Indicates if exporting comments when saving file to html, the default value is false. |
| [setExportCommentsType(int value)](#setExportCommentsType-int-) | Represents type of exporting comments to html files. |
| [setExportDataOptions(int value)](#setExportDataOptions-int-) | Indicating the rule of exporting html file data.The default value is All. |
| [setExportDocumentProperties(boolean value)](#setExportDocumentProperties-boolean-) | Indicating whether exporting document properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [setExportExtraHeadings(boolean value)](#setExportExtraHeadings-boolean-) | Indicates whether exporting extra headings when the length of text is longer than max display column. |
| [setExportFormula(boolean value)](#setExportFormula-boolean-) | Indicates whether exporting formula when saving file to html. |
| [setExportFrameScriptsAndProperties(boolean value)](#setExportFrameScriptsAndProperties-boolean-) | Indicating whether exporting frame scripts and document properties. |
| [setExportGridLines(boolean value)](#setExportGridLines-boolean-) | Indicating whether exporting the gridlines.The default value is false. |
| [setExportHeadings(boolean value)](#setExportHeadings-boolean-) | Indicates whether exports sheet's row and column headings when saving to HTML files. |
| [setExportHiddenWorksheet(boolean value)](#setExportHiddenWorksheet-boolean-) | Indicating if exporting the hidden worksheet content.The default value is true. |
| [setExportImagesAsBase64(boolean value)](#setExportImagesAsBase64-boolean-) | Specifies whether images are saved in Base64 format to HTML, MHTML or EPUB. |
| [setExportObjectListener(IExportObjectListener value)](#setExportObjectListener-com.aspose.cells.IExportObjectListener-) | Sets the ExportObjectListener for exporting objects. |
| [setExportPageFooters(boolean value)](#setExportPageFooters-boolean-) | Indicates whether exporting page headers. |
| [setExportPageHeaders(boolean value)](#setExportPageHeaders-boolean-) | Indicates whether exporting page headers. |
| [setExportPrintAreaOnly(boolean value)](#setExportPrintAreaOnly-boolean-) | Indicates if only exporting the print area to html file. |
| [setExportRowColumnHeadings(boolean value)](#setExportRowColumnHeadings-boolean-) | Indicates whether exports sheet's row and column headings when saving to HTML files. |
| [setExportSimilarBorderStyle(boolean value)](#setExportSimilarBorderStyle-boolean-) | Indicating whether exporting the similar border style when the border style is not supported by browsers. |
| [setExportSingleTab(boolean value)](#setExportSingleTab-boolean-) | Indicates whether exporting the single tab when the file only has one worksheet. |
| [setExportWorkbookProperties(boolean value)](#setExportWorkbookProperties-boolean-) | Indicating whether exporting workbook properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [setExportWorksheetCSSSeparately(boolean value)](#setExportWorksheetCSSSeparately-boolean-) | Indicating whether export the worksheet css separately.The default value is false. |
| [setExportWorksheetProperties(boolean value)](#setExportWorksheetProperties-boolean-) | Indicating whether exporting worksheet properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [setFilePathProvider(IFilePathProvider value)](#setFilePathProvider-com.aspose.cells.IFilePathProvider-) | Sets the IFilePathProvider for exporting Worksheet to html separately. |
| [setFormatDataIgnoreColumnWidth(boolean value)](#setFormatDataIgnoreColumnWidth-boolean-) | Indicating whether show the whole formatted data of cell when overflowing the column. |
| [setFullPathLink(boolean value)](#setFullPathLink-boolean-) | Indicating whether using full path link in sheet00x.htm,filelist.xml and tabstrip.htm. |
| [setHiddenColDisplayType(int value)](#setHiddenColDisplayType-int-) | Hidden column(the width of this column is 0) in excel,before save this into html format, if HtmlHiddenColDisplayType is "Remove",the hidden column would not been output, if the value is "Hidden", the column would been output,but was hidden,the default value is "Hidden" |
| [setHiddenRowDisplayType(int value)](#setHiddenRowDisplayType-int-) | Hidden row(the height of this row is 0) in excel,before save this into html format, if HtmlHiddenRowDisplayType is "Remove",the hidden row would not been output, if the value is "Hidden", the row would been output,but was hidden,the default value is "Hidden" |
| [setHideOverflowWrappedText(boolean value)](#setHideOverflowWrappedText-boolean-) | Indicates whether to hide overflow text when the cell format is set to wrap text. |
| [setHtmlCrossStringType(int value)](#setHtmlCrossStringType-int-) | Indicates if a cross-cell string will be displayed in the same way as MS Excel when saving an Excel file in html format. |
| [setHtmlVersion(int value)](#setHtmlVersion-int-) | Specifies version of HTML standard that should be used when saving the HTML format. |
| [setIECompatible(boolean value)](#setIECompatible-boolean-) | Indicating whether the output HTML is compatible with IE browser. |
| [setIgnoreInvisibleShapes(boolean value)](#setIgnoreInvisibleShapes-boolean-) | Indicate whether exporting those not visible shapes |
| [setImageScalable(boolean value)](#setImageScalable-boolean-) | Indicates whether using scalable unit to describe the image width when using scalable unit to describe the column width. |
| [setJsBrowserCompatible(boolean value)](#setJsBrowserCompatible-boolean-) | Indicates whether JavaScript is compatible with browsers that do not support JavaScript. |
| [setLinkTargetType(int value)](#setLinkTargetType-int-) | Indicating the type of target attribute in `<a>` link. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [setMergeEmptyTdForcely(boolean value)](#setMergeEmptyTdForcely-boolean-) | Indicates whether merging empty TD element forcedly when exporting file to html. |
| [setMergeEmptyTdType(int value)](#setMergeEmptyTdType-int-) | The option to merge contiguous empty cells(empty td elements) The default value is MergeEmptyTdType.Default. |
| [setMobileCompatible(boolean value)](#setMobileCompatible-boolean-) | Indicates whether the output HTML is compatible with mobile devices. |
| [setOfficeMathOutputMode(int value)](#setOfficeMathOutputMode-int-) | Indicates how export OfficeMath objects to HTML, Default value is Image. |
| [setPageTitle(String value)](#setPageTitle-java.lang.String-) | The title of the html page. |
| [setParseHtmlTagInCell(boolean value)](#setParseHtmlTagInCell-boolean-) | Indicates whether html tag(such as `<div></div>`) in cell should be parsed as cell value or preserved as it is. |
| [setPresentationPreference(boolean value)](#setPresentationPreference-boolean-) | Indicating if html or mht file is presentation preference. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Indicates whether refreshing chart cache data |
| [setSaveAsSingleFile(boolean value)](#setSaveAsSingleFile-boolean-) | Indicates whether save the html as single file. |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | Sets the sheets to render. |
| [setShowAllSheets(boolean value)](#setShowAllSheets-boolean-) | Indicates whether showing all sheets when saving as a single html file. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Indicates whether sorting external defined names before saving file. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Indicates whether sorting defined names before saving file. |
| [setStreamProvider(IStreamProvider value)](#setStreamProvider-com.aspose.cells.IStreamProvider-) | Sets the IStreamProvider for exporting objects. |
| [setTableCssId(String value)](#setTableCssId-java.lang.String-) | Sets the prefix of the type css name such as tr,col,td and so on, they are contained in the table element which has the specific TableCssId attribute. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Indicates whether updating smart art setting. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Indicates whether validate merged cells before saving the file. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Sets warning callback. |
| [setWidthScalable(boolean value)](#setWidthScalable-boolean-) | Indicates whether exporting column width in unit of scale to html. |
| [setWorksheetScalable(boolean value)](#setWorksheetScalable-boolean-) | Indicates if zooming in or out the html via worksheet zoom level when saving file to html, the default value is false. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### EbookSaveOptions() {#EbookSaveOptions--}
```
public EbookSaveOptions()
```
Creates options for saving ebook file.
### EbookSaveOptions(int saveFormat) {#EbookSaveOptions-int-}
```
public EbookSaveOptions(int saveFormat)
```
Creates options for saving ebook file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). The file format. It should be [SaveFormat.EPUB](../../com.aspose.cells/saveformat\#EPUB) or [SaveFormat.AZW\_3](../../com.aspose.cells/saveformat\#AZW-3). |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |
**Returns:**
boolean
### getAddGenericFont() {#getAddGenericFont--}
```
public boolean getAddGenericFont()
```
Indicates whether to add a generic font to CSS font-family. The default value is true
**Returns:**
boolean
### getAddTooltipText() {#getAddTooltipText--}
```
public boolean getAddTooltipText()
```
Indicates whether adding tooltip text when the data can't be fully displayed. The default value is false.
**Returns:**
boolean
### getAttachedFilesDirectory() {#getAttachedFilesDirectory--}
```
public String getAttachedFilesDirectory()
```
The directory that the attached files will be saved to. Only for saving to html stream.
**Returns:**
java.lang.String
### getAttachedFilesUrlPrefix() {#getAttachedFilesUrlPrefix--}
```
public String getAttachedFilesUrlPrefix()
```
Specify the Url prefix of attached files such as image in the html file. Only for saving to html stream.
**Returns:**
java.lang.String
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```
The folder for temporary files that may be used as data cache.
**Remarks**
If the folder has not been specified, the default value for it is void
**Returns:**
java.lang.String
### getCalculateFormula() {#getCalculateFormula--}
```
public boolean getCalculateFormula()
```
Indicates whether to calculate formulas before saving html file.
**Remarks**
The default value is false.
**Returns:**
boolean
### getCellCssPrefix() {#getCellCssPrefix--}
```
public String getCellCssPrefix()
```
Gets the prefix of the css name,the default value is "".
**Returns:**
java.lang.String
### getCellNameAttribute() {#getCellNameAttribute--}
```
public String getCellNameAttribute()
```
Specifies the attribute that indicates the CellName to be written. (e.g. If the value is "id", then for cell "A1", the output will be:<td id='A1'>). The default value is null.
**Returns:**
java.lang.String
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```
Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated.
**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getClearData() {#getClearData--}
```
public boolean getClearData()
```
Make the workbook empty after saving the file.
**Returns:**
boolean
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```
If true and the directory does not exist, the directory will be automatically created before saving the file.
**Remarks**
The default value is false.
**Returns:**
boolean
### getCssStyles() {#getCssStyles--}
```
public String getCssStyles()
```
Gets the additional css styles for the formatter. Only works when [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) is True.  CssStyles="body \{ padding: 5px \}";
**Returns:**
java.lang.String
### getDefaultFontName() {#getDefaultFontName--}
```
public String getDefaultFontName()
```
Specify the default font name for exporting html, the default font will be used when the font of style is not existing, If this property is null, Aspose.Cells will use universal font which have the same family with the original font, the default value is null.
**Returns:**
java.lang.String
### getDisableCss() {#getDisableCss--}
```
public boolean getDisableCss()
```
Indicates whether only inline styles are applied, without relying on CSS. The default value is false.
**Returns:**
boolean
### getDisableDownlevelRevealedComments() {#getDisableDownlevelRevealedComments--}
```
public boolean getDisableDownlevelRevealedComments()
```
Indicates if disable Downlevel-revealed conditional comments when exporting file to html, the default value is false.
**Returns:**
boolean
### getEmbeddedFontType() {#getEmbeddedFontType--}
```
public int getEmbeddedFontType()
```
Gets the type of font that embedded in html. Default value is [HtmlEmbeddedFontType.NONE](../../com.aspose.cells/htmlembeddedfonttype\#NONE) which indicates that it will not embed font in html.
See [HtmlEmbeddedFontType](../../com.aspose.cells/htmlembeddedfonttype).
**Returns:**
int
### getEnableCssCustomProperties() {#getEnableCssCustomProperties--}
```
public boolean getEnableCssCustomProperties()
```
Optimize the output of html by using CSS custom properties. For example, for the scenario that there are multiple occurences for one base64 image, with custom property the image data only needs to be saved once so the performance of the resultant html can be improved. The default value is false.
**Returns:**
boolean
### getEncodeEntityAsCode() {#getEncodeEntityAsCode--}
```
public boolean getEncodeEntityAsCode()
```
Indicates whether the html character entities are replaced with decimal code. (e.g. "&nbsp;" is replaced with "&\#160;"). The default value is false.
**Returns:**
boolean
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```
If not set,use Encoding.UTF8 as default enconding type.
**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}
```
public boolean getEncryptDocumentProperties()
```
Indicates whether encrypt document properties when saving as .xls file. The default value is true.
**Remarks**
Only for .xls,xlsx,xlsb and xlsm file.
**Returns:**
boolean
### getExcludeUnusedStyles() {#getExcludeUnusedStyles--}
```
public boolean getExcludeUnusedStyles()
```
Indicating whether excludes unused styles. For the generated html files, excluding unused styles can make the file size smaller without affecting the visual effects. So the default value of this property is true. If user needs to keep all styles in the workbook for the generated html(such as the scenario that user needs to restore the workbook from the generated html later), please set this property as false.
**Returns:**
boolean
### getExportActiveWorksheetOnly() {#getExportActiveWorksheetOnly--}
```
public boolean getExportActiveWorksheetOnly()
```
Indicates if only exporting the active worksheet to html file. If true then only the active worksheet will be exported to html file; If false then the whole workbook will be exported to html file. The default value is false.
**Returns:**
boolean
### getExportArea() {#getExportArea--}
```
public CellArea getExportArea()
```
Gets the exporting CellArea of current active Worksheet. If you set this attribute, the print area of current active Worksheet will be omitted. Only the specified area will be exported when saving the file to html.
**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getExportBogusRowData() {#getExportBogusRowData--}
```
public boolean getExportBogusRowData()
```
Indicating whether exporting bogus bottom row data. The default value is true.If you want to import the html or mht file to excel, please keep the default value.
**Returns:**
boolean
### getExportCellCoordinate() {#getExportCellCoordinate--}
```
public boolean getExportCellCoordinate()
```
Indicates whether exporting excel coordinate of nonblank cells when saving file to html. The default value is false. If you want to import the output html to excel, please keep the default value.
**Returns:**
boolean
### getExportCommentsType() {#getExportCommentsType--}
```
public int getExportCommentsType()
```
Represents type of exporting comments to html files.
See [PrintCommentsType](../../com.aspose.cells/printcommentstype).
**Returns:**
int
### getExportDataOptions() {#getExportDataOptions--}
```
public int getExportDataOptions()
```
Indicating the rule of exporting html file data.The default value is All.
See [HtmlExportDataOptions](../../com.aspose.cells/htmlexportdataoptions).
**Returns:**
int
### getExportDocumentProperties() {#getExportDocumentProperties--}
```
public boolean getExportDocumentProperties()
```
Indicating whether exporting document properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value.
**Returns:**
boolean
### getExportExtraHeadings() {#getExportExtraHeadings--}
```
public boolean getExportExtraHeadings()
```
Indicates whether exporting extra headings when the length of text is longer than max display column. The default value is false. If you want to import the html file to excel, please keep the default value.
**Returns:**
boolean
### getExportFormula() {#getExportFormula--}
```
public boolean getExportFormula()
```
Indicates whether exporting formula when saving file to html. The default value is true. If you want to import the output html to excel, please keep the default value.
**Returns:**
boolean
### getExportFrameScriptsAndProperties() {#getExportFrameScriptsAndProperties--}
```
public boolean getExportFrameScriptsAndProperties()
```
Indicating whether exporting frame scripts and document properties. The default value is true.If you want to import the html or mht file to excel, please keep the default value.
**Returns:**
boolean
### getExportGridLines() {#getExportGridLines--}
```
public boolean getExportGridLines()
```
Indicating whether exporting the gridlines.The default value is false.
**Returns:**
boolean
### getExportHeadings() {#getExportHeadings--}
```
public boolean getExportHeadings()
```
Indicates whether exports sheet's row and column headings when saving to HTML files.
**Remarks**
NOTE: This member is now obsolete. Instead, please use HtmlSaveOptions.ExportRowColumnHeadings property. This property will be removed 12 months later since June 2022. Aspose apologizes for any inconvenience you may have experienced.
**Returns:**
boolean
### getExportHiddenWorksheet() {#getExportHiddenWorksheet--}
```
public boolean getExportHiddenWorksheet()
```
Indicating if exporting the hidden worksheet content.The default value is true.
**Returns:**
boolean
### getExportImagesAsBase64() {#getExportImagesAsBase64--}
```
public boolean getExportImagesAsBase64()
```
Specifies whether images are saved in Base64 format to HTML, MHTML or EPUB.
**Remarks**
When this property is set to true image data is exported directly on the img elements and separate files are not created.
**Returns:**
boolean
### getExportObjectListener() {#getExportObjectListener--}
```
public IExportObjectListener getExportObjectListener()
```
Gets the ExportObjectListener for exporting objects.
**Remarks**
NOTE: This property is now obsolete. Instead, please use HtmlSaveOptions.IStreamProvider property. This property will be removed 12 months later since August 2015. Aspose apologizes for any inconvenience you may have experienced.
**Returns:**
[IExportObjectListener](../../com.aspose.cells/iexportobjectlistener)
### getExportPageFooters() {#getExportPageFooters--}
```
public boolean getExportPageFooters()
```
Indicates whether exporting page headers.
**Remarks**
Only works when [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) is True.
**Returns:**
boolean
### getExportPageHeaders() {#getExportPageHeaders--}
```
public boolean getExportPageHeaders()
```
Indicates whether exporting page headers.
**Remarks**
Only works when [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) is True.
**Returns:**
boolean
### getExportPrintAreaOnly() {#getExportPrintAreaOnly--}
```
public boolean getExportPrintAreaOnly()
```
Indicates if only exporting the print area to html file. The default value is false.
**Returns:**
boolean
### getExportRowColumnHeadings() {#getExportRowColumnHeadings--}
```
public boolean getExportRowColumnHeadings()
```
Indicates whether exports sheet's row and column headings when saving to HTML files.
**Remarks**
The default value is false.
**Returns:**
boolean
### getExportSimilarBorderStyle() {#getExportSimilarBorderStyle--}
```
public boolean getExportSimilarBorderStyle()
```
Indicating whether exporting the similar border style when the border style is not supported by browsers. If you want to import the html or mht file to excel, please keep the default value. The default value is false.
**Returns:**
boolean
### getExportSingleTab() {#getExportSingleTab--}
```
public boolean getExportSingleTab()
```
Indicates whether exporting the single tab when the file only has one worksheet. The default value is false.
**Returns:**
boolean
### getExportWorkbookProperties() {#getExportWorkbookProperties--}
```
public boolean getExportWorkbookProperties()
```
Indicating whether exporting workbook properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value.
**Returns:**
boolean
### getExportWorksheetCSSSeparately() {#getExportWorksheetCSSSeparately--}
```
public boolean getExportWorksheetCSSSeparately()
```
Indicating whether export the worksheet css separately.The default value is false.
**Returns:**
boolean
### getExportWorksheetProperties() {#getExportWorksheetProperties--}
```
public boolean getExportWorksheetProperties()
```
Indicating whether exporting worksheet properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value.
**Returns:**
boolean
### getFilePathProvider() {#getFilePathProvider--}
```
public IFilePathProvider getFilePathProvider()
```
Gets the IFilePathProvider for exporting Worksheet to html separately.
**Returns:**
[IFilePathProvider](../../com.aspose.cells/ifilepathprovider)
### getFormatDataIgnoreColumnWidth() {#getFormatDataIgnoreColumnWidth--}
```
public boolean getFormatDataIgnoreColumnWidth()
```
Indicating whether show the whole formatted data of cell when overflowing the column. If true then ignore the column width and the whole data of cell will be exported. If false then the data will be exported same as Excel. The default value is false.
**Returns:**
boolean
### getHiddenColDisplayType() {#getHiddenColDisplayType--}
```
public int getHiddenColDisplayType()
```
Hidden column(the width of this column is 0) in excel,before save this into html format, if HtmlHiddenColDisplayType is "Remove",the hidden column would not been output, if the value is "Hidden", the column would been output,but was hidden,the default value is "Hidden"
See [HtmlHiddenColDisplayType](../../com.aspose.cells/htmlhiddencoldisplaytype).
**Returns:**
int
### getHiddenRowDisplayType() {#getHiddenRowDisplayType--}
```
public int getHiddenRowDisplayType()
```
Hidden row(the height of this row is 0) in excel,before save this into html format, if HtmlHiddenRowDisplayType is "Remove",the hidden row would not been output, if the value is "Hidden", the row would been output,but was hidden,the default value is "Hidden"
See [HtmlHiddenRowDisplayType](../../com.aspose.cells/htmlhiddenrowdisplaytype).
**Returns:**
int
### getHideOverflowWrappedText() {#getHideOverflowWrappedText--}
```
public boolean getHideOverflowWrappedText()
```
Indicates whether to hide overflow text when the cell format is set to wrap text. The default value is false
**Returns:**
boolean
### getHtmlCrossStringType() {#getHtmlCrossStringType--}
```
public int getHtmlCrossStringType()
```
Indicates if a cross-cell string will be displayed in the same way as MS Excel when saving an Excel file in html format. By default the value is Default, so, for cross-cell strings, there is little difference between the html files created by Aspose.Cells and MS Excel. But the performance for creating large html files,setting the value to Cross would be several times faster than setting it to Default or Fit2Cell.
See [HtmlCrossType](../../com.aspose.cells/htmlcrosstype).
**Returns:**
int
### getHtmlVersion() {#getHtmlVersion--}
```
public int getHtmlVersion()
```
Specifies version of HTML standard that should be used when saving the HTML format. Default value is HtmlVersion.Default.
See [HtmlVersion](../../com.aspose.cells/htmlversion).
**Returns:**
int
### getIgnoreInvisibleShapes() {#getIgnoreInvisibleShapes--}
```
public boolean getIgnoreInvisibleShapes()
```
Indicate whether exporting those not visible shapes
**Remarks**
The default values is false.
**Returns:**
boolean
### getImageOptions() {#getImageOptions--}
```
public ImageOrPrintOptions getImageOptions()
```
Get the ImageOrPrintOptions object before exporting
**Returns:**
[ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions)
### getImageScalable() {#getImageScalable--}
```
public boolean getImageScalable()
```
Indicates whether using scalable unit to describe the image width when using scalable unit to describe the column width. The default value is true.
**Returns:**
boolean
### getLinkTargetType() {#getLinkTargetType--}
```
public int getLinkTargetType()
```
Indicating the type of target attribute in `<a>` link. The default value is HtmlLinkTargetType.Parent.
See [HtmlLinkTargetType](../../com.aspose.cells/htmllinktargettype).
**Returns:**
int
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```
Indicates whether merge the areas of conditional formatting and validation before saving the file.
**Remarks**
The default value is false.
**Returns:**
boolean
### getMergeEmptyTdForcely() {#getMergeEmptyTdForcely--}
```
public boolean getMergeEmptyTdForcely()
```
Indicates whether merging empty TD element forcedly when exporting file to html. The size of html file will be reduced significantly after setting value to true. The default value is false. If you want to import the html file to excel or export perfect grid lines when saving file to html, please keep the default value.
**Returns:**
boolean
### getMergeEmptyTdType() {#getMergeEmptyTdType--}
```
public int getMergeEmptyTdType()
```
The option to merge contiguous empty cells(empty td elements) The default value is MergeEmptyTdType.Default.
See [MergeEmptyTdType](../../com.aspose.cells/mergeemptytdtype).
**Returns:**
int
### getOfficeMathOutputMode() {#getOfficeMathOutputMode--}
```
public int getOfficeMathOutputMode()
```
Indicates how export OfficeMath objects to HTML, Default value is Image.
See [HtmlOfficeMathOutputType](../../com.aspose.cells/htmlofficemathoutputtype).
**Returns:**
int
### getPageTitle() {#getPageTitle--}
```
public String getPageTitle()
```
The title of the html page. Only for saving to html stream.
**Returns:**
java.lang.String
### getParseHtmlTagInCell() {#getParseHtmlTagInCell--}
```
public boolean getParseHtmlTagInCell()
```
Indicates whether html tag(such as `<div></div>`) in cell should be parsed as cell value or preserved as it is. The default value is true.
**Returns:**
boolean
### getPresentationPreference() {#getPresentationPreference--}
```
public boolean getPresentationPreference()
```
Indicating if html or mht file is presentation preference. The default value is false. if you want to get more beautiful presentation,please set the value to true.
**Returns:**
boolean
### getRefreshChartCache() {#getRefreshChartCache--}
```
public boolean getRefreshChartCache()
```
Indicates whether refreshing chart cache data
**Returns:**
boolean
### getSaveAsSingleFile() {#getSaveAsSingleFile--}
```
public boolean getSaveAsSingleFile()
```
Indicates whether save the html as single file. The default value is false.
**Remarks**
If there are multiple worksheets or other required resources such as pictures in the workbook, commonly those worksheets and other resources need to be saved into separate files. For some scenarios, user maybe need to get only one resultant file such as for the convenience of transferring. If so, user may set this property as true.
**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```
Gets the save file format.
See [SaveFormat](../../com.aspose.cells/saveformat).
**Returns:**
int
### getSheetSet() {#getSheetSet--}
```
public SheetSet getSheetSet()
```
Gets the sheets to render. Default is all visible sheets in the workbook: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).
**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getShowAllSheets() {#getShowAllSheets--}
```
public boolean getShowAllSheets()
```
Indicates whether showing all sheets when saving as a single html file.
**Remarks**
Only works when [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) is True.
**Returns:**
boolean
### getSortExternalNames() {#getSortExternalNames--}
```
public boolean getSortExternalNames()
```
Indicates whether sorting external defined names before saving file.
**Returns:**
boolean
### getSortNames() {#getSortNames--}
```
public boolean getSortNames()
```
Indicates whether sorting defined names before saving file.
**Returns:**
boolean
### getStreamProvider() {#getStreamProvider--}
```
public IStreamProvider getStreamProvider()
```
Gets the IStreamProvider for exporting objects.
**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getTableCssId() {#getTableCssId--}
```
public String getTableCssId()
```
Gets the prefix of the type css name such as tr,col,td and so on, they are contained in the table element which has the specific TableCssId attribute. The default value is "".
**Returns:**
java.lang.String
### getUpdateSmartArt() {#getUpdateSmartArt--}
```
public boolean getUpdateSmartArt()
```
Indicates whether updating smart art setting. The default value is false.
**Remarks**
Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.
**Returns:**
boolean
### getValidateMergedAreas() {#getValidateMergedAreas--}
```
public boolean getValidateMergedAreas()
```
Indicates whether validate merged cells before saving the file.
**Remarks**
The default value is false.
**Returns:**
boolean
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```
Gets warning callback.
**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### getWidthScalable() {#getWidthScalable--}
```
public boolean getWidthScalable()
```
Indicates whether exporting column width in unit of scale to html. The default value is false.
**Returns:**
boolean
### getWorksheetScalable() {#getWorksheetScalable--}
```
public boolean getWorksheetScalable()
```
Indicates if zooming in or out the html via worksheet zoom level when saving file to html, the default value is false.
**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### isBorderCollapsed() {#isBorderCollapsed--}
```
public boolean isBorderCollapsed()
```
Indicates whether the table borders are collapsed. The default value is true.
**Returns:**
boolean
### isExpImageToTempDir() {#isExpImageToTempDir--}
```
public boolean isExpImageToTempDir()
```
Indicates whether exporting image files to temp directory. Only for saving to html stream.
**Returns:**
boolean
### isExportComments() {#isExportComments--}
```
public boolean isExportComments()
```
Indicates if exporting comments when saving file to html, the default value is false.
**Returns:**
boolean
### isFullPathLink() {#isFullPathLink--}
```
public boolean isFullPathLink()
```
Indicating whether using full path link in sheet00x.htm,filelist.xml and tabstrip.htm. The default value is false.
**Returns:**
boolean
### isIECompatible() {#isIECompatible--}
```
public boolean isIECompatible()
```
Indicating whether the output HTML is compatible with IE browser. The defalut value is false
**Returns:**
boolean
### isJsBrowserCompatible() {#isJsBrowserCompatible--}
```
public boolean isJsBrowserCompatible()
```
Indicates whether JavaScript is compatible with browsers that do not support JavaScript. The default value is true.
**Returns:**
boolean
### isMobileCompatible() {#isMobileCompatible--}
```
public boolean isMobileCompatible()
```
Indicates whether the output HTML is compatible with mobile devices. The default value is false.
**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
### setAddGenericFont(boolean value) {#setAddGenericFont-boolean-}
```
public void setAddGenericFont(boolean value)
```
Indicates whether to add a generic font to CSS font-family. The default value is true
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setAddTooltipText(boolean value) {#setAddTooltipText-boolean-}
```
public void setAddTooltipText(boolean value)
```
Indicates whether adding tooltip text when the data can't be fully displayed. The default value is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setAttachedFilesDirectory(String value) {#setAttachedFilesDirectory-java.lang.String-}
```
public void setAttachedFilesDirectory(String value)
```
The directory that the attached files will be saved to. Only for saving to html stream.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setAttachedFilesUrlPrefix(String value) {#setAttachedFilesUrlPrefix-java.lang.String-}
```
public void setAttachedFilesUrlPrefix(String value)
```
Specify the Url prefix of attached files such as image in the html file. Only for saving to html stream.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setBorderCollapsed(boolean value) {#setBorderCollapsed-boolean-}
```
public void setBorderCollapsed(boolean value)
```
Indicates whether the table borders are collapsed. The default value is true.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setCachedFileFolder(String value) {#setCachedFileFolder-java.lang.String-}
```
public void setCachedFileFolder(String value)
```
The folder for temporary files that may be used as data cache.
**Remarks**
If the folder has not been specified, the default value for it is void
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setCalculateFormula(boolean value) {#setCalculateFormula-boolean-}
```
public void setCalculateFormula(boolean value)
```
Indicates whether to calculate formulas before saving html file.
**Remarks**
The default value is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setCellCssPrefix(String value) {#setCellCssPrefix-java.lang.String-}
```
public void setCellCssPrefix(String value)
```
Sets the prefix of the css name,the default value is "".
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setCellNameAttribute(String value) {#setCellNameAttribute-java.lang.String-}
```
public void setCellNameAttribute(String value)
```
Specifies the attribute that indicates the CellName to be written. (e.g. If the value is "id", then for cell "A1", the output will be:<td id='A1'>). The default value is null.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```
Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setClearData(boolean value) {#setClearData-boolean-}
```
public void setClearData(boolean value)
```
Make the workbook empty after saving the file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setCreateDirectory(boolean value) {#setCreateDirectory-boolean-}
```
public void setCreateDirectory(boolean value)
```
If true and the directory does not exist, the directory will be automatically created before saving the file.
**Remarks**
The default value is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setCssStyles(String value) {#setCssStyles-java.lang.String-}
```
public void setCssStyles(String value)
```
Sets the additional css styles for the formatter. Only works when [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) is True.  CssStyles="body \{ padding: 5px \}";
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```
Specify the default font name for exporting html, the default font will be used when the font of style is not existing, If this property is null, Aspose.Cells will use universal font which have the same family with the original font, the default value is null.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setDisableCss(boolean value) {#setDisableCss-boolean-}
```
public void setDisableCss(boolean value)
```
Indicates whether only inline styles are applied, without relying on CSS. The default value is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setDisableDownlevelRevealedComments(boolean value) {#setDisableDownlevelRevealedComments-boolean-}
```
public void setDisableDownlevelRevealedComments(boolean value)
```
Indicates if disable Downlevel-revealed conditional comments when exporting file to html, the default value is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setEmbeddedFontType(int value) {#setEmbeddedFontType-int-}
```
public void setEmbeddedFontType(int value)
```
Sets the type of font that embedded in html. Default value is [HtmlEmbeddedFontType.NONE](../../com.aspose.cells/htmlembeddedfonttype\#NONE) which indicates that it will not embed font in html.
See [HtmlEmbeddedFontType](../../com.aspose.cells/htmlembeddedfonttype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setEnableCssCustomProperties(boolean value) {#setEnableCssCustomProperties-boolean-}
```
public void setEnableCssCustomProperties(boolean value)
```
Optimize the output of html by using CSS custom properties. For example, for the scenario that there are multiple occurences for one base64 image, with custom property the image data only needs to be saved once so the performance of the resultant html can be improved. The default value is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setEncodeEntityAsCode(boolean value) {#setEncodeEntityAsCode-boolean-}
```
public void setEncodeEntityAsCode(boolean value)
```
Indicates whether the html character entities are replaced with decimal code. (e.g. "&nbsp;" is replaced with "&\#160;"). The default value is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```
If not set,use Encoding.UTF8 as default enconding type.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |
### setEncryptDocumentProperties(boolean value) {#setEncryptDocumentProperties-boolean-}
```
public void setEncryptDocumentProperties(boolean value)
```
Indicates whether encrypt document properties when saving as .xls file. The default value is true.
**Remarks**
Only for .xls,xlsx,xlsb and xlsm file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setExcludeUnusedStyles(boolean value) {#setExcludeUnusedStyles-boolean-}
```
public void setExcludeUnusedStyles(boolean value)
```
Indicating whether excludes unused styles. For the generated html files, excluding unused styles can make the file size smaller without affecting the visual effects. So the default value of this property is true. If user needs to keep all styles in the workbook for the generated html(such as the scenario that user needs to restore the workbook from the generated html later), please set this property as false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setExpImageToTempDir(boolean value) {#setExpImageToTempDir-boolean-}
```
public void setExpImageToTempDir(boolean value)
```
Indicates whether exporting image files to temp directory. Only for saving to html stream.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setExportActiveWorksheetOnly(boolean value) {#setExportActiveWorksheetOnly-boolean-}
```
public void setExportActiveWorksheetOnly(boolean value)
```
Indicates if only exporting the active worksheet to html file. If true then only the active worksheet will be exported to html file; If false then the whole workbook will be exported to html file. The default value is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setExportArea(CellArea value) {#setExportArea-com.aspose.cells.CellArea-}
```
public void setExportArea(CellArea value)
```
Sets the exporting CellArea of current active Worksheet. If you set this attribute, the print area of current active Worksheet will be omitted. Only the specified area will be exported when saving the file to html.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellArea](../../com.aspose.cells/cellarea) |  |
### setExportBogusRowData(boolean value) {#setExportBogusRowData-boolean-}
```
public void setExportBogusRowData(boolean value)
```
Indicating whether exporting bogus bottom row data. The default value is true.If you want to import the html or mht file to excel, please keep the default value.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setExportCellCoordinate(boolean value) {#setExportCellCoordinate-boolean-}
```
public void setExportCellCoordinate(boolean value)
```
Indicates whether exporting excel coordinate of nonblank cells when saving file to html. The default value is false. If you want to import the output html to excel, please keep the default value.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setExportComments(boolean value) {#setExportComments-boolean-}
```
public void setExportComments(boolean value)
```
Indicates if exporting comments when saving file to html, the default value is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setExportCommentsType(int value) {#setExportCommentsType-int-}
```
public void setExportCommentsType(int value)
```
Represents type of exporting comments to html files.
See [PrintCommentsType](../../com.aspose.cells/printcommentstype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setExportDataOptions(int value) {#setExportDataOptions-int-}
```
public void setExportDataOptions(int value)
```
Indicating the rule of exporting html file data.The default value is All.
See [HtmlExportDataOptions](../../com.aspose.cells/htmlexportdataoptions).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setExportDocumentProperties(boolean value) {#setExportDocumentProperties-boolean-}
```
public void setExportDocumentProperties(boolean value)
```
Indicating whether exporting document properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setExportExtraHeadings(boolean value) {#setExportExtraHeadings-boolean-}
```
public void setExportExtraHeadings(boolean value)
```
Indicates whether exporting extra headings when the length of text is longer than max display column. The default value is false. If you want to import the html file to excel, please keep the default value.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setExportFormula(boolean value) {#setExportFormula-boolean-}
```
public void setExportFormula(boolean value)
```
Indicates whether exporting formula when saving file to html. The default value is true. If you want to import the output html to excel, please keep the default value.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setExportFrameScriptsAndProperties(boolean value) {#setExportFrameScriptsAndProperties-boolean-}
```
public void setExportFrameScriptsAndProperties(boolean value)
```
Indicating whether exporting frame scripts and document properties. The default value is true.If you want to import the html or mht file to excel, please keep the default value.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setExportGridLines(boolean value) {#setExportGridLines-boolean-}
```
public void setExportGridLines(boolean value)
```
Indicating whether exporting the gridlines.The default value is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setExportHeadings(boolean value) {#setExportHeadings-boolean-}
```
public void setExportHeadings(boolean value)
```
Indicates whether exports sheet's row and column headings when saving to HTML files.
**Remarks**
NOTE: This member is now obsolete. Instead, please use HtmlSaveOptions.ExportRowColumnHeadings property. This property will be removed 12 months later since June 2022. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setExportHiddenWorksheet(boolean value) {#setExportHiddenWorksheet-boolean-}
```
public void setExportHiddenWorksheet(boolean value)
```
Indicating if exporting the hidden worksheet content.The default value is true.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setExportImagesAsBase64(boolean value) {#setExportImagesAsBase64-boolean-}
```
public void setExportImagesAsBase64(boolean value)
```
Specifies whether images are saved in Base64 format to HTML, MHTML or EPUB.
**Remarks**
When this property is set to true image data is exported directly on the img elements and separate files are not created.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setExportObjectListener(IExportObjectListener value) {#setExportObjectListener-com.aspose.cells.IExportObjectListener-}
```
public void setExportObjectListener(IExportObjectListener value)
```
Sets the ExportObjectListener for exporting objects.
**Remarks**
NOTE: This property is now obsolete. Instead, please use HtmlSaveOptions.IStreamProvider property. This property will be removed 12 months later since August 2015. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IExportObjectListener](../../com.aspose.cells/iexportobjectlistener) |  |
### setExportPageFooters(boolean value) {#setExportPageFooters-boolean-}
```
public void setExportPageFooters(boolean value)
```
Indicates whether exporting page headers.
**Remarks**
Only works when [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) is True.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setExportPageHeaders(boolean value) {#setExportPageHeaders-boolean-}
```
public void setExportPageHeaders(boolean value)
```
Indicates whether exporting page headers.
**Remarks**
Only works when [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) is True.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setExportPrintAreaOnly(boolean value) {#setExportPrintAreaOnly-boolean-}
```
public void setExportPrintAreaOnly(boolean value)
```
Indicates if only exporting the print area to html file. The default value is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setExportRowColumnHeadings(boolean value) {#setExportRowColumnHeadings-boolean-}
```
public void setExportRowColumnHeadings(boolean value)
```
Indicates whether exports sheet's row and column headings when saving to HTML files.
**Remarks**
The default value is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setExportSimilarBorderStyle(boolean value) {#setExportSimilarBorderStyle-boolean-}
```
public void setExportSimilarBorderStyle(boolean value)
```
Indicating whether exporting the similar border style when the border style is not supported by browsers. If you want to import the html or mht file to excel, please keep the default value. The default value is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setExportSingleTab(boolean value) {#setExportSingleTab-boolean-}
```
public void setExportSingleTab(boolean value)
```
Indicates whether exporting the single tab when the file only has one worksheet. The default value is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setExportWorkbookProperties(boolean value) {#setExportWorkbookProperties-boolean-}
```
public void setExportWorkbookProperties(boolean value)
```
Indicating whether exporting workbook properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setExportWorksheetCSSSeparately(boolean value) {#setExportWorksheetCSSSeparately-boolean-}
```
public void setExportWorksheetCSSSeparately(boolean value)
```
Indicating whether export the worksheet css separately.The default value is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setExportWorksheetProperties(boolean value) {#setExportWorksheetProperties-boolean-}
```
public void setExportWorksheetProperties(boolean value)
```
Indicating whether exporting worksheet properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setFilePathProvider(IFilePathProvider value) {#setFilePathProvider-com.aspose.cells.IFilePathProvider-}
```
public void setFilePathProvider(IFilePathProvider value)
```
Sets the IFilePathProvider for exporting Worksheet to html separately.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IFilePathProvider](../../com.aspose.cells/ifilepathprovider) |  |
### setFormatDataIgnoreColumnWidth(boolean value) {#setFormatDataIgnoreColumnWidth-boolean-}
```
public void setFormatDataIgnoreColumnWidth(boolean value)
```
Indicating whether show the whole formatted data of cell when overflowing the column. If true then ignore the column width and the whole data of cell will be exported. If false then the data will be exported same as Excel. The default value is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setFullPathLink(boolean value) {#setFullPathLink-boolean-}
```
public void setFullPathLink(boolean value)
```
Indicating whether using full path link in sheet00x.htm,filelist.xml and tabstrip.htm. The default value is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setHiddenColDisplayType(int value) {#setHiddenColDisplayType-int-}
```
public void setHiddenColDisplayType(int value)
```
Hidden column(the width of this column is 0) in excel,before save this into html format, if HtmlHiddenColDisplayType is "Remove",the hidden column would not been output, if the value is "Hidden", the column would been output,but was hidden,the default value is "Hidden"
See [HtmlHiddenColDisplayType](../../com.aspose.cells/htmlhiddencoldisplaytype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setHiddenRowDisplayType(int value) {#setHiddenRowDisplayType-int-}
```
public void setHiddenRowDisplayType(int value)
```
Hidden row(the height of this row is 0) in excel,before save this into html format, if HtmlHiddenRowDisplayType is "Remove",the hidden row would not been output, if the value is "Hidden", the row would been output,but was hidden,the default value is "Hidden"
See [HtmlHiddenRowDisplayType](../../com.aspose.cells/htmlhiddenrowdisplaytype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setHideOverflowWrappedText(boolean value) {#setHideOverflowWrappedText-boolean-}
```
public void setHideOverflowWrappedText(boolean value)
```
Indicates whether to hide overflow text when the cell format is set to wrap text. The default value is false
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setHtmlCrossStringType(int value) {#setHtmlCrossStringType-int-}
```
public void setHtmlCrossStringType(int value)
```
Indicates if a cross-cell string will be displayed in the same way as MS Excel when saving an Excel file in html format. By default the value is Default, so, for cross-cell strings, there is little difference between the html files created by Aspose.Cells and MS Excel. But the performance for creating large html files,setting the value to Cross would be several times faster than setting it to Default or Fit2Cell.
See [HtmlCrossType](../../com.aspose.cells/htmlcrosstype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setHtmlVersion(int value) {#setHtmlVersion-int-}
```
public void setHtmlVersion(int value)
```
Specifies version of HTML standard that should be used when saving the HTML format. Default value is HtmlVersion.Default.
See [HtmlVersion](../../com.aspose.cells/htmlversion).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setIECompatible(boolean value) {#setIECompatible-boolean-}
```
public void setIECompatible(boolean value)
```
Indicating whether the output HTML is compatible with IE browser. The defalut value is false
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setIgnoreInvisibleShapes(boolean value) {#setIgnoreInvisibleShapes-boolean-}
```
public void setIgnoreInvisibleShapes(boolean value)
```
Indicate whether exporting those not visible shapes
**Remarks**
The default values is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setImageScalable(boolean value) {#setImageScalable-boolean-}
```
public void setImageScalable(boolean value)
```
Indicates whether using scalable unit to describe the image width when using scalable unit to describe the column width. The default value is true.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setJsBrowserCompatible(boolean value) {#setJsBrowserCompatible-boolean-}
```
public void setJsBrowserCompatible(boolean value)
```
Indicates whether JavaScript is compatible with browsers that do not support JavaScript. The default value is true.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setLinkTargetType(int value) {#setLinkTargetType-int-}
```
public void setLinkTargetType(int value)
```
Indicating the type of target attribute in `<a>` link. The default value is HtmlLinkTargetType.Parent.
See [HtmlLinkTargetType](../../com.aspose.cells/htmllinktargettype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setMergeAreas(boolean value) {#setMergeAreas-boolean-}
```
public void setMergeAreas(boolean value)
```
Indicates whether merge the areas of conditional formatting and validation before saving the file.
**Remarks**
The default value is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setMergeEmptyTdForcely(boolean value) {#setMergeEmptyTdForcely-boolean-}
```
public void setMergeEmptyTdForcely(boolean value)
```
Indicates whether merging empty TD element forcedly when exporting file to html. The size of html file will be reduced significantly after setting value to true. The default value is false. If you want to import the html file to excel or export perfect grid lines when saving file to html, please keep the default value.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setMergeEmptyTdType(int value) {#setMergeEmptyTdType-int-}
```
public void setMergeEmptyTdType(int value)
```
The option to merge contiguous empty cells(empty td elements) The default value is MergeEmptyTdType.Default.
See [MergeEmptyTdType](../../com.aspose.cells/mergeemptytdtype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setMobileCompatible(boolean value) {#setMobileCompatible-boolean-}
```
public void setMobileCompatible(boolean value)
```
Indicates whether the output HTML is compatible with mobile devices. The default value is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setOfficeMathOutputMode(int value) {#setOfficeMathOutputMode-int-}
```
public void setOfficeMathOutputMode(int value)
```
Indicates how export OfficeMath objects to HTML, Default value is Image.
See [HtmlOfficeMathOutputType](../../com.aspose.cells/htmlofficemathoutputtype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setPageTitle(String value) {#setPageTitle-java.lang.String-}
```
public void setPageTitle(String value)
```
The title of the html page. Only for saving to html stream.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setParseHtmlTagInCell(boolean value) {#setParseHtmlTagInCell-boolean-}
```
public void setParseHtmlTagInCell(boolean value)
```
Indicates whether html tag(such as `<div></div>`) in cell should be parsed as cell value or preserved as it is. The default value is true.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setPresentationPreference(boolean value) {#setPresentationPreference-boolean-}
```
public void setPresentationPreference(boolean value)
```
Indicating if html or mht file is presentation preference. The default value is false. if you want to get more beautiful presentation,please set the value to true.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```
Indicates whether refreshing chart cache data
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setSaveAsSingleFile(boolean value) {#setSaveAsSingleFile-boolean-}
```
public void setSaveAsSingleFile(boolean value)
```
Indicates whether save the html as single file. The default value is false.
**Remarks**
If there are multiple worksheets or other required resources such as pictures in the workbook, commonly those worksheets and other resources need to be saved into separate files. For some scenarios, user maybe need to get only one resultant file such as for the convenience of transferring. If so, user may set this property as true.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setSheetSet(SheetSet value) {#setSheetSet-com.aspose.cells.SheetSet-}
```
public void setSheetSet(SheetSet value)
```
Sets the sheets to render. Default is all visible sheets in the workbook: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SheetSet](../../com.aspose.cells/sheetset) |  |
### setShowAllSheets(boolean value) {#setShowAllSheets-boolean-}
```
public void setShowAllSheets(boolean value)
```
Indicates whether showing all sheets when saving as a single html file.
**Remarks**
Only works when [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) is True.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setSortExternalNames(boolean value) {#setSortExternalNames-boolean-}
```
public void setSortExternalNames(boolean value)
```
Indicates whether sorting external defined names before saving file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setSortNames(boolean value) {#setSortNames-boolean-}
```
public void setSortNames(boolean value)
```
Indicates whether sorting defined names before saving file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setStreamProvider(IStreamProvider value) {#setStreamProvider-com.aspose.cells.IStreamProvider-}
```
public void setStreamProvider(IStreamProvider value)
```
Sets the IStreamProvider for exporting objects.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |
### setTableCssId(String value) {#setTableCssId-java.lang.String-}
```
public void setTableCssId(String value)
```
Sets the prefix of the type css name such as tr,col,td and so on, they are contained in the table element which has the specific TableCssId attribute. The default value is "".
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setUpdateSmartArt(boolean value) {#setUpdateSmartArt-boolean-}
```
public void setUpdateSmartArt(boolean value)
```
Indicates whether updating smart art setting. The default value is false.
**Remarks**
Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setValidateMergedAreas(boolean value) {#setValidateMergedAreas-boolean-}
```
public void setValidateMergedAreas(boolean value)
```
Indicates whether validate merged cells before saving the file.
**Remarks**
The default value is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```
Sets warning callback.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IWarningCallback](../../com.aspose.cells/iwarningcallback) |  |
### setWidthScalable(boolean value) {#setWidthScalable-boolean-}
```
public void setWidthScalable(boolean value)
```
Indicates whether exporting column width in unit of scale to html. The default value is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setWorksheetScalable(boolean value) {#setWorksheetScalable-boolean-}
```
public void setWorksheetScalable(boolean value)
```
Indicates if zooming in or out the html via worksheet zoom level when saving file to html, the default value is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### toString() {#toString--}
```
public String toString()
```
**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```
### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |
