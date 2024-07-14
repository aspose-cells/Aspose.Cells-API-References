---
title: GlobalizationSettings
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the globalization settings.
type: docs
url: /nodejs-cpp/globalizationsettings/
---

## GlobalizationSettings class

Represents the globalization settings.

```javascript
abstract class GlobalizationSettings;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Methods

| Method | Description |
| --- | --- |
| [getChartSettings()](#getChartSettings--)| Gets or sets the globalization settings for Chart. |
| [setChartSettings(ChartGlobalizationSettings)](#setChartSettings-chartglobalizationsettings-)| Gets or sets the globalization settings for Chart. |
| [getPivotSettings()](#getPivotSettings--)| Gets or sets the globalization settings for pivot table. |
| [setPivotSettings(PivotGlobalizationSettings)](#setPivotSettings-pivotglobalizationsettings-)| Gets or sets the globalization settings for pivot table. |
| [getTotalName(ConsolidationFunction)](#getTotalName-consolidationfunction-)| Gets the total name of the function. |
| [getGrandTotalName(ConsolidationFunction)](#getGrandTotalName-consolidationfunction-)| Gets the grand total name of the function. |
| [getDefaultSheetName()](#getDefaultSheetName--)| Gets the default sheet name for adding worksheet automatically. Default is "Sheet". |
| [getTableRowTypeOfHeaders()](#getTableRowTypeOfHeaders--)| Gets the type name of table rows that consists of the table header. Default is "Headers", so in formula "#Headers" represents the table header. |
| [getTableRowTypeOfData()](#getTableRowTypeOfData--)| Gets the type name of table rows that consists of data region of referenced table. Default is "Data", so in formula "#Data" represents the data region of the table. |
| [getTableRowTypeOfAll()](#getTableRowTypeOfAll--)| Gets the type name of table rows that consists of all rows in referenced table. Default is "All", so in formula "#All" represents all rows in referenced table. |
| [getTableRowTypeOfTotals()](#getTableRowTypeOfTotals--)| Gets the type name of table rows that consists of the total row of referenced table. Default is "Totals", so in formula "#Totals" represents the total row of referenced table. |
| [getTableRowTypeOfCurrent()](#getTableRowTypeOfCurrent--)| Gets the type name of table rows that consists of the current row in referenced table. Default is "This Row", so in formula "#This Row" represents the current row in referenced table. |
| [getErrorValueString(string)](#getErrorValueString-string-)| Gets the display string value for cell's error value |
| [getBooleanValueString(boolean)](#getBooleanValueString-boolean-)| Gets the display string value for cell's boolean value |
| [getLocalFunctionName(string)](#getLocalFunctionName-string-)| Gets the locale dependent function name according to given standard function name. |
| [getStandardFunctionName(string)](#getStandardFunctionName-string-)| Gets the standard function name according to given locale dependent function name. |
| [getLocalBuiltInName(string)](#getLocalBuiltInName-string-)| Gets the locale dependent text for built-in Name according to given standard text. |
| [getStandardBuiltInName(string)](#getStandardBuiltInName-string-)| Gets the standard text of built-in Name according to given locale dependent text. |
| [getStandardHeaderFooterFontStyleName(string)](#getStandardHeaderFooterFontStyleName-string-)| Gets standard English font style name(Regular, Bold, Italic) for Header/Footer according to given locale font style name. |
| [getCommentTitleName(CommentTitleType)](#getCommentTitleName-commenttitletype-)| Gets the locale dependent comment title name according to comment title type. |
| [compare(string, string, boolean)](#compare-string-string-boolean-)| Compares two string values according to certain collation rules. |
| abstract [getListSeparator()](#getListSeparator--)| Gets the separator for list, parameters of function, ...etc. |
| abstract [getRowSeparatorOfFormulaArray()](#getRowSeparatorOfFormulaArray--)| Gets the separator for rows in array data in formula. |
| abstract [getColumnSeparatorOfFormulaArray()](#getColumnSeparatorOfFormulaArray--)| Gets the separator for the items in array's row data in formula. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### getChartSettings() {#getChartSettings--}

Gets or sets the globalization settings for Chart.

```javascript
getChartSettings() : ChartGlobalizationSettings;
```


**Returns**

[ChartGlobalizationSettings](/nodejs-cpp/chartglobalizationsettings/)

### setChartSettings(ChartGlobalizationSettings) {#setChartSettings-chartglobalizationsettings-}

Gets or sets the globalization settings for Chart.

```javascript
setChartSettings(value: ChartGlobalizationSettings) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ChartGlobalizationSettings](/nodejs-cpp/chartglobalizationsettings/) | The value to set. |

