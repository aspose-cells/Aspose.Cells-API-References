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
| [addTableStyle(string)](#addTableStyle-string-)| Adds a custom table style. |
| [addPivotTableStyle(string)](#addPivotTableStyle-string-)| Adds a custom pivot table style. |
| [getBuiltinTableStyle(TableStyleType)](#getBuiltinTableStyle-tablestyletype-)| Gets the builtin table style |
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
