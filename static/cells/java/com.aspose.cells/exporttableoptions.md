##ExportTableOptions
Represents all export table options.
**Inheritance:**
java.lang.Object
```
public class ExportTableOptions
```
Represents all export table options.
**Remarks**
If there are some special requirements about the exporting, such as ignoring error values, user may extend this class to overwrite corresponding apis to achive the goal.
## Constructors
| Constructor | Description |
| --- | --- |
| [ExportTableOptions()](#ExportTableOptions--) |  |
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllowDBNull()](#getAllowDBNull--) | This value indicates whether DBNulls are allowed in this table. |
| [getCheckMixedValueType()](#getCheckMixedValueType--) | False, Aspose.Cells will set the DataColumn's type by the value type of the first row for performance. |
| [getClass()](#getClass--) |  |
| [getExportAsHtmlString()](#getExportAsHtmlString--) | Exports the html string value of the cells to the DataTable. |
| [getExportAsString()](#getExportAsString--) | Exports the string value of the cells to the DataTable. |
| [getExportColumnName()](#getExportColumnName--) | Indicates whether the data in the first row are exported to the column name of the DataTable. |
| [getFormatStrategy()](#getFormatStrategy--) | Gets the format strategy when exporting the value as string value. |
| [getIndexes()](#getIndexes--) | The indexes of columns/rows which should be exported out. |
| [getPlotVisibleCells()](#getPlotVisibleCells--) | Only exports visible cells. |
| [getPlotVisibleColumns()](#getPlotVisibleColumns--) | Only exports visible columns. |
| [getPlotVisibleRows()](#getPlotVisibleRows--) | Only exports visible rows. |
| [getRenameStrategy()](#getRenameStrategy--) | Strategy for duplicate names of columns. |
| [getSkipErrorValue()](#getSkipErrorValue--) | Indicates whether skip invalid value for the column. |
| [hashCode()](#hashCode--) |  |
| [isVertical()](#isVertical--) | True if a row in Workbook file represents a row in DataTable. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [preprocessExportedValue(int cellRow, int cellColumn, CellValue value)](#preprocessExportedValue-int-int-com.aspose.cells.CellValue-) | Preprocess the value of current cell to be exported. |
| [setAllowDBNull(boolean value)](#setAllowDBNull-boolean-) | This value indicates whether DBNulls are allowed in this table. |
| [setCheckMixedValueType(boolean value)](#setCheckMixedValueType-boolean-) | False, Aspose.Cells will set the DataColumn's type by the value type of the first row for performance. |
| [setExportAsHtmlString(boolean value)](#setExportAsHtmlString-boolean-) | Exports the html string value of the cells to the DataTable. |
| [setExportAsString(boolean value)](#setExportAsString-boolean-) | Exports the string value of the cells to the DataTable. |
| [setExportColumnName(boolean value)](#setExportColumnName-boolean-) | Indicates whether the data in the first row are exported to the column name of the DataTable. |
| [setFormatStrategy(int value)](#setFormatStrategy-int-) | Sets the format strategy when exporting the value as string value. |
| [setIndexes(int[] value)](#setIndexes-int---) | The indexes of columns/rows which should be exported out. |
| [setPlotVisibleCells(boolean value)](#setPlotVisibleCells-boolean-) | Only exports visible cells. |
| [setPlotVisibleColumns(boolean value)](#setPlotVisibleColumns-boolean-) | Only exports visible columns. |
| [setPlotVisibleRows(boolean value)](#setPlotVisibleRows-boolean-) | Only exports visible rows. |
| [setRenameStrategy(int value)](#setRenameStrategy-int-) | Strategy for duplicate names of columns. |
| [setSkipErrorValue(boolean value)](#setSkipErrorValue-boolean-) | Indicates whether skip invalid value for the column. |
| [setVertical(boolean value)](#setVertical-boolean-) | True if a row in Workbook file represents a row in DataTable. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ExportTableOptions() {#ExportTableOptions--}
```
public ExportTableOptions()
```
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
### getAllowDBNull() {#getAllowDBNull--}
```
public boolean getAllowDBNull()
```
This value indicates whether DBNulls are allowed in this table.
**Returns:**
boolean
### getCheckMixedValueType() {#getCheckMixedValueType--}
```
public boolean getCheckMixedValueType()
```
False, Aspose.Cells will set the DataColumn's type by the value type of the first row for performance. True, Aspose.Cells will check whether the value type in the column are mixed before set the DataColumn's type And the value type are mixed, the DataColumn's type will be string.
**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getExportAsHtmlString() {#getExportAsHtmlString--}
```
public boolean getExportAsHtmlString()
```
Exports the html string value of the cells to the DataTable.
**Returns:**
boolean
### getExportAsString() {#getExportAsString--}
```
public boolean getExportAsString()
```
Exports the string value of the cells to the DataTable.
**Returns:**
boolean
### getExportColumnName() {#getExportColumnName--}
```
public boolean getExportColumnName()
```
Indicates whether the data in the first row are exported to the column name of the DataTable. The default value is false.
**Returns:**
boolean
### getFormatStrategy() {#getFormatStrategy--}
```
public int getFormatStrategy()
```
Gets the format strategy when exporting the value as string value.
See [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).
**Returns:**
int
### getIndexes() {#getIndexes--}
```
public int[] getIndexes()
```
The indexes of columns/rows which should be exported out.
**Returns:**
int[]
### getPlotVisibleCells() {#getPlotVisibleCells--}
```
public boolean getPlotVisibleCells()
```
Only exports visible cells.
**Returns:**
boolean
### getPlotVisibleColumns() {#getPlotVisibleColumns--}
```
public boolean getPlotVisibleColumns()
```
Only exports visible columns.
**Returns:**
boolean
### getPlotVisibleRows() {#getPlotVisibleRows--}
```
public boolean getPlotVisibleRows()
```
Only exports visible rows.
**Returns:**
boolean
### getRenameStrategy() {#getRenameStrategy--}
```
public int getRenameStrategy()
```
Strategy for duplicate names of columns.
See [RenameStrategy](../../com.aspose.cells/renamestrategy).
**Returns:**
int
### getSkipErrorValue() {#getSkipErrorValue--}
```
public boolean getSkipErrorValue()
```
Indicates whether skip invalid value for the column. For example,if the column type is decimal ,the value is greater than decimal.MaxValue and this property is true,we will not throw exception again. The default value is false.
**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### isVertical() {#isVertical--}
```
public boolean isVertical()
```
True if a row in Workbook file represents a row in DataTable. False if a column in Workbook file represents a row in DataTable.
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
### preprocessExportedValue(int cellRow, int cellColumn, CellValue value) {#preprocessExportedValue-int-int-com.aspose.cells.CellValue-}
```
public boolean preprocessExportedValue(int cellRow, int cellColumn, CellValue value)
```
Preprocess the value of current cell to be exported.
**Remarks**
The row and column index is cell's absolute index in the worksheet, not index in the exported table. User may check the value of current cell in the override implementation of this method, if current cell needs to be replaced with other type and value, here the implementation should set the expected type and value to the CellValue object and return true. By default this method does nothing and returns false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellRow | int | the row index of current cell |
| cellColumn | int | the column index of cell |
| value | [CellValue](../../com.aspose.cells/cellvalue) | value and type of current cell |
**Returns:**
boolean - Whether current cell has been replaced with different type and/or value.
### setAllowDBNull(boolean value) {#setAllowDBNull-boolean-}
```
public void setAllowDBNull(boolean value)
```
This value indicates whether DBNulls are allowed in this table.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setCheckMixedValueType(boolean value) {#setCheckMixedValueType-boolean-}
```
public void setCheckMixedValueType(boolean value)
```
False, Aspose.Cells will set the DataColumn's type by the value type of the first row for performance. True, Aspose.Cells will check whether the value type in the column are mixed before set the DataColumn's type And the value type are mixed, the DataColumn's type will be string.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setExportAsHtmlString(boolean value) {#setExportAsHtmlString-boolean-}
```
public void setExportAsHtmlString(boolean value)
```
Exports the html string value of the cells to the DataTable.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setExportAsString(boolean value) {#setExportAsString-boolean-}
```
public void setExportAsString(boolean value)
```
Exports the string value of the cells to the DataTable.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setExportColumnName(boolean value) {#setExportColumnName-boolean-}
```
public void setExportColumnName(boolean value)
```
Indicates whether the data in the first row are exported to the column name of the DataTable. The default value is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setFormatStrategy(int value) {#setFormatStrategy-int-}
```
public void setFormatStrategy(int value)
```
Sets the format strategy when exporting the value as string value.
See [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setIndexes(int[] value) {#setIndexes-int---}
```
public void setIndexes(int[] value)
```
The indexes of columns/rows which should be exported out.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int[] |  |
### setPlotVisibleCells(boolean value) {#setPlotVisibleCells-boolean-}
```
public void setPlotVisibleCells(boolean value)
```
Only exports visible cells.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setPlotVisibleColumns(boolean value) {#setPlotVisibleColumns-boolean-}
```
public void setPlotVisibleColumns(boolean value)
```
Only exports visible columns.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setPlotVisibleRows(boolean value) {#setPlotVisibleRows-boolean-}
```
public void setPlotVisibleRows(boolean value)
```
Only exports visible rows.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setRenameStrategy(int value) {#setRenameStrategy-int-}
```
public void setRenameStrategy(int value)
```
Strategy for duplicate names of columns.
See [RenameStrategy](../../com.aspose.cells/renamestrategy).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setSkipErrorValue(boolean value) {#setSkipErrorValue-boolean-}
```
public void setSkipErrorValue(boolean value)
```
Indicates whether skip invalid value for the column. For example,if the column type is decimal ,the value is greater than decimal.MaxValue and this property is true,we will not throw exception again. The default value is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setVertical(boolean value) {#setVertical-boolean-}
```
public void setVertical(boolean value)
```
True if a row in Workbook file represents a row in DataTable. False if a column in Workbook file represents a row in DataTable.
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
