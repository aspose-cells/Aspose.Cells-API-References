##TableStyle
Represents the table style.
## TableStyle class
Represents the table style.
```javascript
class TableStyle;
```
### Example
```javascript
const { Workbook, BackgroundType, Color, TableStyleElementType, CellsHelper, SaveFormat } = AsposeCells;
var workbook = new Workbook();
var firstColumnStyle = workbook.createStyle();
firstColumnStyle.pattern = BackgroundType.Solid;
firstColumnStyle.backgroundColor = Color.Red;
var lastColumnStyle = workbook.createStyle();
lastColumnStyle.font.isBold = true;
lastColumnStyle.pattern = BackgroundType.Solid;
lastColumnStyle.backgroundColor = Color.Red;
var tableStyleName = "Custom1";
var tableStyles = workbook.worksheets.getTableStyles();
var index1 = tableStyles.addTableStyle(tableStyleName);
var tableStyle = tableStyles.get(index1);
var elements = tableStyle.getTableStyleElements();
index1 = elements.add(TableStyleElementType.FirstColumn);
var element = elements.get(index1);
element.setElementStyle(firstColumnStyle);
index1 = elements.add(TableStyleElementType.LastColumn);
element = elements.get(index1);
element.setElementStyle(lastColumnStyle);
var cells = workbook.worksheets.get(0).cells;
for (var i = 0; i < 5; i++) {
cells.get(0, i).putValue(CellsHelper.columnIndexToName(i));
}
for (var row = 1; row < 10; row++) {
for (var column = 0; column < 5; column++) {
cells.get(row, column).putValue(row * column);
}
}
var tables = workbook.worksheets.get(0).getListObjects();
var index = tables.add(0, 0, 9, 4, true);
var table = tables.get(0);
table.showTableStyleFirstColumn = true;
table.showTableStyleLastColumn = true;
table.tableStyleName = tableStyleName;
var uint8Array = workbook.save(SaveFormat.Xlsx);
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [name](#name--)| string | Readonly. Gets the name of table style. |
| [tableStyleElements](#tableStyleElements--)| TableStyleElementCollection | Readonly. Gets all elements of the table style. |
### name {#name--}
Readonly. Gets the name of table style.
```javascript
name : string;
```
### tableStyleElements {#tableStyleElements--}
Readonly. Gets all elements of the table style.
```javascript
tableStyleElements : TableStyleElementCollection;
```
