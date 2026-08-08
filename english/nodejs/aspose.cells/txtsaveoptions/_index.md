---
title: "TxtSaveOptions"
linktitle: "TxtSaveOptions"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents the save options for csv/tab delimited/other text format."
type: docs
weight: 4400
url: /nodejs/aspose.cells/txtsaveoptions/
---

## TxtSaveOptions class

Represents the save options for csv/tab delimited/other text format.

```js
new TxtSaveOptions()
```

Creates text file save options.

## Methods

| Name | Description |
| --- | --- |
| [constructor_overload$1(saveFormat)](#constructor-overload1) | Creates text file save options. |
| [getAlwaysQuoted()](#getalwaysquoted) | Indicates whether always adding '"' for each field. If true then all values will be quoted; If false then values will on |
| [getCachedFileFolder()](#getcachedfilefolder) | The cached file folder is used to store some large data. |
| [getCheckExcelRestriction()](#getcheckexcelrestriction) |  |
| [getClearData()](#getcleardata) | Make the workbook empty after saving the file. |
| [getCreateDirectory()](#getcreatedirectory) | If true and the directory does not exist, the directory will be automatically created before saving the file. The defaul |
| [getEncoding()](#getencoding) | Gets and sets the default encoding. |
| [getEncryptDocumentProperties()](#getencryptdocumentproperties) |  |
| [getExportAllSheets()](#getexportallsheets) | Indicates whether exporting all sheets to the text file. If it is false, only export the activesheet, just like MS Excel |
| [getExportArea()](#getexportarea) | The range of cells to be exported. If the exported area has been specified, TrimLeadingBlankRowAndColumn will takes no e |
| [getExportQuotePrefix()](#getexportquoteprefix) | Indicates whether the single quote sign should be exported as part of the value of one cell when Style.QuotePrefix is tr |
| [getFormatStrategy()](#getformatstrategy) | Gets and sets the format strategy when exporting the cell value as string. The value of the property is CellValueFormatS |
| [getKeepSeparatorsForBlankRow()](#getkeepseparatorsforblankrow) | Indicates whether separators should be output for blank row. Default value is false so by default the content for blank  |
| [getLightCellsDataProvider()](#getlightcellsdataprovider) | The data provider for saving workbook in light mode. |
| [getMergeAreas()](#getmergeareas) | Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is  |
| [getQuoteType()](#getquotetype) | Gets or sets how to quote values in the exported text file. The value of the property is TxtValueQuoteType integer const |
| [getRefreshChartCache()](#getrefreshchartcache) | Indicates whether refreshing chart cache data |
| [getSaveFormat()](#getsaveformat) | Gets the save file format. The value of the property is SaveFormat integer constant. |
| [getSeparator()](#getseparator) | Gets and sets char Delimiter of text file. |
| [getSeparatorString()](#getseparatorstring) | Gets and sets a string value as separator. |
| [getSortExternalNames()](#getsortexternalnames) | Indicates whether sorting external defined names before saving file. |
| [getSortNames()](#getsortnames) | Indicates whether sorting defined names before saving file. |
| [getTrimLeadingBlankRowAndColumn()](#gettrimleadingblankrowandcolumn) | Indicates whether leading blank rows and columns should be trimmed like what ms excel does. Default is true. Same with t |
| [getTrimTailingBlankCells()](#gettrimtailingblankcells) | Indicates whether tailing blank cells in one row should be trimmed. Default is false. When saving with LightCells mode a |
| [getUpdateSmartArt()](#getupdatesmartart) | Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSm |
| [getValidateMergedAreas()](#getvalidatemergedareas) | Indicates whether validate merged cells before saving the file. The default value is false. |
| [setAlwaysQuoted()](#setalwaysquoted) | Indicates whether always adding '"' for each field. If true then all values will be quoted; If false then values will on |
| [setCachedFileFolder()](#setcachedfilefolder) | The cached file folder is used to store some large data. |
| [setCheckExcelRestriction()](#setcheckexcelrestriction) |  |
| [setClearData()](#setcleardata) | Make the workbook empty after saving the file. |
| [setCreateDirectory()](#setcreatedirectory) | If true and the directory does not exist, the directory will be automatically created before saving the file. The defaul |
| [setEncoding()](#setencoding) | Gets and sets the default encoding. |
| [setEncryptDocumentProperties()](#setencryptdocumentproperties) |  |
| [setExportAllSheets()](#setexportallsheets) | Indicates whether exporting all sheets to the text file. If it is false, only export the activesheet, just like MS Excel |
| [setExportArea()](#setexportarea) | The range of cells to be exported. If the exported area has been specified, TrimLeadingBlankRowAndColumn will takes no e |
| [setExportQuotePrefix()](#setexportquoteprefix) | Indicates whether the single quote sign should be exported as part of the value of one cell when Style.QuotePrefix is tr |
| [setFormatStrategy()](#setformatstrategy) | Gets and sets the format strategy when exporting the cell value as string. The value of the property is CellValueFormatS |
| [setKeepSeparatorsForBlankRow()](#setkeepseparatorsforblankrow) | Indicates whether separators should be output for blank row. Default value is false so by default the content for blank  |
| [setLightCellsDataProvider()](#setlightcellsdataprovider) | The data provider for saving workbook in light mode. |
| [setMergeAreas()](#setmergeareas) | Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is  |
| [setQuoteType()](#setquotetype) | Gets or sets how to quote values in the exported text file. The value of the property is TxtValueQuoteType integer const |
| [setRefreshChartCache()](#setrefreshchartcache) | Indicates whether refreshing chart cache data |
| [setSeparator()](#setseparator) | Gets and sets char Delimiter of text file. |
| [setSeparatorString()](#setseparatorstring) | Gets and sets a string value as separator. |
| [setSortExternalNames()](#setsortexternalnames) | Indicates whether sorting external defined names before saving file. |
| [setSortNames()](#setsortnames) | Indicates whether sorting defined names before saving file. |
| [setTrimLeadingBlankRowAndColumn()](#settrimleadingblankrowandcolumn) | Indicates whether leading blank rows and columns should be trimmed like what ms excel does. Default is true. Same with t |
| [setTrimTailingBlankCells()](#settrimtailingblankcells) | Indicates whether tailing blank cells in one row should be trimmed. Default is false. When saving with LightCells mode a |
| [setUpdateSmartArt()](#setupdatesmartart) | Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSm |
| [setValidateMergedAreas()](#setvalidatemergedareas) | Indicates whether validate merged cells before saving the file. The default value is false. |

### constructor_overload$1(saveFormat) {#constructor-overload1}

Creates text file save options.

| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | Number | SaveFormat |

### getAlwaysQuoted() {#getalwaysquoted}

Indicates whether always adding '"' for each field. If true then all values will be quoted; If false then values will only be quoted when needed(for example, when values contain special characters such as '"' , '\n' or separator character). Default is false. NOTE: This member is now obsolete. Instead, please use QuoteType property instead. This property will be removed 12 months later since August 2012. Aspose apologizes for any inconvenience you may have experienced.

### getCachedFileFolder() {#getcachedfilefolder}

The cached file folder is used to store some large data.

### getCheckExcelRestriction() {#getcheckexcelrestriction}

### getClearData() {#getcleardata}

Make the workbook empty after saving the file.

### getCreateDirectory() {#getcreatedirectory}

If true and the directory does not exist, the directory will be automatically created before saving the file. The default value is false.

### getEncoding() {#getencoding}

Gets and sets the default encoding.

### getEncryptDocumentProperties() {#getencryptdocumentproperties}

### getExportAllSheets() {#getexportallsheets}

Indicates whether exporting all sheets to the text file. If it is false, only export the activesheet, just like MS Excel. The defult value is false.

### getExportArea() {#getexportarea}

The range of cells to be exported. If the exported area has been specified, TrimLeadingBlankRowAndColumn will takes no effect.

### getExportQuotePrefix() {#getexportquoteprefix}

Indicates whether the single quote sign should be exported as part of the value of one cell when Style.QuotePrefix is true for it. Default is false.

### getFormatStrategy() {#getformatstrategy}

Gets and sets the format strategy when exporting the cell value as string. The value of the property is CellValueFormatStrategy integer constant.

### getKeepSeparatorsForBlankRow() {#getkeepseparatorsforblankrow}

Indicates whether separators should be output for blank row. Default value is false so by default the content for blank row will be empty.

### getLightCellsDataProvider() {#getlightcellsdataprovider}

The data provider for saving workbook in light mode.

### getMergeAreas() {#getmergeareas}

Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is false.

### getQuoteType() {#getquotetype}

Gets or sets how to quote values in the exported text file. The value of the property is TxtValueQuoteType integer constant.

### getRefreshChartCache() {#getrefreshchartcache}

Indicates whether refreshing chart cache data

### getSaveFormat() {#getsaveformat}

Gets the save file format. The value of the property is SaveFormat integer constant.

### getSeparator() {#getseparator}

Gets and sets char Delimiter of text file.

### getSeparatorString() {#getseparatorstring}

Gets and sets a string value as separator.

### getSortExternalNames() {#getsortexternalnames}

Indicates whether sorting external defined names before saving file.

### getSortNames() {#getsortnames}

Indicates whether sorting defined names before saving file.

### getTrimLeadingBlankRowAndColumn() {#gettrimleadingblankrowandcolumn}

Indicates whether leading blank rows and columns should be trimmed like what ms excel does. Default is true. Same with the rule in ms excel, a row/column will not be taken as blank if it has custom style, even if it contains no cell data. When saving with LightCells mode, this option takes no effect. User should control the output range by the implementation of LightCellsDataProvider or by speicifing ExportArea

### getTrimTailingBlankCells() {#gettrimtailingblankcells}

Indicates whether tailing blank cells in one row should be trimmed. Default is false. When saving with LightCells mode and the ExportArea has not been specified, this option takes no effect and one row will be extended to just the last cell provided by the implementation LightCellsDataProvider

### getUpdateSmartArt() {#getupdatesmartart}

Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

### getValidateMergedAreas() {#getvalidatemergedareas}

Indicates whether validate merged cells before saving the file. The default value is false.

### setAlwaysQuoted() {#setalwaysquoted}

Indicates whether always adding '"' for each field. If true then all values will be quoted; If false then values will only be quoted when needed(for example, when values contain special characters such as '"' , '\n' or separator character). Default is false. NOTE: This member is now obsolete. Instead, please use QuoteType property instead. This property will be removed 12 months later since August 2012. Aspose apologizes for any inconvenience you may have experienced.

### setCachedFileFolder() {#setcachedfilefolder}

The cached file folder is used to store some large data.

### setCheckExcelRestriction() {#setcheckexcelrestriction}

### setClearData() {#setcleardata}

Make the workbook empty after saving the file.

### setCreateDirectory() {#setcreatedirectory}

If true and the directory does not exist, the directory will be automatically created before saving the file. The default value is false.

### setEncoding() {#setencoding}

Gets and sets the default encoding.

### setEncryptDocumentProperties() {#setencryptdocumentproperties}

### setExportAllSheets() {#setexportallsheets}

Indicates whether exporting all sheets to the text file. If it is false, only export the activesheet, just like MS Excel. The defult value is false.

### setExportArea() {#setexportarea}

The range of cells to be exported. If the exported area has been specified, TrimLeadingBlankRowAndColumn will takes no effect.

### setExportQuotePrefix() {#setexportquoteprefix}

Indicates whether the single quote sign should be exported as part of the value of one cell when Style.QuotePrefix is true for it. Default is false.

### setFormatStrategy() {#setformatstrategy}

Gets and sets the format strategy when exporting the cell value as string. The value of the property is CellValueFormatStrategy integer constant.

### setKeepSeparatorsForBlankRow() {#setkeepseparatorsforblankrow}

Indicates whether separators should be output for blank row. Default value is false so by default the content for blank row will be empty.

### setLightCellsDataProvider() {#setlightcellsdataprovider}

The data provider for saving workbook in light mode.

### setMergeAreas() {#setmergeareas}

Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is false.

### setQuoteType() {#setquotetype}

Gets or sets how to quote values in the exported text file. The value of the property is TxtValueQuoteType integer constant.

### setRefreshChartCache() {#setrefreshchartcache}

Indicates whether refreshing chart cache data

### setSeparator() {#setseparator}

Gets and sets char Delimiter of text file.

### setSeparatorString() {#setseparatorstring}

Gets and sets a string value as separator.

### setSortExternalNames() {#setsortexternalnames}

Indicates whether sorting external defined names before saving file.

### setSortNames() {#setsortnames}

Indicates whether sorting defined names before saving file.

### setTrimLeadingBlankRowAndColumn() {#settrimleadingblankrowandcolumn}

Indicates whether leading blank rows and columns should be trimmed like what ms excel does. Default is true. Same with the rule in ms excel, a row/column will not be taken as blank if it has custom style, even if it contains no cell data. When saving with LightCells mode, this option takes no effect. User should control the output range by the implementation of LightCellsDataProvider or by speicifing ExportArea

### setTrimTailingBlankCells() {#settrimtailingblankcells}

Indicates whether tailing blank cells in one row should be trimmed. Default is false. When saving with LightCells mode and the ExportArea has not been specified, this option takes no effect and one row will be extended to just the last cell provided by the implementation LightCellsDataProvider

### setUpdateSmartArt() {#setupdatesmartart}

Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

### setValidateMergedAreas() {#setvalidatemergedareas}

Indicates whether validate merged cells before saving the file. The default value is false.
