##ScenarioInputCell
Represents input cell for the scenario.
## ScenarioInputCell class
Represents input cell for the scenario.
```javascript
class ScenarioInputCell;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [row](#row--)| number | Readonly. Gets and sets the row index of the input cell. |
| [column](#column--)| number | Readonly. Gets and sets the column index of the input cell. |
| [name](#name--)| string | Readonly. Gets and sets the input cell address. |
| [value](#value--)| string | Gets and sets value of the input cell. |
| [isDeleted](#isDeleted--)| boolean | Indicates whether input cell is deleted. |
## Methods
| Method | Description |
| --- | --- |
| [getRow()](#getRow--)| <b>@deprecated.</b> Please use the 'row' property instead. Gets and sets the row index of the input cell. |
| [getColumn()](#getColumn--)| <b>@deprecated.</b> Please use the 'column' property instead. Gets and sets the column index of the input cell. |
| [getName()](#getName--)| <b>@deprecated.</b> Please use the 'name' property instead. Gets and sets the input cell address. |
| [getValue()](#getValue--)| <b>@deprecated.</b> Please use the 'value' property instead. Gets and sets value of the input cell. |
| [setValue(string)](#setValue-string-)| <b>@deprecated.</b> Please use the 'value' property instead. Gets and sets value of the input cell. |
| [isDeleted()](#isDeleted--)| <b>@deprecated.</b> Please use the 'isDeleted' property instead. Indicates whether input cell is deleted. |
| [setIsDeleted(boolean)](#setIsDeleted-boolean-)| <b>@deprecated.</b> Please use the 'isDeleted' property instead. Indicates whether input cell is deleted. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### row {#row--}
Readonly. Gets and sets the row index of the input cell.
```javascript
row : number;
```
### column {#column--}
Readonly. Gets and sets the column index of the input cell.
```javascript
column : number;
```
### name {#name--}
Readonly. Gets and sets the input cell address.
```javascript
name : string;
```
### value {#value--}
Gets and sets value of the input cell.
```javascript
value : string;
```
### isDeleted {#isDeleted--}
Indicates whether input cell is deleted.
```javascript
isDeleted : boolean;
```
### getRow() {#getRow--}
```javascript
getRow() : number;
```
### getColumn() {#getColumn--}
```javascript
getColumn() : number;
```
### getName() {#getName--}
```javascript
getName() : string;
```
### getValue() {#getValue--}
```javascript
getValue() : string;
```
### setValue(string) {#setValue-string-}
```javascript
setValue(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### isDeleted() {#isDeleted--}
```javascript
isDeleted() : boolean;
```
### setIsDeleted(boolean) {#setIsDeleted-boolean-}
```javascript
setIsDeleted(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
