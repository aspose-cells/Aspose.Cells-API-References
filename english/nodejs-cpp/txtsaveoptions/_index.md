---
title: TxtSaveOptions
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the save options for csvtab delimitedother text format.
type: docs
url: /nodejs-cpp/txtsaveoptions/
---

## TxtSaveOptions class

Represents the save options for csv/tab delimited/other text format.

```javascript
class TxtSaveOptions extends SaveOptions;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Creates text file save options. |
| [constructor(SaveOptions)](#constructor-saveoptions-)| Constructs from a parent object convertible to this. |
| [constructor(SaveFormat)](#constructor-saveformat-)| Creates text file save options. |

## Methods

| Method | Description |
| --- | --- |
| [getSeparator()](#getSeparator--)| Gets and sets char Delimiter of text file. |
| [setSeparator(string)](#setSeparator-string-)| Gets and sets char Delimiter of text file. |
| [getSeparatorString()](#getSeparatorString--)| Gets and sets a string value as separator. |
| [setSeparatorString(string)](#setSeparatorString-string-)| Gets and sets a string value as separator. |
| [getEncoding()](#getEncoding--)| Gets and sets the default encoding. |
| [setEncoding(EncodingType)](#setEncoding-encodingtype-)| Gets and sets the default encoding. |
| [getQuoteType()](#getQuoteType--)| Gets or sets how to quote values in the exported text file. |
| [setQuoteType(TxtValueQuoteType)](#setQuoteType-txtvaluequotetype-)| Gets or sets how to quote values in the exported text file. |
| [getFormatStrategy()](#getFormatStrategy--)| Gets and sets the format strategy when exporting the cell value as string. |
| [setFormatStrategy(CellValueFormatStrategy)](#setFormatStrategy-cellvalueformatstrategy-)| Gets and sets the format strategy when exporting the cell value as string. |
| [getLightCellsDataProvider()](#getLightCellsDataProvider--)| The data provider for saving workbook in light mode. |
| [setLightCellsDataProvider(LightCellsDataProvider)](#setLightCellsDataProvider-lightcellsdataprovider-)| The data provider for saving workbook in light mode. |
| [getTrimLeadingBlankRowAndColumn()](#getTrimLeadingBlankRowAndColumn--)| Indicates whether leading blank rows and columns should be trimmed like what ms excel does. Default is true. |
| [setTrimLeadingBlankRowAndColumn(boolean)](#setTrimLeadingBlankRowAndColumn-boolean-)| Indicates whether leading blank rows and columns should be trimmed like what ms excel does. Default is true. |
| [getTrimTailingBlankCells()](#getTrimTailingBlankCells--)| Indicates whether tailing blank cells in one row should be trimmed. Default is false. |
| [setTrimTailingBlankCells(boolean)](#setTrimTailingBlankCells-boolean-)| Indicates whether tailing blank cells in one row should be trimmed. Default is false. |
| [getKeepSeparatorsForBlankRow()](#getKeepSeparatorsForBlankRow--)| Indicates whether separators should be output for blank row. Default value is false so by default the content for blank row will be empty. |
| [setKeepSeparatorsForBlankRow(boolean)](#setKeepSeparatorsForBlankRow-boolean-)| Indicates whether separators should be output for blank row. Default value is false so by default the content for blank row will be empty. |
| [getExportArea()](#getExportArea--)| The range of cells to be exported. |
| [setExportArea(CellArea)](#setExportArea-cellarea-)| The range of cells to be exported. |
| [getExportQuotePrefix()](#getExportQuotePrefix--)| Indicates whether the single quote sign should be exported as part of the value of one cell when [Style.QuotePrefix](../style.quoteprefix/) is true for it. Default is false. |
| [setExportQuotePrefix(boolean)](#setExportQuotePrefix-boolean-)| Indicates whether the single quote sign should be exported as part of the value of one cell when [Style.QuotePrefix](../style.quoteprefix/) is true for it. Default is false. |
| [getExportAllSheets()](#getExportAllSheets--)| Indicates whether exporting all sheets to the text file. If it is false, only export the activesheet, just like MS Excel. |
| [setExportAllSheets(boolean)](#setExportAllSheets-boolean-)| Indicates whether exporting all sheets to the text file. If it is false, only export the activesheet, just like MS Excel. |
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

Creates text file save options.

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

Creates text file save options.

```javascript
constructor(saveFormat: SaveFormat);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | [SaveFormat](../saveformat/) | The file format.         /// It should be [SaveFormat.Csv](../saveformat.csv/) or [SaveFormat.Csv](../saveformat.csv/),         /// otherwise the saved format will be set as [SaveFormat.Csv](../saveformat.csv/) automatically. |

