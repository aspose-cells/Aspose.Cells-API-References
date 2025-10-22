##LightCellsDataProvider
Represents Data provider for saving large spreadsheet files in light weight mode.
## LightCellsDataProvider interface
Represents Data provider for saving large spreadsheet files in light weight mode.
### Remarks
When saving a workbook by this mode, [StartSheet(int)](../startsheet(int)/) will be checked when saving every worksheet in the workbook. For one sheet, if [StartSheet(int)](../startsheet(int)/) gives true, then all data and properties to be saved for rows/cells of this sheet will be provided by the implementation of this interface. In the first place, [NextRow()](../nextrow()/) will be called to get the next row index to be saved. If a valid row index is returned(the row index must be in ascending order for the rows to be saved), then a Row object representing this row will be provided by [StartRow(Row)](../startrow(row)/) for the implementation to set its properties. For one row, [NextCell()](../nextcell()/) will be checked firstly. If a valid column index be returned(the column index must be in ascending order for all cells of current row), then a Cell object representing this cell will be provided by [StartCell(Cell)](../startcell(cell)/) for implementation to set its data and properties. After [StartCell(Cell)](../startcell(cell)/) the cell will be saved directly to the resultant spreadsheet file. Then the next cell will be checked and processed. <br></br> Please note, user should only update values and properties for current Row/Cell object provided by corresponding method. Because the cells data is written to the resultant file in streaming manner, most of other objects may have been written to the resultant file, or have been gathered and written some global data for them. So when user updating other objects while saving cells data, those operations may be not able to affect the saved data. Or even worse, those operations may cause inconsistent data be save to the resultant file and finally make the file corrupted. So, for all other objects such as shapes, column width and styles, conditional formattings, ...etc., please do not operate them in any methods of this implementation. Instead, please manage them and adjust them to the final state before calling "Save" method of the Workbook.
## Methods
| Method | Description |
| --- | --- |
| [startSheet(number)](#startSheet-number-)| Starts to save a worksheet. |
| [nextRow()](#nextRow--)| Gets the next row to be saved. |
| [startRow(Row)](#startRow-row-)| Starts to save data of one row. |
| [nextCell()](#nextCell--)| Gets next cell to be saved. |
| [startCell(Cell)](#startCell-cell-)| Starts to save data of one cell. |
| [isGatherString()](#isGatherString--)| Checks whether the current string value of cell needs to be gathered into a global pool. |
### startSheet(number) {#startSheet-number-}
Starts to save a worksheet.
```javascript
startSheet(sheetIndex: number) : boolean;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | number | index of current sheet to be saved. |
**Returns**
true if this provider will provide data for the given sheet; false if given sheet should use its normal data model(Cells).
**Remarks**
It will be called at the beginning of saving a worksheet during saving a workbook. If the provider needs to refer to <i><code>sheetIndex</code></i> later in startRow(Row) or startCell(Cell) method, that is, if the process needs to know which worksheet is being processed, the implementation should retain the <i><code>sheetIndex</code></i> value here.
### nextRow() {#nextRow--}
Gets the next row to be saved.
```javascript
nextRow() : number;
```
**Returns**
the next row index to be saved. -1 means the end of current sheet data has been reached and no further row of current sheet to be saved.
**Remarks**
It will be called at the beginning of saving a row and its cells data(before [StartRow(Row)](../startrow(row)/)).
### startRow(Row) {#startRow-row-}
Starts to save data of one row.
```javascript
startRow(row: Row) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | [Row](../row/) | Row object for implementation to fill data. Its row index is the returned value of latest call of [NextRow()](../nextrow()/).         /// If the row has been initialized in the inner cells model, the existing row object will be used.         /// Otherwise a temporary Row object will be used for implementation to fill data. |
**Remarks**
It will be called at the beginning of saving a row and its cells data. If current row has some custom properties such as height, style, ...etc., implementation should set those properties to given Row object here.
### nextCell() {#nextCell--}
Gets next cell to be saved.
```javascript
nextCell() : number;
```
**Returns**
column index of the next cell to be saved. -1 means the end of current row data has been reached and no further cell of current row to be saved.
**Remarks**
It will be called at the beginning of saving one cell.
### startCell(Cell) {#startCell-cell-}
Starts to save data of one cell.
```javascript
startCell(cell: Cell) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cell | [Cell](../cell/) | Cell object for implementation to fill data. Its column index is the returned value of latest call of [NextCell()](../nextcell()/).         /// If the cell has been initialized in the inner cells model, the existed cell object will be used.         /// Otherwise a temporary Cell object will be used for implementation to fill data. |
### isGatherString() {#isGatherString--}
Checks whether the current string value of cell needs to be gathered into a global pool.
```javascript
isGatherString() : boolean;
```
**Returns**
true if string value need to be gathered into a global pool for the resultant file.
**Remarks**
Gathering string values will take advantage only when there are many duplicated string values for the cells provided by this implementation. In this situation gathering string will save much memory and generate smaller resultant file. If there are many string values for the cells provided by LightCellsDataProvider but few of them are same, gathering string will cost more memory and time and has no advantage for the resultant file.
