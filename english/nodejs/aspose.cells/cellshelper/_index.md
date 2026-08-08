---
title: "CellsHelper"
linktitle: "CellsHelper"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Provides helper functions."
type: docs
weight: 460
url: /nodejs/aspose.cells/cellshelper/
---

## CellsHelper class

Provides helper functions.

## Methods

| Name | Description |
| --- | --- |
| [getAltStartPath()](#getaltstartpath) | Gets or sets the alternate startup path, which is referred to by some external formula references. |
| [getCustomImplementationFactory()](#getcustomimplementationfactory) | Gets or sets the factory for creating instances with special implementation. |
| [getDPI()](#getdpi) | Gets the DPI of the machine. |
| [getLibraryPath()](#getlibrarypath) | Gets or sets the library path which is referred to by some external formula references. |
| [getSignificantDigits()](#getsignificantdigits) | Gets and sets the number of significant digits. The default value is 17. Only could be 15 or 17 now. |
| [getSignificantDigitsType()](#getsignificantdigitstype) | The value of the property is SignificantDigitsType integer constant. |
| [getStartupPath()](#getstartuppath) | Gets or sets the startup path, which is referred to by some external formula references. |
| [isCloudPlatform()](#iscloudplatform) | Please set this property True when running on a cloud platform, such as: Azure, AWSLambda, etc, |
| [setAltStartPath()](#setaltstartpath) | Gets or sets the alternate startup path, which is referred to by some external formula references. |
| [setCloudPlatform()](#setcloudplatform) | Please set this property True when running on a cloud platform, such as: Azure, AWSLambda, etc, |
| [setCustomImplementationFactory()](#setcustomimplementationfactory) | Gets or sets the factory for creating instances with special implementation. |
| [setDPI()](#setdpi) | Gets the DPI of the machine. |
| [setLibraryPath()](#setlibrarypath) | Gets or sets the library path which is referred to by some external formula references. |
| [setSignificantDigits()](#setsignificantdigits) | Gets and sets the number of significant digits. The default value is 17. Only could be 15 or 17 now. |
| [setSignificantDigitsType()](#setsignificantdigitstype) | The value of the property is SignificantDigitsType integer constant. |
| [setStartupPath()](#setstartuppath) | Gets or sets the startup path, which is referred to by some external formula references. |
| [addAddInFunction(function, minCountOfParameters, maxCountOfParameters, paramersType, functionValueType)](#addaddinfunction) *(static)* | Add addin function. NOTE: This member is now obsolete. Instead, please use WorksheetCollection.RegisterAddInFunction() m |
| [cellIndexToName(row, column)](#cellindextoname) *(static)* | Gets cell name according to its row and column indexes. |
| [cellNameToIndex(cellName)](#cellnametoindex) *(static)* | Gets the cell row and column indexes according to its name. |
| [columnIndexToName(column)](#columnindextoname) *(static)* | Gets column name according to column index. |
| [columnNameToIndex(columnName)](#columnnametoindex) *(static)* | Gets column index according to column name. |
| [convertA1FormulaToR1C1(formula, row, column)](#converta1formulator1c1) *(static)* | Converts A1 formula of the cell to the r1c1 formula. NOTE: This member is now obsolete. Instead, please use Worksheet.Co |
| [convertR1C1FormulaToA1(r1c1Formula, row, column)](#convertr1c1formulatoa1) *(static)* | Converts the r1c1 formula of the cell to A1 formula. NOTE: This member is now obsolete. Instead, please use Worksheet.Co |
| [createSafeSheetName(nameProposal)](#createsafesheetname) *(static)* | Checks given sheet name and create a valid one when needed. If given sheet name conforms to the rules of excel sheet nam |
| [createSafeSheetName(nameProposal, replaceChar)](#createsafesheetname-1) *(static)* | Checks given sheet name and create a valid one when needed. If given sheet name conforms to the rules of excel sheet nam |
| [getCacheFolder()](#getcachefolder) *(static)* |  |
| [getDateTimeFromDouble(doubleValue, date1904)](#getdatetimefromdouble) *(static)* | Convert the double value to the date time value. |
| [getDoubleFromDateTime(dateTime, date1904)](#getdoublefromdatetime) *(static)* | Convert the date time to double value. |
| [getTextWidth(text, font, scaling)](#gettextwidth) *(static)* | Get width of text in unit of points. |
| [getUsedColors(workbook)](#getusedcolors) *(static)* | Gets all used colors in the workbook. |
| [getVersion()](#getversion) *(static)* | Get the release version. |
| [mergeFiles(files, cachedFile, destFile)](#mergefiles) *(static)* | Merges some large xls files to a xls file. This method only supports merging data, style and formulas to the new file. T |
| [needQuoteInFormula(sheetName)](#needquoteinformula) *(static)* | Indicates whether the name of the sheet should be enclosed in single quotes |
| [rowIndexToName(row)](#rowindextoname) *(static)* | Gets row name according to row index. |
| [rowNameToIndex(rowName)](#rownametoindex) *(static)* | Gets row index according to row name. |
| [setCacheFolder()](#setcachefolder) *(static)* |  |

### getAltStartPath() {#getaltstartpath}

Gets or sets the alternate startup path, which is referred to by some external formula references.

### getCustomImplementationFactory() {#getcustomimplementationfactory}

Gets or sets the factory for creating instances with special implementation.

### getDPI() {#getdpi}

Gets the DPI of the machine.

### getLibraryPath() {#getlibrarypath}

Gets or sets the library path which is referred to by some external formula references.

### getSignificantDigits() {#getsignificantdigits}

Gets and sets the number of significant digits. The default value is 17. Only could be 15 or 17 now.

### getSignificantDigitsType() {#getsignificantdigitstype}

The value of the property is SignificantDigitsType integer constant.

### getStartupPath() {#getstartuppath}

Gets or sets the startup path, which is referred to by some external formula references.

### isCloudPlatform() {#iscloudplatform}

Please set this property True when running on a cloud platform, such as: Azure, AWSLambda, etc,

### setAltStartPath() {#setaltstartpath}

Gets or sets the alternate startup path, which is referred to by some external formula references.

### setCloudPlatform() {#setcloudplatform}

Please set this property True when running on a cloud platform, such as: Azure, AWSLambda, etc,

### setCustomImplementationFactory() {#setcustomimplementationfactory}

Gets or sets the factory for creating instances with special implementation.

### setDPI() {#setdpi}

Gets the DPI of the machine.

### setLibraryPath() {#setlibrarypath}

Gets or sets the library path which is referred to by some external formula references.

### setSignificantDigits() {#setsignificantdigits}

Gets and sets the number of significant digits. The default value is 17. Only could be 15 or 17 now.

### setSignificantDigitsType() {#setsignificantdigitstype}

The value of the property is SignificantDigitsType integer constant.

### setStartupPath() {#setstartuppath}

Gets or sets the startup path, which is referred to by some external formula references.

### addAddInFunction(function, minCountOfParameters, maxCountOfParameters, paramersType, functionValueType) (static) {#addaddinfunction}

Add addin function. NOTE: This member is now obsolete. Instead, please use WorksheetCollection.RegisterAddInFunction() methods. This method will be removed 12 months later since January 2022. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| function | String | The function name. |
| minCountOfParameters | Number | Minimum number of parameters this function requires |
| maxCountOfParameters | Number | Maximum number of parameters this function allows. |
| paramersType | Array of Number | The excepted parameters type of the function |
| functionValueType | Number | ParameterType |

### cellIndexToName(row, column) (static) {#cellindextoname}

Gets cell name according to its row and column indexes.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Row index. |
| column | Number | Column index. |

**Returns:** String — `String` Name of cell.

### cellNameToIndex(cellName) (static) {#cellnametoindex}

Gets the cell row and column indexes according to its name.

| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | Name of cell |

**Returns:** Array of Number — `Array of Number` [0] is the row index and [1] is the column index.

### columnIndexToName(column) (static) {#columnindextoname}

Gets column name according to column index.

| Parameter | Type | Description |
| --- | --- | --- |
| column | Number | Column index. |

**Returns:** String — `String` Name of column.

### columnNameToIndex(columnName) (static) {#columnnametoindex}

Gets column index according to column name.

| Parameter | Type | Description |
| --- | --- | --- |
| columnName | String | Column name. |

**Returns:** Number — `Number` Column index.

### convertA1FormulaToR1C1(formula, row, column) (static) {#converta1formulator1c1}

Converts A1 formula of the cell to the r1c1 formula. NOTE: This member is now obsolete. Instead, please use Worksheet.ConvertFormulaReferenceStyle() method. This property will be removed 12 months later since August 2023. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | The A1 formula. |
| row | Number | The row index of the cell. |
| column | Number | The column index of the cell. |

**Returns:** String — `String` The R1C1 formula.

### convertR1C1FormulaToA1(r1c1Formula, row, column) (static) {#convertr1c1formulatoa1}

Converts the r1c1 formula of the cell to A1 formula. NOTE: This member is now obsolete. Instead, please use Worksheet.ConvertFormulaReferenceStyle() method. This property will be removed 12 months later since August 2023. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| r1c1Formula | String | The r1c1 formula. |
| row | Number | The row index of the cell. |
| column | Number | The column index of the cell. |

**Returns:** String — `String` The A1 formula.

### createSafeSheetName(nameProposal) (static) {#createsafesheetname}

Checks given sheet name and create a valid one when needed. If given sheet name conforms to the rules of excel sheet name, then return it. Otherwise string will be truncated if length exceeds the limit and invalid characters will be replaced with ' ', then return the rebuilt string value.

| Parameter | Type | Description |
| --- | --- | --- |
| nameProposal | String | sheet name to be used |

**Returns:** String — `String`

### createSafeSheetName(nameProposal, replaceChar) (static) {#createsafesheetname-1}

Checks given sheet name and create a valid one when needed. If given sheet name conforms to the rules of excel sheet name, then return it. Otherwise string will be truncated if length exceeds the limit and invalid characters will be replaced with given character, then return the rebuilt string value.

| Parameter | Type | Description |
| --- | --- | --- |
| nameProposal | String | sheet name to be used |
| replaceChar | char | character which will be used to replace invalid characters in given sheet name |

**Returns:** String — `String`

### getCacheFolder() (static) {#getcachefolder}

### getDateTimeFromDouble(doubleValue, date1904) (static) {#getdatetimefromdouble}

Convert the double value to the date time value.

| Parameter | Type | Description |
| --- | --- | --- |
| doubleValue | Number | The double value. |
| date1904 | boolean | Date 1904 system. |

**Returns:** DateTime — `DateTime`

### getDoubleFromDateTime(dateTime, date1904) (static) {#getdoublefromdatetime}

Convert the date time to double value.

| Parameter | Type | Description |
| --- | --- | --- |
| dateTime | DateTime | The date time. |
| date1904 | boolean | Date 1904 system. |

**Returns:** Number — `Number`

### getTextWidth(text, font, scaling) (static) {#gettextwidth}

Get width of text in unit of points.

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | The text. |
| font | Font | The font of the text. |
| scaling | Number | The scaling of text. |

**Returns:** Number — `Number`

### getUsedColors(workbook) (static) {#getusedcolors}

Gets all used colors in the workbook.

| Parameter | Type | Description |
| --- | --- | --- |
| workbook | Workbook | The workbook object. |

**Returns:** Array ofColor — `Array ofColor` The used colors.

### getVersion() (static) {#getversion}

Get the release version.

**Returns:** String — `String` The release version.

### mergeFiles(files, cachedFile, destFile) (static) {#mergefiles}

Merges some large xls files to a xls file. This method only supports merging data, style and formulas to the new file. The cached file is used to store some temporary data.

| Parameter | Type | Description |
| --- | --- | --- |
| files | Array of String | The files. |
| cachedFile | String | The cached file. |
| destFile | String | The dest file. |

### needQuoteInFormula(sheetName) (static) {#needquoteinformula}

Indicates whether the name of the sheet should be enclosed in single quotes

| Parameter | Type | Description |
| --- | --- | --- |
| sheetName | String | The name of the sheet |

**Returns:** boolean — `boolean`

### rowIndexToName(row) (static) {#rowindextoname}

Gets row name according to row index.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Row index. |

**Returns:** String — `String` Name of row.

### rowNameToIndex(rowName) (static) {#rownametoindex}

Gets row index according to row name.

| Parameter | Type | Description |
| --- | --- | --- |
| rowName | String | Row name. |

**Returns:** Number — `Number` Row index.

### setCacheFolder() (static) {#setcachefolder}
