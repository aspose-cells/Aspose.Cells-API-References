##WebWorksheet
Represents a web worksheet.
**Inheritance:**
java.lang.Object, [com.aspose.gridweb.Control](../../com.aspose.gridweb/control)
```
public class WebWorksheet extends Control
```
Represents a web worksheet.
**Remarks**
NOTE: This class is now obsolete. please use GridWorksheet Instead. This class will be removed after 6 months since Aug. 2014. Aspose apologizes for any inconvenience you may have experienced.
**Example**
```
```
## Constructors
| Constructor | Description |
| --- | --- |
| [WebWorksheet(MainWeb mw, GridWorksheet gwk)](#WebWorksheet-com.aspose.gridweb.MainWeb-com.aspose.gridweb.GridWorksheet-) | the constructor of the WebWorksheet. |
| [WebWorksheet()](#WebWorksheet--) | the constructor of the WebWorksheet. |
## Methods
| Method | Description |
| --- | --- |
| [autoFitColumn(int columnIndex)](#autoFitColumn-int-) | Autofits the column width. |
| [autoFitColumn(int columnIndex, int startRow, int endRow)](#autoFitColumn-int-int-int-) | Autofits the column width. |
| [cancelNewBindRow()](#cancelNewBindRow--) | Cancels and deletes the new added bind row. |
| [commitNewBindRow()](#commitNewBindRow--) | Commits the new added bind row and add it to the datasource. |
| [copy(WebWorksheet source)](#copy-com.aspose.gridweb.WebWorksheet-) | Copies from another worksheet object. |
| [createAutoGenratedColumns()](#createAutoGenratedColumns--) | After setting a datasource for the worksheet, call this method to generate the bind columns automatically. |
| [createNewBindRow()](#createNewBindRow--) | Creates a new bind row and bind to the datasource. |
| [createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString)](#createSubtotal-int-int-int-int-int---java.lang.String-com.aspose.gridweb.GridTableItemStyle-com.aspose.gridweb.GridTableItemStyle-int-java.lang.String-) | Creates subtotal in the sheet. |
| [dataBind()](#dataBind--) | Bind the sheet to the DataSource. |
| [deleteBindRow(int rowNum)](#deleteBindRow-int-) | Deletes a bind row. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [freezePanes(int row, int column, int freezedRows, int freezedColumns)](#freezePanes-int-int-int-int-) | Freezes panes at the specified cell in the worksheet. |
| [getBindStartColumn()](#getBindStartColumn--) | In data-binding mode, BindStartRow and BindStartColumn indicate the position of the grid to bind bo the datasource. |
| [getBindStartRow()](#getBindStartRow--) | In data-binding mode, BindStartRow and BindStartColumn indicate the position of the grid to bind bo the datasource. |
| [getBindingSource()](#getBindingSource--) | The actually binding datasource object at run-time. |
| [getClass()](#getClass--) |  |
| [getCurrentBindRows()](#getCurrentBindRows--) | Gets the binding rows number in data-binding mode. |
| [getDataMember()](#getDataMember--) | Gets the DataMember from the multi-member DataSource. |
| [getDataSource()](#getDataSource--) | Gets the DataSource. |
| [getEnableCreateBindColumnHeader()](#getEnableCreateBindColumnHeader--) | In data-binding mode, indicates whether to create bind column header captions in the sheet. |
| [getIndex()](#getIndex--) | Gets the index of itself within the worksheets. |
| [getName()](#getName--) | Gets the name of the sheet. |
| [getUniqueID()](#getUniqueID--) | Gets the UniqueID in the Control |
| [getValidations()](#getValidations--) | Gets the data validation setting collection in the worksheet. |
| [getVisible()](#getVisible--) | Indicates whether this sheet's name is shown in the sheet tabs of the control. |
| [groupRows(int firstIndex, int lastIndex)](#groupRows-int-int-) | Groups rows. |
| [groupRows(int firstIndex, int lastIndex, boolean isHidden)](#groupRows-int-int-boolean-) | Groups rows. |
| [hashCode()](#hashCode--) |  |
| [isProtected()](#isProtected--) | Gets whether the worksheet is protected. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllCellsEditable()](#setAllCellsEditable--) | Makes all cells editable.this is extended attribute |
| [setAllCellsReadonly()](#setAllCellsReadonly--) | Makes all cells readonly.this is extended attribute notice this attribute can not keep in actual cell,if you want to keep protect please use setProtect |
| [setBindStartColumn(int value)](#setBindStartColumn-int-) | In data-binding mode, BindStartRow and BindStartColumn indicate the position of the grid to bind bo the datasource. |
| [setBindStartRow(int value)](#setBindStartRow-int-) | In data-binding mode, BindStartRow and BindStartColumn indicate the position of the grid to bind bo the datasource. |
| [setCurrentBindRows(int value)](#setCurrentBindRows-int-) | Gets the binding rows number in data-binding mode. |
| [setDataMember(String value)](#setDataMember-java.lang.String-) | Sets the DataMember from the multi-member DataSource. |
| [setDataSource(Object value)](#setDataSource-java.lang.Object-) | Sets the DataSource. |
| [setEditableRange(int startRow, int startColumn, int rows, int columns)](#setEditableRange-int-int-int-int-) | Makes a range of cells editable. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Make all cells read only by calling the SetAllCellsReadonly method. |
| [setEnableCreateBindColumnHeader(boolean value)](#setEnableCreateBindColumnHeader-boolean-) | In data-binding mode, indicates whether to create bind column header captions in the sheet. |
| [setName(String value)](#setName-java.lang.String-) | Sets the name of the sheet. |
| [setProtected(boolean value)](#setProtected-boolean-) | Sets whether the worksheet is protected. |
| [setReadonlyRange(int startRow, int startColumn, int rows, int columns)](#setReadonlyRange-int-int-int-int-) | Makes a range of cells readonly. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells First make all cells editable by calling the SetAllCellsEditable method. |
| [setVisible(boolean value)](#setVisible-boolean-) | Indicates whether this sheet's name is shown in the sheet tabs of the control. |
| [toString()](#toString--) |  |
| [unfreezePanes()](#unfreezePanes--) | Unfreezes panes in the worksheet. |
| [ungroupRows(int firstIndex, int lastIndex)](#ungroupRows-int-int-) | Ungroups rows. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### WebWorksheet(MainWeb mw, GridWorksheet gwk) {#WebWorksheet-com.aspose.gridweb.MainWeb-com.aspose.gridweb.GridWorksheet-}
```
public WebWorksheet(MainWeb mw, GridWorksheet gwk)
```
the constructor of the WebWorksheet.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| mw | [MainWeb](../../com.aspose.gridweb/mainweb) |  |
| gwk | [GridWorksheet](../../com.aspose.gridweb/gridworksheet) |  |
### WebWorksheet() {#WebWorksheet--}
```
public WebWorksheet()
```
the constructor of the WebWorksheet.
### autoFitColumn(int columnIndex) {#autoFitColumn-int-}
```
public void autoFitColumn(int columnIndex)
```
Autofits the column width.
**Remarks**
AutoFitColumn is an imprecise function.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | int | Column index. |
### autoFitColumn(int columnIndex, int startRow, int endRow) {#autoFitColumn-int-int-int-}
```
public void autoFitColumn(int columnIndex, int startRow, int endRow)
```
Autofits the column width. This method autofits a column based on content in a range of cells within the column from startRow to endRow. AutoFitColumn is an imprecise function.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | int | column index, zero based |
| startRow | int | start row index, zero based |
| endRow | int | end row index, zero based |
### cancelNewBindRow() {#cancelNewBindRow--}
```
public int cancelNewBindRow()
```
Cancels and deletes the new added bind row.
**Returns:**
int - The row index. If there is no new created bind row, returns -1.
### commitNewBindRow() {#commitNewBindRow--}
```
public int commitNewBindRow()
```
Commits the new added bind row and add it to the datasource.
**Returns:**
int - The row index of the new row. If no row is created, returns -1.
### copy(WebWorksheet source) {#copy-com.aspose.gridweb.WebWorksheet-}
```
public void copy(WebWorksheet source)
```
Copies from another worksheet object.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | [WebWorksheet](../../com.aspose.gridweb/webworksheet) | The other sheet. |
### createAutoGenratedColumns() {#createAutoGenratedColumns--}
```
public void createAutoGenratedColumns()
```
After setting a datasource for the worksheet, call this method to generate the bind columns automatically.
### createNewBindRow() {#createNewBindRow--}
```
public int createNewBindRow()
```
Creates a new bind row and bind to the datasource.
**Returns:**
int - The row index of the new row. If no row is created, returns -1.
### createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString) {#createSubtotal-int-int-int-int-int---java.lang.String-com.aspose.gridweb.GridTableItemStyle-com.aspose.gridweb.GridTableItemStyle-int-java.lang.String-}
```
public void createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString)
```
Creates subtotal in the sheet.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnNameRowIndex | int | The row index of the column name row. |
| dataRows | int | The number of the data rows. |
| groupByColumnIndex | int | The column index of the column to be grouped. |
| subtotalFunction | int | [SubtotalFunction](../../com.aspose.gridweb/subtotalfunction). The subtotal function type. |
| subtotalColumnIndexList | int[] | The column indexes to be subtotaled. |
| functionLabel | java.lang.String | The label of subtotal function. |
| grandCellStyle | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | The style of the grand total line. |
| subtotalCellStyle | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | The style of the subtotal line. |
| numberType | int | [NumberType](../../com.aspose.gridweb/numbertype). The number type of the subtotal result cells. |
| customString | java.lang.String | The custome format string of the subtotal result cells. Can be null. |
### dataBind() {#dataBind--}
```
public void dataBind()
```
Bind the sheet to the DataSource.
### deleteBindRow(int rowNum) {#deleteBindRow-int-}
```
public int deleteBindRow(int rowNum)
```
Deletes a bind row.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowNum | int | The row index. |
**Returns:**
int - The deleted row index. If no bind row is deleted, returns -1.
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
### freezePanes(int row, int column, int freezedRows, int freezedColumns) {#freezePanes-int-int-int-int-}
```
public void freezePanes(int row, int column, int freezedRows, int freezedColumns)
```
Freezes panes at the specified cell in the worksheet.
**Remarks**
Row index and column index cannot all be zero. Number of rows and number of columns also cannot all be zero.
The first two parameters specify the freezed position and the last two parameters specify the area freezed on the left top pane.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Row index. |
| column | int | Column index. |
| freezedRows | int | Number of visible rows in top pane, no more than row index. |
| freezedColumns | int | Number of visible columns in left pane, no more than column index. |
### getBindStartColumn() {#getBindStartColumn--}
```
public int getBindStartColumn()
```
In data-binding mode, BindStartRow and BindStartColumn indicate the position of the grid to bind bo the datasource.
**Returns:**
int
### getBindStartRow() {#getBindStartRow--}
```
public int getBindStartRow()
```
In data-binding mode, BindStartRow and BindStartColumn indicate the position of the grid to bind bo the datasource.
**Returns:**
int
### getBindingSource() {#getBindingSource--}
```
public Iterable getBindingSource()
```
The actually binding datasource object at run-time. It is a DataView object when the DataSource property is a DataSet, DataTable or DataView object.
**Returns:**
java.lang.Iterable
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getCurrentBindRows() {#getCurrentBindRows--}
```
public int getCurrentBindRows()
```
Gets the binding rows number in data-binding mode.
**Returns:**
int
### getDataMember() {#getDataMember--}
```
public String getDataMember()
```
Gets the DataMember from the multi-member DataSource. Generally it represents a DataTable object of a DataSet.
**Returns:**
java.lang.String
### getDataSource() {#getDataSource--}
```
public Object getDataSource()
```
Gets the DataSource. Generally it's a DataSet object.
**Returns:**
java.lang.Object
### getEnableCreateBindColumnHeader() {#getEnableCreateBindColumnHeader--}
```
public boolean getEnableCreateBindColumnHeader()
```
In data-binding mode, indicates whether to create bind column header captions in the sheet.
**Returns:**
boolean
### getIndex() {#getIndex--}
```
public int getIndex()
```
Gets the index of itself within the worksheets.
**Returns:**
int
### getName() {#getName--}
```
public String getName()
```
Gets the name of the sheet.
**Returns:**
java.lang.String
### getUniqueID() {#getUniqueID--}
```
public String getUniqueID()
```
Gets the UniqueID in the Control
**Returns:**
java.lang.String
### getValidations() {#getValidations--}
```
public GridValidationCollection getValidations()
```
Gets the data validation setting collection in the worksheet.
**Returns:**
[GridValidationCollection](../../com.aspose.gridweb/gridvalidationcollection)
### getVisible() {#getVisible--}
```
public boolean getVisible()
```
Indicates whether this sheet's name is shown in the sheet tabs of the control.
**Returns:**
boolean
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
### groupRows(int firstIndex, int lastIndex, boolean isHidden) {#groupRows-int-int-boolean-}
```
public void groupRows(int firstIndex, int lastIndex, boolean isHidden)
```
Groups rows.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | int | The first row index to be grouped. |
| lastIndex | int | The last row index to be grouped. |
| isHidden | boolean | Specifies if the grouped rows are hidden. |
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### isProtected() {#isProtected--}
```
public boolean isProtected()
```
Gets whether the worksheet is protected. When a worksheet is protected, all the cells can not be edit except the cell whose IsLocked property is false.
**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
### setAllCellsEditable() {#setAllCellsEditable--}
```
public void setAllCellsEditable()
```
Makes all cells editable.this is extended attribute
### setAllCellsReadonly() {#setAllCellsReadonly--}
```
public void setAllCellsReadonly()
```
Makes all cells readonly.this is extended attribute notice this attribute can not keep in actual cell,if you want to keep protect please use setProtect
### setBindStartColumn(int value) {#setBindStartColumn-int-}
```
public void setBindStartColumn(int value)
```
In data-binding mode, BindStartRow and BindStartColumn indicate the position of the grid to bind bo the datasource.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setBindStartRow(int value) {#setBindStartRow-int-}
```
public void setBindStartRow(int value)
```
In data-binding mode, BindStartRow and BindStartColumn indicate the position of the grid to bind bo the datasource.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setCurrentBindRows(int value) {#setCurrentBindRows-int-}
```
public void setCurrentBindRows(int value)
```
Gets the binding rows number in data-binding mode.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setDataMember(String value) {#setDataMember-java.lang.String-}
```
public void setDataMember(String value)
```
Sets the DataMember from the multi-member DataSource. Generally it represents a DataTable object of a DataSet.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setDataSource(Object value) {#setDataSource-java.lang.Object-}
```
public void setDataSource(Object value)
```
Sets the DataSource. Generally it's a DataSet object.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.Object |  |
### setEditableRange(int startRow, int startColumn, int rows, int columns) {#setEditableRange-int-int-int-int-}
```
public void setEditableRange(int startRow, int startColumn, int rows, int columns)
```
Makes a range of cells editable. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Make all cells read only by calling the SetAllCellsReadonly method. then call this method to Specify the range of cells that to be editable
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | int | The start row of the range. |
| startColumn | int | The start column of the range. |
| rows | int | The number of the rows. |
| columns | int | The number of the columns. |
### setEnableCreateBindColumnHeader(boolean value) {#setEnableCreateBindColumnHeader-boolean-}
```
public void setEnableCreateBindColumnHeader(boolean value)
```
In data-binding mode, indicates whether to create bind column header captions in the sheet.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```
Sets the name of the sheet.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setProtected(boolean value) {#setProtected-boolean-}
```
public void setProtected(boolean value)
```
Sets whether the worksheet is protected. When a worksheet is protected, all the cells can not be edit except the cell whose IsLocked property is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setReadonlyRange(int startRow, int startColumn, int rows, int columns) {#setReadonlyRange-int-int-int-int-}
```
public void setReadonlyRange(int startRow, int startColumn, int rows, int columns)
```
Makes a range of cells readonly. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells First make all cells editable by calling the SetAllCellsEditable method. then call this method to Specify the range of cells that to be readonly
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | int | The start row of the range. |
| startColumn | int | The start column of the range. |
| rows | int | The number of the rows. |
| columns | int | The number of the columns. |
### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```
Indicates whether this sheet's name is shown in the sheet tabs of the control.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### toString() {#toString--}
```
public String toString()
```
**Returns:**
java.lang.String
### unfreezePanes() {#unfreezePanes--}
```
public void unfreezePanes()
```
Unfreezes panes in the worksheet.
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