### getPivotSettings() {#getPivotSettings--}

Gets or sets the globalization settings for pivot table.

```javascript
getPivotSettings() : PivotGlobalizationSettings;
```


**Returns**

[PivotGlobalizationSettings](/nodejs-cpp/pivotglobalizationsettings/)

### setPivotSettings(PivotGlobalizationSettings) {#setPivotSettings-pivotglobalizationsettings-}

Gets or sets the globalization settings for pivot table.

```javascript
setPivotSettings(value: PivotGlobalizationSettings) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PivotGlobalizationSettings](/nodejs-cpp/pivotglobalizationsettings/) | The value to set. |

### getTotalName(ConsolidationFunction) {#getTotalName-consolidationfunction-}

Gets the total name of the function.

```javascript
getTotalName(functionType: ConsolidationFunction) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| functionType | [ConsolidationFunction](/nodejs-cpp/consolidationfunction/) | The function type. |

**Returns**

The total name of the function.

### getGrandTotalName(ConsolidationFunction) {#getGrandTotalName-consolidationfunction-}

Gets the grand total name of the function.

```javascript
getGrandTotalName(functionType: ConsolidationFunction) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| functionType | [ConsolidationFunction](/nodejs-cpp/consolidationfunction/) | The function type. |

**Returns**

The grand total name of the function.

### getDefaultSheetName() {#getDefaultSheetName--}

Gets the default sheet name for adding worksheet automatically. Default is "Sheet".

```javascript
getDefaultSheetName() : string;
```


**Returns**

the default sheet name for adding worksheet automatically

**Remarks**

The automatically added(such as by [WorksheetCollection.Add()](/nodejs-cpp/worksheetcollection.add()/)) sheet's name will be the specified name plus sequence number. For example, for Germany user maybe wants the sheet name to be "Tabellenblatt2" instead of "Sheet2". Then user may implement this method to return "Tabellenblatt".

### getTableRowTypeOfHeaders() {#getTableRowTypeOfHeaders--}

Gets the type name of table rows that consists of the table header. Default is "Headers", so in formula "#Headers" represents the table header.

```javascript
getTableRowTypeOfHeaders() : string;
```


**Returns**

the type name of table rows

### getTableRowTypeOfData() {#getTableRowTypeOfData--}

Gets the type name of table rows that consists of data region of referenced table. Default is "Data", so in formula "#Data" represents the data region of the table.

```javascript
getTableRowTypeOfData() : string;
```


**Returns**

the type name of table rows

### getTableRowTypeOfAll() {#getTableRowTypeOfAll--}

Gets the type name of table rows that consists of all rows in referenced table. Default is "All", so in formula "#All" represents all rows in referenced table.

```javascript
getTableRowTypeOfAll() : string;
```


**Returns**

the type name of table rows

### getTableRowTypeOfTotals() {#getTableRowTypeOfTotals--}

Gets the type name of table rows that consists of the total row of referenced table. Default is "Totals", so in formula "#Totals" represents the total row of referenced table.

```javascript
getTableRowTypeOfTotals() : string;
```


**Returns**

the type name of table rows

### getTableRowTypeOfCurrent() {#getTableRowTypeOfCurrent--}

Gets the type name of table rows that consists of the current row in referenced table. Default is "This Row", so in formula "#This Row" represents the current row in referenced table.

```javascript
getTableRowTypeOfCurrent() : string;
```


**Returns**

the type name of table rows

### getErrorValueString(string) {#getErrorValueString-string-}

Gets the display string value for cell's error value

```javascript
getErrorValueString(err: string) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| err | string | error values such as #VALUE!,#NAME? |

