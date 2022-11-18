---
title: HtmlSaveOptions
second_title: Aspose.Cells for Java API Reference
description: Represents the options for saving html file.
type: docs
weight: 265
url: /java/com.aspose.cells/htmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class HtmlSaveOptions extends SaveOptions
```

Represents the options for saving html file.
## Constructors

| Constructor | Description |
| --- | --- |
| [HtmlSaveOptions()](#HtmlSaveOptions--) | Creates options for saving html file. |
| [HtmlSaveOptions(int format)](#HtmlSaveOptions-int-) | Creates options for saving htm file. |
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAddTooltipText()](#getAddTooltipText--) | Indicates whether adding tooltip text when the data can't be fully displayed. |
| [getAttachedFilesDirectory()](#getAttachedFilesDirectory--) | The directory that the attached files will be saved to. |
| [getAttachedFilesUrlPrefix()](#getAttachedFilesUrlPrefix--) | Specify the Url prefix of attached files such as image in the html file. |
| [getCachedFileFolder()](#getCachedFileFolder--) | The cached file folder is used to store some large data. |
| [getCellCssPrefix()](#getCellCssPrefix--) | Gets and sets the prefix of the css name,the default value is "". |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Make the workbook empty after saving the file. |
| [getCreateDirectory()](#getCreateDirectory--) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [getDefaultFontName()](#getDefaultFontName--) | Specify the default font name for exporting html, the default font will be used when the font of style is not existing, If this property is null, Aspose.Cells will use universal font which have the same family with the original font, the default value is null. |
| [getDisableDownlevelRevealedComments()](#getDisableDownlevelRevealedComments--) | Indicates if disable Downlevel-revealed conditional comments when exporting file to html, the default value is false. |
| [getEncoding()](#getEncoding--) | If not set,use Encoding.UTF8 as default enconding type. |
| [getExcludeUnusedStyles()](#getExcludeUnusedStyles--) | Indicating whether excludes unused styles. |
| [getExportActiveWorksheetOnly()](#getExportActiveWorksheetOnly--) | Indicates if exporting the whole workbook to html file. |
| [getExportArea()](#getExportArea--) | Gets or Sets the exporting CellArea of current active Worksheet. |
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
| [getExportObjectListener()](#getExportObjectListener--) | Gets or sets the ExportObjectListener for exporting objects. |
| [getExportPageFooters()](#getExportPageFooters--) | Indicates whether exporting page headers. |
| [getExportPageHeaders()](#getExportPageHeaders--) | Indicates whether exporting page headers. |
| [getExportPrintAreaOnly()](#getExportPrintAreaOnly--) | Indicates if only exporting the print area to html file. |
| [getExportRowColumnHeadings()](#getExportRowColumnHeadings--) | Indicates whether exports sheet's row and column headings when saving to HTML files. |
| [getExportSimilarBorderStyle()](#getExportSimilarBorderStyle--) | Indicating whether exporting the similar border style when the border style is not supported by browsers. |
| [getExportSingleTab()](#getExportSingleTab--) | Indicates whether exporting the single tab when the file only has one worksheet. |
| [getExportWorkbookProperties()](#getExportWorkbookProperties--) | Indicating whether exporting workbook properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [getExportWorksheetCSSSeparately()](#getExportWorksheetCSSSeparately--) | Indicating whether export the worksheet css separately.The default value is false. |
| [getExportWorksheetProperties()](#getExportWorksheetProperties--) | Indicating whether exporting worksheet properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [getFilePathProvider()](#getFilePathProvider--) | Gets or sets the IFilePathProvider for exporting Worksheet to html separately. |
| [getHiddenColDisplayType()](#getHiddenColDisplayType--) | Hidden column(the width of this column is 0) in excel,before save this into html format, if HtmlHiddenColDisplayType is "Remove",the hidden column would not been output, if the value is "Hidden", the column would been output,but was hidden,the default value is "Hidden" |
| [getHiddenRowDisplayType()](#getHiddenRowDisplayType--) | Hidden row(the height of this row is 0) in excel,before save this into html format, if HtmlHiddenRowDisplayType is "Remove",the hidden row would not been output, if the value is "Hidden", the row would been output,but was hidden,the default value is "Hidden" |
| [getHtmlCrossStringType()](#getHtmlCrossStringType--) | Indicates if a cross-cell string will be displayed in the same way as MS Excel when saving an Excel file in html format. |
| [getIgnoreInvisibleShapes()](#getIgnoreInvisibleShapes--) | Indicate whether exporting those not visible shapes The default values is false. |
| [getImageOptions()](#getImageOptions--) | Get the ImageOrPrintOptions object before exporting |
| [getImageScalable()](#getImageScalable--) | Indicates whether using scalable unit to describe the image width when using scalable unit to describe the column width. |
| [getLinkTargetType()](#getLinkTargetType--) | Indicating the type of target attribute in <a> link,The default value is HtmlLinkTargetType.Parent. |
| [getMergeAreas()](#getMergeAreas--) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [getMergeEmptyTdForcely()](#getMergeEmptyTdForcely--) | Indicates whether merging empty TD element forcedly when exporting file to html. |
| [getPageTitle()](#getPageTitle--) | The title of the html page. |
| [getParseHtmlTagInCell()](#getParseHtmlTagInCell--) | Parse html tag in cell,like

,as cell value,or as html tag,default is true |
| [getPresentationPreference()](#getPresentationPreference--) | Indicating if html or mht file is presentation preference. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Indicates whether refreshing chart cache data |
| [getSaveAsSingleFile()](#getSaveAsSingleFile--) | Indicates whether save the html as single file. |
| [getSaveFormat()](#getSaveFormat--) | Gets the save file format. |
| [getShowAllSheets()](#getShowAllSheets--) | Indicates whether showing all sheets when saving as a single html file. |
| [getSortExternalNames()](#getSortExternalNames--) | Indicates whether sorting external defined names before saving file. |
| [getSortNames()](#getSortNames--) | Indicates whether sorting defined names before saving file. |
| [getStreamProvider()](#getStreamProvider--) | Gets or sets the IStreamProvider for exporting objects. |
| [getTableCssId()](#getTableCssId--) | Gets and sets the prefix of the type css name such as tr,col,td and so on, they are contained in the table element which has the specific TableCssId attribute. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Indicates whether updating smart art setting. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Indicates whether validate merged cells before saving the file. |
| [getWarningCallback()](#getWarningCallback--) | Gets or sets warning callback. |
| [getWidthScalable()](#getWidthScalable--) | Indicates whether using scalable unit to describe the column width when exporting file to html. |
| [getWorksheetScalable()](#getWorksheetScalable--) | Indicates if zooming in or out the html via worksheet zoom level when saving file to html, the default value is false. |
| [hashCode()](#hashCode--) |  |
| [isExpImageToTempDir()](#isExpImageToTempDir--) | Indicates whether exporting image files to temp directory. |
| [isExportComments()](#isExportComments--) | Indicates if exporting comments when saving file to html, the default value is false. |
| [isFullPathLink()](#isFullPathLink--) | Indicating whether using full path link in sheet00x.htm,filelist.xml and tabstrip.htm. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAddTooltipText(boolean value)](#setAddTooltipText-boolean-) | Please see the getter of this property: [getAddTooltipText()](../../com.aspose.cells/htmlsaveoptions\#getAddTooltipText--) |
| [setAttachedFilesDirectory(String value)](#setAttachedFilesDirectory-java.lang.String-) | Please see the getter of this property: [getAttachedFilesDirectory()](../../com.aspose.cells/htmlsaveoptions\#getAttachedFilesDirectory--) |
| [setAttachedFilesUrlPrefix(String value)](#setAttachedFilesUrlPrefix-java.lang.String-) | Please see the getter of this property: [getAttachedFilesUrlPrefix()](../../com.aspose.cells/htmlsaveoptions\#getAttachedFilesUrlPrefix--) |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | Please see the getter of this property: @CREF1852\_ |
| [setCellCssPrefix(String value)](#setCellCssPrefix-java.lang.String-) | Please see the getter of this property: [getCellCssPrefix()](../../com.aspose.cells/htmlsaveoptions\#getCellCssPrefix--) |
| [setClearData(boolean value)](#setClearData-boolean-) | Please see the getter of this property: @CREF1851\_ |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Please see the getter of this property: @CREF1855\_ |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Please see the getter of this property: [getDefaultFontName()](../../com.aspose.cells/htmlsaveoptions\#getDefaultFontName--) |
| [setDisableDownlevelRevealedComments(boolean value)](#setDisableDownlevelRevealedComments-boolean-) | Please see the getter of this property: [getDisableDownlevelRevealedComments()](../../com.aspose.cells/htmlsaveoptions\#getDisableDownlevelRevealedComments--) |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | Please see the getter of this property: [getEncoding()](../../com.aspose.cells/htmlsaveoptions\#getEncoding--) |
| [setExcludeUnusedStyles(boolean value)](#setExcludeUnusedStyles-boolean-) | Please see the getter of this property: [getExcludeUnusedStyles()](../../com.aspose.cells/htmlsaveoptions\#getExcludeUnusedStyles--) |
| [setExpImageToTempDir(boolean value)](#setExpImageToTempDir-boolean-) | Please see the getter of this property: [isExpImageToTempDir()](../../com.aspose.cells/htmlsaveoptions\#isExpImageToTempDir--) |
| [setExportActiveWorksheetOnly(boolean value)](#setExportActiveWorksheetOnly-boolean-) | Please see the getter of this property: [getExportActiveWorksheetOnly()](../../com.aspose.cells/htmlsaveoptions\#getExportActiveWorksheetOnly--) |
| [setExportArea(CellArea value)](#setExportArea-com.aspose.cells.CellArea-) | Please see the getter of this property: [getExportArea()](../../com.aspose.cells/htmlsaveoptions\#getExportArea--) |
| [setExportBogusRowData(boolean value)](#setExportBogusRowData-boolean-) | Please see the getter of this property: [getExportBogusRowData()](../../com.aspose.cells/htmlsaveoptions\#getExportBogusRowData--) |
| [setExportCellCoordinate(boolean value)](#setExportCellCoordinate-boolean-) | Please see the getter of this property: [getExportCellCoordinate()](../../com.aspose.cells/htmlsaveoptions\#getExportCellCoordinate--) |
| [setExportComments(boolean value)](#setExportComments-boolean-) | Please see the getter of this property: [isExportComments()](../../com.aspose.cells/htmlsaveoptions\#isExportComments--) |
| [setExportCommentsType(int value)](#setExportCommentsType-int-) | Please see the getter of this property: [getExportCommentsType()](../../com.aspose.cells/htmlsaveoptions\#getExportCommentsType--) |
| [setExportDataOptions(int value)](#setExportDataOptions-int-) | Please see the getter of this property: [getExportDataOptions()](../../com.aspose.cells/htmlsaveoptions\#getExportDataOptions--) |
| [setExportDocumentProperties(boolean value)](#setExportDocumentProperties-boolean-) | Please see the getter of this property: [getExportDocumentProperties()](../../com.aspose.cells/htmlsaveoptions\#getExportDocumentProperties--) |
| [setExportExtraHeadings(boolean value)](#setExportExtraHeadings-boolean-) | Please see the getter of this property: [getExportExtraHeadings()](../../com.aspose.cells/htmlsaveoptions\#getExportExtraHeadings--) |
| [setExportFormula(boolean value)](#setExportFormula-boolean-) | Please see the getter of this property: [getExportFormula()](../../com.aspose.cells/htmlsaveoptions\#getExportFormula--) |
| [setExportFrameScriptsAndProperties(boolean value)](#setExportFrameScriptsAndProperties-boolean-) | Please see the getter of this property: [getExportFrameScriptsAndProperties()](../../com.aspose.cells/htmlsaveoptions\#getExportFrameScriptsAndProperties--) |
| [setExportGridLines(boolean value)](#setExportGridLines-boolean-) | Please see the getter of this property: [getExportGridLines()](../../com.aspose.cells/htmlsaveoptions\#getExportGridLines--) |
| [setExportHeadings(boolean value)](#setExportHeadings-boolean-) | Please see the getter of this property: [getExportHeadings()](../../com.aspose.cells/htmlsaveoptions\#getExportHeadings--) |
| [setExportHiddenWorksheet(boolean value)](#setExportHiddenWorksheet-boolean-) | Please see the getter of this property: [getExportHiddenWorksheet()](../../com.aspose.cells/htmlsaveoptions\#getExportHiddenWorksheet--) |
| [setExportImagesAsBase64(boolean value)](#setExportImagesAsBase64-boolean-) | Please see the getter of this property: [getExportImagesAsBase64()](../../com.aspose.cells/htmlsaveoptions\#getExportImagesAsBase64--) |
| [setExportObjectListener(IExportObjectListener value)](#setExportObjectListener-com.aspose.cells.IExportObjectListener-) | Please see the getter of this property: [getExportObjectListener()](../../com.aspose.cells/htmlsaveoptions\#getExportObjectListener--) |
| [setExportPageFooters(boolean value)](#setExportPageFooters-boolean-) | Please see the getter of this property: [getExportPageFooters()](../../com.aspose.cells/htmlsaveoptions\#getExportPageFooters--) |
| [setExportPageHeaders(boolean value)](#setExportPageHeaders-boolean-) | Please see the getter of this property: [getExportPageHeaders()](../../com.aspose.cells/htmlsaveoptions\#getExportPageHeaders--) |
| [setExportPrintAreaOnly(boolean value)](#setExportPrintAreaOnly-boolean-) | Please see the getter of this property: [getExportPrintAreaOnly()](../../com.aspose.cells/htmlsaveoptions\#getExportPrintAreaOnly--) |
| [setExportRowColumnHeadings(boolean value)](#setExportRowColumnHeadings-boolean-) | Please see the getter of this property: [getExportRowColumnHeadings()](../../com.aspose.cells/htmlsaveoptions\#getExportRowColumnHeadings--) |
| [setExportSimilarBorderStyle(boolean value)](#setExportSimilarBorderStyle-boolean-) | Please see the getter of this property: [getExportSimilarBorderStyle()](../../com.aspose.cells/htmlsaveoptions\#getExportSimilarBorderStyle--) |
| [setExportSingleTab(boolean value)](#setExportSingleTab-boolean-) | Please see the getter of this property: [getExportSingleTab()](../../com.aspose.cells/htmlsaveoptions\#getExportSingleTab--) |
| [setExportWorkbookProperties(boolean value)](#setExportWorkbookProperties-boolean-) | Please see the getter of this property: [getExportWorkbookProperties()](../../com.aspose.cells/htmlsaveoptions\#getExportWorkbookProperties--) |
| [setExportWorksheetCSSSeparately(boolean value)](#setExportWorksheetCSSSeparately-boolean-) | Please see the getter of this property: [getExportWorksheetCSSSeparately()](../../com.aspose.cells/htmlsaveoptions\#getExportWorksheetCSSSeparately--) |
| [setExportWorksheetProperties(boolean value)](#setExportWorksheetProperties-boolean-) | Please see the getter of this property: [getExportWorksheetProperties()](../../com.aspose.cells/htmlsaveoptions\#getExportWorksheetProperties--) |
| [setFilePathProvider(IFilePathProvider value)](#setFilePathProvider-com.aspose.cells.IFilePathProvider-) | Please see the getter of this property: [getFilePathProvider()](../../com.aspose.cells/htmlsaveoptions\#getFilePathProvider--) |
| [setFullPathLink(boolean value)](#setFullPathLink-boolean-) | Please see the getter of this property: [isFullPathLink()](../../com.aspose.cells/htmlsaveoptions\#isFullPathLink--) |
| [setHiddenColDisplayType(int value)](#setHiddenColDisplayType-int-) | Please see the getter of this property: [getHiddenColDisplayType()](../../com.aspose.cells/htmlsaveoptions\#getHiddenColDisplayType--) |
| [setHiddenRowDisplayType(int value)](#setHiddenRowDisplayType-int-) | Please see the getter of this property: [getHiddenRowDisplayType()](../../com.aspose.cells/htmlsaveoptions\#getHiddenRowDisplayType--) |
| [setHtmlCrossStringType(int value)](#setHtmlCrossStringType-int-) | Please see the getter of this property: [getHtmlCrossStringType()](../../com.aspose.cells/htmlsaveoptions\#getHtmlCrossStringType--) |
| [setIgnoreInvisibleShapes(boolean value)](#setIgnoreInvisibleShapes-boolean-) | Please see the getter of this property: [getIgnoreInvisibleShapes()](../../com.aspose.cells/htmlsaveoptions\#getIgnoreInvisibleShapes--) |
| [setImageScalable(boolean value)](#setImageScalable-boolean-) | Please see the getter of this property: [getImageScalable()](../../com.aspose.cells/htmlsaveoptions\#getImageScalable--) |
| [setLinkTargetType(int value)](#setLinkTargetType-int-) | Please see the getter of this property: [getLinkTargetType()](../../com.aspose.cells/htmlsaveoptions\#getLinkTargetType--) |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Please see the getter of this property: @CREF1854\_ |
| [setMergeEmptyTdForcely(boolean value)](#setMergeEmptyTdForcely-boolean-) | Please see the getter of this property: [getMergeEmptyTdForcely()](../../com.aspose.cells/htmlsaveoptions\#getMergeEmptyTdForcely--) |
| [setPageTitle(String value)](#setPageTitle-java.lang.String-) | Please see the getter of this property: [getPageTitle()](../../com.aspose.cells/htmlsaveoptions\#getPageTitle--) |
| [setParseHtmlTagInCell(boolean value)](#setParseHtmlTagInCell-boolean-) | Please see the getter of this property: [getParseHtmlTagInCell()](../../com.aspose.cells/htmlsaveoptions\#getParseHtmlTagInCell--) |
| [setPresentationPreference(boolean value)](#setPresentationPreference-boolean-) | Please see the getter of this property: [getPresentationPreference()](../../com.aspose.cells/htmlsaveoptions\#getPresentationPreference--) |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Please see the getter of this property: @CREF1858\_ |
| [setSaveAsSingleFile(boolean value)](#setSaveAsSingleFile-boolean-) | Please see the getter of this property: [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) |
| [setShowAllSheets(boolean value)](#setShowAllSheets-boolean-) | Please see the getter of this property: [getShowAllSheets()](../../com.aspose.cells/htmlsaveoptions\#getShowAllSheets--) |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Please see the getter of this property: @CREF1857\_ |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Please see the getter of this property: @CREF1856\_ |
| [setStreamProvider(IStreamProvider value)](#setStreamProvider-com.aspose.cells.IStreamProvider-) | Please see the getter of this property: [getStreamProvider()](../../com.aspose.cells/htmlsaveoptions\#getStreamProvider--) |
| [setTableCssId(String value)](#setTableCssId-java.lang.String-) | Please see the getter of this property: [getTableCssId()](../../com.aspose.cells/htmlsaveoptions\#getTableCssId--) |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Please see the getter of this property: @CREF1860\_ |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Please see the getter of this property: @CREF1853\_ |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) |  |
| [setWidthScalable(boolean value)](#setWidthScalable-boolean-) | Please see the getter of this property: [getWidthScalable()](../../com.aspose.cells/htmlsaveoptions\#getWidthScalable--) |
| [setWorksheetScalable(boolean value)](#setWorksheetScalable-boolean-) | Please see the getter of this property: [getWorksheetScalable()](../../com.aspose.cells/htmlsaveoptions\#getWorksheetScalable--) |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### HtmlSaveOptions() {#HtmlSaveOptions--}
```
public HtmlSaveOptions()
```


Creates options for saving html file.

### HtmlSaveOptions(int format) {#HtmlSaveOptions-int-}
```
public HtmlSaveOptions(int format)
```


Creates options for saving htm file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| format | int | The saving file format. |

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


The cached file folder is used to store some large data.

**Returns:**
java.lang.String
### getCellCssPrefix() {#getCellCssPrefix--}
```
public String getCellCssPrefix()
```


Gets and sets the prefix of the css name,the default value is "".

**Returns:**
java.lang.String
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


If true and the directory does not exist, the directory will be automatically created before saving the file. The default value is false.

**Returns:**
boolean
### getDefaultFontName() {#getDefaultFontName--}
```
public String getDefaultFontName()
```


Specify the default font name for exporting html, the default font will be used when the font of style is not existing, If this property is null, Aspose.Cells will use universal font which have the same family with the original font, the default value is null.

**Returns:**
java.lang.String
### getDisableDownlevelRevealedComments() {#getDisableDownlevelRevealedComments--}
```
public boolean getDisableDownlevelRevealedComments()
```


Indicates if disable Downlevel-revealed conditional comments when exporting file to html, the default value is false.

**Returns:**
boolean
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


If not set,use Encoding.UTF8 as default enconding type.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
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


Indicates if exporting the whole workbook to html file.

**Returns:**
boolean
### getExportArea() {#getExportArea--}
```
public CellArea getExportArea()
```


Gets or Sets the exporting CellArea of current active Worksheet. If you set this attribute, the print area of current active Worksheet will be omitted. Only the specified area will be exported when saving the file to html.

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

**Returns:**
int
### getExportDataOptions() {#getExportDataOptions--}
```
public int getExportDataOptions()
```


Indicating the rule of exporting html file data.The default value is All.

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


Indicates whether exports sheet's row and column headings when saving to HTML files. NOTE: This member is now obsolete. Instead, please use HtmlSaveOptions.ExportRowColumnHeadings property. This property will be removed 12 months later since June 2022. Aspose apologizes for any inconvenience you may have experienced.

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


Specifies whether images are saved in Base64 format to HTML, MHTML or EPUB. When this property is set to true image data is exported directly on the img elements and separate files are not created.

**Returns:**
boolean
### getExportObjectListener() {#getExportObjectListener--}
```
public IExportObjectListener getExportObjectListener()
```


Gets or sets the ExportObjectListener for exporting objects. NOTE: This property is now obsolete. Instead, please use HtmlSaveOptions.IStreamProvider property. This property will be removed 12 months later since August 2015. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
[IExportObjectListener](../../com.aspose.cells/iexportobjectlistener)
### getExportPageFooters() {#getExportPageFooters--}
```
public boolean getExportPageFooters()
```


Indicates whether exporting page headers. Only works when [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) is True.

**Returns:**
boolean
### getExportPageHeaders() {#getExportPageHeaders--}
```
public boolean getExportPageHeaders()
```


Indicates whether exporting page headers. Only works when [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) is True.

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


Indicates whether exports sheet's row and column headings when saving to HTML files. The default value is false.

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


Gets or sets the IFilePathProvider for exporting Worksheet to html separately.

**Returns:**
[IFilePathProvider](../../com.aspose.cells/ifilepathprovider)
### getHiddenColDisplayType() {#getHiddenColDisplayType--}
```
public int getHiddenColDisplayType()
```


Hidden column(the width of this column is 0) in excel,before save this into html format, if HtmlHiddenColDisplayType is "Remove",the hidden column would not been output, if the value is "Hidden", the column would been output,but was hidden,the default value is "Hidden"

**Returns:**
int
### getHiddenRowDisplayType() {#getHiddenRowDisplayType--}
```
public int getHiddenRowDisplayType()
```


Hidden row(the height of this row is 0) in excel,before save this into html format, if HtmlHiddenRowDisplayType is "Remove",the hidden row would not been output, if the value is "Hidden", the row would been output,but was hidden,the default value is "Hidden"

**Returns:**
int
### getHtmlCrossStringType() {#getHtmlCrossStringType--}
```
public int getHtmlCrossStringType()
```


Indicates if a cross-cell string will be displayed in the same way as MS Excel when saving an Excel file in html format. By default the value is Default, so, for cross-cell strings, there is little difference between the html files created by Aspose.Cells and MS Excel. But the performance for creating large html files,setting the value to Cross would be several times faster than setting it to Default or Fit2Cell.

**Returns:**
int
### getIgnoreInvisibleShapes() {#getIgnoreInvisibleShapes--}
```
public boolean getIgnoreInvisibleShapes()
```


Indicate whether exporting those not visible shapes The default values is false.

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


Indicating the type of target attribute in <a> link,The default value is HtmlLinkTargetType.Parent.

**Returns:**
int
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is false.

**Returns:**
boolean
### getMergeEmptyTdForcely() {#getMergeEmptyTdForcely--}
```
public boolean getMergeEmptyTdForcely()
```


Indicates whether merging empty TD element forcedly when exporting file to html. The size of html file will be reduced significantly after setting value to true. The default value is false. If you want to import the html file to excel or export perfect grid lines when saving file to html, please keep the default value.

**Returns:**
boolean
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


Parse html tag in cell,like

,as cell value,or as html tag,default is true

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


Indicates whether save the html as single file. The default value is false. If there are multiple worksheets or other required resources such as pictures in the workbook, commonly those worksheets and other resources need to be saved into separate files. For some scenarios, user maybe need to get only one resultant file such as for the convenience of transferring. If so, user may set this property as true.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Gets the save file format.

**Returns:**
int
### getShowAllSheets() {#getShowAllSheets--}
```
public boolean getShowAllSheets()
```


Indicates whether showing all sheets when saving as a single html file. Only works when [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) is True.

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


Gets or sets the IStreamProvider for exporting objects.

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getTableCssId() {#getTableCssId--}
```
public String getTableCssId()
```


Gets and sets the prefix of the type css name such as tr,col,td and so on, they are contained in the table element which has the specific TableCssId attribute. The default value is "".

**Returns:**
java.lang.String
### getUpdateSmartArt() {#getUpdateSmartArt--}
```
public boolean getUpdateSmartArt()
```


Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

**Returns:**
boolean
### getValidateMergedAreas() {#getValidateMergedAreas--}
```
public boolean getValidateMergedAreas()
```


Indicates whether validate merged cells before saving the file. The default value is false.

**Returns:**
boolean
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Gets or sets warning callback.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### getWidthScalable() {#getWidthScalable--}
```
public boolean getWidthScalable()
```


Indicates whether using scalable unit to describe the column width when exporting file to html. The default value is false.

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
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAddTooltipText(boolean value) {#setAddTooltipText-boolean-}
```
public void setAddTooltipText(boolean value)
```


Please see the getter of this property: [getAddTooltipText()](../../com.aspose.cells/htmlsaveoptions\#getAddTooltipText--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAttachedFilesDirectory(String value) {#setAttachedFilesDirectory-java.lang.String-}
```
public void setAttachedFilesDirectory(String value)
```


Please see the getter of this property: [getAttachedFilesDirectory()](../../com.aspose.cells/htmlsaveoptions\#getAttachedFilesDirectory--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setAttachedFilesUrlPrefix(String value) {#setAttachedFilesUrlPrefix-java.lang.String-}
```
public void setAttachedFilesUrlPrefix(String value)
```


Please see the getter of this property: [getAttachedFilesUrlPrefix()](../../com.aspose.cells/htmlsaveoptions\#getAttachedFilesUrlPrefix--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setCachedFileFolder(String value) {#setCachedFileFolder-java.lang.String-}
```
public void setCachedFileFolder(String value)
```


Please see the getter of this property: @CREF1852\_

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setCellCssPrefix(String value) {#setCellCssPrefix-java.lang.String-}
```
public void setCellCssPrefix(String value)
```


Please see the getter of this property: [getCellCssPrefix()](../../com.aspose.cells/htmlsaveoptions\#getCellCssPrefix--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setClearData(boolean value) {#setClearData-boolean-}
```
public void setClearData(boolean value)
```


Please see the getter of this property: @CREF1851\_

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setCreateDirectory(boolean value) {#setCreateDirectory-boolean-}
```
public void setCreateDirectory(boolean value)
```


Please see the getter of this property: @CREF1855\_

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```


