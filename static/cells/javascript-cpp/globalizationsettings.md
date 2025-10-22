##GlobalizationSettings
Represents the globalization settings.
## GlobalizationSettings class
Represents the globalization settings.
```javascript
class GlobalizationSettings;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [chartSettings](#chartSettings--)| ChartGlobalizationSettings | Gets or sets the globalization settings for Chart. |
| [pivotSettings](#pivotSettings--)| PivotGlobalizationSettings | Gets or sets the globalization settings for pivot table. |
## Methods
| Method | Description |
| --- | --- |
| abstract [getListSeparator()](#getListSeparator--)| Gets the separator for list, parameters of function, ...etc. |
| abstract [getRowSeparatorOfFormulaArray()](#getRowSeparatorOfFormulaArray--)| Gets the separator for rows in array data in formula. |
| abstract [getColumnSeparatorOfFormulaArray()](#getColumnSeparatorOfFormulaArray--)| Gets the separator for the items in array's row data in formula. |
| abstract [getTotalName(ConsolidationFunction)](#getTotalName-consolidationfunction-)| Gets the total name of the function. |
| abstract [getGrandTotalName(ConsolidationFunction)](#getGrandTotalName-consolidationfunction-)| Gets the grand total name of the function. |
| abstract [getDefaultSheetName()](#getDefaultSheetName--)| Gets the default sheet name for adding worksheet automatically. Default is "Sheet". |
| abstract [getTableRowTypeOfHeaders()](#getTableRowTypeOfHeaders--)| Gets the type name of table rows that consists of the table header. Default is "Headers", so in formula "#Headers" represents the table header. |
| abstract [getTableRowTypeOfData()](#getTableRowTypeOfData--)| Gets the type name of table rows that consists of data region of referenced table. Default is "Data", so in formula "#Data" represents the data region of the table. |
| abstract [getTableRowTypeOfAll()](#getTableRowTypeOfAll--)| Gets the type name of table rows that consists of all rows in referenced table. Default is "All", so in formula "#All" represents all rows in referenced table. |
| abstract [getTableRowTypeOfTotals()](#getTableRowTypeOfTotals--)| Gets the type name of table rows that consists of the total row of referenced table. Default is "Totals", so in formula "#Totals" represents the total row of referenced table. |
| abstract [getTableRowTypeOfCurrent()](#getTableRowTypeOfCurrent--)| Gets the type name of table rows that consists of the current row in referenced table. Default is "This Row", so in formula "#This Row" represents the current row in referenced table. |
| abstract [getErrorValueString(string)](#getErrorValueString-string-)| Gets the display string value for cell's error value |
| abstract [getBooleanValueString(boolean)](#getBooleanValueString-boolean-)| Gets the display string value for cell's boolean value |
| abstract [getLocalFunctionName(string)](#getLocalFunctionName-string-)| Gets the locale dependent function name according to given standard function name. |
| abstract [getStandardFunctionName(string)](#getStandardFunctionName-string-)| Gets the standard function name according to given locale dependent function name. |
| abstract [getLocalBuiltInName(string)](#getLocalBuiltInName-string-)| Gets the locale dependent text for built-in Name according to given standard text. |
| abstract [getStandardBuiltInName(string)](#getStandardBuiltInName-string-)| Gets the standard text of built-in Name according to given locale dependent text. |
| abstract [getStandardHeaderFooterFontStyleName(string)](#getStandardHeaderFooterFontStyleName-string-)| Gets standard English font style name(Regular, Bold, Italic) for Header/Footer according to given locale font style name. |
| abstract [getCommentTitleName(CommentTitleType)](#getCommentTitleName-commenttitletype-)| Gets the locale dependent comment title name according to comment title type. |
| abstract [compare(string, string, boolean)](#compare-string-string-boolean-)| Compares two string values according to certain collation rules. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### chartSettings {#chartSettings--}
Gets or sets the globalization settings for Chart.
```javascript
chartSettings : ChartGlobalizationSettings;
```
### pivotSettings {#pivotSettings--}
Gets or sets the globalization settings for pivot table.
```javascript
pivotSettings : PivotGlobalizationSettings;
```
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
### getTotalName(ConsolidationFunction) {#getTotalName-consolidationfunction-}
Gets the total name of the function.
```javascript
abstract getTotalName(functionType: ConsolidationFunction) : string;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| functionType | [ConsolidationFunction](../consolidationfunction/) | The function type. |
**Returns**
The total name of the function.
### getGrandTotalName(ConsolidationFunction) {#getGrandTotalName-consolidationfunction-}
Gets the grand total name of the function.
```javascript
abstract getGrandTotalName(functionType: ConsolidationFunction) : string;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| functionType | [ConsolidationFunction](../consolidationfunction/) | The function type. |
**Returns**
The grand total name of the function.
### getDefaultSheetName() {#getDefaultSheetName--}
Gets the default sheet name for adding worksheet automatically. Default is "Sheet".
```javascript
abstract getDefaultSheetName() : string;
```
**Returns**
the default sheet name for adding worksheet automatically
**Remarks**
The automatically added(such as by [WorksheetCollection.Add()](../worksheetcollection.add()/)) sheet's name will be the specified name plus sequence number. For example, for Germany user maybe wants the sheet name to be "Tabellenblatt2" instead of "Sheet2". Then user may implement this method to return "Tabellenblatt".
### getTableRowTypeOfHeaders() {#getTableRowTypeOfHeaders--}
Gets the type name of table rows that consists of the table header. Default is "Headers", so in formula "#Headers" represents the table header.
```javascript
abstract getTableRowTypeOfHeaders() : string;
```
**Returns**
the type name of table rows
### getTableRowTypeOfData() {#getTableRowTypeOfData--}
Gets the type name of table rows that consists of data region of referenced table. Default is "Data", so in formula "#Data" represents the data region of the table.
```javascript
abstract getTableRowTypeOfData() : string;
```
**Returns**
the type name of table rows
### getTableRowTypeOfAll() {#getTableRowTypeOfAll--}
Gets the type name of table rows that consists of all rows in referenced table. Default is "All", so in formula "#All" represents all rows in referenced table.
```javascript
abstract getTableRowTypeOfAll() : string;
```
**Returns**
the type name of table rows
### getTableRowTypeOfTotals() {#getTableRowTypeOfTotals--}
Gets the type name of table rows that consists of the total row of referenced table. Default is "Totals", so in formula "#Totals" represents the total row of referenced table.
```javascript
abstract getTableRowTypeOfTotals() : string;
```
**Returns**
the type name of table rows
### getTableRowTypeOfCurrent() {#getTableRowTypeOfCurrent--}
Gets the type name of table rows that consists of the current row in referenced table. Default is "This Row", so in formula "#This Row" represents the current row in referenced table.
```javascript
abstract getTableRowTypeOfCurrent() : string;
```
**Returns**
the type name of table rows
### getErrorValueString(string) {#getErrorValueString-string-}
Gets the display string value for cell's error value
```javascript
abstract getErrorValueString(err: string) : string;
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
abstract getBooleanValueString(bv: boolean) : string;
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
abstract getLocalFunctionName(standardName: string) : string;
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
abstract getStandardFunctionName(localName: string) : string;
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
abstract getLocalBuiltInName(standardName: string) : string;
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
abstract getStandardBuiltInName(localName: string) : string;
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
abstract getStandardHeaderFooterFontStyleName(localfontStyleName: string) : string;
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
abstract getCommentTitleName(type: CommentTitleType) : string;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [CommentTitleType](../commenttitletype/) |  |
### compare(string, string, boolean) {#compare-string-string-boolean-}
Compares two string values according to certain collation rules.
```javascript
abstract compare(v1: string, v2: string, ignoreCase: boolean) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| v1 | string | the first string |
| v2 | string | the second string |
| ignoreCase | boolean | whether ignore case when comparing values |
**Returns**
Integer that indicates the lexical relationship between the two comparands
