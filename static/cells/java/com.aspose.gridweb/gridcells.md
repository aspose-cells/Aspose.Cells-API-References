##GridCells
Encapsulates a collection of  objects.
**Inheritance:**
java.lang.Object
**All Implemented Interfaces:**
java.lang.Iterable
```
public class GridCells implements Iterable
```
Encapsulates a collection of [GridCell](../../com.aspose.gridweb/gridcell) objects.
## Methods
| Method | Description |
| --- | --- |
| [cellIndexToName(int row, int column)](#cellIndexToName-int-int-) | Gets cell name according to its row and column indexes. |
| [cellNameToIndex(String cellName, int row, int column)](#cellNameToIndex-java.lang.String-int-int-) | Gets the cell row and column indexes according to its name |
| [checkCell(int row, int column)](#checkCell-int-int-) | Gets the [GridCell](../../com.aspose.gridweb/gridcell) element or null at the specified cell row index and column index. |
| [checkColumn(int col)](#checkColumn-int-) | Gets the [GridColumn](../../com.aspose.gridweb/gridcolumn) element or null at the specified column index. |
| [checkRow(int i)](#checkRow-int-) | Gets the [GridRow](../../com.aspose.gridweb/gridrow) element or null at the specified cell row index. |
| [clear()](#clear--) | Clear all cells in the collection. |
| [clearContents(GridCellArea range)](#clearContents-com.aspose.gridweb.GridCellArea-) | Clears contents of a range. |
| [clearContents(int startRow, int startColumn, int endRow, int endColumn)](#clearContents-int-int-int-int-) | Clears contents of a range. |
| [clearFormats(GridCellArea range)](#clearFormats-com.aspose.gridweb.GridCellArea-) | Clears formatting of a range. |
| [clearFormats(int startRow, int startColumn, int endRow, int endColumn)](#clearFormats-int-int-int-int-) | Clears formatting of a range. |
| [clearRange(GridCellArea range)](#clearRange-com.aspose.gridweb.GridCellArea-) | Clears contents and formatting of a range. |
| [clearRange(int startRow, int startColumn, int endRow, int endColumn)](#clearRange-int-int-int-int-) | Clears contents and formatting of a range. |
| [columnIndexToName(int column)](#columnIndexToName-int-) | Gets column name according to column index. |
| [columnNameToIndex(String columnName)](#columnNameToIndex-java.lang.String-) | Gets column index according to column name. |
| [copyColumn(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex)](#copyColumn-com.aspose.gridweb.GridCells-int-int-) | Copies data and formattings of a whole column. |
| [copyColumns(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber)](#copyColumns-com.aspose.gridweb.GridCells-int-int-int-) | Copies data and formattings of a whole column. |
| [copyRow(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex)](#copyRow-com.aspose.gridweb.GridCells-int-int-) | Copies data and formattings of a whole row. |
| [copyRows(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)](#copyRows-com.aspose.gridweb.GridCells-int-int-int-) | Copies data and formattings of some whole rows. |
| [deleteBlankColumns()](#deleteBlankColumns--) | Delete all blank columns which do not contain any data. |
| [deleteBlankRows()](#deleteBlankRows--) | Delete all blank rows which do not contain any data. |
| [deleteColumn(int columnIndex)](#deleteColumn-int-) | Deletes a column. |
| [deleteColumn(int columnIndex, boolean updateReference)](#deleteColumn-int-boolean-) | Deletes a column. |
| [deleteColumns(int columnIndex, int totalColumns, boolean updateReference)](#deleteColumns-int-int-boolean-) | Deletes several columns. |
| [deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType)](#deleteRange-int-int-int-int-int-) | Deletes a range of cells and shift cells according to the shift option. |
| [deleteRow(int rowIndex)](#deleteRow-int-) | Deletes a row. |
| [deleteRows(int rowIndex, int totalRows)](#deleteRows-int-int-) | Deletes several rows. |
| [deleteRows(int rowIndex, int totalRows, boolean updateReference)](#deleteRows-int-int-boolean-) | Deletes multiple rows in the worksheet. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)](#exportArray-int-int-int-int-) | Exports data in the [GridCells](../../com.aspose.gridweb/gridcells) collection to a two-dimension array object. |
| [get(int row, int column)](#get-int-int-) | Gets the [GridCell](../../com.aspose.gridweb/gridcell) element at the specified cell row index and column index. |
| [get(String cellName)](#get-java.lang.String-) | Gets the [GridCell](../../com.aspose.gridweb/gridcell) element at the specified cell name. |
| [getCell(int row, int column)](#getCell-int-int-) | Gets the [GridCell](../../com.aspose.gridweb/gridcell) element at the specified cell row index and column index. |
| [getClass()](#getClass--) |  |
| [getColumnWidth(int column)](#getColumnWidth-int-) | Gets the width of the specified column |
| [getColumnWidthInch(int column)](#getColumnWidthInch-int-) | Gets the width of the specified column, in units of inches. |
| [getColumnWidthPixel(int column)](#getColumnWidthPixel-int-) | Gets the width of the specified column, in units of pixel. |
| [getColumns()](#getColumns--) | Gets the collection of [GridColumn](../../com.aspose.gridweb/gridcolumn) objects that represents the individual columns in this worksheet. |
| [getCount()](#getCount--) | Gets the number of cells. |
| [getFirstCell()](#getFirstCell--) | Gets the first cell in this worksheet. |
| [getLastCell()](#getLastCell--) | Gets the last cell in this worksheet. |
| [getMaxColumn()](#getMaxColumn--) | Maximum column index of cell which contains data or style. |
| [getMaxDataColumn()](#getMaxDataColumn--) | Maximum column index of cell which contains data. |
| [getMaxDataRow()](#getMaxDataRow--) | Maximum row index of cell which contains data. |
| [getMaxRow()](#getMaxRow--) | Maximum row index of cell which contains data or style. |
| [getMergedCells()](#getMergedCells--) | Gets the collection of merged cells. |
| [getMinColumn()](#getMinColumn--) | Minimum column index of those cells that have been instantiated in the collection(does not include the column where style is defined for the whole column but no cell has been instantiated in it). |
| [getMinDataColumn()](#getMinDataColumn--) | Minimum column index of cell which contains data. |
| [getMinDataRow()](#getMinDataRow--) | Minimum row index of cell which contains data. |
| [getMinRow()](#getMinRow--) | Minimum row index of cell which contains data or style. |
| [getRow(int i)](#getRow-int-) | Gets the [GridRow](../../com.aspose.gridweb/gridrow) element or at the specified cell row index. |
| [getRowEnumerator()](#getRowEnumerator--) | Gets the rows enumerator |
| [getRowHeight(int row)](#getRowHeight-int-) | Gets the height of a specified row. |
| [getRowHeightInch(int row)](#getRowHeightInch-int-) | Gets the height of a specified row in unit of inches. |
| [getRowHeightPixel(int row)](#getRowHeightPixel-int-) | Gets the height of a specified row in unit of pixel. |
| [getRowOutlineLevel(int rowIndex)](#getRowOutlineLevel-int-) | Gets the outline level of the row. |
| [getRows()](#getRows--) | Gets the collection of [GridRow](../../com.aspose.gridweb/gridrow) objects that represents the individual rows in this worksheet. |
| [getStandardHeight()](#getStandardHeight--) | Gets the default row height in this worksheet,in unit of points. |
| [getStandardHeightPixels()](#getStandardHeightPixels--) | Gets the default row height in this worksheet,in unit of pixels. |
| [getStandardWidth()](#getStandardWidth--) | Gets the default column width in the worksheet,in unit of characters. |
| [getStandardWidthInch()](#getStandardWidthInch--) | Gets the default column width in the worksheet, in unit of inches. |
| [getStandardWidthPixels()](#getStandardWidthPixels--) | Gets the default column width in the worksheet, in unit of pixels. |
| [getViewColumnWidthPixel(int column)](#getViewColumnWidthPixel-int-) | Get the width in different view type. |
| [groupColumns(int firstIndex, int lastIndex)](#groupColumns-int-int-) | Groups columns. |
| [groupColumns(int firstIndex, int lastIndex, boolean isHidden)](#groupColumns-int-int-boolean-) | Groups columns. |
| [groupRows(int firstIndex, int lastIndex)](#groupRows-int-int-) | Groups rows. |
| [hashCode()](#hashCode--) |  |
| [hideColumn(int column)](#hideColumn-int-) | Hides a column. |
| [hideRow(int row)](#hideRow-int-) | Hides a row. |
| [insertColumn(int columnIndex)](#insertColumn-int-) | Inserts a new column into the worksheet. |
| [insertColumn(int columnIndex, boolean updateReference)](#insertColumn-int-boolean-) | Inserts a new column into the worksheet. |
| [insertColumns(int columnIndex, int totalColumns)](#insertColumns-int-int-) | Inserts some columns into the worksheet. |
| [insertColumns(int columnIndex, int totalColumns, boolean updateReference)](#insertColumns-int-int-boolean-) | Inserts some columns into the worksheet. |
| [insertRange(GridCellArea area, int shiftType)](#insertRange-com.aspose.gridweb.GridCellArea-int-) | Inserts a range of cells and shift cells according to the shift option. |
| [insertRange(GridCellArea area, int shiftNumber, int shiftType, boolean updateReference)](#insertRange-com.aspose.gridweb.GridCellArea-int-int-boolean-) | Inserts a range of cells and shift cells according to the shift option. |
| [insertRow(int rowIndex)](#insertRow-int-) | Inserts a new row into the worksheet. |
| [insertRows(int rowIndex, int totalRows)](#insertRows-int-int-) | Inserts multiple rows into the worksheet. |
| [insertRows(int rowIndex, int totalRows, boolean updateReference)](#insertRows-int-int-boolean-) | Inserts multiple rows into the worksheet. |
| [isBlankColumn(int columnIndex)](#isBlankColumn-int-) | Checks whether given column is blank(does not contain any data). |
| [isColumnHidden(int columnIndex)](#isColumnHidden-int-) | Checks whether a column at given index is hidden. |
| [isRowHidden(int rowIndex)](#isRowHidden-int-) | Checks whether a row at given index is hidden. |
| [iterator()](#iterator--) | Gets the rows enumerator |
| [merge(int firstRow, int firstColumn, int totalRows, int totalColumns)](#merge-int-int-int-int-) | Merges a specified range of cells into a single cell. |
| [moveRange(GridCellArea sourceArea, int destRow, int destColumn)](#moveRange-com.aspose.gridweb.GridCellArea-int-int-) | Moves the range. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeDuplicates(int startRow, int startColumn, int endRow, int endColumn)](#removeDuplicates-int-int-int-int-) | Remove duplicate values in the range. |
| [removeFormulas()](#removeFormulas--) | Removes all formula and replaces with the value of the formula. |
| [setBorders(int firstRow, int firstColumn, int rowNumber, int columnNumber, int position, WebBorderStyle borderStyle)](#setBorders-int-int-int-int-int-com.aspose.gridweb.WebBorderStyle-) | Sets borders for a cells range. |
| [setColumnWidth(int column, double width)](#setColumnWidth-int-double-) | Sets the width of the specified column. |
| [setColumnWidthInch(int column, double inches)](#setColumnWidthInch-int-double-) | Sets column width in unit of inches. |
| [setColumnWidthPixel(int column, int pixel)](#setColumnWidthPixel-int-int-) | Sets column width in unit of pixels. |
| [setRowHeight(int row, double height)](#setRowHeight-int-double-) | Sets the height of the specified row. |
| [setRowHeightInch(int row, double inches)](#setRowHeightInch-int-double-) | Sets row height in unit of inches. |
| [setRowHeightPixel(int row, int pixels)](#setRowHeightPixel-int-int-) | Sets row height in unit of pixels. |
| [setRowOutlineLevel(int rowIndex, int outlineLevel)](#setRowOutlineLevel-int-int-) | Sets the outline level of the row. |
| [setStandardHeight(double value)](#setStandardHeight-double-) | Sets the default row height in this worksheet,in unit of points. |
| [setStandardHeightPixels(int value)](#setStandardHeightPixels-int-) | Sets the default row height in this worksheet,in unit of pixels. |
| [setStandardWidth(double value)](#setStandardWidth-double-) | Sets the default column width in the worksheet,in unit of characters. |
| [setStandardWidthInch(double value)](#setStandardWidthInch-double-) | Sets the default column width in the worksheet, in unit of inches. |
| [setStandardWidthPixels(int value)](#setStandardWidthPixels-int-) | Sets the default column width in the worksheet, in unit of pixels. |
| [setStyle(int firstRow, int firstColumn, int rowNumber, int columnNumber, GridTableItemStyle style)](#setStyle-int-int-int-int-com.aspose.gridweb.GridTableItemStyle-) | Sets the style to a specified range of cells. |
| [setStyle(String cellRange, GridTableItemStyle style)](#setStyle-java.lang.String-com.aspose.gridweb.GridTableItemStyle-) | Sets the style to a specified range of cells. |
| [sort(int startRow, int startColumn, int rows, int columns, int index, boolean isAsending, boolean isCaseSensitive, boolean islefttoright)](#sort-int-int-int-int-int-boolean-boolean-boolean-) | Sorts the datas ascend/decend top to bottom in a range of a Worksheet by specified column index. |
| [sort(int startRow, int startColumn, int rows, int columns, int[] indexes, int[] orders, int orientation, boolean isCaseSensitive)](#sort-int-int-int-int-int---int---int-boolean-) | Sorts the datas ascend/decend top to bottom in a range of a Worksheet by specified column index. |
| [toString()](#toString--) |  |
| [unMerge(int firstRow, int firstColumn, int totalRows, int totalColumns)](#unMerge-int-int-int-int-) | Unmerges a specified range of merged cells. |
| [ungroupColumns(int firstIndex, int lastIndex)](#ungroupColumns-int-int-) | Ungroups columns. |
| [ungroupRows(int firstIndex, int lastIndex)](#ungroupRows-int-int-) | Ungroups rows. |
| [unhideColumn(int column, double width)](#unhideColumn-int-double-) | Unhides a column |
| [unhideRow(int row)](#unhideRow-int-) | Unhides a row. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### cellIndexToName(int row, int column) {#cellIndexToName-int-int-}
```
public static String cellIndexToName(int row, int column)
```
Gets cell name according to its row and column indexes.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Row index. |
| column | int | Column index. |
**Returns:**
java.lang.String - Name of cell.
### cellNameToIndex(String cellName, int row, int column) {#cellNameToIndex-java.lang.String-int-int-}
```
public static void cellNameToIndex(String cellName, int row, int column)
```
Gets the cell row and column indexes according to its name
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | java.lang.String | Name of cell. |
| row | int | Output row index |
| column | int | Output column index |
### checkCell(int row, int column) {#checkCell-int-int-}
```
public GridCell checkCell(int row, int column)
```
Gets the [GridCell](../../com.aspose.gridweb/gridcell) element or null at the specified cell row index and column index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Row index |
| column | int | Column index |
**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - Return GridCell object if a GridCell object exists. Return null if the GridCell does not exist.
### checkColumn(int col) {#checkColumn-int-}
```
public GridColumn checkColumn(int col)
```
Gets the [GridColumn](../../com.aspose.gridweb/gridcolumn) element or null at the specified column index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| col | int | The column index. |
**Returns:**
[GridColumn](../../com.aspose.gridweb/gridcolumn) - The Column object.
### checkRow(int i) {#checkRow-int-}
```
public GridRow checkRow(int i)
```
Gets the [GridRow](../../com.aspose.gridweb/gridrow) element or null at the specified cell row index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| i | int | Row index |
**Returns:**
[GridRow](../../com.aspose.gridweb/gridrow) - Returns [GridRow](../../com.aspose.gridweb/gridrow) object If the row object does exist, otherwise returns null.
### clear() {#clear--}
```
public void clear()
```
Clear all cells in the collection.
### clearContents(GridCellArea range) {#clearContents-com.aspose.gridweb.GridCellArea-}
```
public void clearContents(GridCellArea range)
```
Clears contents of a range.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| range | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Range to be cleared. |
### clearContents(int startRow, int startColumn, int endRow, int endColumn) {#clearContents-int-int-int-int-}
```
public void clearContents(int startRow, int startColumn, int endRow, int endColumn)
```
Clears contents of a range.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | int | Start row index. |
| startColumn | int | Start column index. |
| endRow | int | End row index. |
| endColumn | int | End column index. |
### clearFormats(GridCellArea range) {#clearFormats-com.aspose.gridweb.GridCellArea-}
```
public void clearFormats(GridCellArea range)
```
Clears formatting of a range.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| range | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Range to be cleared. |
### clearFormats(int startRow, int startColumn, int endRow, int endColumn) {#clearFormats-int-int-int-int-}
```
public void clearFormats(int startRow, int startColumn, int endRow, int endColumn)
```
Clears formatting of a range.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | int | Start row index. |
| startColumn | int | Start column index. |
| endRow | int | End row index. |
| endColumn | int | End column index. |
### clearRange(GridCellArea range) {#clearRange-com.aspose.gridweb.GridCellArea-}
```
public void clearRange(GridCellArea range)
```
Clears contents and formatting of a range.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| range | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Range to be cleared. |
### clearRange(int startRow, int startColumn, int endRow, int endColumn) {#clearRange-int-int-int-int-}
```
public void clearRange(int startRow, int startColumn, int endRow, int endColumn)
```
Clears contents and formatting of a range.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | int | Start row index. |
| startColumn | int | Start column index. |
| endRow | int | End row index. |
| endColumn | int | End column index. |
### columnIndexToName(int column) {#columnIndexToName-int-}
```
public static String columnIndexToName(int column)
```
Gets column name according to column index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | int | Column index. |
**Returns:**
java.lang.String - Name of column.
### columnNameToIndex(String columnName) {#columnNameToIndex-java.lang.String-}
```
public static int columnNameToIndex(String columnName)
```
Gets column index according to column name.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnName | java.lang.String | Column name. |
**Returns:**
int - Column index.
### copyColumn(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex) {#copyColumn-com.aspose.gridweb.GridCells-int-int-}
```
public void copyColumn(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex)
```
Copies data and formattings of a whole column.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells | [GridCells](../../com.aspose.gridweb/gridcells) | Source Cells object contains data and formattings to copy. |
| sourceColumnIndex | int | Source column index. |
| destinationColumnIndex | int | Destination column index. |
### copyColumns(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber) {#copyColumns-com.aspose.gridweb.GridCells-int-int-int-}
```
public void copyColumns(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber)
```
Copies data and formattings of a whole column.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells | [GridCells](../../com.aspose.gridweb/gridcells) | Source Cells object contains data and formattings to copy. |
| sourceColumnIndex | int | Source column index. |
| destinationColumnIndex | int | Destination column index. |
| columnNumber | int | The copied column number. |
### copyRow(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex) {#copyRow-com.aspose.gridweb.GridCells-int-int-}
```
public void copyRow(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex)
```
Copies data and formattings of a whole row.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells | [GridCells](../../com.aspose.gridweb/gridcells) | Source Cells object contains data and formattings to copy. |
| sourceRowIndex | int | Source row index. |
| destinationRowIndex | int | Destination row index. |
### copyRows(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber) {#copyRows-com.aspose.gridweb.GridCells-int-int-int-}
```
public void copyRows(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)
```
Copies data and formattings of some whole rows.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells | [GridCells](../../com.aspose.gridweb/gridcells) | Source Cells object contains data and formattings to copy. |
| sourceRowIndex | int | Source row index. |
| destinationRowIndex | int | Destination row index. |
| rowNumber | int | The copied row number. |
### deleteBlankColumns() {#deleteBlankColumns--}
```
public void deleteBlankColumns()
```
Delete all blank columns which do not contain any data.
### deleteBlankRows() {#deleteBlankRows--}
```
public void deleteBlankRows()
```
Delete all blank rows which do not contain any data.
### deleteColumn(int columnIndex) {#deleteColumn-int-}
```
public void deleteColumn(int columnIndex)
```
Deletes a column.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | int | Column index. |
### deleteColumn(int columnIndex, boolean updateReference) {#deleteColumn-int-boolean-}
```
public void deleteColumn(int columnIndex, boolean updateReference)
```
Deletes a column.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | int | Column index. |
| updateReference | boolean | Indicates if update references in other worksheets. |
### deleteColumns(int columnIndex, int totalColumns, boolean updateReference) {#deleteColumns-int-int-boolean-}
```
public void deleteColumns(int columnIndex, int totalColumns, boolean updateReference)
```
Deletes several columns.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | int | Column index. |
| totalColumns | int | Number of columns to be deleted. |
| updateReference | boolean | Indicates if update references in other worksheets. |
### deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType) {#deleteRange-int-int-int-int-int-}
```
public void deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType)
```
Deletes a range of cells and shift cells according to the shift option.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | int | Start row index. |
| startColumn | int | Start column index. |
| endRow | int | End row index. |
| endColumn | int | End column index. |
| shiftType | int | [GridShiftType](../../com.aspose.gridweb/gridshifttype). Shift cells option. |
### deleteRow(int rowIndex) {#deleteRow-int-}
```
public void deleteRow(int rowIndex)
```
Deletes a row.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | int | Row index. |
### deleteRows(int rowIndex, int totalRows) {#deleteRows-int-int-}
```
public boolean deleteRows(int rowIndex, int totalRows)
```
Deletes several rows.
**Remarks**
If the deleted range contains the top part(not whole) of the table(ListObject), the ranged could not be deleted and nothing will be done.It works as MS Excel.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | int | The first row index to be deleted. |
| totalRows | int | Number of rows to be deleted. |
**Returns:**
boolean
### deleteRows(int rowIndex, int totalRows, boolean updateReference) {#deleteRows-int-int-boolean-}
```
public boolean deleteRows(int rowIndex, int totalRows, boolean updateReference)
```
Deletes multiple rows in the worksheet.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | int | Row index. |
| totalRows | int | Number of rows to be deleted. |
| updateReference | boolean | Indicates if update references in other worksheets. |
**Returns:**
boolean -
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |
**Returns:**
boolean
### exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns) {#exportArray-int-int-int-int-}
```
public Object[][] exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)
```
Exports data in the [GridCells](../../com.aspose.gridweb/gridcells) collection to a two-dimension array object.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | int | The row number of the first cell to export out. |
| firstColumn | int | The column number of the first cell to export out. |
| totalRows | int | Number of rows to be exported |
| totalColumns | int | Number of columns to be exported |
**Returns:**
java.lang.Object[][] - Exported cell value array object.
### get(int row, int column) {#get-int-int-}
```
public GridCell get(int row, int column)
```
Gets the [GridCell](../../com.aspose.gridweb/gridcell) element at the specified cell row index and column index.
**Example**
```
GridWeb GridWeb1 = new GridWeb();
GridCells cells = GridWeb1.getWorkSheets().get(0).getCells();
//Gets the cell at "A1"
GridCell cell = cells.get(0, 0);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Row index. |
| column | int | Column index. |
**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - The [GridCell](../../com.aspose.gridweb/gridcell) object.
### get(String cellName) {#get-java.lang.String-}
```
public GridCell get(String cellName)
```
Gets the [GridCell](../../com.aspose.gridweb/gridcell) element at the specified cell name.
**Example**
```
GridWeb GridWeb1 = new GridWeb();
GridCells cells = GridWeb1.getWorkSheets().get(0).getCells();
GridCell cell = cells.get("A1");	//Gets the cell at "A1"
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | java.lang.String | Cell name,including its column letter and row number, for example A5. |
**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - A [GridCell](../../com.aspose.gridweb/gridcell) object
### getCell(int row, int column) {#getCell-int-int-}
```
public GridCell getCell(int row, int column)
```
Gets the [GridCell](../../com.aspose.gridweb/gridcell) element at the specified cell row index and column index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Row index |
| column | int | Column index |
**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - Return Cell object
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getColumnWidth(int column) {#getColumnWidth-int-}
```
public double getColumnWidth(int column)
```
Gets the width of the specified column
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | int | Column index |
**Returns:**
double - Width of column
### getColumnWidthInch(int column) {#getColumnWidthInch-int-}
```
public double getColumnWidthInch(int column)
```
Gets the width of the specified column, in units of inches.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | int | Column index |
**Returns:**
double - Width of column
### getColumnWidthPixel(int column) {#getColumnWidthPixel-int-}
```
public int getColumnWidthPixel(int column)
```
Gets the width of the specified column, in units of pixel.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | int | Column index |
**Returns:**
int - Width of column in normal view.
### getColumns() {#getColumns--}
```
public GridColumnCollection getColumns()
```
Gets the collection of [GridColumn](../../com.aspose.gridweb/gridcolumn) objects that represents the individual columns in this worksheet.
**Returns:**
[GridColumnCollection](../../com.aspose.gridweb/gridcolumncollection)
### getCount() {#getCount--}
```
public int getCount()
```
Gets the number of cells.
**Returns:**
int
### getFirstCell() {#getFirstCell--}
```
public GridCell getFirstCell()
```
Gets the first cell in this worksheet.
**Remarks**
Returns null if there is no data in the worksheet.
**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getLastCell() {#getLastCell--}
```
public GridCell getLastCell()
```
Gets the last cell in this worksheet.
**Remarks**
Returns null if there is no data in the worksheet.
**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getMaxColumn() {#getMaxColumn--}
```
public int getMaxColumn()
```
Maximum column index of cell which contains data or style.
**Remarks**
Return -1 if ther is not cell.
**Returns:**
int
### getMaxDataColumn() {#getMaxDataColumn--}
```
public int getMaxDataColumn()
```
Maximum column index of cell which contains data.
**Remarks**
\-1 will be returned if there is no cell which contains data. This property needs to iterate and check all cells in a worksheet, so it is a time-consumed progress and should not be invoked repeatedly.
**Returns:**
int
### getMaxDataRow() {#getMaxDataRow--}
```
public int getMaxDataRow()
```
Maximum row index of cell which contains data.
**Remarks**
Return -1 if there is no cell which contains data.
**Returns:**
int
### getMaxRow() {#getMaxRow--}
```
public int getMaxRow()
```
Maximum row index of cell which contains data or style.
**Remarks**
Return -1 if there is no cell whiche contains data or style in the worksheet.
**Returns:**
int
### getMergedCells() {#getMergedCells--}
```
public ArrayList getMergedCells()
```
Gets the collection of merged cells.
**Remarks**
In this collection, each item is a [GridCellArea](../../com.aspose.gridweb/gridcellarea) structure which represents an area of merged cells.
**Returns:**
java.util.ArrayList
### getMinColumn() {#getMinColumn--}
```
public int getMinColumn()
```
Minimum column index of those cells that have been instantiated in the collection(does not include the column where style is defined for the whole column but no cell has been instantiated in it).
**Returns:**
int
### getMinDataColumn() {#getMinDataColumn--}
```
public int getMinDataColumn()
```
Minimum column index of cell which contains data.
**Remarks**
\-1 will be returned if there is no cell which contains data. This property needs to iterate and check all cells in a worksheet, so it is a time-consumed progress and should not be invoked repeatedly.
**Returns:**
int
### getMinDataRow() {#getMinDataRow--}
```
public int getMinDataRow()
```
Minimum row index of cell which contains data.
**Returns:**
int
### getMinRow() {#getMinRow--}
```
public int getMinRow()
```
Minimum row index of cell which contains data or style.
**Returns:**
int
### getRow(int i) {#getRow-int-}
```
public GridRow getRow(int i)
```
Gets the [GridRow](../../com.aspose.gridweb/gridrow) element or at the specified cell row index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| i | int | Row index |
**Returns:**
[GridRow](../../com.aspose.gridweb/gridrow) - the row object
### getRowEnumerator() {#getRowEnumerator--}
```
public Iterator getRowEnumerator()
```
Gets the rows enumerator
**Returns:**
java.util.Iterator - The rows enuerator.
### getRowHeight(int row) {#getRowHeight-int-}
```
public double getRowHeight(int row)
```
Gets the height of a specified row.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Row index |
**Returns:**
double - Height of row
### getRowHeightInch(int row) {#getRowHeightInch-int-}
```
public double getRowHeightInch(int row)
```
Gets the height of a specified row in unit of inches.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Row index |
**Returns:**
double - Height of row
### getRowHeightPixel(int row) {#getRowHeightPixel-int-}
```
public int getRowHeightPixel(int row)
```
Gets the height of a specified row in unit of pixel.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Row index |
**Returns:**
int - Height of row
### getRowOutlineLevel(int rowIndex) {#getRowOutlineLevel-int-}
```
public int getRowOutlineLevel(int rowIndex)
```
Gets the outline level of the row.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | int | row index. |
**Returns:**
int - the outline level.
### getRows() {#getRows--}
```
public GridRowCollection getRows()
```
Gets the collection of [GridRow](../../com.aspose.gridweb/gridrow) objects that represents the individual rows in this worksheet.
**Returns:**
[GridRowCollection](../../com.aspose.gridweb/gridrowcollection)
### getStandardHeight() {#getStandardHeight--}
```
public double getStandardHeight()
```
Gets the default row height in this worksheet,in unit of points.
**Returns:**
double
### getStandardHeightPixels() {#getStandardHeightPixels--}
```
public int getStandardHeightPixels()
```
Gets the default row height in this worksheet,in unit of pixels.
**Returns:**
int
### getStandardWidth() {#getStandardWidth--}
```
public double getStandardWidth()
```
Gets the default column width in the worksheet,in unit of characters.
**Returns:**
double
### getStandardWidthInch() {#getStandardWidthInch--}
```
public double getStandardWidthInch()
```
Gets the default column width in the worksheet, in unit of inches.
**Returns:**
double
### getStandardWidthPixels() {#getStandardWidthPixels--}
```
public int getStandardWidthPixels()
```
Gets the default column width in the worksheet, in unit of pixels.
**Returns:**
int
### getViewColumnWidthPixel(int column) {#getViewColumnWidthPixel-int-}
```
public int getViewColumnWidthPixel(int column)
```
Get the width in different view type.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | int | The column index. |
**Returns:**
int - the column width in unit of pixels
### groupColumns(int firstIndex, int lastIndex) {#groupColumns-int-int-}
```
public void groupColumns(int firstIndex, int lastIndex)
```
Groups columns.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | int | The first column index to be grouped. |
| lastIndex | int | The last column index to be grouped. |
### groupColumns(int firstIndex, int lastIndex, boolean isHidden) {#groupColumns-int-int-boolean-}
```
public void groupColumns(int firstIndex, int lastIndex, boolean isHidden)
```
Groups columns.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | int | The first column index to be grouped. |
| lastIndex | int | The last column index to be grouped. |
| isHidden | boolean | Specifies if the grouped columns are hidden. |
### groupRows(int firstIndex, int lastIndex) {#groupRows-int-int-}
```
public void groupRows(int firstIndex, int lastIndex)
```
Groups rows.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | int | The first row index to be grouped. |
| lastIndex | int | The last row index to be grouped. |
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### hideColumn(int column) {#hideColumn-int-}
```
public void hideColumn(int column)
```
Hides a column.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | int | Column index. |
### hideRow(int row) {#hideRow-int-}
```
public void hideRow(int row)
```
Hides a row.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Row index. |
### insertColumn(int columnIndex) {#insertColumn-int-}
```
public void insertColumn(int columnIndex)
```
Inserts a new column into the worksheet.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | int | Column index. |
### insertColumn(int columnIndex, boolean updateReference) {#insertColumn-int-boolean-}
```
public void insertColumn(int columnIndex, boolean updateReference)
```
Inserts a new column into the worksheet.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | int | Column index. |
| updateReference | boolean | Indicates if references in other worksheets will be updated. |
### insertColumns(int columnIndex, int totalColumns) {#insertColumns-int-int-}
```
public void insertColumns(int columnIndex, int totalColumns)
```
Inserts some columns into the worksheet.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | int | Column index. |
| totalColumns | int | The number of columns. |
### insertColumns(int columnIndex, int totalColumns, boolean updateReference) {#insertColumns-int-int-boolean-}
```
public void insertColumns(int columnIndex, int totalColumns, boolean updateReference)
```
Inserts some columns into the worksheet.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | int | Column index. |
| totalColumns | int | The number of columns. |
| updateReference | boolean | Indicates if references in other worksheets will be updated. |
### insertRange(GridCellArea area, int shiftType) {#insertRange-com.aspose.gridweb.GridCellArea-int-}
```
public void insertRange(GridCellArea area, int shiftType)
```
Inserts a range of cells and shift cells according to the shift option.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| area | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Shift area. |
| shiftType | int | [GridShiftType](../../com.aspose.gridweb/gridshifttype). Shift cells option. |
### insertRange(GridCellArea area, int shiftNumber, int shiftType, boolean updateReference) {#insertRange-com.aspose.gridweb.GridCellArea-int-int-boolean-}
```
public void insertRange(GridCellArea area, int shiftNumber, int shiftType, boolean updateReference)
```
Inserts a range of cells and shift cells according to the shift option.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| area | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Shift area. |
| shiftNumber | int | Number of rows or columns to be inserted. |
| shiftType | int | [GridShiftType](../../com.aspose.gridweb/gridshifttype). Shift cells option. |
| updateReference | boolean | Indicates if update references in other worksheets. |
### insertRow(int rowIndex) {#insertRow-int-}
```
public void insertRow(int rowIndex)
```
Inserts a new row into the worksheet.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | int | Row index. |
### insertRows(int rowIndex, int totalRows) {#insertRows-int-int-}
```
public void insertRows(int rowIndex, int totalRows)
```
Inserts multiple rows into the worksheet.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | int | Row index. |
| totalRows | int | Number of rows to be inserted. |
### insertRows(int rowIndex, int totalRows, boolean updateReference) {#insertRows-int-int-boolean-}
```
public void insertRows(int rowIndex, int totalRows, boolean updateReference)
```
Inserts multiple rows into the worksheet.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | int | Row index. |
| totalRows | int | Number of rows to be inserted. |
| updateReference | boolean | Indicates if references in other worksheets will be updated. |
### isBlankColumn(int columnIndex) {#isBlankColumn-int-}
```
public boolean isBlankColumn(int columnIndex)
```
Checks whether given column is blank(does not contain any data).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | int | the column index |
**Returns:**
boolean - true if given column does not contain any data
### isColumnHidden(int columnIndex) {#isColumnHidden-int-}
```
public boolean isColumnHidden(int columnIndex)
```
Checks whether a column at given index is hidden.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | int | column index |
**Returns:**
boolean - true if the column is hidden.
### isRowHidden(int rowIndex) {#isRowHidden-int-}
```
public boolean isRowHidden(int rowIndex)
```
Checks whether a row at given index is hidden.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | int | row index |
**Returns:**
boolean - true if the row is hidden
### iterator() {#iterator--}
```
public Iterator iterator()
```
Gets the rows enumerator
**Returns:**
java.util.Iterator - The rows enumerator
### merge(int firstRow, int firstColumn, int totalRows, int totalColumns) {#merge-int-int-int-int-}
```
public void merge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```
Merges a specified range of cells into a single cell.
**Remarks**
Reference the merged cell via the address of the upper-left cell in the range.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | int | First row of this range(zero based) |
| firstColumn | int | First column of this range(zero based) |
| totalRows | int | Number of rows(one based) |
| totalColumns | int | Number of columns(one based) |
### moveRange(GridCellArea sourceArea, int destRow, int destColumn) {#moveRange-com.aspose.gridweb.GridCellArea-int-int-}
```
public void moveRange(GridCellArea sourceArea, int destRow, int destColumn)
```
Moves the range.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | The range which should be moved. |
| destRow | int | The dest row. |
| destColumn | int | The dest column. |
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
### removeDuplicates(int startRow, int startColumn, int endRow, int endColumn) {#removeDuplicates-int-int-int-int-}
```
public void removeDuplicates(int startRow, int startColumn, int endRow, int endColumn)
```
Remove duplicate values in the range.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | int | The start row. |
| startColumn | int | The start column |
| endRow | int | The end row index. |
| endColumn | int | The end column index. |
### removeFormulas() {#removeFormulas--}
```
public void removeFormulas()
```
Removes all formula and replaces with the value of the formula.
### setBorders(int firstRow, int firstColumn, int rowNumber, int columnNumber, int position, WebBorderStyle borderStyle) {#setBorders-int-int-int-int-int-com.aspose.gridweb.WebBorderStyle-}
```
public void setBorders(int firstRow, int firstColumn, int rowNumber, int columnNumber, int position, WebBorderStyle borderStyle)
```
Sets borders for a cells range.
**Example**
```
GridWeb GridWeb1 = new GridWeb();
WebBorderStyle borderStyle1 = new WebBorderStyle();
GridWeb1.getWorkSheets().get(0).getCells().setBorders(0, 0, 5, 8, SetBorderPosition.OUTLINE, borderStyle1);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | int | The first row number of the range(zero based). |
| firstColumn | int | The first column number of the range(zero based). |
| rowNumber | int | The rows number. |
| columnNumber | int | The columns number. |
| position | int | [SetBorderPosition](../../com.aspose.gridweb/setborderposition). The border position. |
| borderStyle | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) | The border style. |
### setColumnWidth(int column, double width) {#setColumnWidth-int-double-}
```
public void setColumnWidth(int column, double width)
```
Sets the width of the specified column.
**Remarks**
To hide a column, sets column width to zero.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | int | Column index. |
| width | double | Width of column.Column width must be between 0 and 255. |
### setColumnWidthInch(int column, double inches) {#setColumnWidthInch-int-double-}
```
public void setColumnWidthInch(int column, double inches)
```
Sets column width in unit of inches.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | int | Column index. |
| inches | double | Number of inches. |
### setColumnWidthPixel(int column, int pixel) {#setColumnWidthPixel-int-int-}
```
public void setColumnWidthPixel(int column, int pixel)
```
Sets column width in unit of pixels.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | int | Column index. |
| pixel | int | Number of pixels. |
### setRowHeight(int row, double height) {#setRowHeight-int-double-}
```
public void setRowHeight(int row, double height)
```
Sets the height of the specified row.
**Remarks**
To hide a row, sets row height to zero.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Row index. |
| height | double | Height of row.In unit of point It should be between 0 and 409.5. |
### setRowHeightInch(int row, double inches) {#setRowHeightInch-int-double-}
```
public void setRowHeightInch(int row, double inches)
```
Sets row height in unit of inches.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Row index. |
| inches | double | Number of inches.It should be between 0 and 409.5/72. |
### setRowHeightPixel(int row, int pixels) {#setRowHeightPixel-int-int-}
```
public void setRowHeightPixel(int row, int pixels)
```
Sets row height in unit of pixels.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Row index. |
| pixels | int | Number of pixels. |
### setRowOutlineLevel(int rowIndex, int outlineLevel) {#setRowOutlineLevel-int-int-}
```
public void setRowOutlineLevel(int rowIndex, int outlineLevel)
```
Sets the outline level of the row.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | int | row index. |
| outlineLevel | int | outline level. |
### setStandardHeight(double value) {#setStandardHeight-double-}
```
public void setStandardHeight(double value)
```
Sets the default row height in this worksheet,in unit of points.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |
### setStandardHeightPixels(int value) {#setStandardHeightPixels-int-}
```
public void setStandardHeightPixels(int value)
```
Sets the default row height in this worksheet,in unit of pixels.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setStandardWidth(double value) {#setStandardWidth-double-}
```
public void setStandardWidth(double value)
```
Sets the default column width in the worksheet,in unit of characters.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |
### setStandardWidthInch(double value) {#setStandardWidthInch-double-}
```
public void setStandardWidthInch(double value)
```
Sets the default column width in the worksheet, in unit of inches.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |
### setStandardWidthPixels(int value) {#setStandardWidthPixels-int-}
```
public void setStandardWidthPixels(int value)
```
Sets the default column width in the worksheet, in unit of pixels.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setStyle(int firstRow, int firstColumn, int rowNumber, int columnNumber, GridTableItemStyle style) {#setStyle-int-int-int-int-com.aspose.gridweb.GridTableItemStyle-}
```
public void setStyle(int firstRow, int firstColumn, int rowNumber, int columnNumber, GridTableItemStyle style)
```
Sets the style to a specified range of cells.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | int | First row of this range(zero based) |
| firstColumn | int | First column of this range(zero based) |
| rowNumber | int | Number of rows(one based) |
| columnNumber | int | Number of columns(one based) |
| style | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | The style object to be set |
### setStyle(String cellRange, GridTableItemStyle style) {#setStyle-java.lang.String-com.aspose.gridweb.GridTableItemStyle-}
```
public void setStyle(String cellRange, GridTableItemStyle style)
```
Sets the style to a specified range of cells.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellRange | java.lang.String | The range of cells' names, like "A1:D6" |
| style | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | The style object to be set |
### sort(int startRow, int startColumn, int rows, int columns, int index, boolean isAsending, boolean isCaseSensitive, boolean islefttoright) {#sort-int-int-int-int-int-boolean-boolean-boolean-}
```
public void sort(int startRow, int startColumn, int rows, int columns, int index, boolean isAsending, boolean isCaseSensitive, boolean islefttoright)
```
Sorts the datas ascend/decend top to bottom in a range of a Worksheet by specified column index. Sorts the datas ascend/decend left to right in a range of a Worksheet by specified row index.
**Example**
```
GridWeb GridWeb1 = new GridWeb();
GridWeb1.getWorkSheets().get(0).getCells().sort(1,0,25,6,3,true,true,false);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | int | The row number of the first cell to sort. |
| startColumn | int | The column number of the first cell to sort. |
| rows | int | Number of rows to be imported. |
| columns | int | Number of columns to be imported. |
| index | int | The column index that specifis the sort column. if the Orientation is top to bottom ,it stand for the column index that specifis the sort column. if the Orientation is from left to right,it stand for the row index that specifis the sort row. |
| isAsending | boolean | whether the sorting order is asending . |
| isCaseSensitive | boolean | whether the sort is casesensitive . |
| islefttoright | boolean | whether the sort orientation is from left to right |
### sort(int startRow, int startColumn, int rows, int columns, int[] indexes, int[] orders, int orientation, boolean isCaseSensitive) {#sort-int-int-int-int-int---int---int-boolean-}
```
public void sort(int startRow, int startColumn, int rows, int columns, int[] indexes, int[] orders, int orientation, boolean isCaseSensitive)
```
Sorts the datas ascend/decend top to bottom in a range of a Worksheet by specified column index. Sorts the datas ascend/decend left to right in a range of a Worksheet by specified row index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | int | The row number of the first cell to sort. |
| startColumn | int | The column number of the first cell to sort. |
| rows | int | Number of rows to be imported. |
| columns | int | Number of columns to be imported. |
| indexes | int[] | The column index array that specifis the sort column. if the Orientation is top to bottom ,it stand for the column index that specifis the sort column. if the Orientation is from left to right,it stand for the row index that specifis the sort row. |
| orders | int[] | [SortByOrder](../../com.aspose.gridweb/sortbyorder). the the sorting order array . |
| orientation | int | [SortOrientation](../../com.aspose.gridweb/sortorientation). sorting orientation |
| isCaseSensitive | boolean | whether the sort is casesensitive . |
### toString() {#toString--}
```
public String toString()
```
**Returns:**
java.lang.String
### unMerge(int firstRow, int firstColumn, int totalRows, int totalColumns) {#unMerge-int-int-int-int-}
```
public void unMerge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```
Unmerges a specified range of merged cells.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | int | First row of this range(zero based) |
| firstColumn | int | First column of this range(zero based) |
| totalRows | int | Number of rows(one based) |
| totalColumns | int | Number of columns(one based) |
### ungroupColumns(int firstIndex, int lastIndex) {#ungroupColumns-int-int-}
```
public void ungroupColumns(int firstIndex, int lastIndex)
```
Ungroups columns.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | int | The first column index to be ungrouped. |
| lastIndex | int | The last column index to be ungrouped. |
### ungroupRows(int firstIndex, int lastIndex) {#ungroupRows-int-int-}
```
public void ungroupRows(int firstIndex, int lastIndex)
```
Ungroups rows.
**Remarks**
Only removes outter group info.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | int | The first row index to be ungrouped. |
| lastIndex | int | The last row index to be ungrouped. |
### unhideColumn(int column, double width) {#unhideColumn-int-double-}
```
public void unhideColumn(int column, double width)
```
Unhides a column
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | int | Column index. |
| width | double | Column width..Column width must be between 0 and 255 |
### unhideRow(int row) {#unhideRow-int-}
```
public void unhideRow(int row)
```
Unhides a row.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Row index. |
### wait() {#wait--}
```
public final void wait()
```
### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |
