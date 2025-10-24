##VerticalPageBreak
Encapsulates the object that represents a vertical page break.
## VerticalPageBreak class
Encapsulates the object that represents a vertical page break.
```javascript
class VerticalPageBreak;
```
### Example
```javascript
const { Workbook } = require("aspose.cells.node");
var excel = new Workbook();
//Add a pagebreak at G5
excel.worksheets.get(0).horizontalPageBreaks.add("G5");
excel.worksheets.get(0).verticalPageBreaks.add("G5");
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [startRow](#startRow--)| number | Readonly. Gets the start row index of the vertical page break. |
| [endRow](#endRow--)| number | Readonly. Gets the end row index of the vertical page break. |
| [column](#column--)| number | Readonly. Gets the column index of the vertical page break. |
## Methods
| Method | Description |
| --- | --- |
| [getStartRow()](#getStartRow--)| <b>@deprecated.</b> Please use the 'startRow' property instead. Gets the start row index of the vertical page break. |
| [getEndRow()](#getEndRow--)| <b>@deprecated.</b> Please use the 'endRow' property instead. Gets the end row index of the vertical page break. |
| [getColumn()](#getColumn--)| <b>@deprecated.</b> Please use the 'column' property instead. Gets the column index of the vertical page break. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### startRow {#startRow--}
Readonly. Gets the start row index of the vertical page break.
```javascript
startRow : number;
```
### endRow {#endRow--}
Readonly. Gets the end row index of the vertical page break.
```javascript
endRow : number;
```
### column {#column--}
Readonly. Gets the column index of the vertical page break.
```javascript
column : number;
```
### getStartRow() {#getStartRow--}
```javascript
getStartRow() : number;
```
### getEndRow() {#getEndRow--}
```javascript
getEndRow() : number;
```
### getColumn() {#getColumn--}
```javascript
getColumn() : number;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