Please see the getter of this property: [getDefaultFontName()](../../com.aspose.cells/htmlsaveoptions\#getDefaultFontName--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setDisableDownlevelRevealedComments(boolean value) {#setDisableDownlevelRevealedComments-boolean-}
```
public void setDisableDownlevelRevealedComments(boolean value)
```


Please see the getter of this property: [getDisableDownlevelRevealedComments()](../../com.aspose.cells/htmlsaveoptions\#getDisableDownlevelRevealedComments--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```


Please see the getter of this property: [getEncoding()](../../com.aspose.cells/htmlsaveoptions\#getEncoding--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

### setExcludeUnusedStyles(boolean value) {#setExcludeUnusedStyles-boolean-}
```
public void setExcludeUnusedStyles(boolean value)
```


Please see the getter of this property: [getExcludeUnusedStyles()](../../com.aspose.cells/htmlsaveoptions\#getExcludeUnusedStyles--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExpImageToTempDir(boolean value) {#setExpImageToTempDir-boolean-}
```
public void setExpImageToTempDir(boolean value)
```


Please see the getter of this property: [isExpImageToTempDir()](../../com.aspose.cells/htmlsaveoptions\#isExpImageToTempDir--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportActiveWorksheetOnly(boolean value) {#setExportActiveWorksheetOnly-boolean-}
```
public void setExportActiveWorksheetOnly(boolean value)
```


Please see the getter of this property: [getExportActiveWorksheetOnly()](../../com.aspose.cells/htmlsaveoptions\#getExportActiveWorksheetOnly--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportArea(CellArea value) {#setExportArea-com.aspose.cells.CellArea-}
```
public void setExportArea(CellArea value)
```


Please see the getter of this property: [getExportArea()](../../com.aspose.cells/htmlsaveoptions\#getExportArea--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellArea](../../com.aspose.cells/cellarea) |  |

### setExportBogusRowData(boolean value) {#setExportBogusRowData-boolean-}
```
public void setExportBogusRowData(boolean value)
```


Please see the getter of this property: [getExportBogusRowData()](../../com.aspose.cells/htmlsaveoptions\#getExportBogusRowData--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportCellCoordinate(boolean value) {#setExportCellCoordinate-boolean-}
```
public void setExportCellCoordinate(boolean value)
```


Please see the getter of this property: [getExportCellCoordinate()](../../com.aspose.cells/htmlsaveoptions\#getExportCellCoordinate--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportComments(boolean value) {#setExportComments-boolean-}
```
public void setExportComments(boolean value)
```


Please see the getter of this property: [isExportComments()](../../com.aspose.cells/htmlsaveoptions\#isExportComments--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportCommentsType(int value) {#setExportCommentsType-int-}
```
public void setExportCommentsType(int value)
```


Please see the getter of this property: [getExportCommentsType()](../../com.aspose.cells/htmlsaveoptions\#getExportCommentsType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setExportDataOptions(int value) {#setExportDataOptions-int-}
```
public void setExportDataOptions(int value)
```


Please see the getter of this property: [getExportDataOptions()](../../com.aspose.cells/htmlsaveoptions\#getExportDataOptions--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setExportDocumentProperties(boolean value) {#setExportDocumentProperties-boolean-}
```
public void setExportDocumentProperties(boolean value)
```


Please see the getter of this property: [getExportDocumentProperties()](../../com.aspose.cells/htmlsaveoptions\#getExportDocumentProperties--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportExtraHeadings(boolean value) {#setExportExtraHeadings-boolean-}
```
public void setExportExtraHeadings(boolean value)
```


Please see the getter of this property: [getExportExtraHeadings()](../../com.aspose.cells/htmlsaveoptions\#getExportExtraHeadings--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportFormula(boolean value) {#setExportFormula-boolean-}
```
public void setExportFormula(boolean value)
```


Please see the getter of this property: [getExportFormula()](../../com.aspose.cells/htmlsaveoptions\#getExportFormula--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportFrameScriptsAndProperties(boolean value) {#setExportFrameScriptsAndProperties-boolean-}
```
public void setExportFrameScriptsAndProperties(boolean value)
```


Please see the getter of this property: [getExportFrameScriptsAndProperties()](../../com.aspose.cells/htmlsaveoptions\#getExportFrameScriptsAndProperties--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportGridLines(boolean value) {#setExportGridLines-boolean-}
```
public void setExportGridLines(boolean value)
```


Please see the getter of this property: [getExportGridLines()](../../com.aspose.cells/htmlsaveoptions\#getExportGridLines--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportHeadings(boolean value) {#setExportHeadings-boolean-}
```
public void setExportHeadings(boolean value)
```


Please see the getter of this property: [getExportHeadings()](../../com.aspose.cells/htmlsaveoptions\#getExportHeadings--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportHiddenWorksheet(boolean value) {#setExportHiddenWorksheet-boolean-}
```
public void setExportHiddenWorksheet(boolean value)
```


Please see the getter of this property: [getExportHiddenWorksheet()](../../com.aspose.cells/htmlsaveoptions\#getExportHiddenWorksheet--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportImagesAsBase64(boolean value) {#setExportImagesAsBase64-boolean-}
```
public void setExportImagesAsBase64(boolean value)
```


Please see the getter of this property: [getExportImagesAsBase64()](../../com.aspose.cells/htmlsaveoptions\#getExportImagesAsBase64--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportObjectListener(IExportObjectListener value) {#setExportObjectListener-com.aspose.cells.IExportObjectListener-}
```
public void setExportObjectListener(IExportObjectListener value)
```


Please see the getter of this property: [getExportObjectListener()](../../com.aspose.cells/htmlsaveoptions\#getExportObjectListener--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IExportObjectListener](../../com.aspose.cells/iexportobjectlistener) |  |

### setExportPageFooters(boolean value) {#setExportPageFooters-boolean-}
```
public void setExportPageFooters(boolean value)
```


Please see the getter of this property: [getExportPageFooters()](../../com.aspose.cells/htmlsaveoptions\#getExportPageFooters--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportPageHeaders(boolean value) {#setExportPageHeaders-boolean-}
```
public void setExportPageHeaders(boolean value)
```


Please see the getter of this property: [getExportPageHeaders()](../../com.aspose.cells/htmlsaveoptions\#getExportPageHeaders--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportPrintAreaOnly(boolean value) {#setExportPrintAreaOnly-boolean-}
```
public void setExportPrintAreaOnly(boolean value)
```


Please see the getter of this property: [getExportPrintAreaOnly()](../../com.aspose.cells/htmlsaveoptions\#getExportPrintAreaOnly--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportRowColumnHeadings(boolean value) {#setExportRowColumnHeadings-boolean-}
```
public void setExportRowColumnHeadings(boolean value)
```


Please see the getter of this property: [getExportRowColumnHeadings()](../../com.aspose.cells/htmlsaveoptions\#getExportRowColumnHeadings--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportSimilarBorderStyle(boolean value) {#setExportSimilarBorderStyle-boolean-}
```
public void setExportSimilarBorderStyle(boolean value)
```


Please see the getter of this property: [getExportSimilarBorderStyle()](../../com.aspose.cells/htmlsaveoptions\#getExportSimilarBorderStyle--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportSingleTab(boolean value) {#setExportSingleTab-boolean-}
```
public void setExportSingleTab(boolean value)
```


Please see the getter of this property: [getExportSingleTab()](../../com.aspose.cells/htmlsaveoptions\#getExportSingleTab--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportWorkbookProperties(boolean value) {#setExportWorkbookProperties-boolean-}
```
public void setExportWorkbookProperties(boolean value)
```


Please see the getter of this property: [getExportWorkbookProperties()](../../com.aspose.cells/htmlsaveoptions\#getExportWorkbookProperties--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportWorksheetCSSSeparately(boolean value) {#setExportWorksheetCSSSeparately-boolean-}
```
public void setExportWorksheetCSSSeparately(boolean value)
```


Please see the getter of this property: [getExportWorksheetCSSSeparately()](../../com.aspose.cells/htmlsaveoptions\#getExportWorksheetCSSSeparately--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportWorksheetProperties(boolean value) {#setExportWorksheetProperties-boolean-}
```
public void setExportWorksheetProperties(boolean value)
```


Please see the getter of this property: [getExportWorksheetProperties()](../../com.aspose.cells/htmlsaveoptions\#getExportWorksheetProperties--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setFilePathProvider(IFilePathProvider value) {#setFilePathProvider-com.aspose.cells.IFilePathProvider-}
```
public void setFilePathProvider(IFilePathProvider value)
```


Please see the getter of this property: [getFilePathProvider()](../../com.aspose.cells/htmlsaveoptions\#getFilePathProvider--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IFilePathProvider](../../com.aspose.cells/ifilepathprovider) |  |

### setFullPathLink(boolean value) {#setFullPathLink-boolean-}
```
public void setFullPathLink(boolean value)
```


Please see the getter of this property: [isFullPathLink()](../../com.aspose.cells/htmlsaveoptions\#isFullPathLink--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHiddenColDisplayType(int value) {#setHiddenColDisplayType-int-}
```
public void setHiddenColDisplayType(int value)
```


Please see the getter of this property: [getHiddenColDisplayType()](../../com.aspose.cells/htmlsaveoptions\#getHiddenColDisplayType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setHiddenRowDisplayType(int value) {#setHiddenRowDisplayType-int-}
```
public void setHiddenRowDisplayType(int value)
```


Please see the getter of this property: [getHiddenRowDisplayType()](../../com.aspose.cells/htmlsaveoptions\#getHiddenRowDisplayType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setHtmlCrossStringType(int value) {#setHtmlCrossStringType-int-}
```
public void setHtmlCrossStringType(int value)
```


Please see the getter of this property: [getHtmlCrossStringType()](../../com.aspose.cells/htmlsaveoptions\#getHtmlCrossStringType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setIgnoreInvisibleShapes(boolean value) {#setIgnoreInvisibleShapes-boolean-}
```
public void setIgnoreInvisibleShapes(boolean value)
```


Please see the getter of this property: [getIgnoreInvisibleShapes()](../../com.aspose.cells/htmlsaveoptions\#getIgnoreInvisibleShapes--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setImageScalable(boolean value) {#setImageScalable-boolean-}
```
public void setImageScalable(boolean value)
```


Please see the getter of this property: [getImageScalable()](../../com.aspose.cells/htmlsaveoptions\#getImageScalable--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setLinkTargetType(int value) {#setLinkTargetType-int-}
```
public void setLinkTargetType(int value)
```


Please see the getter of this property: [getLinkTargetType()](../../com.aspose.cells/htmlsaveoptions\#getLinkTargetType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setMergeAreas(boolean value) {#setMergeAreas-boolean-}
```
public void setMergeAreas(boolean value)
```


Please see the getter of this property: @CREF1854\_

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setMergeEmptyTdForcely(boolean value) {#setMergeEmptyTdForcely-boolean-}
```
public void setMergeEmptyTdForcely(boolean value)
```


Please see the getter of this property: [getMergeEmptyTdForcely()](../../com.aspose.cells/htmlsaveoptions\#getMergeEmptyTdForcely--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setPageTitle(String value) {#setPageTitle-java.lang.String-}
```
public void setPageTitle(String value)
```


Please see the getter of this property: [getPageTitle()](../../com.aspose.cells/htmlsaveoptions\#getPageTitle--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setParseHtmlTagInCell(boolean value) {#setParseHtmlTagInCell-boolean-}
```
public void setParseHtmlTagInCell(boolean value)
```


Please see the getter of this property: [getParseHtmlTagInCell()](../../com.aspose.cells/htmlsaveoptions\#getParseHtmlTagInCell--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setPresentationPreference(boolean value) {#setPresentationPreference-boolean-}
```
public void setPresentationPreference(boolean value)
```


Please see the getter of this property: [getPresentationPreference()](../../com.aspose.cells/htmlsaveoptions\#getPresentationPreference--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


Please see the getter of this property: @CREF1858\_

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSaveAsSingleFile(boolean value) {#setSaveAsSingleFile-boolean-}
```
public void setSaveAsSingleFile(boolean value)
```


Please see the getter of this property: [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowAllSheets(boolean value) {#setShowAllSheets-boolean-}
```
public void setShowAllSheets(boolean value)
```


Please see the getter of this property: [getShowAllSheets()](../../com.aspose.cells/htmlsaveoptions\#getShowAllSheets--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSortExternalNames(boolean value) {#setSortExternalNames-boolean-}
```
public void setSortExternalNames(boolean value)
```


Please see the getter of this property: @CREF1857\_

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSortNames(boolean value) {#setSortNames-boolean-}
```
public void setSortNames(boolean value)
```


Please see the getter of this property: @CREF1856\_

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setStreamProvider(IStreamProvider value) {#setStreamProvider-com.aspose.cells.IStreamProvider-}
```
public void setStreamProvider(IStreamProvider value)
```


Please see the getter of this property: [getStreamProvider()](../../com.aspose.cells/htmlsaveoptions\#getStreamProvider--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setTableCssId(String value) {#setTableCssId-java.lang.String-}
```
public void setTableCssId(String value)
```


Please see the getter of this property: [getTableCssId()](../../com.aspose.cells/htmlsaveoptions\#getTableCssId--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setUpdateSmartArt(boolean value) {#setUpdateSmartArt-boolean-}
```
public void setUpdateSmartArt(boolean value)
```


Please see the getter of this property: @CREF1860\_

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setValidateMergedAreas(boolean value) {#setValidateMergedAreas-boolean-}
```
public void setValidateMergedAreas(boolean value)
```


Please see the getter of this property: @CREF1853\_

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IWarningCallback](../../com.aspose.cells/iwarningcallback) |  |

### setWidthScalable(boolean value) {#setWidthScalable-boolean-}
```
public void setWidthScalable(boolean value)
```


Please see the getter of this property: [getWidthScalable()](../../com.aspose.cells/htmlsaveoptions\#getWidthScalable--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setWorksheetScalable(boolean value) {#setWorksheetScalable-boolean-}
```
public void setWorksheetScalable(boolean value)
```


Please see the getter of this property: [getWorksheetScalable()](../../com.aspose.cells/htmlsaveoptions\#getWorksheetScalable--)

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

