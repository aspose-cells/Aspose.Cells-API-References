##VerticalPageBreak
Encapsulates the object that represents a vertical page break.
## VerticalPageBreak class
Encapsulates the object that represents a vertical page break.
```javascript
class VerticalPageBreak;
```
### Example
```javascript
const { Workbook } = AsposeCells;
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
