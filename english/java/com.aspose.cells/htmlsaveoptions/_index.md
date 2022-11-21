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
| [getCellCssPrefix()](#getCellCssPrefix--) | the prefix of the css name,the default value is "". |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Make the workbook empty after saving the file. |
| [getCreateDirectory()](#getCreateDirectory--) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [getDefaultFontName()](#getDefaultFontName--) | Specify the default font name for exporting html, the default font will be used when the font of style is not existing, If this property is null, Aspose.Cells will use universal font which have the same family with the original font, the default value is null. |
| [getDisableDownlevelRevealedComments()](#getDisableDownlevelRevealedComments--) | Indicates if disable Downlevel-revealed conditional comments when exporting file to html, the default value is false. |
| [getEncoding()](#getEncoding--) | If not set,use Encoding.UTF8 as default enconding type. |
| [getExcludeUnusedStyles()](#getExcludeUnusedStyles--) | Indicating whether excludes unused styles. |
| [getExportActiveWorksheetOnly()](#getExportActiveWorksheetOnly--) | Indicates if exporting the whole workbook to html file. |
| [getExportArea()](#getExportArea--) | the exporting CellArea of current active Worksheet. |
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
| [getExportObjectListener()](#getExportObjectListener--) | the ExportObjectListener for exporting objects. |
| [getExportPageFooters()](#getExportPageFooters--) | Indicates whether exporting page headers. |
| [getExportPageHeaders()](#getExportPageHeaders--) | Indicates whether exporting page headers. |
| [getExportPrintAreaOnly()](#getExportPrintAreaOnly--) | Indicates if only exporting the print area to html file. |
| [getExportRowColumnHeadings()](#getExportRowColumnHeadings--) | Indicates whether exports sheet's row and column headings when saving to HTML files. |
| [getExportSimilarBorderStyle()](#getExportSimilarBorderStyle--) | Indicating whether exporting the similar border style when the border style is not supported by browsers. |
| [getExportSingleTab()](#getExportSingleTab--) | Indicates whether exporting the single tab when the file only has one worksheet. |
| [getExportWorkbookProperties()](#getExportWorkbookProperties--) | Indicating whether exporting workbook properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [getExportWorksheetCSSSeparately()](#getExportWorksheetCSSSeparately--) | Indicating whether export the worksheet css separately.The default value is false. |
| [getExportWorksheetProperties()](#getExportWorksheetProperties--) | Indicating whether exporting worksheet properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [getFilePathProvider()](#getFilePathProvider--) | the IFilePathProvider for exporting Worksheet to html separately. |
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
| [getStreamProvider()](#getStreamProvider--) | the IStreamProvider for exporting objects. |
| [getTableCssId()](#getTableCssId--) | the prefix of the type css name such as tr,col,td and so on, they are contained in the table element which has the specific TableCssId attribute. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Indicates whether updating smart art setting. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Indicates whether validate merged cells before saving the file. |
| [getWarningCallback()](#getWarningCallback--) | warning callback. |
| [getWidthScalable()](#getWidthScalable--) | Indicates whether using scalable unit to describe the column width when exporting file to html. |
| [getWorksheetScalable()](#getWorksheetScalable--) | Indicates if zooming in or out the html via worksheet zoom level when saving file to html, the default value is false. |
| [hashCode()](#hashCode--) |  |
| [isExpImageToTempDir()](#isExpImageToTempDir--) | Indicates whether exporting image files to temp directory. |
| [isExportComments()](#isExportComments--) | Indicates if exporting comments when saving file to html, the default value is false. |
| [isFullPathLink()](#isFullPathLink--) | Indicating whether using full path link in sheet00x.htm,filelist.xml and tabstrip.htm. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAddTooltipText(boolean value)](#setAddTooltipText-boolean-) | For the description of this property, please see [getAddTooltipText()](../../com.aspose.cells/htmlsaveoptions\#getAddTooltipText--) |
| [setAttachedFilesDirectory(String value)](#setAttachedFilesDirectory-java.lang.String-) | For the description of this property, please see [getAttachedFilesDirectory()](../../com.aspose.cells/htmlsaveoptions\#getAttachedFilesDirectory--) |
| [setAttachedFilesUrlPrefix(String value)](#setAttachedFilesUrlPrefix-java.lang.String-) | For the description of this property, please see [getAttachedFilesUrlPrefix()](../../com.aspose.cells/htmlsaveoptions\#getAttachedFilesUrlPrefix--) |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | For the description of this property, please see [getCachedFileFolder()](../../com.aspose.cells/saveoptions\#getCachedFileFolder--) |
| [setCellCssPrefix(String value)](#setCellCssPrefix-java.lang.String-) | For the description of this property, please see [getCellCssPrefix()](../../com.aspose.cells/htmlsaveoptions\#getCellCssPrefix--) |
| [setClearData(boolean value)](#setClearData-boolean-) | For the description of this property, please see [getClearData()](../../com.aspose.cells/saveoptions\#getClearData--) |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | For the description of this property, please see [getCreateDirectory()](../../com.aspose.cells/saveoptions\#getCreateDirectory--) |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | For the description of this property, please see [getDefaultFontName()](../../com.aspose.cells/htmlsaveoptions\#getDefaultFontName--) |
| [setDisableDownlevelRevealedComments(boolean value)](#setDisableDownlevelRevealedComments-boolean-) | For the description of this property, please see [getDisableDownlevelRevealedComments()](../../com.aspose.cells/htmlsaveoptions\#getDisableDownlevelRevealedComments--) |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | For the description of this property, please see [getEncoding()](../../com.aspose.cells/htmlsaveoptions\#getEncoding--) |
| [setExcludeUnusedStyles(boolean value)](#setExcludeUnusedStyles-boolean-) | For the description of this property, please see [getExcludeUnusedStyles()](../../com.aspose.cells/htmlsaveoptions\#getExcludeUnusedStyles--) |
| [setExpImageToTempDir(boolean value)](#setExpImageToTempDir-boolean-) | For the description of this property, please see [isExpImageToTempDir()](../../com.aspose.cells/htmlsaveoptions\#isExpImageToTempDir--) |
| [setExportActiveWorksheetOnly(boolean value)](#setExportActiveWorksheetOnly-boolean-) | For the description of this property, please see [getExportActiveWorksheetOnly()](../../com.aspose.cells/htmlsaveoptions\#getExportActiveWorksheetOnly--) |
| [setExportArea(CellArea value)](#setExportArea-com.aspose.cells.CellArea-) | For the description of this property, please see [getExportArea()](../../com.aspose.cells/htmlsaveoptions\#getExportArea--) |
| [setExportBogusRowData(boolean value)](#setExportBogusRowData-boolean-) | For the description of this property, please see [getExportBogusRowData()](../../com.aspose.cells/htmlsaveoptions\#getExportBogusRowData--) |
| [setExportCellCoordinate(boolean value)](#setExportCellCoordinate-boolean-) | For the description of this property, please see [getExportCellCoordinate()](../../com.aspose.cells/htmlsaveoptions\#getExportCellCoordinate--) |
| [setExportComments(boolean value)](#setExportComments-boolean-) | For the description of this property, please see [isExportComments()](../../com.aspose.cells/htmlsaveoptions\#isExportComments--) |
| [setExportCommentsType(int value)](#setExportCommentsType-int-) | For the description of this property, please see [getExportCommentsType()](../../com.aspose.cells/htmlsaveoptions\#getExportCommentsType--) |
| [setExportDataOptions(int value)](#setExportDataOptions-int-) | For the description of this property, please see [getExportDataOptions()](../../com.aspose.cells/htmlsaveoptions\#getExportDataOptions--) |
| [setExportDocumentProperties(boolean value)](#setExportDocumentProperties-boolean-) | For the description of this property, please see [getExportDocumentProperties()](../../com.aspose.cells/htmlsaveoptions\#getExportDocumentProperties--) |
| [setExportExtraHeadings(boolean value)](#setExportExtraHeadings-boolean-) | For the description of this property, please see [getExportExtraHeadings()](../../com.aspose.cells/htmlsaveoptions\#getExportExtraHeadings--) |
| [setExportFormula(boolean value)](#setExportFormula-boolean-) | For the description of this property, please see [getExportFormula()](../../com.aspose.cells/htmlsaveoptions\#getExportFormula--) |
| [setExportFrameScriptsAndProperties(boolean value)](#setExportFrameScriptsAndProperties-boolean-) | For the description of this property, please see [getExportFrameScriptsAndProperties()](../../com.aspose.cells/htmlsaveoptions\#getExportFrameScriptsAndProperties--) |
| [setExportGridLines(boolean value)](#setExportGridLines-boolean-) | For the description of this property, please see [getExportGridLines()](../../com.aspose.cells/htmlsaveoptions\#getExportGridLines--) |
| [setExportHeadings(boolean value)](#setExportHeadings-boolean-) | For the description of this property, please see [getExportHeadings()](../../com.aspose.cells/htmlsaveoptions\#getExportHeadings--) |
| [setExportHiddenWorksheet(boolean value)](#setExportHiddenWorksheet-boolean-) | For the description of this property, please see [getExportHiddenWorksheet()](../../com.aspose.cells/htmlsaveoptions\#getExportHiddenWorksheet--) |
| [setExportImagesAsBase64(boolean value)](#setExportImagesAsBase64-boolean-) | For the description of this property, please see [getExportImagesAsBase64()](../../com.aspose.cells/htmlsaveoptions\#getExportImagesAsBase64--) |
| [setExportObjectListener(IExportObjectListener value)](#setExportObjectListener-com.aspose.cells.IExportObjectListener-) | For the description of this property, please see [getExportObjectListener()](../../com.aspose.cells/htmlsaveoptions\#getExportObjectListener--) |
| [setExportPageFooters(boolean value)](#setExportPageFooters-boolean-) | For the description of this property, please see [getExportPageFooters()](../../com.aspose.cells/htmlsaveoptions\#getExportPageFooters--) |
| [setExportPageHeaders(boolean value)](#setExportPageHeaders-boolean-) | For the description of this property, please see [getExportPageHeaders()](../../com.aspose.cells/htmlsaveoptions\#getExportPageHeaders--) |
| [setExportPrintAreaOnly(boolean value)](#setExportPrintAreaOnly-boolean-) | For the description of this property, please see [getExportPrintAreaOnly()](../../com.aspose.cells/htmlsaveoptions\#getExportPrintAreaOnly--) |
| [setExportRowColumnHeadings(boolean value)](#setExportRowColumnHeadings-boolean-) | For the description of this property, please see [getExportRowColumnHeadings()](../../com.aspose.cells/htmlsaveoptions\#getExportRowColumnHeadings--) |
| [setExportSimilarBorderStyle(boolean value)](#setExportSimilarBorderStyle-boolean-) | For the description of this property, please see [getExportSimilarBorderStyle()](../../com.aspose.cells/htmlsaveoptions\#getExportSimilarBorderStyle--) |
| [setExportSingleTab(boolean value)](#setExportSingleTab-boolean-) | For the description of this property, please see [getExportSingleTab()](../../com.aspose.cells/htmlsaveoptions\#getExportSingleTab--) |
| [setExportWorkbookProperties(boolean value)](#setExportWorkbookProperties-boolean-) | For the description of this property, please see [getExportWorkbookProperties()](../../com.aspose.cells/htmlsaveoptions\#getExportWorkbookProperties--) |
| [setExportWorksheetCSSSeparately(boolean value)](#setExportWorksheetCSSSeparately-boolean-) | For the description of this property, please see [getExportWorksheetCSSSeparately()](../../com.aspose.cells/htmlsaveoptions\#getExportWorksheetCSSSeparately--) |
| [setExportWorksheetProperties(boolean value)](#setExportWorksheetProperties-boolean-) | For the description of this property, please see [getExportWorksheetProperties()](../../com.aspose.cells/htmlsaveoptions\#getExportWorksheetProperties--) |
| [setFilePathProvider(IFilePathProvider value)](#setFilePathProvider-com.aspose.cells.IFilePathProvider-) | For the description of this property, please see [getFilePathProvider()](../../com.aspose.cells/htmlsaveoptions\#getFilePathProvider--) |
| [setFullPathLink(boolean value)](#setFullPathLink-boolean-) | For the description of this property, please see [isFullPathLink()](../../com.aspose.cells/htmlsaveoptions\#isFullPathLink--) |
| [setHiddenColDisplayType(int value)](#setHiddenColDisplayType-int-) | For the description of this property, please see [getHiddenColDisplayType()](../../com.aspose.cells/htmlsaveoptions\#getHiddenColDisplayType--) |
| [setHiddenRowDisplayType(int value)](#setHiddenRowDisplayType-int-) | For the description of this property, please see [getHiddenRowDisplayType()](../../com.aspose.cells/htmlsaveoptions\#getHiddenRowDisplayType--) |
| [setHtmlCrossStringType(int value)](#setHtmlCrossStringType-int-) | For the description of this property, please see [getHtmlCrossStringType()](../../com.aspose.cells/htmlsaveoptions\#getHtmlCrossStringType--) |
| [setIgnoreInvisibleShapes(boolean value)](#setIgnoreInvisibleShapes-boolean-) | For the description of this property, please see [getIgnoreInvisibleShapes()](../../com.aspose.cells/htmlsaveoptions\#getIgnoreInvisibleShapes--) |
| [setImageScalable(boolean value)](#setImageScalable-boolean-) | For the description of this property, please see [getImageScalable()](../../com.aspose.cells/htmlsaveoptions\#getImageScalable--) |
| [setLinkTargetType(int value)](#setLinkTargetType-int-) | For the description of this property, please see [getLinkTargetType()](../../com.aspose.cells/htmlsaveoptions\#getLinkTargetType--) |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | For the description of this property, please see [getMergeAreas()](../../com.aspose.cells/saveoptions\#getMergeAreas--) |
| [setMergeEmptyTdForcely(boolean value)](#setMergeEmptyTdForcely-boolean-) | For the description of this property, please see [getMergeEmptyTdForcely()](../../com.aspose.cells/htmlsaveoptions\#getMergeEmptyTdForcely--) |
| [setPageTitle(String value)](#setPageTitle-java.lang.String-) | For the description of this property, please see [getPageTitle()](../../com.aspose.cells/htmlsaveoptions\#getPageTitle--) |
| [setParseHtmlTagInCell(boolean value)](#setParseHtmlTagInCell-boolean-) | For the description of this property, please see [getParseHtmlTagInCell()](../../com.aspose.cells/htmlsaveoptions\#getParseHtmlTagInCell--) |
| [setPresentationPreference(boolean value)](#setPresentationPreference-boolean-) | For the description of this property, please see [getPresentationPreference()](../../com.aspose.cells/htmlsaveoptions\#getPresentationPreference--) |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | For the description of this property, please see [getRefreshChartCache()](../../com.aspose.cells/saveoptions\#getRefreshChartCache--) |
| [setSaveAsSingleFile(boolean value)](#setSaveAsSingleFile-boolean-) | For the description of this property, please see [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) |
| [setShowAllSheets(boolean value)](#setShowAllSheets-boolean-) | For the description of this property, please see [getShowAllSheets()](../../com.aspose.cells/htmlsaveoptions\#getShowAllSheets--) |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | For the description of this property, please see [getSortExternalNames()](../../com.aspose.cells/saveoptions\#getSortExternalNames--) |
| [setSortNames(boolean value)](#setSortNames-boolean-) | For the description of this property, please see [getSortNames()](../../com.aspose.cells/saveoptions\#getSortNames--) |
| [setStreamProvider(IStreamProvider value)](#setStreamProvider-com.aspose.cells.IStreamProvider-) | For the description of this property, please see [getStreamProvider()](../../com.aspose.cells/htmlsaveoptions\#getStreamProvider--) |
| [setTableCssId(String value)](#setTableCssId-java.lang.String-) | For the description of this property, please see [getTableCssId()](../../com.aspose.cells/htmlsaveoptions\#getTableCssId--) |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | For the description of this property, please see [getUpdateSmartArt()](../../com.aspose.cells/saveoptions\#getUpdateSmartArt--) |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | For the description of this property, please see [getValidateMergedAreas()](../../com.aspose.cells/saveoptions\#getValidateMergedAreas--) |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) |  |
| [setWidthScalable(boolean value)](#setWidthScalable-boolean-) | For the description of this property, please see [getWidthScalable()](../../com.aspose.cells/htmlsaveoptions\#getWidthScalable--) |
| [setWorksheetScalable(boolean value)](#setWorksheetScalable-boolean-) | For the description of this property, please see [getWorksheetScalable()](../../com.aspose.cells/htmlsaveoptions\#getWorksheetScalable--) |
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


the prefix of the css name,the default value is "".

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


the exporting CellArea of current active Worksheet. If you set this attribute, the print area of current active Worksheet will be omitted. Only the specified area will be exported when saving the file to html.

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


the ExportObjectListener for exporting objects. NOTE: This property is now obsolete. Instead, please use HtmlSaveOptions.IStreamProvider property. This property will be removed 12 months later since August 2015. Aspose apologizes for any inconvenience you may have experienced.

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


the IFilePathProvider for exporting Worksheet to html separately.

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


the IStreamProvider for exporting objects.

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getTableCssId() {#getTableCssId--}
```
public String getTableCssId()
```


the prefix of the type css name such as tr,col,td and so on, they are contained in the table element which has the specific TableCssId attribute. The default value is "".

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


warning callback.

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


For the description of this property, please see [getAddTooltipText()](../../com.aspose.cells/htmlsaveoptions\#getAddTooltipText--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAttachedFilesDirectory(String value) {#setAttachedFilesDirectory-java.lang.String-}
```
public void setAttachedFilesDirectory(String value)
```


For the description of this property, please see [getAttachedFilesDirectory()](../../com.aspose.cells/htmlsaveoptions\#getAttachedFilesDirectory--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setAttachedFilesUrlPrefix(String value) {#setAttachedFilesUrlPrefix-java.lang.String-}
```
public void setAttachedFilesUrlPrefix(String value)
```


For the description of this property, please see [getAttachedFilesUrlPrefix()](../../com.aspose.cells/htmlsaveoptions\#getAttachedFilesUrlPrefix--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setCachedFileFolder(String value) {#setCachedFileFolder-java.lang.String-}
```
public void setCachedFileFolder(String value)
```


For the description of this property, please see [getCachedFileFolder()](../../com.aspose.cells/saveoptions\#getCachedFileFolder--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setCellCssPrefix(String value) {#setCellCssPrefix-java.lang.String-}
```
public void setCellCssPrefix(String value)
```


For the description of this property, please see [getCellCssPrefix()](../../com.aspose.cells/htmlsaveoptions\#getCellCssPrefix--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setClearData(boolean value) {#setClearData-boolean-}
```
public void setClearData(boolean value)
```


For the description of this property, please see [getClearData()](../../com.aspose.cells/saveoptions\#getClearData--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setCreateDirectory(boolean value) {#setCreateDirectory-boolean-}
```
public void setCreateDirectory(boolean value)
```


For the description of this property, please see [getCreateDirectory()](../../com.aspose.cells/saveoptions\#getCreateDirectory--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```


For the description of this property, please see [getDefaultFontName()](../../com.aspose.cells/htmlsaveoptions\#getDefaultFontName--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setDisableDownlevelRevealedComments(boolean value) {#setDisableDownlevelRevealedComments-boolean-}
```
public void setDisableDownlevelRevealedComments(boolean value)
```


For the description of this property, please see [getDisableDownlevelRevealedComments()](../../com.aspose.cells/htmlsaveoptions\#getDisableDownlevelRevealedComments--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```


For the description of this property, please see [getEncoding()](../../com.aspose.cells/htmlsaveoptions\#getEncoding--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

### setExcludeUnusedStyles(boolean value) {#setExcludeUnusedStyles-boolean-}
```
public void setExcludeUnusedStyles(boolean value)
```


For the description of this property, please see [getExcludeUnusedStyles()](../../com.aspose.cells/htmlsaveoptions\#getExcludeUnusedStyles--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExpImageToTempDir(boolean value) {#setExpImageToTempDir-boolean-}
```
public void setExpImageToTempDir(boolean value)
```


For the description of this property, please see [isExpImageToTempDir()](../../com.aspose.cells/htmlsaveoptions\#isExpImageToTempDir--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportActiveWorksheetOnly(boolean value) {#setExportActiveWorksheetOnly-boolean-}
```
public void setExportActiveWorksheetOnly(boolean value)
```


For the description of this property, please see [getExportActiveWorksheetOnly()](../../com.aspose.cells/htmlsaveoptions\#getExportActiveWorksheetOnly--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportArea(CellArea value) {#setExportArea-com.aspose.cells.CellArea-}
```
public void setExportArea(CellArea value)
```


For the description of this property, please see [getExportArea()](../../com.aspose.cells/htmlsaveoptions\#getExportArea--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellArea](../../com.aspose.cells/cellarea) |  |

### setExportBogusRowData(boolean value) {#setExportBogusRowData-boolean-}
```
public void setExportBogusRowData(boolean value)
```


For the description of this property, please see [getExportBogusRowData()](../../com.aspose.cells/htmlsaveoptions\#getExportBogusRowData--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportCellCoordinate(boolean value) {#setExportCellCoordinate-boolean-}
```
public void setExportCellCoordinate(boolean value)
```


For the description of this property, please see [getExportCellCoordinate()](../../com.aspose.cells/htmlsaveoptions\#getExportCellCoordinate--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportComments(boolean value) {#setExportComments-boolean-}
```
public void setExportComments(boolean value)
```


For the description of this property, please see [isExportComments()](../../com.aspose.cells/htmlsaveoptions\#isExportComments--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportCommentsType(int value) {#setExportCommentsType-int-}
```
public void setExportCommentsType(int value)
```


For the description of this property, please see [getExportCommentsType()](../../com.aspose.cells/htmlsaveoptions\#getExportCommentsType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setExportDataOptions(int value) {#setExportDataOptions-int-}
```
public void setExportDataOptions(int value)
```


For the description of this property, please see [getExportDataOptions()](../../com.aspose.cells/htmlsaveoptions\#getExportDataOptions--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setExportDocumentProperties(boolean value) {#setExportDocumentProperties-boolean-}
```
public void setExportDocumentProperties(boolean value)
```


For the description of this property, please see [getExportDocumentProperties()](../../com.aspose.cells/htmlsaveoptions\#getExportDocumentProperties--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportExtraHeadings(boolean value) {#setExportExtraHeadings-boolean-}
```
public void setExportExtraHeadings(boolean value)
```


For the description of this property, please see [getExportExtraHeadings()](../../com.aspose.cells/htmlsaveoptions\#getExportExtraHeadings--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportFormula(boolean value) {#setExportFormula-boolean-}
```
public void setExportFormula(boolean value)
```


For the description of this property, please see [getExportFormula()](../../com.aspose.cells/htmlsaveoptions\#getExportFormula--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportFrameScriptsAndProperties(boolean value) {#setExportFrameScriptsAndProperties-boolean-}
```
public void setExportFrameScriptsAndProperties(boolean value)
```


For the description of this property, please see [getExportFrameScriptsAndProperties()](../../com.aspose.cells/htmlsaveoptions\#getExportFrameScriptsAndProperties--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportGridLines(boolean value) {#setExportGridLines-boolean-}
```
public void setExportGridLines(boolean value)
```


For the description of this property, please see [getExportGridLines()](../../com.aspose.cells/htmlsaveoptions\#getExportGridLines--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportHeadings(boolean value) {#setExportHeadings-boolean-}
```
public void setExportHeadings(boolean value)
```


For the description of this property, please see [getExportHeadings()](../../com.aspose.cells/htmlsaveoptions\#getExportHeadings--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportHiddenWorksheet(boolean value) {#setExportHiddenWorksheet-boolean-}
```
public void setExportHiddenWorksheet(boolean value)
```


For the description of this property, please see [getExportHiddenWorksheet()](../../com.aspose.cells/htmlsaveoptions\#getExportHiddenWorksheet--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportImagesAsBase64(boolean value) {#setExportImagesAsBase64-boolean-}
```
public void setExportImagesAsBase64(boolean value)
```


For the description of this property, please see [getExportImagesAsBase64()](../../com.aspose.cells/htmlsaveoptions\#getExportImagesAsBase64--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportObjectListener(IExportObjectListener value) {#setExportObjectListener-com.aspose.cells.IExportObjectListener-}
```
public void setExportObjectListener(IExportObjectListener value)
```


For the description of this property, please see [getExportObjectListener()](../../com.aspose.cells/htmlsaveoptions\#getExportObjectListener--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IExportObjectListener](../../com.aspose.cells/iexportobjectlistener) |  |

### setExportPageFooters(boolean value) {#setExportPageFooters-boolean-}
```
public void setExportPageFooters(boolean value)
```


For the description of this property, please see [getExportPageFooters()](../../com.aspose.cells/htmlsaveoptions\#getExportPageFooters--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportPageHeaders(boolean value) {#setExportPageHeaders-boolean-}
```
public void setExportPageHeaders(boolean value)
```


For the description of this property, please see [getExportPageHeaders()](../../com.aspose.cells/htmlsaveoptions\#getExportPageHeaders--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportPrintAreaOnly(boolean value) {#setExportPrintAreaOnly-boolean-}
```
public void setExportPrintAreaOnly(boolean value)
```


For the description of this property, please see [getExportPrintAreaOnly()](../../com.aspose.cells/htmlsaveoptions\#getExportPrintAreaOnly--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportRowColumnHeadings(boolean value) {#setExportRowColumnHeadings-boolean-}
```
public void setExportRowColumnHeadings(boolean value)
```


For the description of this property, please see [getExportRowColumnHeadings()](../../com.aspose.cells/htmlsaveoptions\#getExportRowColumnHeadings--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportSimilarBorderStyle(boolean value) {#setExportSimilarBorderStyle-boolean-}
```
public void setExportSimilarBorderStyle(boolean value)
```


For the description of this property, please see [getExportSimilarBorderStyle()](../../com.aspose.cells/htmlsaveoptions\#getExportSimilarBorderStyle--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportSingleTab(boolean value) {#setExportSingleTab-boolean-}
```
public void setExportSingleTab(boolean value)
```


For the description of this property, please see [getExportSingleTab()](../../com.aspose.cells/htmlsaveoptions\#getExportSingleTab--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportWorkbookProperties(boolean value) {#setExportWorkbookProperties-boolean-}
```
public void setExportWorkbookProperties(boolean value)
```


For the description of this property, please see [getExportWorkbookProperties()](../../com.aspose.cells/htmlsaveoptions\#getExportWorkbookProperties--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportWorksheetCSSSeparately(boolean value) {#setExportWorksheetCSSSeparately-boolean-}
```
public void setExportWorksheetCSSSeparately(boolean value)
```


For the description of this property, please see [getExportWorksheetCSSSeparately()](../../com.aspose.cells/htmlsaveoptions\#getExportWorksheetCSSSeparately--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportWorksheetProperties(boolean value) {#setExportWorksheetProperties-boolean-}
```
public void setExportWorksheetProperties(boolean value)
```


For the description of this property, please see [getExportWorksheetProperties()](../../com.aspose.cells/htmlsaveoptions\#getExportWorksheetProperties--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setFilePathProvider(IFilePathProvider value) {#setFilePathProvider-com.aspose.cells.IFilePathProvider-}
```
public void setFilePathProvider(IFilePathProvider value)
```


For the description of this property, please see [getFilePathProvider()](../../com.aspose.cells/htmlsaveoptions\#getFilePathProvider--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IFilePathProvider](../../com.aspose.cells/ifilepathprovider) |  |

### setFullPathLink(boolean value) {#setFullPathLink-boolean-}
```
public void setFullPathLink(boolean value)
```


For the description of this property, please see [isFullPathLink()](../../com.aspose.cells/htmlsaveoptions\#isFullPathLink--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHiddenColDisplayType(int value) {#setHiddenColDisplayType-int-}
```
public void setHiddenColDisplayType(int value)
```


For the description of this property, please see [getHiddenColDisplayType()](../../com.aspose.cells/htmlsaveoptions\#getHiddenColDisplayType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setHiddenRowDisplayType(int value) {#setHiddenRowDisplayType-int-}
```
public void setHiddenRowDisplayType(int value)
```


For the description of this property, please see [getHiddenRowDisplayType()](../../com.aspose.cells/htmlsaveoptions\#getHiddenRowDisplayType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setHtmlCrossStringType(int value) {#setHtmlCrossStringType-int-}
```
public void setHtmlCrossStringType(int value)
```


For the description of this property, please see [getHtmlCrossStringType()](../../com.aspose.cells/htmlsaveoptions\#getHtmlCrossStringType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setIgnoreInvisibleShapes(boolean value) {#setIgnoreInvisibleShapes-boolean-}
```
public void setIgnoreInvisibleShapes(boolean value)
```


For the description of this property, please see [getIgnoreInvisibleShapes()](../../com.aspose.cells/htmlsaveoptions\#getIgnoreInvisibleShapes--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setImageScalable(boolean value) {#setImageScalable-boolean-}
```
public void setImageScalable(boolean value)
```


For the description of this property, please see [getImageScalable()](../../com.aspose.cells/htmlsaveoptions\#getImageScalable--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setLinkTargetType(int value) {#setLinkTargetType-int-}
```
public void setLinkTargetType(int value)
```


For the description of this property, please see [getLinkTargetType()](../../com.aspose.cells/htmlsaveoptions\#getLinkTargetType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setMergeAreas(boolean value) {#setMergeAreas-boolean-}
```
public void setMergeAreas(boolean value)
```


For the description of this property, please see [getMergeAreas()](../../com.aspose.cells/saveoptions\#getMergeAreas--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setMergeEmptyTdForcely(boolean value) {#setMergeEmptyTdForcely-boolean-}
```
public void setMergeEmptyTdForcely(boolean value)
```


For the description of this property, please see [getMergeEmptyTdForcely()](../../com.aspose.cells/htmlsaveoptions\#getMergeEmptyTdForcely--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setPageTitle(String value) {#setPageTitle-java.lang.String-}
```
public void setPageTitle(String value)
```


For the description of this property, please see [getPageTitle()](../../com.aspose.cells/htmlsaveoptions\#getPageTitle--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setParseHtmlTagInCell(boolean value) {#setParseHtmlTagInCell-boolean-}
```
public void setParseHtmlTagInCell(boolean value)
```


For the description of this property, please see [getParseHtmlTagInCell()](../../com.aspose.cells/htmlsaveoptions\#getParseHtmlTagInCell--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setPresentationPreference(boolean value) {#setPresentationPreference-boolean-}
```
public void setPresentationPreference(boolean value)
```


For the description of this property, please see [getPresentationPreference()](../../com.aspose.cells/htmlsaveoptions\#getPresentationPreference--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


For the description of this property, please see [getRefreshChartCache()](../../com.aspose.cells/saveoptions\#getRefreshChartCache--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSaveAsSingleFile(boolean value) {#setSaveAsSingleFile-boolean-}
```
public void setSaveAsSingleFile(boolean value)
```


For the description of this property, please see [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowAllSheets(boolean value) {#setShowAllSheets-boolean-}
```
public void setShowAllSheets(boolean value)
```


For the description of this property, please see [getShowAllSheets()](../../com.aspose.cells/htmlsaveoptions\#getShowAllSheets--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSortExternalNames(boolean value) {#setSortExternalNames-boolean-}
```
public void setSortExternalNames(boolean value)
```


For the description of this property, please see [getSortExternalNames()](../../com.aspose.cells/saveoptions\#getSortExternalNames--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSortNames(boolean value) {#setSortNames-boolean-}
```
public void setSortNames(boolean value)
```


For the description of this property, please see [getSortNames()](../../com.aspose.cells/saveoptions\#getSortNames--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setStreamProvider(IStreamProvider value) {#setStreamProvider-com.aspose.cells.IStreamProvider-}
```
public void setStreamProvider(IStreamProvider value)
```


For the description of this property, please see [getStreamProvider()](../../com.aspose.cells/htmlsaveoptions\#getStreamProvider--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setTableCssId(String value) {#setTableCssId-java.lang.String-}
```
public void setTableCssId(String value)
```


For the description of this property, please see [getTableCssId()](../../com.aspose.cells/htmlsaveoptions\#getTableCssId--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setUpdateSmartArt(boolean value) {#setUpdateSmartArt-boolean-}
```
public void setUpdateSmartArt(boolean value)
```


For the description of this property, please see [getUpdateSmartArt()](../../com.aspose.cells/saveoptions\#getUpdateSmartArt--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setValidateMergedAreas(boolean value) {#setValidateMergedAreas-boolean-}
```
public void setValidateMergedAreas(boolean value)
```


For the description of this property, please see [getValidateMergedAreas()](../../com.aspose.cells/saveoptions\#getValidateMergedAreas--)

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


For the description of this property, please see [getWidthScalable()](../../com.aspose.cells/htmlsaveoptions\#getWidthScalable--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setWorksheetScalable(boolean value) {#setWorksheetScalable-boolean-}
```
public void setWorksheetScalable(boolean value)
```


For the description of this property, please see [getWorksheetScalable()](../../com.aspose.cells/htmlsaveoptions\#getWorksheetScalable--)

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

