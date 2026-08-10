---
title: "CellsHelper Class"
linktitle: "CellsHelper"
articleTitle: "CellsHelper"
second_title: "Aspose.Cells for PHP via Java"
description: "Provides helper functions."
type: docs
weight: 680
url: /php/aspose.cells/cellshelper/
---

## CellsHelper class

Provides helper functions.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [SignificantDigits](#significantdigits) | Number | Gets and sets the number of significant digits. The default value is 17. Only could be 15 or 17 now. |
| [SignificantDigitsType](#significantdigitstype) | Number | The value of the property is SignificantDigitsType integer constant. |
| [DPI](#dpi) | Number | Gets the DPI of the machine. |
| [StartupPath](#startuppath) | String | Gets or sets the startup path, which is referred to by some external formula references. |
| [AltStartPath](#altstartpath) | String | Gets or sets the alternate startup path, which is referred to by some external formula references. |
| [LibraryPath](#librarypath) | String | Gets or sets the library path which is referred to by some external formula references. |
| [CustomImplementationFactory](#customimplementationfactory) | CustomImplementationFactory | Gets or sets the factory for creating instances with special implementation. |
| [IsCloudPlatform](#iscloudplatform) | boolean | Please set this property True when running on a cloud platform, such as: Azure, AWSLambda, etc, |

## Methods

| Name | Description |
| --- | --- |
| [getTextWidth](#gettextwidth) | Get width of text in unit of points. |
| [getVersion](#getversion) | Get the release version. |
| [cellNameToIndex](#cellnametoindex) | Gets the cell row and column indexes according to its name. |
| [cellIndexToName](#cellindextoname) | Gets cell name according to its row and column indexes. |
| [columnIndexToName](#columnindextoname) | Gets column name according to column index. |
| [columnNameToIndex](#columnnametoindex) | Gets column index according to column name. |
| [rowIndexToName](#rowindextoname) | Gets row name according to row index. |
| [rowNameToIndex](#rownametoindex) | Gets row index according to row name. |
| [convertR1C1FormulaToA1](#convertr1c1formulatoa1) | Converts the r1c1 formula of the cell to A1 formula.

NOTE: This member is now obsolete. Instead, please use Worksheet.C |
| [convertA1FormulaToR1C1](#converta1formulator1c1) | Converts A1 formula of the cell to the r1c1 formula.

NOTE: This member is now obsolete. Instead, please use Worksheet.C |
| [getDateTimeFromDouble](#getdatetimefromdouble) | Convert the double value to the date time value. |
| [getDoubleFromDateTime](#getdoublefromdatetime) | Convert the date time to double value. |
| [getUsedColors](#getusedcolors) | Gets all used colors in the workbook. |
| [addAddInFunction](#addaddinfunction) | Add addin function.

NOTE: This member is now obsolete. Instead, please use WorksheetCollection.RegisterAddInFunction()  |
| [mergeFiles](#mergefiles) | Merges some large xls files to a xls file.

This method only supports merging data, style and formulas to the new file.  |
| [getCacheFolder](#getcachefolder) |  |
| [setCacheFolder](#setcachefolder) |  |
| [createSafeSheetName](#createsafesheetname) | Checks given sheet name and create a valid one when needed. If given sheet name conforms to the rules of excel sheet nam |
| [needQuoteInFormula](#needquoteinformula) | Indicates whether the name of the sheet should be enclosed in single quotes |

### CellsHelper.SignificantDigits property {#significantdigits}

Gets and sets the number of significant digits. The default value is 17. Only could be 15 or 17 now.

**Type:** Number

### CellsHelper.SignificantDigitsType property {#significantdigitstype}

The value of the property is SignificantDigitsType integer constant.

**Type:** Number

### CellsHelper.DPI property {#dpi}

Gets the DPI of the machine.

**Type:** Number

### CellsHelper.StartupPath property {#startuppath}

Gets or sets the startup path, which is referred to by some external formula references.

**Type:** String

### CellsHelper.AltStartPath property {#altstartpath}

Gets or sets the alternate startup path, which is referred to by some external formula references.

**Type:** String

### CellsHelper.LibraryPath property {#librarypath}

Gets or sets the library path which is referred to by some external formula references.

**Type:** String

### CellsHelper.CustomImplementationFactory property {#customimplementationfactory}

Gets or sets the factory for creating instances with special implementation.

**Type:** CustomImplementationFactory

### CellsHelper.IsCloudPlatform property {#iscloudplatform}

Please set this property True when running on a cloud platform, such as: Azure, AWSLambda, etc,

**Type:** boolean

### getTextWidth(text, font, scaling) {#gettextwidth}

Get width of text in unit of points.

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | The text. |
| font | Font | The font of the text. |
| scaling | Number | The scaling of text. |

### getVersion() {#getversion}

Get the release version.

**Returns:** The release version.

### cellNameToIndex(cellName) {#cellnametoindex}

Gets the cell row and column indexes according to its name.

| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | Name of cell |

**Returns:** [0] is the row index and [1] is the column index.

### cellIndexToName(row, column) {#cellindextoname}

Gets cell name according to its row and column indexes.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Row index. |
| column | Number | Column index. |

**Returns:** Name of cell.

### columnIndexToName(column) {#columnindextoname}

Gets column name according to column index.

| Parameter | Type | Description |
| --- | --- | --- |
| column | Number | Column index. |

**Returns:** Name of column.

### columnNameToIndex(columnName) {#columnnametoindex}

Gets column index according to column name.

| Parameter | Type | Description |
| --- | --- | --- |
| columnName | String | Column name. |

**Returns:** Column index.

### rowIndexToName(row) {#rowindextoname}

Gets row name according to row index.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Row index. |

**Returns:** Name of row.

### rowNameToIndex(rowName) {#rownametoindex}

Gets row index according to row name.

| Parameter | Type | Description |
| --- | --- | --- |
| rowName | String | Row name. |

**Returns:** Row index.

### convertR1C1FormulaToA1(r1c1Formula, row, column) {#convertr1c1formulatoa1}

Converts the r1c1 formula of the cell to A1 formula.

NOTE: This member is now obsolete. Instead, please use Worksheet.ConvertFormulaReferenceStyle() method. This property will be removed 12 months later since August 2023. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| r1c1Formula | String | The r1c1 formula. |
| row | Number | The row index of the cell. |
| column | Number | The column index of the cell. |

**Returns:** The A1 formula.

### convertA1FormulaToR1C1(formula, row, column) {#converta1formulator1c1}

Converts A1 formula of the cell to the r1c1 formula.

NOTE: This member is now obsolete. Instead, please use Worksheet.ConvertFormulaReferenceStyle() method. This property will be removed 12 months later since August 2023. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | The A1 formula. |
| row | Number | The row index of the cell. |
| column | Number | The column index of the cell. |

**Returns:** The R1C1 formula.

### getDateTimeFromDouble(doubleValue, date1904) {#getdatetimefromdouble}

Convert the double value to the date time value.

| Parameter | Type | Description |
| --- | --- | --- |
| doubleValue | Number | The double value. |
| date1904 | boolean | Date 1904 system. |

### getDoubleFromDateTime(dateTime, date1904) {#getdoublefromdatetime}

Convert the date time to double value.

| Parameter | Type | Description |
| --- | --- | --- |
| dateTime | DateTime | The date time. |
| date1904 | boolean | Date 1904 system. |

### getUsedColors(workbook) {#getusedcolors}

Gets all used colors in the workbook.

| Parameter | Type | Description |
| --- | --- | --- |
| workbook | Workbook | The workbook object. |

**Returns:** The used colors.

### addAddInFunction(function, minCountOfParameters, maxCountOfParameters, paramersType, functionValueType) {#addaddinfunction}

Add addin function.

NOTE: This member is now obsolete. Instead, please use WorksheetCollection.RegisterAddInFunction() methods. This method will be removed 12 months later since January 2022. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| function | String | The function name. |
| minCountOfParameters | Number | Minimum number of parameters this function requires |
| maxCountOfParameters | Number | Maximum number of parameters this function allows. |
| paramersType | Number Array | The excepted parameters type of the function |
| functionValueType | Number | A ParameterType value. The function value type. |

### mergeFiles(files, cachedFile, destFile) {#mergefiles}

Merges some large xls files to a xls file.

This method only supports merging data, style and formulas to the new file. The cached file is used to store some temporary data.

| Parameter | Type | Description |
| --- | --- | --- |
| files | String[] | The files. |
| cachedFile | String | The cached file. |
| destFile | String | The dest file. |

### getCacheFolder() {#getcachefolder}

### setCacheFolder(cache) {#setcachefolder}

### createSafeSheetName(nameProposal) (1 of 2) {#createsafesheetname}

Checks given sheet name and create a valid one when needed. If given sheet name conforms to the rules of excel sheet name, then return it. Otherwise string will be truncated if length exceeds the limit and invalid characters will be replaced with ' ', then return the rebuilt string value.

| Parameter | Type | Description |
| --- | --- | --- |
| nameProposal | String | sheet name to be used |

---

### createSafeSheetName(nameProposal, replaceChar) (2 of 2) {#createsafesheetname-1}

Checks given sheet name and create a valid one when needed. If given sheet name conforms to the rules of excel sheet name, then return it. Otherwise string will be truncated if length exceeds the limit and invalid characters will be replaced with given character, then return the rebuilt string value.

| Parameter | Type | Description |
| --- | --- | --- |
| nameProposal | String | sheet name to be used |
| replaceChar | char | character which will be used to replace invalid characters in given sheet name |

### needQuoteInFormula(sheetName) {#needquoteinformula}

Indicates whether the name of the sheet should be enclosed in single quotes

| Parameter | Type | Description |
| --- | --- | --- |
| sheetName | String | The name of the sheet |