**Returns**

By default returns the error value itself

### getBooleanValueString(boolean) {#getBooleanValueString-boolean-}

Gets the display string value for cell's boolean value

```javascript
getBooleanValueString(bv: boolean) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| bv | boolean | boolean value |

**Returns**

By default returns "TRUE" for true value and "FALSE" for false value.

### getLocalFunctionName(string) {#getLocalFunctionName-string-}

Gets the locale dependent function name according to given standard function name.

```javascript
getLocalFunctionName(standardName: string) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| standardName | string | Standard(en-US locale) function name. |

**Returns**

Locale dependent function name. The locale was specified by the Workbook for which this settings is used.

### getStandardFunctionName(string) {#getStandardFunctionName-string-}

Gets the standard function name according to given locale dependent function name.

```javascript
getStandardFunctionName(localName: string) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| localName | string | Locale dependent function name. The locale was specified by the Workbook for which this settings is used. |

**Returns**

Standard(en-US locale) function name.

### getLocalBuiltInName(string) {#getLocalBuiltInName-string-}

Gets the locale dependent text for built-in Name according to given standard text.

```javascript
getLocalBuiltInName(standardName: string) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| standardName | string | Standard(en-US locale) text of built-in Name. |

**Returns**

Locale dependent text. The locale was specified by the Workbook for which this settings is used.

### getStandardBuiltInName(string) {#getStandardBuiltInName-string-}

Gets the standard text of built-in Name according to given locale dependent text.

```javascript
getStandardBuiltInName(localName: string) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| localName | string | Locale dependent text of built-in Name. The locale was specified by the Workbook for which this settings is used. |

**Returns**

Standard(en-US locale) text.

### getStandardHeaderFooterFontStyleName(string) {#getStandardHeaderFooterFontStyleName-string-}

Gets standard English font style name(Regular, Bold, Italic) for Header/Footer according to given locale font style name.

```javascript
getStandardHeaderFooterFontStyleName(localfontStyleName: string) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| localfontStyleName | string | Locale font style name for Header/Footer. |

**Returns**

Standard English font style name(Regular, Bold, Italic)

### getCommentTitleName(CommentTitleType) {#getCommentTitleName-commenttitletype-}

Gets the locale dependent comment title name according to comment title type.

```javascript
getCommentTitleName(type: CommentTitleType) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [CommentTitleType](/nodejs-cpp/commenttitletype/) |  |

### compare(string, string, boolean) {#compare-string-string-boolean-}

Compares two string values according to certain collation rules.

```javascript
compare(v1: string, v2: string, ignoreCase: boolean) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| v1 | string | the first string |
| v2 | string | the second string |
| ignoreCase | boolean | whether ignore case when comparing values |

**Returns**

Integer that indicates the lexical relationship between the two comparands

### getListSeparator() {#getListSeparator--}

Gets the separator for list, parameters of function, ...etc.

```javascript
abstract getListSeparator() : string;
```


### getRowSeparatorOfFormulaArray() {#getRowSeparatorOfFormulaArray--}

Gets the separator for rows in array data in formula.

```javascript
abstract getRowSeparatorOfFormulaArray() : string;
```


### getColumnSeparatorOfFormulaArray() {#getColumnSeparatorOfFormulaArray--}

Gets the separator for the items in array's row data in formula.

```javascript
abstract getColumnSeparatorOfFormulaArray() : string;
```



