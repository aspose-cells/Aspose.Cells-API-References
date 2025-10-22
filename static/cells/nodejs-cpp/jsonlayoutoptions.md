##JsonLayoutOptions
Represents the options of json layout type.
## JsonLayoutOptions class
Represents the options of json layout type.
```javascript
class JsonLayoutOptions;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Constructor of loading JSON layout options. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [arrayAsTable](#arrayAsTable--)| boolean | Processes Array as table. |
| [ignoreNull](#ignoreNull--)| boolean | Indicates whether ignoring null value. |
| [ignoreTitle](#ignoreTitle--)| boolean | Ingores titles of attributes |
| [convertNumericOrDate](#convertNumericOrDate--)| boolean | Indicates whether converting the string in json to numeric or date value. |
| [numberFormat](#numberFormat--)| string | Gets and sets the format of numeric value. |
| [dateFormat](#dateFormat--)| string | Gets and sets the format of date value. |
| [titleStyle](#titleStyle--)| Style | Gets and sets the style of the title. |
| [keptSchema](#keptSchema--)| boolean | Indicates whether keeping schema of this json. |
## Methods
| Method | Description |
| --- | --- |
| [getArrayAsTable()](#getArrayAsTable--)| <b>@deprecated.</b> Please use the 'arrayAsTable' property instead. Processes Array as table. |
| [setArrayAsTable(boolean)](#setArrayAsTable-boolean-)| <b>@deprecated.</b> Please use the 'arrayAsTable' property instead. Processes Array as table. |
| [getIgnoreNull()](#getIgnoreNull--)| <b>@deprecated.</b> Please use the 'ignoreNull' property instead. Indicates whether ignoring null value. |
| [setIgnoreNull(boolean)](#setIgnoreNull-boolean-)| <b>@deprecated.</b> Please use the 'ignoreNull' property instead. Indicates whether ignoring null value. |
| [getIgnoreTitle()](#getIgnoreTitle--)| <b>@deprecated.</b> Please use the 'ignoreTitle' property instead. Ingores titles of attributes |
| [setIgnoreTitle(boolean)](#setIgnoreTitle-boolean-)| <b>@deprecated.</b> Please use the 'ignoreTitle' property instead. Ingores titles of attributes |
| [getConvertNumericOrDate()](#getConvertNumericOrDate--)| <b>@deprecated.</b> Please use the 'convertNumericOrDate' property instead. Indicates whether converting the string in json to numeric or date value. |
| [setConvertNumericOrDate(boolean)](#setConvertNumericOrDate-boolean-)| <b>@deprecated.</b> Please use the 'convertNumericOrDate' property instead. Indicates whether converting the string in json to numeric or date value. |
| [get_NumberFormat()](#get_NumberFormat--)| <b>@deprecated.</b> Please use the 'numberFormat' property instead. Gets and sets the format of numeric value. |
| [setNumberFormat(string)](#setNumberFormat-string-)| <b>@deprecated.</b> Please use the 'numberFormat' property instead. Gets and sets the format of numeric value. |
| [get_DateFormat()](#get_DateFormat--)| <b>@deprecated.</b> Please use the 'dateFormat' property instead. Gets and sets the format of date value. |
| [setDateFormat(string)](#setDateFormat-string-)| <b>@deprecated.</b> Please use the 'dateFormat' property instead. Gets and sets the format of date value. |
| [getTitleStyle()](#getTitleStyle--)| <b>@deprecated.</b> Please use the 'titleStyle' property instead. Gets and sets the style of the title. |
| [setTitleStyle(Style)](#setTitleStyle-style-)| <b>@deprecated.</b> Please use the 'titleStyle' property instead. Gets and sets the style of the title. |
| [getKeptSchema()](#getKeptSchema--)| <b>@deprecated.</b> Please use the 'keptSchema' property instead. Indicates whether keeping schema of this json. |
| [setKeptSchema(boolean)](#setKeptSchema-boolean-)| <b>@deprecated.</b> Please use the 'keptSchema' property instead. Indicates whether keeping schema of this json. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### constructor() {#constructor--}
Constructor of loading JSON layout options.
```javascript
constructor();
```
### arrayAsTable {#arrayAsTable--}
Processes Array as table.
```javascript
arrayAsTable : boolean;
```
### ignoreNull {#ignoreNull--}
Indicates whether ignoring null value.
```javascript
ignoreNull : boolean;
```
### ignoreTitle {#ignoreTitle--}
Ingores titles of attributes
```javascript
ignoreTitle : boolean;
```
### convertNumericOrDate {#convertNumericOrDate--}
Indicates whether converting the string in json to numeric or date value.
```javascript
convertNumericOrDate : boolean;
```
### numberFormat {#numberFormat--}
Gets and sets the format of numeric value.
```javascript
numberFormat : string;
```
### dateFormat {#dateFormat--}
Gets and sets the format of date value.
```javascript
dateFormat : string;
```
### titleStyle {#titleStyle--}
Gets and sets the style of the title.
```javascript
titleStyle : Style;
```
### keptSchema {#keptSchema--}
Indicates whether keeping schema of this json.
```javascript
keptSchema : boolean;
```
**Remarks**
Sometimes we will save the file to JSON after loading JSON file.
### getArrayAsTable() {#getArrayAsTable--}
```javascript
getArrayAsTable() : boolean;
```
### setArrayAsTable(boolean) {#setArrayAsTable-boolean-}
```javascript
setArrayAsTable(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getIgnoreNull() {#getIgnoreNull--}
```javascript
getIgnoreNull() : boolean;
```
### setIgnoreNull(boolean) {#setIgnoreNull-boolean-}
```javascript
setIgnoreNull(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getIgnoreTitle() {#getIgnoreTitle--}
```javascript
getIgnoreTitle() : boolean;
```
### setIgnoreTitle(boolean) {#setIgnoreTitle-boolean-}
```javascript
setIgnoreTitle(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getConvertNumericOrDate() {#getConvertNumericOrDate--}
```javascript
getConvertNumericOrDate() : boolean;
```
### setConvertNumericOrDate(boolean) {#setConvertNumericOrDate-boolean-}
```javascript
setConvertNumericOrDate(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### get_NumberFormat() {#get_NumberFormat--}
```javascript
get_NumberFormat() : string;
```
### setNumberFormat(string) {#setNumberFormat-string-}
```javascript
setNumberFormat(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### get_DateFormat() {#get_DateFormat--}
```javascript
get_DateFormat() : string;
```
### setDateFormat(string) {#setDateFormat-string-}
```javascript
setDateFormat(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getTitleStyle() {#getTitleStyle--}
```javascript
getTitleStyle() : Style;
```
**Returns**
[Style](../style/)
### setTitleStyle(Style) {#setTitleStyle-style-}
```javascript
setTitleStyle(value: Style) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Style](../style/) | The value to set. |
### getKeptSchema() {#getKeptSchema--}
```javascript
getKeptSchema() : boolean;
```
**Remarks**
Sometimes we will save the file to JSON after loading JSON file.
### setKeptSchema(boolean) {#setKeptSchema-boolean-}
```javascript
setKeptSchema(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
Sometimes we will save the file to JSON after loading JSON file.
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
