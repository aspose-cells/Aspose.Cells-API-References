##SettableGlobalizationSettings
Implementation of GlobalizationSettings that supports user to setchange predefined texts.
## SettableGlobalizationSettings class
Implementation of GlobalizationSettings that supports user to set/change pre-defined texts.
```javascript
class SettableGlobalizationSettings;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Methods
| Method | Description |
| --- | --- |
| [setTotalName(ConsolidationFunction, string)](#setTotalName-consolidationfunction-string-)| Sets the total name of specific function. |
| [setGrandTotalName(ConsolidationFunction, string)](#setGrandTotalName-consolidationfunction-string-)| Sets the grand total name of specific function. |
| [setTableRowTypeOfHeaders(string)](#setTableRowTypeOfHeaders-string-)| Sets the type name of table rows that consists of the table header. |
| [setTableRowTypeOfData(string)](#setTableRowTypeOfData-string-)| Sets the type name of table rows that consists of data region of referenced table. |
| [setTableRowTypeOfAll(string)](#setTableRowTypeOfAll-string-)| Sets the type name of table rows that consists of all rows in referenced table. |
| [setTableRowTypeOfTotals(string)](#setTableRowTypeOfTotals-string-)| Sets the type name of table rows that consists of the total row of referenced table. |
| [setTableRowTypeOfCurrent(string)](#setTableRowTypeOfCurrent-string-)| Sets the type name of table rows that consists of the current row in referenced table. |
| [setBooleanValueString(boolean, string)](#setBooleanValueString-boolean-string-)| Sets the display string value for cell's boolean value |
| [setLocalFunctionName(string, string, boolean)](#setLocalFunctionName-string-string-boolean-)| Sets the locale dependent function name corresponding to given standard function name. |
| [setStandardFunctionName(string, string, boolean)](#setStandardFunctionName-string-string-boolean-)| Sets the locale dependent function name according to given standard function name. |
| [setLocalBuiltInName(string, string, boolean)](#setLocalBuiltInName-string-string-boolean-)| Sets the locale dependent text for the built-in name with given standard name text. |
| [setStandardBuiltInName(string, string, boolean)](#setStandardBuiltInName-string-string-boolean-)| Sets the locale dependent function name according to given standard function name. |
| [setListSeparator(string)](#setListSeparator-string-)| Sets the separator for list, parameters of function, ...etc. |
| [setRowSeparatorOfFormulaArray(string)](#setRowSeparatorOfFormulaArray-string-)| Sets the separator for rows in array data in formula. |
| [setColumnSeparatorOfFormulaArray(string)](#setColumnSeparatorOfFormulaArray-string-)| Sets the separator for the items in array's row data in formula. |
| [setStandardHeaderFooterFontStyleName(string, string)](#setStandardHeaderFooterFontStyleName-string-string-)| Sets the locale dependent function name according to given standard function name. |
| [setCommentTitleName(CommentTitleType, string)](#setCommentTitleName-commenttitletype-string-)| Gets the locale dependent comment title name according to comment title type. |
| [getListSeparator()](#getListSeparator--)| Gets the separator for list, parameters of function, ...etc. |
| [getRowSeparatorOfFormulaArray()](#getRowSeparatorOfFormulaArray--)| Gets the separator for rows in array data in formula. |
| [getColumnSeparatorOfFormulaArray()](#getColumnSeparatorOfFormulaArray--)| Gets the separator for the items in array's row data in formula. |
| [getTotalName(ConsolidationFunction)](#getTotalName-consolidationfunction-)| Gets the total name of specific function. |
| [getGrandTotalName(ConsolidationFunction)](#getGrandTotalName-consolidationfunction-)| Gets the grand total name of the function. |
| [getTableRowTypeOfHeaders()](#getTableRowTypeOfHeaders--)| Gets the type name of table rows that consists of the table header. Default is "Headers", so in formula "#Headers" represents the table header. |
| [getTableRowTypeOfData()](#getTableRowTypeOfData--)| Gets the type name of table rows that consists of data region of referenced table. Default is "Data", so in formula "#Data" represents the data region of the table. |
| [getTableRowTypeOfAll()](#getTableRowTypeOfAll--)| Gets the type name of table rows that consists of all rows in referenced table. |
| [getTableRowTypeOfTotals()](#getTableRowTypeOfTotals--)| Gets the type name of table rows that consists of the total row of referenced table. |
| [getTableRowTypeOfCurrent()](#getTableRowTypeOfCurrent--)| Gets the type name of table rows that consists of the current row in referenced table. |
| [getErrorValueString(string)](#getErrorValueString-string-)| Gets the display string value for cell's error value |
| [getBooleanValueString(boolean)](#getBooleanValueString-boolean-)| Gets the display string value for cell's boolean value |
| [getLocalFunctionName(string)](#getLocalFunctionName-string-)| Gets the locale dependent function name according to given standard function name. |
| [getStandardFunctionName(string)](#getStandardFunctionName-string-)| Gets the standard function name according to given locale dependent function name. |
| [getLocalBuiltInName(string)](#getLocalBuiltInName-string-)| Gets the locale dependent text for built-in Name according to given standard text. |
| [getStandardBuiltInName(string)](#getStandardBuiltInName-string-)| Gets the standard text of built-in Name according to given locale dependent text. |
| [getStandardHeaderFooterFontStyleName(string)](#getStandardHeaderFooterFontStyleName-string-)| Gets standard English font style name(Regular, Bold, Italic) for Header/Footer according to given locale font style name. |
| [getCommentTitleName(CommentTitleType)](#getCommentTitleName-commenttitletype-)| Gets the locale dependent comment title name according to comment title type. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### setTotalName(ConsolidationFunction, string) {#setTotalName-consolidationfunction-string-}
Sets the total name of specific function.
```javascript
setTotalName(functionType: ConsolidationFunction, name: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| functionType | [ConsolidationFunction](../consolidationfunction/) | The function type. |
| name | string | The total name of the function. |
### setGrandTotalName(ConsolidationFunction, string) {#setGrandTotalName-consolidationfunction-string-}
Sets the grand total name of specific function.
```javascript
setGrandTotalName(functionType: ConsolidationFunction, name: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| functionType | [ConsolidationFunction](../consolidationfunction/) | The function type. |
| name | string | The grand total name of the function. |
### setTableRowTypeOfHeaders(string) {#setTableRowTypeOfHeaders-string-}
Sets the type name of table rows that consists of the table header.
```javascript
setTableRowTypeOfHeaders(name: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | the type name of table rows |
### setTableRowTypeOfData(string) {#setTableRowTypeOfData-string-}
Sets the type name of table rows that consists of data region of referenced table.
```javascript
setTableRowTypeOfData(name: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | the type name of table rows |
### setTableRowTypeOfAll(string) {#setTableRowTypeOfAll-string-}
Sets the type name of table rows that consists of all rows in referenced table.
```javascript
setTableRowTypeOfAll(name: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | the type name of table rows |
### setTableRowTypeOfTotals(string) {#setTableRowTypeOfTotals-string-}
Sets the type name of table rows that consists of the total row of referenced table.
```javascript
setTableRowTypeOfTotals(name: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | the type name of table rows |
### setTableRowTypeOfCurrent(string) {#setTableRowTypeOfCurrent-string-}
Sets the type name of table rows that consists of the current row in referenced table.
```javascript
setTableRowTypeOfCurrent(name: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | the type name of table rows |
### setBooleanValueString(boolean, string) {#setBooleanValueString-boolean-string-}
Sets the display string value for cell's boolean value
```javascript
setBooleanValueString(bv: boolean, name: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| bv | boolean | boolean value |
| name | string | string value of the boolean value |
### setLocalFunctionName(string, string, boolean) {#setLocalFunctionName-string-string-boolean-}
Sets the locale dependent function name corresponding to given standard function name.
```javascript
setLocalFunctionName(standardName: string, localName: string, bidirectional: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| standardName | string | Standard(en-US locale) function name. |
| localName | string | Locale dependent function name |
| bidirectional | boolean | Whether map the local function name to standard function name automatically.         /// If true, the local name will be mapped to standard name automatically         /// so user does not need to call [SetStandardFunctionName(string, string, bool)](../setstandardfunctionname(string, string, bool)/) again         /// for the same standard and local names pair |
### setStandardFunctionName(string, string, boolean) {#setStandardFunctionName-string-string-boolean-}
Sets the locale dependent function name according to given standard function name.
```javascript
setStandardFunctionName(localName: string, standardName: string, bidirectional: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| localName | string | Locale dependent function name |
| standardName | string | Standard(en-US locale) function name. |
| bidirectional | boolean | Whether map the standard function name to local function name automatically.         /// If true, the standar name will be mapped to local name automatically         /// so user does not need to call [SetLocalFunctionName(string, string, bool)](../setlocalfunctionname(string, string, bool)/) again         /// for the same standard and local names pair |
### setLocalBuiltInName(string, string, boolean) {#setLocalBuiltInName-string-string-boolean-}
Sets the locale dependent text for the built-in name with given standard name text.
```javascript
setLocalBuiltInName(standardName: string, localName: string, bidirectional: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| standardName | string | Standard(en-US locale) name text of built-in name. |
| localName | string | Locale dependent name text |
| bidirectional | boolean | Whether map the local name text to standard name text automatically.         /// If true, the local name text will be mapped to standard name text automatically         /// so user does not need to call [SetStandardBuiltInName(string, string, bool)](../setstandardbuiltinname(string, string, bool)/) again         /// for the same standard and local names pair |
### setStandardBuiltInName(string, string, boolean) {#setStandardBuiltInName-string-string-boolean-}
Sets the locale dependent function name according to given standard function name.
```javascript
setStandardBuiltInName(localName: string, standardName: string, bidirectional: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| localName | string | Locale dependent function name |
| standardName | string | Standard(en-US locale) function name. |
| bidirectional | boolean | Whether map the standard name text to local name text automatically.         /// If true, the standar name text will be mapped to local name text automatically         /// so user does not need to call [SetLocalBuiltInName(string, string, bool)](../setlocalbuiltinname(string, string, bool)/) again         /// for the same standard and local names pair |
### setListSeparator(string) {#setListSeparator-string-}
Sets the separator for list, parameters of function, ...etc.
```javascript
setListSeparator(c: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| c | string | the specified separator |
### setRowSeparatorOfFormulaArray(string) {#setRowSeparatorOfFormulaArray-string-}
Sets the separator for rows in array data in formula.
```javascript
setRowSeparatorOfFormulaArray(c: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| c | string | the specified separator |
### setColumnSeparatorOfFormulaArray(string) {#setColumnSeparatorOfFormulaArray-string-}
Sets the separator for the items in array's row data in formula.
```javascript
setColumnSeparatorOfFormulaArray(c: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| c | string | the specified separator |
### setStandardHeaderFooterFontStyleName(string, string) {#setStandardHeaderFooterFontStyleName-string-string-}
Sets the locale dependent function name according to given standard function name.
```javascript
setStandardHeaderFooterFontStyleName(localfontStyleName: string, standardName: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| localfontStyleName | string | Locale font style name for Header/Footer. |
| standardName | string | Standard(en-US locale) function name. |
### setCommentTitleName(CommentTitleType, string) {#setCommentTitleName-commenttitletype-string-}
Gets the locale dependent comment title name according to comment title type.
```javascript
setCommentTitleName(type: CommentTitleType, name: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [CommentTitleType](../commenttitletype/) | type of comment title |
| name | string | locale dependent comment title name |
### getListSeparator() {#getListSeparator--}
Gets the separator for list, parameters of function, ...etc.
```javascript
getListSeparator() : string;
```
### getRowSeparatorOfFormulaArray() {#getRowSeparatorOfFormulaArray--}
Gets the separator for rows in array data in formula.
```javascript
getRowSeparatorOfFormulaArray() : string;
```
### getColumnSeparatorOfFormulaArray() {#getColumnSeparatorOfFormulaArray--}
Gets the separator for the items in array's row data in formula.
```javascript
getColumnSeparatorOfFormulaArray() : string;
```
### getTotalName(ConsolidationFunction) {#getTotalName-consolidationfunction-}
Gets the total name of specific function.
```javascript
getTotalName(functionType: ConsolidationFunction) : string;
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
getGrandTotalName(functionType: ConsolidationFunction) : string;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| functionType | [ConsolidationFunction](../consolidationfunction/) | The function type. |
**Returns**
The grand total name of the function.
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
Gets the type name of table rows that consists of all rows in referenced table.
```javascript
getTableRowTypeOfAll() : string;
```
**Returns**
the type name of table rows
### getTableRowTypeOfTotals() {#getTableRowTypeOfTotals--}
Gets the type name of table rows that consists of the total row of referenced table.
```javascript
getTableRowTypeOfTotals() : string;
```
**Returns**
the type name of table rows
### getTableRowTypeOfCurrent() {#getTableRowTypeOfCurrent--}
Gets the type name of table rows that consists of the current row in referenced table.
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
| type | [CommentTitleType](../commenttitletype/) | type of comment title |
**Returns**
locale dependent comment title name
