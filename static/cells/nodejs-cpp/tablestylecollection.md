##TableStyleCollection
Represents all custom table styles.
## TableStyleCollection class
Represents all custom table styles.
```javascript
class TableStyleCollection;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [defaultTableStyleName](#defaultTableStyleName--)| string | Gets and sets the default style name of the table. |
| [defaultPivotStyleName](#defaultPivotStyleName--)| string | Gets and sets the  default style name of pivot table . |
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the table style by the index. |
| [get(string)](#get-string-)| Gets the table style by the name. |
| [getDefaultTableStyleName()](#getDefaultTableStyleName--)| <b>@deprecated.</b> Please use the 'defaultTableStyleName' property instead. Gets and sets the default style name of the table. |
| [setDefaultTableStyleName(string)](#setDefaultTableStyleName-string-)| <b>@deprecated.</b> Please use the 'defaultTableStyleName' property instead. Gets and sets the default style name of the table. |
| [getDefaultPivotStyleName()](#getDefaultPivotStyleName--)| <b>@deprecated.</b> Please use the 'defaultPivotStyleName' property instead. Gets and sets the  default style name of pivot table . |
| [setDefaultPivotStyleName(string)](#setDefaultPivotStyleName-string-)| <b>@deprecated.</b> Please use the 'defaultPivotStyleName' property instead. Gets and sets the  default style name of pivot table . |
| [addTableStyle(string)](#addTableStyle-string-)| Adds a custom table style. |
| [addPivotTableStyle(string)](#addPivotTableStyle-string-)| Adds a custom pivot table style. |
| [getBuiltinTableStyle(TableStyleType)](#getBuiltinTableStyle-tablestyletype-)| Gets the builtin table style |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### defaultTableStyleName {#defaultTableStyleName--}
Gets and sets the default style name of the table.
```javascript
defaultTableStyleName : string;
```
### defaultPivotStyleName {#defaultPivotStyleName--}
Gets and sets the  default style name of pivot table .
```javascript
defaultPivotStyleName : string;
```
### get(number) {#get-number-}
Gets the table style by the index.
```javascript
get(index: number) : TableStyle;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The position of the table style in the list. |
**Returns**
The table style object.
### get(string) {#get-string-}
Gets the table style by the name.
```javascript
get(name: string) : TableStyle;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The table style name. |
**Returns**
The table style object.
### getDefaultTableStyleName() {#getDefaultTableStyleName--}
```javascript
getDefaultTableStyleName() : string;
```
### setDefaultTableStyleName(string) {#setDefaultTableStyleName-string-}
```javascript
setDefaultTableStyleName(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getDefaultPivotStyleName() {#getDefaultPivotStyleName--}
```javascript
getDefaultPivotStyleName() : string;
```
### setDefaultPivotStyleName(string) {#setDefaultPivotStyleName-string-}
```javascript
setDefaultPivotStyleName(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### addTableStyle(string) {#addTableStyle-string-}
Adds a custom table style.
```javascript
addTableStyle(name: string) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The table style name. |
**Returns**
The index of the table style.
### addPivotTableStyle(string) {#addPivotTableStyle-string-}
Adds a custom pivot table style.
```javascript
addPivotTableStyle(name: string) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The pivot table style name. |
**Returns**
The index of the pivot table style.
### getBuiltinTableStyle(TableStyleType) {#getBuiltinTableStyle-tablestyletype-}
Gets the builtin table style
```javascript
getBuiltinTableStyle(type: TableStyleType) : TableStyle;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [TableStyleType](../tablestyletype/) | The builtin table style type. |
**Returns**
[TableStyle](../tablestyle/)
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
