---
title: GridWorksheet
second_title: Aspose.Cells for Java API Reference
description: Encapsulates the object that represents a single worksheet.
type: docs
url: /java/com.aspose.gridweb/gridworksheet/
---

**Inheritance:**
java.lang.Object
```
public class GridWorksheet
```

Encapsulates the object that represents a single worksheet.
## Methods

| Method | Description |
| --- | --- |
| [addAutoFilter(int row, int startColumn, int endColumn)](#addAutoFilter-int-int-int-) | Sets the range to which the specified AutoFilter applies. |
| [addCustomFilter(int row, String critira)](#addCustomFilter-int-java.lang.String-) | Add custom filter for the specified row. |
| [autoFitColumn(int columnIndex)](#autoFitColumn-int-) | Autofits the column width. |
| [autoFitColumn(int columnIndex, int firstRow, int lastRow)](#autoFitColumn-int-int-int-) | Autofits the column width. |
| [autoFitRow(int rowIndex)](#autoFitRow-int-) | Autofits the row height. |
| [autoFitRow(int rowIndex, int firstColumn, int lastColumn)](#autoFitRow-int-int-int-) | Autofits the row height. |
| [autoFitRow(int startRow, int endRow, int startColumn, int endColumn)](#autoFitRow-int-int-int-int-) | Autofits row height in a rectangle range. |
| [autoFitRows()](#autoFitRows--) | Autofits all rows in this worksheet. |
| [autoFitRows(boolean onlyAuto)](#autoFitRows-boolean-) | Autofits all rows in this worksheet. |
| [autoFitRows(int startRow, int endRow)](#autoFitRows-int-int-) | Autofits row height in a range. |
| [calculateFormula(String formula)](#calculateFormula-java.lang.String-) | Calculates a formula. |
| [clearComments()](#clearComments--) | Clears all comments in designer spreadsheet. |
| [copy(GridWorksheet sourceSheet)](#copy-com.aspose.gridweb.GridWorksheet-) | Copies contents and formats from another worksheet. |
| [createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList)](#createSubtotal-int-int-int-int-int---) | Creates subtotal in the sheet. |
| [createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString)](#createSubtotal-int-int-int-int-int---java.lang.String-com.aspose.gridweb.GridTableItemStyle-com.aspose.gridweb.GridTableItemStyle-int-java.lang.String-) | Creates subtotal in the sheet. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filterString(int column, String criteria)](#filterString-int-java.lang.String-) | Sets the filter for the column.notice we shall call AddAutoFilter before calling of filterString The filter criteria string. notice we use comma->"," as split char,so the cell value you want to filter shall not contains with comma filterString(10,"123,456") means column 10 shall contain 123 or 456, filterString(10,"123") means column10 shall contain 123 value split with comma,eg. 123,456,789 or abc |
| [freezePanes(int row, int column, int freezedRows, int freezedColumns)](#freezePanes-int-int-int-int-) | Freezes panes at the specified cell in the worksheet. |
| [freezePanes(String cellName, int freezedRows, int freezedColumns)](#freezePanes-java.lang.String-int-int-) | Freezes panes at the specified cell in the worksheet. |
| [getActiveCell()](#getActiveCell--) |  |
| [getBackgroundImage()](#getBackgroundImage--) | worksheet background image. |
| [getCells()](#getCells--) |  |
| [getClass()](#getClass--) |  |
| [getCodeName()](#getCodeName--) | Represents worksheet code name. |
| [getColumnCaption(int column)](#getColumnCaption-int-) | Gets the column caption. |
| [getColumnHeaderToolTip(int colIndex)](#getColumnHeaderToolTip-int-) | Gets the columnheader's tooltip text. |
| [getColumnReadonly(int columnIndex)](#getColumnReadonly-int-) | Gets if a column is readonly. |
| [getComments()](#getComments--) |  |
| [getDisplayRightToLeft()](#getDisplayRightToLeft--) |  |
| [getDisplayZeros()](#getDisplayZeros--) | True if zero values are displayed. |
| [getFirstVisibleColumn()](#getFirstVisibleColumn--) |  |
| [getFirstVisibleRow()](#getFirstVisibleRow--) |  |
| [getFreezedPanes()](#getFreezedPanes--) | Gets the freeze panes. |
| [getGridActiveCell()](#getGridActiveCell--) |  |
| [getHyperlinks()](#getHyperlinks--) | Gets the [GridHyperlinkCollection](../../com.aspose.gridweb/gridhyperlinkcollection) collection. |
| [getIndex()](#getIndex--) |  |
| [getIsReadonly(int row, int col)](#getIsReadonly-int-int-) | Gets whether the cell is readonly.this is an extended attribute of GridWeb ,it will not keep in actual excel file |
| [getName()](#getName--) | the name of the worksheet. |
| [getOutlineShown()](#getOutlineShown--) | Indicates whether show outline. |
| [getPictures()](#getPictures--) | Gets a [getPictures()](../../com.aspose.gridweb/gridworksheet\#getPictures--) collection. |
| [getPivotTables()](#getPivotTables--) | Gets the pivotTables in the worksheet. |
| [getRowCaption(int row)](#getRowCaption-int-) | Gets the row caption. |
| [getRowHeaderToolTip(int rowIndex)](#getRowHeaderToolTip-int-) | Gets the rowheader's tooltip text. |
| [getRowReadonly(int rowIndex)](#getRowReadonly-int-) | Gets if a row is readonly. |
| [getSelected()](#getSelected--) | Indicates whether this worksheet is selected when the workbook is opened. |
| [getShapes()](#getShapes--) | Gets a [getPictures()](../../com.aspose.gridweb/gridworksheet\#getPictures--) collection. |
| [getStandardHeight()](#getStandardHeight--) | the default row height in this worksheet,in unit of points. |
| [getStandardHeightPixels()](#getStandardHeightPixels--) | the default row height in this worksheet,in unit of pixels. |
| [getTabColor()](#getTabColor--) | Represents worksheet tab color. |
| [getValidations()](#getValidations--) | Gets the data validation setting collection in the worksheet. |
| [getVisible()](#getVisible--) | Indicates whether this sheet's name is shown in the sheet tabs of the control. |
| [getWorkbook()](#getWorkbook--) |  |
| [getZoom()](#getZoom--) |  |
| [groupRows(int firstIndex, int lastIndex, boolean isHidden)](#groupRows-int-int-boolean-) | Groups rows. |
| [hashCode()](#hashCode--) |  |
| [isGridlinesVisible()](#isGridlinesVisible--) | a value indicating whether the grid lines are visible.Default is true. |
| [isProtected()](#isProtected--) | Indicates if the worksheet is protected. |
| [isSummaryRowBelow()](#isSummaryRowBelow--) | Indicates if the summary row will be positioned below the detail rows in the outline. |
| [moveTo(int index)](#moveTo-int-) | Moves the sheet to another location in the spreadsheet. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshFilter()](#refreshFilter--) | Refresh auto filters to hide or unhide the rows. |
| [removeAutoFilter()](#removeAutoFilter--) | Remove the auto filter of the worksheet. |
| [removeSubtotal()](#removeSubtotal--) | Removes subtotal created by the CreateSubtotal method in the sheet. |
| [resetFilter(int fieldIndex)](#resetFilter-int-) | The integer offset of the field on which you want to apply ,based on the first filter column (from the left of the list; the leftmost field is field 0). |
| [setActiveCell(String value)](#setActiveCell-java.lang.String-) | For the description of this property, please see [getActiveCell()](../../com.aspose.gridweb/gridworksheet\#getActiveCell--) |
| [setAllCellsEditable()](#setAllCellsEditable--) | Makes all cells editable.this is extended attribute |
| [setAllCellsReadonly()](#setAllCellsReadonly--) | Makes all cells readonly.this is extended attribute notice this attribute can not keep in actual cell,if you want to keep protect please use setProtect |
| [setBackgroundImage(byte[] value)](#setBackgroundImage-byte---) | For the description of this property, please see [getBackgroundImage()](../../com.aspose.gridweb/gridworksheet\#getBackgroundImage--) |
| [setColumnCaption(int column, String caption)](#setColumnCaption-int-java.lang.String-) | Sets the caption for the column.please note this is an extension attribute and can not keep in excel file |
| [setColumnHeaderToolTip(int colIndex, String toolTip)](#setColumnHeaderToolTip-int-java.lang.String-) | Sets the columnheader's tooltip text. |
| [setColumnReadonly(int columnIndex, boolean isReadonly)](#setColumnReadonly-int-boolean-) | Sets a column to readonly so user can't delete it from client side. |
| [setDisplayRightToLeft(boolean value)](#setDisplayRightToLeft-boolean-) | For the description of this property, please see [getDisplayRightToLeft()](../../com.aspose.gridweb/gridworksheet\#getDisplayRightToLeft--) |
| [setDisplayZeros(boolean value)](#setDisplayZeros-boolean-) | For the description of this property, please see [getDisplayZeros()](../../com.aspose.gridweb/gridworksheet\#getDisplayZeros--) |
| [setEditableRange(int startRow, int startColumn, int rows, int columns)](#setEditableRange-int-int-int-int-) | Makes a range of cells editable. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Make all cells read only by calling the SetAllCellsReadonly method. |
| [setFirstVisibleColumn(int value)](#setFirstVisibleColumn-int-) | For the description of this property, please see [getFirstVisibleColumn()](../../com.aspose.gridweb/gridworksheet\#getFirstVisibleColumn--) |
| [setFirstVisibleRow(int value)](#setFirstVisibleRow-int-) | For the description of this property, please see [getFirstVisibleRow()](../../com.aspose.gridweb/gridworksheet\#getFirstVisibleRow--) |
| [setGridActiveCell(GridCell value)](#setGridActiveCell-com.aspose.gridweb.GridCell-) | For the description of this property, please see [getGridActiveCell()](../../com.aspose.gridweb/gridworksheet\#getGridActiveCell--) |
| [setGridlinesVisible(boolean value)](#setGridlinesVisible-boolean-) | For the description of this property, please see [isGridlinesVisible()](../../com.aspose.gridweb/gridworksheet\#isGridlinesVisible--) |
| [setIsReadonly(int row, int col, boolean value)](#setIsReadonly-int-int-boolean-) | Sets whether the cell is readonly.this is an extended attribute of GridWeb ,it will not keep in actual excel file |
| [setName(String value)](#setName-java.lang.String-) | For the description of this property, please see [getName()](../../com.aspose.gridweb/gridworksheet\#getName--) |
| [setOutlineShown(boolean value)](#setOutlineShown-boolean-) |  |
| [setProtect()](#setProtect--) | Protects worksheet. |
| [setReadonlyRange(int startRow, int startColumn, int rows, int columns)](#setReadonlyRange-int-int-int-int-) | Makes a range of cells readonly. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells First make all cells editable by calling the SetAllCellsEditable method. |
| [setRowCaption(int row, String caption)](#setRowCaption-int-java.lang.String-) | Sets the caption for the row. |
| [setRowHeaderToolTip(int rowIndex, String toolTip)](#setRowHeaderToolTip-int-java.lang.String-) | Sets the rowheader's tooltip text. |
| [setRowReadonly(int rowIndex, boolean isReadonly)](#setRowReadonly-int-boolean-) | Sets a row to readonly so user can't delete it from client side. |
| [setSelected(boolean value)](#setSelected-boolean-) |  |
| [setStandardHeight(double value)](#setStandardHeight-double-) | For the description of this property, please see [getStandardHeight()](../../com.aspose.gridweb/gridworksheet\#getStandardHeight--) |
| [setStandardHeightPixels(int value)](#setStandardHeightPixels-int-) | For the description of this property, please see [getStandardHeightPixels()](../../com.aspose.gridweb/gridworksheet\#getStandardHeightPixels--) |
| [setSummaryRowBelow(boolean value)](#setSummaryRowBelow-boolean-) | For the description of this property, please see [isSummaryRowBelow()](../../com.aspose.gridweb/gridworksheet\#isSummaryRowBelow--) |
| [setTabColor(Color value)](#setTabColor-com.aspose.gridweb.Color-) | For the description of this property, please see [getTabColor()](../../com.aspose.gridweb/gridworksheet\#getTabColor--) |
| [setVisible(boolean value)](#setVisible-boolean-) | For the description of this property, please see [getVisible()](../../com.aspose.gridweb/gridworksheet\#getVisible--) |
| [setZoom(int value)](#setZoom-int-) | For the description of this property, please see [getZoom()](../../com.aspose.gridweb/gridworksheet\#getZoom--) |
| [toString()](#toString--) |  |
| [unFreezePanes()](#unFreezePanes--) | Unfreezes panes in the worksheet. |
| [unGroupRows(int firstIndex, int lastIndex)](#unGroupRows-int-int-) | Ungroups rows. |
| [unProtect()](#unProtect--) | unProtects worksheet. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addAutoFilter(int row, int startColumn, int endColumn) {#addAutoFilter-int-int-int-}
```
public void addAutoFilter(int row, int startColumn, int endColumn)
```


Sets the range to which the specified AutoFilter applies.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Row index. |
| startColumn | int | Start column index. |
| endColumn | int | End column Index. |

### addCustomFilter(int row, String critira) {#addCustomFilter-int-java.lang.String-}
```
public void addCustomFilter(int row, String critira)
```


Add custom filter for the specified row. The filter criteria string. notice we use , and ; as split char,so the cell value shall not contains with those split char below are the criteria string examples //column 0 with value 12.3 CELL0 = 12.3 //column 1 with value ABC CELL1 = ABC //column 0 with value 123 or 456 or ABC and column 1 with value ABC CELL0 = 123,456,ABC; CELL1 = ABC

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int |  |
| critira | java.lang.String |  |

### autoFitColumn(int columnIndex) {#autoFitColumn-int-}
```
public void autoFitColumn(int columnIndex)
```


Autofits the column width. AutoFitColumn is an imprecise function.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | int | Column index. |

### autoFitColumn(int columnIndex, int firstRow, int lastRow) {#autoFitColumn-int-int-int-}
```
public void autoFitColumn(int columnIndex, int firstRow, int lastRow)
```


Autofits the column width. This method autofits a row based on content in a range of cells within the row.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | int | Column index. |
| firstRow | int | First row index. |
| lastRow | int | Last row index. |

### autoFitRow(int rowIndex) {#autoFitRow-int-}
```
public void autoFitRow(int rowIndex)
```


Autofits the row height. AutoFitRow is an imprecise function.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | int | Row index. |

### autoFitRow(int rowIndex, int firstColumn, int lastColumn) {#autoFitRow-int-int-int-}
```
public void autoFitRow(int rowIndex, int firstColumn, int lastColumn)
```


Autofits the row height. This method autofits a row based on content in a range of cells within the row.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | int | Row index. |
| firstColumn | int | First column index. |
| lastColumn | int | Last column index. |

### autoFitRow(int startRow, int endRow, int startColumn, int endColumn) {#autoFitRow-int-int-int-int-}
```
public void autoFitRow(int startRow, int endRow, int startColumn, int endColumn)
```


Autofits row height in a rectangle range.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | int | Start row index. |
| endRow | int | End row index. |
| startColumn | int | Start column index. |
| endColumn | int | End column index. |

### autoFitRows() {#autoFitRows--}
```
public void autoFitRows()
```


Autofits all rows in this worksheet.

### autoFitRows(boolean onlyAuto) {#autoFitRows-boolean-}
```
public void autoFitRows(boolean onlyAuto)
```


Autofits all rows in this worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| onlyAuto | boolean | True,only autofits the row height when row height is not customed. |

### autoFitRows(int startRow, int endRow) {#autoFitRows-int-int-}
```
public void autoFitRows(int startRow, int endRow)
```


Autofits row height in a range.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | int | Start row index. |
| endRow | int | End row index. |

### calculateFormula(String formula) {#calculateFormula-java.lang.String-}
```
public Object calculateFormula(String formula)
```


Calculates a formula.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | java.lang.String |  |

**Returns:**
java.lang.Object - 
### clearComments() {#clearComments--}
```
public void clearComments()
```


Clears all comments in designer spreadsheet.

### copy(GridWorksheet sourceSheet) {#copy-com.aspose.gridweb.GridWorksheet-}
```
public void copy(GridWorksheet sourceSheet)
```


Copies contents and formats from another worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceSheet | [GridWorksheet](../../com.aspose.gridweb/gridworksheet) | Source worksheet. |

### createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList) {#createSubtotal-int-int-int-int-int---}
```
public void createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList)
```


Creates subtotal in the sheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnNameRowIndex | int | The row index of the column name row. |
| dataRows | int | The number of the data rows. |
| groupByColumnIndex | int | The column index of the column to be grouped. |
| subtotalFunction | int | The subtotal function type. |
| subtotalColumnIndexList | int[] | The column indexes to be subtotaled. |

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
| subtotalFunction | int | The subtotal function type. |
| subtotalColumnIndexList | int[] | The column indexes to be subtotaled. |
| functionLabel | java.lang.String | The label of subtotal function. |
| grandCellStyle | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | The style of the grand total line. |
| subtotalCellStyle | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | The style of the subtotal line. |
| numberType | int | The number type of the subtotal result cells. |
| customString | java.lang.String | The custome format string of the subtotal result cells. Can be null. |

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
### filterString(int column, String criteria) {#filterString-int-java.lang.String-}
```
public void filterString(int column, String criteria)
```


Sets the filter for the column.notice we shall call AddAutoFilter before calling of filterString The filter criteria string. notice we use comma->"," as split char,so the cell value you want to filter shall not contains with comma filterString(10,"123,456") means column 10 shall contain 123 or 456, filterString(10,"123") means column10 shall contain 123 value split with comma,eg. 123,456,789 or abc

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | int |  |
| criteria | java.lang.String |  |

### freezePanes(int row, int column, int freezedRows, int freezedColumns) {#freezePanes-int-int-int-int-}
```
public void freezePanes(int row, int column, int freezedRows, int freezedColumns)
```


Freezes panes at the specified cell in the worksheet.

Row index and column index cannot all be zero. Number of rows and number of columns also cannot all be zero.

The first two parameters specify the freezed position and the last two parameters specify the area freezed on the left top pane.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Row index. |
| column | int | Column index. |
| freezedRows | int | Number of visible rows in top pane, no more than row index. |
| freezedColumns | int | Number of visible columns in left pane, no more than column index. |

### freezePanes(String cellName, int freezedRows, int freezedColumns) {#freezePanes-java.lang.String-int-int-}
```
public void freezePanes(String cellName, int freezedRows, int freezedColumns)
```


Freezes panes at the specified cell in the worksheet. Row index and column index cannot all be zero. Number of rows and number of columns also cannot all be zero.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | java.lang.String | Cell name. |
| freezedRows | int | Number of visible rows in top pane, no more than row index. |
| freezedColumns | int | Number of visible columns in left pane, no more than column index. |

### getActiveCell() {#getActiveCell--}
```
public String getActiveCell()
```




**Returns:**
java.lang.String
### getBackgroundImage() {#getBackgroundImage--}
```
public byte[] getBackgroundImage()
```


worksheet background image.

**Returns:**
byte[]
### getCells() {#getCells--}
```
public GridCells getCells()
```




**Returns:**
[GridCells](../../com.aspose.gridweb/gridcells)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCodeName() {#getCodeName--}
```
public String getCodeName()
```


Represents worksheet code name. You cannot change the code name while the template file contains VBA/macro.

**Returns:**
java.lang.String
### getColumnCaption(int column) {#getColumnCaption-int-}
```
public String getColumnCaption(int column)
```


Gets the column caption. If the caption is not set, returns empty string.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | int | Column index. |

**Returns:**
java.lang.String - The column caption. If the caption is not set, returns empty string.
### getColumnHeaderToolTip(int colIndex) {#getColumnHeaderToolTip-int-}
```
public String getColumnHeaderToolTip(int colIndex)
```


Gets the columnheader's tooltip text.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| colIndex | int | The column's index. |

**Returns:**
java.lang.String - The tooltip text.
### getColumnReadonly(int columnIndex) {#getColumnReadonly-int-}
```
public boolean getColumnReadonly(int columnIndex)
```


Gets if a column is readonly. this is extended method of GridWeb specifically,it will not keep and take affect in actual excel file

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | int | column index. |

**Returns:**
boolean - If readonly returns true.
### getComments() {#getComments--}
```
public GridCommentCollection getComments()
```




**Returns:**
[GridCommentCollection](../../com.aspose.gridweb/gridcommentcollection)
### getDisplayRightToLeft() {#getDisplayRightToLeft--}
```
public boolean getDisplayRightToLeft()
```




**Returns:**
boolean
### getDisplayZeros() {#getDisplayZeros--}
```
public boolean getDisplayZeros()
```


True if zero values are displayed.

**Returns:**
boolean
### getFirstVisibleColumn() {#getFirstVisibleColumn--}
```
public int getFirstVisibleColumn()
```




**Returns:**
int
### getFirstVisibleRow() {#getFirstVisibleRow--}
```
public int getFirstVisibleRow()
```




**Returns:**
int
### getFreezedPanes() {#getFreezedPanes--}
```
public int[] getFreezedPanes()
```


Gets the freeze panes.

**Returns:**
int[] - Return null means the worksheet is not frozen 0:Row index;1:column;2:freezedRows;3:freezedRows
### getGridActiveCell() {#getGridActiveCell--}
```
public GridCell getGridActiveCell()
```




**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getHyperlinks() {#getHyperlinks--}
```
public GridHyperlinkCollection getHyperlinks()
```


Gets the [GridHyperlinkCollection](../../com.aspose.gridweb/gridhyperlinkcollection) collection.

**Returns:**
[GridHyperlinkCollection](../../com.aspose.gridweb/gridhyperlinkcollection)
### getIndex() {#getIndex--}
```
public int getIndex()
```




**Returns:**
int
### getIsReadonly(int row, int col) {#getIsReadonly-int-int-}
```
public boolean getIsReadonly(int row, int col)
```


Gets whether the cell is readonly.this is an extended attribute of GridWeb ,it will not keep in actual excel file

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int |  |
| col | int |  |

**Returns:**
boolean
### getName() {#getName--}
```
public String getName()
```


the name of the worksheet. The max length of sheet name is 31. And you cannot assign same name(case insensitive) to two worksheets. For example, you cannot set "SheetName1" to the first worksheet and set "SHEETNAME1" to the second worksheet.

**Returns:**
java.lang.String
### getOutlineShown() {#getOutlineShown--}
```
public boolean getOutlineShown()
```


Indicates whether show outline.

**Returns:**
boolean
### getPictures() {#getPictures--}
```
public GridPictureCollection getPictures()
```


Gets a [getPictures()](../../com.aspose.gridweb/gridworksheet\#getPictures--) collection.

**Returns:**
[GridPictureCollection](../../com.aspose.gridweb/gridpicturecollection)
### getPivotTables() {#getPivotTables--}
```
public GridPivotTableCollection getPivotTables()
```


Gets the pivotTables in the worksheet.

**Returns:**
[GridPivotTableCollection](../../com.aspose.gridweb/gridpivottablecollection)
### getRowCaption(int row) {#getRowCaption-int-}
```
public String getRowCaption(int row)
```


Gets the row caption. If the caption is not set, returns empty string.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Row index. |

**Returns:**
java.lang.String - The row caption. If the caption is not set, returns empty string.
### getRowHeaderToolTip(int rowIndex) {#getRowHeaderToolTip-int-}
```
public String getRowHeaderToolTip(int rowIndex)
```


Gets the rowheader's tooltip text.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | int | The row's index. |

**Returns:**
java.lang.String - The tooltip text.
### getRowReadonly(int rowIndex) {#getRowReadonly-int-}
```
public boolean getRowReadonly(int rowIndex)
```


Gets if a row is readonly. this is extended method of GridWeb specifically,it will not keep and take affect in actual excel file

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | int | row index. |

**Returns:**
boolean - If readonly returns true.
### getSelected() {#getSelected--}
```
public boolean getSelected()
```


Indicates whether this worksheet is selected when the workbook is opened.

**Returns:**
boolean
### getShapes() {#getShapes--}
```
public GridShapeCollection getShapes()
```


Gets a [getPictures()](../../com.aspose.gridweb/gridworksheet\#getPictures--) collection.

**Returns:**
[GridShapeCollection](../../com.aspose.gridweb/gridshapecollection)
### getStandardHeight() {#getStandardHeight--}
```
public double getStandardHeight()
```


the default row height in this worksheet,in unit of points.

**Returns:**
double
### getStandardHeightPixels() {#getStandardHeightPixels--}
```
public int getStandardHeightPixels()
```


the default row height in this worksheet,in unit of pixels.

**Returns:**
int
### getTabColor() {#getTabColor--}
```
public Color getTabColor()
```


Represents worksheet tab color. This feature is only supported in ExcelXP(Excel2002) and above version. If you save file as Excel97 or Excel2000 format, it will be omitted.

**Returns:**
[Color](../../com.aspose.gridweb/color)
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
### getWorkbook() {#getWorkbook--}
```
public GridWorkbook getWorkbook()
```




**Returns:**
[GridWorkbook](../../com.aspose.gridweb/gridworkbook)
### getZoom() {#getZoom--}
```
public int getZoom()
```




**Returns:**
int
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
### isGridlinesVisible() {#isGridlinesVisible--}
```
public boolean isGridlinesVisible()
```


a value indicating whether the grid lines are visible.Default is true.

**Returns:**
boolean
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


Indicates if the worksheet is protected.

**Returns:**
boolean
### isSummaryRowBelow() {#isSummaryRowBelow--}
```
public boolean isSummaryRowBelow()
```


Indicates if the summary row will be positioned below the detail rows in the outline.

**Returns:**
boolean
### moveTo(int index) {#moveTo-int-}
```
public void moveTo(int index)
```


Moves the sheet to another location in the spreadsheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | Destination sheet index. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refreshFilter() {#refreshFilter--}
```
public void refreshFilter()
```


Refresh auto filters to hide or unhide the rows.

### removeAutoFilter() {#removeAutoFilter--}
```
public void removeAutoFilter()
```


Remove the auto filter of the worksheet.

### removeSubtotal() {#removeSubtotal--}
```
public void removeSubtotal()
```


Removes subtotal created by the CreateSubtotal method in the sheet.

### resetFilter(int fieldIndex) {#resetFilter-int-}
```
public void resetFilter(int fieldIndex)
```


The integer offset of the field on which you want to apply ,based on the first filter column (from the left of the list; the leftmost field is field 0).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | int |  |

### setActiveCell(String value) {#setActiveCell-java.lang.String-}
```
public void setActiveCell(String value)
```


For the description of this property, please see [getActiveCell()](../../com.aspose.gridweb/gridworksheet\#getActiveCell--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

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

### setBackgroundImage(byte[] value) {#setBackgroundImage-byte---}
```
public void setBackgroundImage(byte[] value)
```


For the description of this property, please see [getBackgroundImage()](../../com.aspose.gridweb/gridworksheet\#getBackgroundImage--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | byte[] |  |

### setColumnCaption(int column, String caption) {#setColumnCaption-int-java.lang.String-}
```
public void setColumnCaption(int column, String caption)
```


Sets the caption for the column.please note this is an extension attribute and can not keep in excel file

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | int | Column index. |
| caption | java.lang.String | The column caption. Pass null or empty string if you want cancel the caption. |

### setColumnHeaderToolTip(int colIndex, String toolTip) {#setColumnHeaderToolTip-int-java.lang.String-}
```
public void setColumnHeaderToolTip(int colIndex, String toolTip)
```


Sets the columnheader's tooltip text.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| colIndex | int | The column's index. |
| toolTip | java.lang.String | The tooltip text. |

### setColumnReadonly(int columnIndex, boolean isReadonly) {#setColumnReadonly-int-boolean-}
```
public void setColumnReadonly(int columnIndex, boolean isReadonly)
```


Sets a column to readonly so user can't delete it from client side. this is extended method of GridWeb specifically,it will not keep and take affect in actual excel file

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | int | column index. |
| isReadonly | boolean | true or false. |

### setDisplayRightToLeft(boolean value) {#setDisplayRightToLeft-boolean-}
```
public void setDisplayRightToLeft(boolean value)
```


For the description of this property, please see [getDisplayRightToLeft()](../../com.aspose.gridweb/gridworksheet\#getDisplayRightToLeft--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDisplayZeros(boolean value) {#setDisplayZeros-boolean-}
```
public void setDisplayZeros(boolean value)
```


For the description of this property, please see [getDisplayZeros()](../../com.aspose.gridweb/gridworksheet\#getDisplayZeros--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

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

### setFirstVisibleColumn(int value) {#setFirstVisibleColumn-int-}
```
public void setFirstVisibleColumn(int value)
```


For the description of this property, please see [getFirstVisibleColumn()](../../com.aspose.gridweb/gridworksheet\#getFirstVisibleColumn--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setFirstVisibleRow(int value) {#setFirstVisibleRow-int-}
```
public void setFirstVisibleRow(int value)
```


For the description of this property, please see [getFirstVisibleRow()](../../com.aspose.gridweb/gridworksheet\#getFirstVisibleRow--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setGridActiveCell(GridCell value) {#setGridActiveCell-com.aspose.gridweb.GridCell-}
```
public void setGridActiveCell(GridCell value)
```


For the description of this property, please see [getGridActiveCell()](../../com.aspose.gridweb/gridworksheet\#getGridActiveCell--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [GridCell](../../com.aspose.gridweb/gridcell) |  |

### setGridlinesVisible(boolean value) {#setGridlinesVisible-boolean-}
```
public void setGridlinesVisible(boolean value)
```


For the description of this property, please see [isGridlinesVisible()](../../com.aspose.gridweb/gridworksheet\#isGridlinesVisible--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setIsReadonly(int row, int col, boolean value) {#setIsReadonly-int-int-boolean-}
```
public void setIsReadonly(int row, int col, boolean value)
```


Sets whether the cell is readonly.this is an extended attribute of GridWeb ,it will not keep in actual excel file

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int |  |
| col | int |  |
| value | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


For the description of this property, please see [getName()](../../com.aspose.gridweb/gridworksheet\#getName--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setOutlineShown(boolean value) {#setOutlineShown-boolean-}
```
public void setOutlineShown(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setProtect() {#setProtect--}
```
public void setProtect()
```


Protects worksheet. This method protects worksheet without password. It can protect worksheet in all versions of Excel file.

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

### setRowCaption(int row, String caption) {#setRowCaption-int-java.lang.String-}
```
public void setRowCaption(int row, String caption)
```


Sets the caption for the row.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Row index. |
| caption | java.lang.String | The row caption. Pass null or empty string if you want cancel the caption. |

### setRowHeaderToolTip(int rowIndex, String toolTip) {#setRowHeaderToolTip-int-java.lang.String-}
```
public void setRowHeaderToolTip(int rowIndex, String toolTip)
```


Sets the rowheader's tooltip text.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | int | The row's index. |
| toolTip | java.lang.String | The tooltip text. |

### setRowReadonly(int rowIndex, boolean isReadonly) {#setRowReadonly-int-boolean-}
```
public void setRowReadonly(int rowIndex, boolean isReadonly)
```


Sets a row to readonly so user can't delete it from client side. this is extended method of GridWeb specifically,it will not keep and take affect in actual excel file

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | int | row index. |
| isReadonly | boolean | true or false. |

### setSelected(boolean value) {#setSelected-boolean-}
```
public void setSelected(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setStandardHeight(double value) {#setStandardHeight-double-}
```
public void setStandardHeight(double value)
```


For the description of this property, please see [getStandardHeight()](../../com.aspose.gridweb/gridworksheet\#getStandardHeight--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setStandardHeightPixels(int value) {#setStandardHeightPixels-int-}
```
public void setStandardHeightPixels(int value)
```


For the description of this property, please see [getStandardHeightPixels()](../../com.aspose.gridweb/gridworksheet\#getStandardHeightPixels--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setSummaryRowBelow(boolean value) {#setSummaryRowBelow-boolean-}
```
public void setSummaryRowBelow(boolean value)
```


For the description of this property, please see [isSummaryRowBelow()](../../com.aspose.gridweb/gridworksheet\#isSummaryRowBelow--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setTabColor(Color value) {#setTabColor-com.aspose.gridweb.Color-}
```
public void setTabColor(Color value)
```


For the description of this property, please see [getTabColor()](../../com.aspose.gridweb/gridworksheet\#getTabColor--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


For the description of this property, please see [getVisible()](../../com.aspose.gridweb/gridworksheet\#getVisible--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setZoom(int value) {#setZoom-int-}
```
public void setZoom(int value)
```


For the description of this property, please see [getZoom()](../../com.aspose.gridweb/gridworksheet\#getZoom--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### unFreezePanes() {#unFreezePanes--}
```
public void unFreezePanes()
```


Unfreezes panes in the worksheet.

### unGroupRows(int firstIndex, int lastIndex) {#unGroupRows-int-int-}
```
public void unGroupRows(int firstIndex, int lastIndex)
```


Ungroups rows. Only removes outter group info.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | int | The first row index to be ungrouped. |
| lastIndex | int | The last row index to be ungrouped. |

### unProtect() {#unProtect--}
```
public void unProtect()
```


unProtects worksheet.

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
