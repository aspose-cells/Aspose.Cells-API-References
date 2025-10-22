##LightCellsDataHandler
Represents cells data handler for reading large spreadsheet files in light weight mode.
## LightCellsDataHandler interface
Represents cells data handler for reading large spreadsheet files in light weight mode.
### Remarks
When reading a workbook by this mode, [StartSheet(Worksheet)](../startsheet(worksheet)/) will be checked when reading every worksheet in the workbook. For one sheet, if [StartSheet(Worksheet)](../startsheet(worksheet)/) gives true, then all data and properties of rows/cells of this sheet will be checked and processed by the implementation of this interface. For every row, [StartRow(int)](../startrow(int)/) will be called to check whether it need to be processed. If a row needs to be processed, properties of this row will be read firstly and user can access its properties by [ProcessRow(Row)](../processrow(row)/). if row's cells need to be processed too, then [ProcessRow(Row)](../processrow(row)/) should returns true and then [StartCell(int)](../startcell(int)/) will be called for every existing cell in this row to check whether one cell need to be processed. If one cell needs to be processed, then [ProcessCell(Cell)](../processcell(cell)/) will be called to process the cell by the implementation of this interface. <br></br> Please note, user should only operate on the values and properties of current Row/Cell object provided by corresponding method. Because the cells data is read from the template file in streaming manner, most of other objects may be reset/update later after cells data has been loaded. So when user operating other objects in this implementation, those operations may be not able to affect the objects existing in the workbook. Or even worse, those operations may cause inconsistent data in the workbook and then cause unpected issue or exception later. So, for all other objects such as shapes, column width and styles, conditional formattings, ...etc., please do not operate them in any methods of this implementation. Instead, please manage them after the workbook has been constructed.
## Methods
| Method | Description |
| --- | --- |
| [startSheet(Worksheet)](#startSheet-worksheet-)| Starts to process a worksheet. |
| [startRow(number)](#startRow-number-)| Prepares to process a row. |
| [processRow(Row)](#processRow-row-)| Starts to process one row. |
| [startCell(number)](#startCell-number-)| Prepares to process a cell. |
| [processCell(Cell)](#processCell-cell-)| Starts to process one cell. |
### startSheet(Worksheet) {#startSheet-worksheet-}
Starts to process a worksheet.
```javascript
startSheet(sheet: Worksheet) : boolean;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheet | [Worksheet](../worksheet/) | the worksheet to read cells data. |
**Returns**
whether this sheet's cells data needs to be processed. false to ignore this sheet.
**Remarks**
It will be called before reading cells data of a worksheet.
### startRow(number) {#startRow-number-}
Prepares to process a row.
```javascript
startRow(rowIndex: number) : boolean;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | number | the index of next row to be processed |
**Returns**
whether this row(properties or cells data) needs to be processed. false to ignore this row and its cells and check the next row.
### processRow(Row) {#processRow-row-}
Starts to process one row.
```javascript
processRow(row: Row) : boolean;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | [Row](../row/) | Row object which is being processed currently. |
**Returns**
whether this row's cells need to be processed. false to ignore all cells in this row.
**Remarks**
It will be called after row's properties such as height, style, ...etc. have been read. However, cells in this row has not been read yet.
### startCell(number) {#startCell-number-}
Prepares to process a cell.
```javascript
startCell(columnIndex: number) : boolean;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | number | column index of the cell to be processed |
**Returns**
whether this cell needs to be processed. false to ignore the cell and check the next one until reach the end of cells data of current row
**Remarks**
It will be called when reaching an existing cell in current row. Current row is the row of last call of [ProcessRow(Row)](../processrow(row)/).
### processCell(Cell) {#processCell-cell-}
Starts to process one cell.
```javascript
processCell(cell: Cell) : boolean;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cell | [Cell](../cell/) | Cell object which is being processed currently |
**Returns**
whether this cell needs to be kept in cells model of current sheet. Commonly it should be false so that all cells will not be kept in memory after being processed and then memory be saved. For some special purpose such as user needs to access some cells later after the whole workbook having been processed, user can make this method return true to keep those special cells in Cells model and access them later by APIs such as Cells[row, column]. However, keeping cells data in Cells model will requires more memory and if all cells are kept then reading template file in LightCells mode will become same with reading it in normal way.
**Remarks**
It will be called after one cell's data has been read.