### getSeparator() {#getSeparator--}

Gets and sets char Delimiter of text file.

```javascript
getSeparator() : string;
```


### setSeparator(string) {#setSeparator-string-}

Gets and sets char Delimiter of text file.

```javascript
setSeparator(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getSeparatorString() {#getSeparatorString--}

Gets and sets a string value as separator.

```javascript
getSeparatorString() : string;
```


### setSeparatorString(string) {#setSeparatorString-string-}

Gets and sets a string value as separator.

```javascript
setSeparatorString(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getEncoding() {#getEncoding--}

Gets and sets the default encoding.

```javascript
getEncoding() : EncodingType;
```


**Returns**

[EncodingType](../encodingtype/)

### setEncoding(EncodingType) {#setEncoding-encodingtype-}

Gets and sets the default encoding.

```javascript
setEncoding(value: EncodingType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [EncodingType](../encodingtype/) | The value to set. |

### getQuoteType() {#getQuoteType--}

Gets or sets how to quote values in the exported text file.

```javascript
getQuoteType() : TxtValueQuoteType;
```


**Returns**

[TxtValueQuoteType](../txtvaluequotetype/)

### setQuoteType(TxtValueQuoteType) {#setQuoteType-txtvaluequotetype-}

Gets or sets how to quote values in the exported text file.

```javascript
setQuoteType(value: TxtValueQuoteType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TxtValueQuoteType](../txtvaluequotetype/) | The value to set. |

### getFormatStrategy() {#getFormatStrategy--}

Gets and sets the format strategy when exporting the cell value as string.

```javascript
getFormatStrategy() : CellValueFormatStrategy;
```


**Returns**

[CellValueFormatStrategy](../cellvalueformatstrategy/)

### setFormatStrategy(CellValueFormatStrategy) {#setFormatStrategy-cellvalueformatstrategy-}

Gets and sets the format strategy when exporting the cell value as string.

```javascript
setFormatStrategy(value: CellValueFormatStrategy) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellValueFormatStrategy](../cellvalueformatstrategy/) | The value to set. |

### getLightCellsDataProvider() {#getLightCellsDataProvider--}

The data provider for saving workbook in light mode.

```javascript
getLightCellsDataProvider() : LightCellsDataProvider;
```


**Returns**

[LightCellsDataProvider](../lightcellsdataprovider/)

### setLightCellsDataProvider(LightCellsDataProvider) {#setLightCellsDataProvider-lightcellsdataprovider-}

The data provider for saving workbook in light mode.

```javascript
setLightCellsDataProvider(value: LightCellsDataProvider) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LightCellsDataProvider](../lightcellsdataprovider/) | The value to set. |

### getTrimLeadingBlankRowAndColumn() {#getTrimLeadingBlankRowAndColumn--}

Indicates whether leading blank rows and columns should be trimmed like what ms excel does. Default is true.

```javascript
getTrimLeadingBlankRowAndColumn() : boolean;
```


**Remarks**

Same with the rule in ms excel, a row/column will not be taken as blank if it has custom style, even if it contains no cell data. When saving with LightCells mode, this option takes no effect. User should control the output range by the implementation of [LightCellsDataProvider](../lightcellsdataprovider/) or by speicifing [ExportArea](../exportarea/)

### setTrimLeadingBlankRowAndColumn(boolean) {#setTrimLeadingBlankRowAndColumn-boolean-}

Indicates whether leading blank rows and columns should be trimmed like what ms excel does. Default is true.

```javascript
setTrimLeadingBlankRowAndColumn(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Same with the rule in ms excel, a row/column will not be taken as blank if it has custom style, even if it contains no cell data. When saving with LightCells mode, this option takes no effect. User should control the output range by the implementation of [LightCellsDataProvider](../lightcellsdataprovider/) or by speicifing [ExportArea](../exportarea/)

### getTrimTailingBlankCells() {#getTrimTailingBlankCells--}

Indicates whether tailing blank cells in one row should be trimmed. Default is false.

```javascript
getTrimTailingBlankCells() : boolean;
```


**Remarks**

When saving with LightCells mode and the [ExportArea](../exportarea/) has not been specified, this option takes no effect and one row will be extended to just the last cell provided by the implementation [LightCellsDataProvider](../lightcellsdataprovider/)

### setTrimTailingBlankCells(boolean) {#setTrimTailingBlankCells-boolean-}

Indicates whether tailing blank cells in one row should be trimmed. Default is false.

```javascript
setTrimTailingBlankCells(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

When saving with LightCells mode and the [ExportArea](../exportarea/) has not been specified, this option takes no effect and one row will be extended to just the last cell provided by the implementation [LightCellsDataProvider](../lightcellsdataprovider/)

### getKeepSeparatorsForBlankRow() {#getKeepSeparatorsForBlankRow--}

Indicates whether separators should be output for blank row. Default value is false so by default the content for blank row will be empty.

```javascript
getKeepSeparatorsForBlankRow() : boolean;
```


### setKeepSeparatorsForBlankRow(boolean) {#setKeepSeparatorsForBlankRow-boolean-}

Indicates whether separators should be output for blank row. Default value is false so by default the content for blank row will be empty.

```javascript
setKeepSeparatorsForBlankRow(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExportArea() {#getExportArea--}

The range of cells to be exported.

```javascript
getExportArea() : CellArea;
```


**Returns**

[CellArea](../cellarea/)

**Remarks**

If the exported area has been specified, [TrimLeadingBlankRowAndColumn](../trimleadingblankrowandcolumn/) will takes no effect.

### setExportArea(CellArea) {#setExportArea-cellarea-}

The range of cells to be exported.

```javascript
setExportArea(value: CellArea) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellArea](../cellarea/) | The value to set. |

**Remarks**

If the exported area has been specified, [TrimLeadingBlankRowAndColumn](../trimleadingblankrowandcolumn/) will takes no effect.

### getExportQuotePrefix() {#getExportQuotePrefix--}

Indicates whether the single quote sign should be exported as part of the value of one cell when [Style.QuotePrefix](../style.quoteprefix/) is true for it. Default is false.

```javascript
getExportQuotePrefix() : boolean;
```


### setExportQuotePrefix(boolean) {#setExportQuotePrefix-boolean-}

Indicates whether the single quote sign should be exported as part of the value of one cell when [Style.QuotePrefix](../style.quoteprefix/) is true for it. Default is false.

```javascript
setExportQuotePrefix(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExportAllSheets() {#getExportAllSheets--}

Indicates whether exporting all sheets to the text file. If it is false, only export the activesheet, just like MS Excel.

```javascript
getExportAllSheets() : boolean;
```


**Remarks**

The defult value is false.

### setExportAllSheets(boolean) {#setExportAllSheets-boolean-}

Indicates whether exporting all sheets to the text file. If it is false, only export the activesheet, just like MS Excel.

```javascript
setExportAllSheets(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

The defult value is false.

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


