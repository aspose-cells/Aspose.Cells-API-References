##CellWatch
Represents Cell Watch Item in the watch window.
## CellWatch class
Represents Cell Watch Item in the 'watch window'.
```javascript
class CellWatch;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [row](#row--)| number | Gets and sets the row of the cell. |
| [column](#column--)| number | Gets and sets the column of the cell. |
| [cellName](#cellName--)| string | Gets and sets the name of the cell. |
## Methods
| Method | Description |
| --- | --- |
| [getRow()](#getRow--)| <b>@deprecated.</b> Please use the 'row' property instead. Gets and sets the row of the cell. |
| [setRow(number)](#setRow-number-)| <b>@deprecated.</b> Please use the 'row' property instead. Gets and sets the row of the cell. |
| [getColumn()](#getColumn--)| <b>@deprecated.</b> Please use the 'column' property instead. Gets and sets the column of the cell. |
| [setColumn(number)](#setColumn-number-)| <b>@deprecated.</b> Please use the 'column' property instead. Gets and sets the column of the cell. |
| [getCellName()](#getCellName--)| <b>@deprecated.</b> Please use the 'cellName' property instead. Gets and sets the name of the cell. |
| [setCellName(string)](#setCellName-string-)| <b>@deprecated.</b> Please use the 'cellName' property instead. Gets and sets the name of the cell. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### row {#row--}
Gets and sets the row of the cell.
```javascript
row : number;
```
### column {#column--}
Gets and sets the column of the cell.
```javascript
column : number;
```
### cellName {#cellName--}
Gets and sets the name of the cell.
```javascript
cellName : string;
```
### getRow() {#getRow--}
```javascript
getRow() : number;
```
### setRow(number) {#setRow-number-}
```javascript
setRow(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getColumn() {#getColumn--}
```javascript
getColumn() : number;
```
### setColumn(number) {#setColumn-number-}
```javascript
setColumn(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getCellName() {#getCellName--}
```javascript
getCellName() : string;
```
### setCellName(string) {#setCellName-string-}
```javascript
setCellName(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
