##CalculationCell
Represents the calculation relevant data about one cell which is being calculated.
## CalculationCell class
Represents the calculation relevant data about one cell which is being calculated.
```javascript
class CalculationCell;
```
### Remarks
All objects provided by this class are for "read" purpose only. User should not change any data in the Workbook during the formula calculation process, Otherwise unexpected result or Exception may be caused.
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [workbook](#workbook--)| Workbook | Readonly. Gets the Workbook object. |
| [worksheet](#worksheet--)| Worksheet | Readonly. Gets the Worksheet object where the cell is in. |
| [cellRow](#cellRow--)| number | Readonly. Gets the row index of the cell. |
| [cellColumn](#cellColumn--)| number | Readonly. Gets the column index of the cell. |
| [cell](#cell--)| Cell | Readonly. Gets the Cell object which is being calculated. |
## Methods
| Method | Description |
| --- | --- |
| [setCalculatedValue(VObject)](#setCalculatedValue-vobject-)| Sets the calculated value for the cell. |
### workbook {#workbook--}
Readonly. Gets the Workbook object.
```javascript
workbook : Workbook;
```
### worksheet {#worksheet--}
Readonly. Gets the Worksheet object where the cell is in.
```javascript
worksheet : Worksheet;
```
### cellRow {#cellRow--}
Readonly. Gets the row index of the cell.
```javascript
cellRow : number;
```
### cellColumn {#cellColumn--}
Readonly. Gets the column index of the cell.
```javascript
cellColumn : number;
```
### cell {#cell--}
Readonly. Gets the Cell object which is being calculated.
```javascript
cell : Cell;
```
### setCalculatedValue(VObject) {#setCalculatedValue-vobject-}
Sets the calculated value for the cell.
```javascript
setCalculatedValue(v: VObject) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| v | VObject |  |
**Remarks**
User can set the calculated result by this method to ignore the automatic calculation for the cell.
