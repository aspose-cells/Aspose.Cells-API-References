##HorizontalPageBreak
Encapsulates the object that represents a horizontal page break.
## HorizontalPageBreak class
Encapsulates the object that represents a horizontal page break.
```javascript
class HorizontalPageBreak;
```
### Example
```javascript
const { Workbook } = AsposeCells;
//Instantiating a Workbook object
var workbook = new Workbook();
//Obtaining the reference of the newly added worksheet by passing its sheet index
var worksheet = workbook.worksheets.get(0);
//Add a page break at cell Y30
var Index = worksheet.horizontalPageBreaks.add("Y30");
//get the newly added horizontal page break
var hPageBreak = worksheet.horizontalPageBreaks.get(Index);
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [startColumn](#startColumn--)| number | Readonly. Gets the start column index of this horizontal page break. |
| [endColumn](#endColumn--)| number | Readonly. Gets the end column index of this horizontal page break. |
| [row](#row--)| number | Readonly. Gets the zero based row index. |
### startColumn {#startColumn--}
Readonly. Gets the start column index of this horizontal page break.
```javascript
startColumn : number;
```
### endColumn {#endColumn--}
Readonly. Gets the end column index of this horizontal page break.
```javascript
endColumn : number;
```
### row {#row--}
Readonly. Gets the zero based row index.
```javascript
row : number;
```
