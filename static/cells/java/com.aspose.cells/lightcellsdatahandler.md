##LightCellsDataHandler
Represents cells data handler for reading large spreadsheet files in light weight mode.
```
public interface LightCellsDataHandler
```
Represents cells data handler for reading large spreadsheet files in light weight mode.
**Remarks**
When reading a workbook by this mode, [startSheet(Worksheet)](../../com.aspose.cells/lightcellsdatahandler\#startSheet-Worksheet-) will be checked when reading every worksheet in the workbook. For one sheet, if [startSheet(Worksheet)](../../com.aspose.cells/lightcellsdatahandler\#startSheet-Worksheet-) gives true, then all data and properties of rows/cells of this sheet will be checked and processed by the implementation of this interface. For every row, [startRow(int)](../../com.aspose.cells/lightcellsdatahandler\#startRow-int-) will be called to check whether it need to be processed. If a row needs to be processed, properties of this row will be read firstly and user can access its properties by [processRow(Row)](../../com.aspose.cells/lightcellsdatahandler\#processRow-Row-). if row's cells need to be processed too, then [processRow(Row)](../../com.aspose.cells/lightcellsdatahandler\#processRow-Row-) should returns true and then [startCell(int)](../../com.aspose.cells/lightcellsdatahandler\#startCell-int-) will be called for every existing cell in this row to check whether one cell need to be processed. If one cell needs to be processed, then [processCell(Cell)](../../com.aspose.cells/lightcellsdatahandler\#processCell-Cell-) will be called to process the cell by the implementation of this interface.
Please note, user should only operate on the values and properties of current Row/Cell object provided by corresponding method. Because the cells data is read from the template file in streaming manner, most of other objects may be reset/update later after cells data has been loaded. So when user operating other objects in this implementation, those operations may be not able to affect the objects existing in the workbook. Or even worse, those operations may cause inconsistent data in the workbook and then cause unpected issue or exception later. So, for all other objects such as shapes, column width and styles, conditional formattings, ...etc., please do not operate them in any methods of this implementation. Instead, please manage them after the workbook has been constructed.
## Methods
| Method | Description |
| --- | --- |
| [processCell(Cell cell)](#processCell-com.aspose.cells.Cell-) | Starts to process one cell. |
| [processRow(Row row)](#processRow-com.aspose.cells.Row-) | Starts to process one row. |
| [startCell(int columnIndex)](#startCell-int-) | Prepares to process a cell. |
| [startRow(int rowIndex)](#startRow-int-) | Prepares to process a row. |
| [startSheet(Worksheet sheet)](#startSheet-com.aspose.cells.Worksheet-) | Starts to process a worksheet. |
### processCell(Cell cell) {#processCell-com.aspose.cells.Cell-}
```
public abstract boolean processCell(Cell cell)
```
Starts to process one cell.
**Remarks**
It will be called after one cell's data has been read.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | Cell object which is being processed currently |
**Returns:**
boolean - whether this cell needs to be kept in cells model of current sheet. Commonly it should be false so that all cells will not be kept in memory after being processed and then memory be saved. For some special purpose such as user needs to access some cells later after the whole workbook having been processed, user can make this method return true to keep those special cells in Cells model and access them later by APIs such as Cells[row, column]. However, keeping cells data in Cells model will requires more memory and if all cells are kept then reading template file in LightCells mode will become same with reading it in normal way.
### processRow(Row row) {#processRow-com.aspose.cells.Row-}
```
public abstract boolean processRow(Row row)
```
Starts to process one row.
**Remarks**
It will be called after row's properties such as height, style, ...etc. have been read. However, cells in this row has not been read yet.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | [Row](../../com.aspose.cells/row) | Row object which is being processed currently. |
**Returns:**
boolean - whether this row's cells need to be processed. false to ignore all cells in this row.
### startCell(int columnIndex) {#startCell-int-}
```
public abstract boolean startCell(int columnIndex)
```
Prepares to process a cell.
**Remarks**
It will be called when reaching an existing cell in current row. Current row is the row of last call of [processRow(Row)](../../com.aspose.cells/lightcellsdatahandler\#processRow-Row-).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | int | column index of the cell to be processed |
**Returns:**
boolean - whether this cell needs to be processed. false to ignore the cell and check the next one until reach the end of cells data of current row
### startRow(int rowIndex) {#startRow-int-}
```
public abstract boolean startRow(int rowIndex)
```
Prepares to process a row.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | int | the index of next row to be processed |
**Returns:**
boolean - whether this row(properties or cells data) needs to be processed. false to ignore this row and its cells and check the next row.
### startSheet(Worksheet sheet) {#startSheet-com.aspose.cells.Worksheet-}
```
public abstract boolean startSheet(Worksheet sheet)
```
Starts to process a worksheet.
**Remarks**
It will be called before reading cells data of a worksheet.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheet | [Worksheet](../../com.aspose.cells/worksheet) | the worksheet to read cells data. |
**Returns:**
boolean - whether this sheet's cells data needs to be processed. false to ignore this sheet.
