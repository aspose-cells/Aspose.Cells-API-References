---
title: CellsHelper
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Provides helper functions.
type: docs
url: /javascript-cpp/cellshelper/
---

## CellsHelper class

Provides helper functions.

```javascript
class CellsHelper;
```


## Properties

| Property | Type | Description |
| --- | --- | --- |
| static [significantDigitsType](#significantDigitsType--)| SignificantDigitsType | Gets and sets the default type of significant digits for outputing numeric values. Default value is [SignificantDigitsType.G17](../significantdigitstype.g17/). |
| static [dPI](#dPI--)| number | Gets the DPI of the machine. |
| static [startupPath](#startupPath--)| string | Gets or sets the startup path, which is referred to by some external formula references. |
| static [altStartPath](#altStartPath--)| string | Gets or sets the alternate startup path, which is referred to by some external formula references. |
| static [libraryPath](#libraryPath--)| string | Gets or sets the library path which is referred to by some external formula references. |
| static [isCloudPlatform](#isCloudPlatform--)| boolean | Please set this property True when running on a cloud platform, such as: Azure, AWSLambda, etc, |

## Methods

| Method | Description |
| --- | --- |
| static [getTextWidth(string, Font, number)](#getTextWidth-string-font-number-)| Get width of text in unit of points. |
| static [getVersion()](#getVersion--)| Get the release version. |
| static [cellNameToIndex(string)](#cellNameToIndex-string-)| Gets the cell row and column indexes according to its name. |
| static [cellIndexToName(number, number)](#cellIndexToName-number-number-)| Gets cell name according to its row and column indexes. |
| static [columnIndexToName(number)](#columnIndexToName-number-)| Gets column name according to column index. |
| static [columnNameToIndex(string)](#columnNameToIndex-string-)| Gets column index according to column name. |
| static [rowIndexToName(number)](#rowIndexToName-number-)| Gets row name according to row index. |
| static [rowNameToIndex(string)](#rowNameToIndex-string-)| Gets row index according to row name. |
| static [getDateTimeFromDouble(number, boolean)](#getDateTimeFromDouble-number-boolean-)| Convert the double value to the date time value. |
| static [getDoubleFromDateTime(Date, boolean)](#getDoubleFromDateTime-date-boolean-)| Convert the date time to double value. |
| static [getUsedColors(Workbook)](#getUsedColors-workbook-)| Gets all used colors in the workbook. |
| static [mergeFiles(string[], string, string)](#mergeFiles-stringarray-string-string-)| Merges some large xls files to a xls file. |
| static [getCacheFolder()](#getCacheFolder--)| Gets the folder for temporary files that may be used as data cache. |
| static [setCacheFolder(string)](#setCacheFolder-string-)| Sets the folder for temporary files that may be used as data cache. |
| static [createSafeSheetName(string)](#createSafeSheetName-string-)| Checks given sheet name and create a valid one when needed. If given sheet name conforms to the rules of excel sheet name, then return it. Otherwise string will be truncated if length exceeds the limit and invalid characters will be replaced with ' ', then return the rebuilt string value. |
| static [needQuoteInFormula(string)](#needQuoteInFormula-string-)| Indicates whether the name of the sheet should be enclosed in single quotes |


### significantDigitsType {#significantDigitsType--}

Gets and sets the default type of significant digits for outputing numeric values. Default value is [SignificantDigitsType.G17](../significantdigitstype.g17/).

```javascript
static significantDigitsType : SignificantDigitsType;
```


### dPI {#dPI--}

Gets the DPI of the machine.

```javascript
static dPI : number;
```


### startupPath {#startupPath--}

Gets or sets the startup path, which is referred to by some external formula references.

```javascript
static startupPath : string;
```


### altStartPath {#altStartPath--}

Gets or sets the alternate startup path, which is referred to by some external formula references.

```javascript
static altStartPath : string;
```


### libraryPath {#libraryPath--}

Gets or sets the library path which is referred to by some external formula references.

```javascript
static libraryPath : string;
```


### isCloudPlatform {#isCloudPlatform--}

Please set this property True when running on a cloud platform, such as: Azure, AWSLambda, etc,

```javascript
static isCloudPlatform : boolean;
```


### getTextWidth(string, Font, number) {#getTextWidth-string-font-number-}

Get width of text in unit of points.

```javascript
static getTextWidth(text: string, font: Font, scaling: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| text | string | The text. |
| font | [Font](../font/) | The font of the text. |
| scaling | number | The scaling of text. |

### getVersion() {#getVersion--}

Get the release version.

```javascript
static getVersion() : string;
```


**Returns**

The release version.

### cellNameToIndex(string) {#cellNameToIndex-string-}

Gets the cell row and column indexes according to its name.

```javascript
static cellNameToIndex(cellName: string) : number[];
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | string | Name of cell |

**Returns**

[0] is the row index and [1] is the column index.

### cellIndexToName(number, number) {#cellIndexToName-number-number-}

Gets cell name according to its row and column indexes.

```javascript
static cellIndexToName(row: number, column: number) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | Row index. |
| column | number | Column index. |

**Returns**

Name of cell.

### columnIndexToName(number) {#columnIndexToName-number-}

Gets column name according to column index.

```javascript
static columnIndexToName(column: number) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | number | Column index. |

**Returns**

Name of column.

### columnNameToIndex(string) {#columnNameToIndex-string-}

Gets column index according to column name.

```javascript
static columnNameToIndex(columnName: string) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnName | string | Column name. |

**Returns**

Column index.

### rowIndexToName(number) {#rowIndexToName-number-}

Gets row name according to row index.

```javascript
static rowIndexToName(row: number) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | Row index. |

**Returns**

Name of row.

### rowNameToIndex(string) {#rowNameToIndex-string-}

Gets row index according to row name.

```javascript
static rowNameToIndex(rowName: string) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowName | string | Row name. |

**Returns**

Row index.

### getDateTimeFromDouble(number, boolean) {#getDateTimeFromDouble-number-boolean-}

Convert the double value to the date time value.

```javascript
static getDateTimeFromDouble(doubleValue: number, date1904: boolean) : Date;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| doubleValue | number | The double value. |
| date1904 | boolean | Date 1904 system. |

### getDoubleFromDateTime(Date, boolean) {#getDoubleFromDateTime-date-boolean-}

Convert the date time to double value.

```javascript
static getDoubleFromDateTime(dateTime: Date, date1904: boolean) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dateTime | Date | The date time. |
| date1904 | boolean | Date 1904 system. |

### getUsedColors(Workbook) {#getUsedColors-workbook-}

Gets all used colors in the workbook.

```javascript
static getUsedColors(workbook: Workbook) : Color[];
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| workbook | [Workbook](../workbook/) | The workbook object. |

**Returns**

The used colors.

### mergeFiles(string[], string, string) {#mergeFiles-stringarray-string-string-}

Merges some large xls files to a xls file.

```javascript
static mergeFiles(files: string[], cachedFile: string, destFile: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| files | string[] | The files. |
| cachedFile | string | The cached file. |
| destFile | string | The dest file. |

**Remarks**

This method only supports merging data, style and formulas to the new file. The cached file is used to store some temporary data.

### getCacheFolder() {#getCacheFolder--}

Gets the folder for temporary files that may be used as data cache.

```javascript
static getCacheFolder() : string;
```


**Returns**

Folder for cache files that has been specified. If it has not been specified, null will be returned and system's temporary path will be used when needed.

**Remarks**

Cache files are used generally for some features for memory performance consideration, such as saving large data set to xls file, or using memory mode with file cache for cells model.

### setCacheFolder(string) {#setCacheFolder-string-}

Sets the folder for temporary files that may be used as data cache.

```javascript
static setCacheFolder(cache: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cache | string | Folder for for temporary files that may be used as data cache. |

**Remarks**

Cache files are used generally for some features for memory performance consideration, such as saving large data set to xls file, or using memory mode with file cache for cells model.

### createSafeSheetName(string) {#createSafeSheetName-string-}

Checks given sheet name and create a valid one when needed. If given sheet name conforms to the rules of excel sheet name, then return it. Otherwise string will be truncated if length exceeds the limit and invalid characters will be replaced with ' ', then return the rebuilt string value.

```javascript
static createSafeSheetName(nameProposal: string) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| nameProposal | string | sheet name to be used |

### needQuoteInFormula(string) {#needQuoteInFormula-string-}

Indicates whether the name of the sheet should be enclosed in single quotes

```javascript
static needQuoteInFormula(sheetName: string) : boolean;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheetName | string | The name of the sheet |


