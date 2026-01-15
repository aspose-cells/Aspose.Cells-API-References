---
title: Cells
second_title: Aspose.Cells for Java API Reference
description: Encapsulates a collection of cell relevant objects such as   ...etc.
type: docs
url: /java/com.aspose.cells/cells/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Cells implements Iterable
```

Encapsulates a collection of cell relevant objects, such as [Cell](../../com.aspose.cells/cell), [Row](../../com.aspose.cells/row), ...etc.

**Remarks**

**Example**

```
         Workbook excel = new Workbook();
         	Cells cells = excel.getWorksheets().get(0).getCells();
 
         	//Set default row height
         	cells.setStandardHeight(20);
         	//Set row height
         	cells.setRowHeight(2, 20.5);
 
         	//Set default colum width
         	cells.setStandardWidth(15);
         	//Set column width
         	cells.setColumnWidth(3, 12.57);
 
         	//Merge cells
         	cells.merge(5, 4, 2, 2);
 
         	//Put values to cells
         	cells.get(0, 0).putValue(true);
         	cells.get(0, 1).putValue(1);
         	cells.get(0, 2).putValue("abc");
 
         //Export data
         Object[][] arr = cells.exportArray(0, 0, 10, 10);
```
## Methods

| Method | Description |
| --- | --- |
| [addRange(Range rangeObject)](#addRange-com.aspose.cells.Range-) | Adds a range object reference to cells |
| [applyColumnStyle(int column, Style style, StyleFlag flag)](#applyColumnStyle-int-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Applies formats for a whole column. |
| [applyRowStyle(int row, Style style, StyleFlag flag)](#applyRowStyle-int-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Applies formats for a whole row. |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Applies formats for a whole worksheet. |
| [checkCell(int row, int column)](#checkCell-int-int-) | Gets the [Cell](../../com.aspose.cells/cell) element or null at the specified cell row index and column index. |
| [checkColumn(int columnIndex)](#checkColumn-int-) | Gets the [Column](../../com.aspose.cells/column) element or null at the specified column index. |
| [checkRow(int row)](#checkRow-int-) | Gets the [Row](../../com.aspose.cells/row) element or null at the specified cell row index. |
| [clear()](#clear--) | Clears all data of the worksheet. |
| [clearContents(CellArea range)](#clearContents-com.aspose.cells.CellArea-) | Clears contents of a range. |
| [clearContents(int startRow, int startColumn, int endRow, int endColumn)](#clearContents-int-int-int-int-) | Clears contents of a range. |
| [clearFormats(CellArea range)](#clearFormats-com.aspose.cells.CellArea-) | Clears formatting of a range. |
| [clearFormats(int startRow, int startColumn, int endRow, int endColumn)](#clearFormats-int-int-int-int-) | Clears formatting of a range. |
| [clearMergedCells()](#clearMergedCells--) | Clears all merged ranges. |
| [clearRange(CellArea range)](#clearRange-com.aspose.cells.CellArea-) | Clears contents and formatting of a range. |
| [clearRange(int startRow, int startColumn, int endRow, int endColumn)](#clearRange-int-int-int-int-) | Clears contents and formatting of a range. |
| [convertStringToNumericValue()](#convertStringToNumericValue--) | Converts all string data in the worksheet to numeric value if possible. |
| [copyColumn(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex)](#copyColumn-com.aspose.cells.Cells-int-int-) | Copies data and formats of a whole column. |
| [copyColumns(Cells sourceCells0, int sourceColumnIndex, int destinationColumnIndex, int columnNumber)](#copyColumns-com.aspose.cells.Cells-int-int-int-) | Copies data and formats of a whole column. |
| [copyColumns(Cells sourceCells0, int sourceColumnIndex, int destinationColumnIndex, int columnNumber, PasteOptions pasteOptions)](#copyColumns-com.aspose.cells.Cells-int-int-int-com.aspose.cells.PasteOptions-) | Copies data and formats of a whole column. |
| [copyColumns(Cells sourceCells, int sourceColumnIndex, int sourceTotalColumns, int destinationColumnIndex, int destinationTotalColumns)](#copyColumns-com.aspose.cells.Cells-int-int-int-int-) | Copies data and formats of the whole columns. |
| [copyRow(Cells sourceCells, int sourceRowIndex, int destinationRowIndex)](#copyRow-com.aspose.cells.Cells-int-int-) | Copies data and formats of a whole row. |
| [copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)](#copyRows-com.aspose.cells.Cells-int-int-int-) | Copies data and formats of some whole rows. |
| [copyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions)](#copyRows-com.aspose.cells.Cells-int-int-int-com.aspose.cells.CopyOptions-) | Copies data and formats of some whole rows. |
| [copyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions)](#copyRows-com.aspose.cells.Cells-int-int-int-com.aspose.cells.CopyOptions-com.aspose.cells.PasteOptions-) | Copies data and formats of some whole rows. |
| [createRange(int firstIndex, int number, boolean isVertical)](#createRange-int-int-boolean-) | Creates a [Range](../../com.aspose.cells/range) object from rows of cells or columns of cells. |
| [createRange(int firstRow, int firstColumn, int totalRows, int totalColumns)](#createRange-int-int-int-int-) | Creates a [Range](../../com.aspose.cells/range) object from a range of cells. |
| [createRange(String address)](#createRange-java.lang.String-) | Creates a [Range](../../com.aspose.cells/range) object from an address of the range. |
| [createRange(String upperLeftCell, String lowerRightCell)](#createRange-java.lang.String-java.lang.String-) | Creates a [Range](../../com.aspose.cells/range) object from a range of cells. |
| [deleteBlankColumns()](#deleteBlankColumns--) | Delete all blank columns which do not contain any data. |
| [deleteBlankColumns(DeleteOptions options)](#deleteBlankColumns-com.aspose.cells.DeleteOptions-) | Delete all blank columns which do not contain any data. |
| [deleteBlankRows()](#deleteBlankRows--) | Delete all blank rows which do not contain any data or other object. |
| [deleteBlankRows(DeleteOptions options)](#deleteBlankRows-com.aspose.cells.DeleteOptions-) | Delete all blank rows which do not contain any data or some special objects such as visible comment, pivot table. |
| [deleteColumn(int columnIndex)](#deleteColumn-int-) | Deletes a column. |
| [deleteColumn(int columnIndex, boolean updateReference)](#deleteColumn-int-boolean-) | Deletes a column. |
| [deleteColumns(int columnIndex, int totalColumns, boolean updateReference)](#deleteColumns-int-int-boolean-) | Deletes several columns. |
| [deleteColumns(int columnIndex, int totalColumns, DeleteOptions options)](#deleteColumns-int-int-com.aspose.cells.DeleteOptions-) | Deletes several columns. |
| [deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType)](#deleteRange-int-int-int-int-int-) | Deletes a range of cells and shift cells according to the shift option. |
| [deleteRow(int rowIndex)](#deleteRow-int-) | Deletes a row. |
| [deleteRow(int rowIndex, boolean updateReference)](#deleteRow-int-boolean-) | Deletes a row. |
| [deleteRows(int rowIndex, int totalRows)](#deleteRows-int-int-) | Deletes multiple rows. |
| [deleteRows(int rowIndex, int totalRows, boolean updateReference)](#deleteRows-int-int-boolean-) | Deletes multiple rows in the worksheet. |
| [deleteRows(int rowIndex, int totalRows, DeleteOptions options)](#deleteRows-int-int-com.aspose.cells.DeleteOptions-) | Deletes multiple rows in the worksheet. |
| [dispose()](#dispose--) | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [endCellInColumn(int columnIndex)](#endCellInColumn-int-) | Gets the last cell in this column. |
| [endCellInColumn(int startRow, int endRow, int startColumn, int endColumn)](#endCellInColumn-int-int-int-int-) | Gets the last cell with maximum column index in this range. |
| [endCellInRow(int rowIndex)](#endCellInRow-int-) | Gets the last cell in this row. |
| [endCellInRow(int startRow, int endRow, int startColumn, int endColumn)](#endCellInRow-int-int-int-int-) | Gets the last cell with maximum row index in this range. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)](#exportArray-int-int-int-int-) | Exports data in the [Cells](../../com.aspose.cells/cells) collection to a two-dimension array object. |
| [exportTypeArray(int firstRow, int firstColumn, int totalRows, int totalColumns)](#exportTypeArray-int-int-int-int-) | Exports cell value type in the [Cells](../../com.aspose.cells/cells) collection to a two-dimension array object. |
| [find(Object what, Cell previousCell)](#find-java.lang.Object-com.aspose.cells.Cell-) | Finds the cell containing with the input object. |
| [find(Object what, Cell previousCell, FindOptions findOptions)](#find-java.lang.Object-com.aspose.cells.Cell-com.aspose.cells.FindOptions-) | Finds the cell containing with the input object. |
| [get(int row, int column)](#get-int-int-) | Gets the [Cell](../../com.aspose.cells/cell) element at the specified cell row index and column index. |
| [get(String cellName)](#get-java.lang.String-) | Gets the [Cell](../../com.aspose.cells/cell) element at the specified cell name. |
| [getCellDisplayStyle(int row, int column)](#getCellDisplayStyle-int-int-) | Get the display style of given cell. |
| [getCellDisplayStyle(int row, int column, int adjacentBorders)](#getCellDisplayStyle-int-int-int-) | Get the display style of given cell. |
| [getCellStyle(int row, int column)](#getCellStyle-int-int-) | Get the style of given cell. |
| [getCellsWithPlaceInCellPicture()](#getCellsWithPlaceInCellPicture--) | Gets all cells that contain embedded picture. |
| [getClass()](#getClass--) |  |
| [getColumnOriginalWidthPoint(int column)](#getColumnOriginalWidthPoint-int-) | Gets original column's height in unit of point if the column is hidden |
| [getColumnWidth(int column)](#getColumnWidth-int-) | Gets the width(in unit of characters) of the specified column in normal view |
| [getColumnWidth(int column, boolean isOriginal, int unitType)](#getColumnWidth-int-boolean-int-) | Gets the column width. |
| [getColumnWidthInch(int column)](#getColumnWidthInch-int-) | Gets the width of the specified column in normal view, in units of inches. |
| [getColumnWidthPixel(int column)](#getColumnWidthPixel-int-) | Gets the width of the specified column in normal view, in units of pixel. |
| [getColumnWidthPixel(int column, boolean original)](#getColumnWidthPixel-int-boolean-) | Gets the width of the specified column in normal view, in units of pixel. |
| [getColumns()](#getColumns--) | Gets the collection of [Column](../../com.aspose.cells/column) objects that represents the individual columns in this worksheet. |
| [getCount()](#getCount--) | Gets the total count of instantiated Cell objects. |
| [getCountLarge()](#getCountLarge--) | Gets the total count of instantiated Cell objects. |
| [getDependents(boolean isAll, int row, int column)](#getDependents-boolean-int-int-) | Get all cells which refer to the specific cell. |
| [getDependentsInCalculation(int row, int column, boolean recursive)](#getDependentsInCalculation-int-int-boolean-) | Gets all cells whose calculated result depends on specific cell. |
| [getFirstCell()](#getFirstCell--) | Gets the first cell in this worksheet. |
| [getFirstDataRow(int column)](#getFirstDataRow-int-) | Gets the first row index of cell which contains data in the specified column. |
| [getGroupedColumnOutlineLevel(int columnIndex)](#getGroupedColumnOutlineLevel-int-) | Gets the outline level (zero-based) of the column. |
| [getGroupedRowOutlineLevel(int rowIndex)](#getGroupedRowOutlineLevel-int-) | Gets the outline level (zero-based) of the row. |
| [getLastCell()](#getLastCell--) | Gets the last cell in this worksheet. |
| [getLastDataRow(int column)](#getLastDataRow-int-) | Gets the last row index of cell which contains data in the specified column. |
| [getMaxColumn()](#getMaxColumn--) | Maximum column index of those cells that have been instantiated in the collection(does not include the column where style is defined for the whole column but no cell has been instantiated in it). |
| [getMaxDataColumn()](#getMaxDataColumn--) | Maximum column index of cell which contains data. |
| [getMaxDataRow()](#getMaxDataRow--) | Maximum row index of cell which contains data. |
| [getMaxDisplayRange()](#getMaxDisplayRange--) | Gets the max range which includes data, merged cells and shapes. |
| [getMaxGroupedColumnOutlineLevel()](#getMaxGroupedColumnOutlineLevel--) | Gets the max grouped column outline level (zero-based). |
| [getMaxGroupedRowOutlineLevel()](#getMaxGroupedRowOutlineLevel--) | Gets the max grouped row outline level (zero-based). |
| [getMaxRow()](#getMaxRow--) | Maximum row index of cell which contains data or style. |
| [getMemorySetting()](#getMemorySetting--) | Gets the memory usage option for this cells. |
| [getMergedAreas()](#getMergedAreas--) | Gets all merged cells. |
| [getMergedCells()](#getMergedCells--) | Gets the collection of merged cells. |
| [getMinColumn()](#getMinColumn--) | Minimum column index of those cells that have been instantiated in the collection(does not include the column where style is defined for the whole column but no cell has been instantiated in it). |
| [getMinDataColumn()](#getMinDataColumn--) | Minimum column index of cell which contains data. |
| [getMinDataRow()](#getMinDataRow--) | Minimum row index of cell which contains data. |
| [getMinRow()](#getMinRow--) | Minimum row index of cell which contains data or style. |
| [getMultiThreadReading()](#getMultiThreadReading--) | Gets whether the cells data model should support Multi-Thread reading. |
| [getOdsCellFields()](#getOdsCellFields--) | Gets the list of fields of ods. |
| [getPreserveString()](#getPreserveString--) | Gets a value indicating whether all worksheet values are preserved as strings. |
| [getRanges()](#getRanges--) | Gets the collection of [Range](../../com.aspose.cells/range) objects created at run time. |
| [getRowEnumerator()](#getRowEnumerator--) | Gets the rows enumerator. |
| [getRowHeight(int row)](#getRowHeight-int-) | Gets the height of a specified row, in unit of points. |
| [getRowHeight(int row, boolean isOriginal, int unitType)](#getRowHeight-int-boolean-int-) | Gets row's height. |
| [getRowHeightInch(int row)](#getRowHeightInch-int-) | Gets the height of a specified row in unit of inches. |
| [getRowHeightPixel(int row)](#getRowHeightPixel-int-) | Gets the height of a specified row in unit of pixel. |
| [getRowOriginalHeightPoint(int row)](#getRowOriginalHeightPoint-int-) | Gets original row's height in unit of point if the row is hidden |
| [getRows()](#getRows--) | Gets the collection of [Row](../../com.aspose.cells/row) objects that represents the individual rows in this worksheet. |
| [getStandardHeight()](#getStandardHeight--) | Gets the default row height in this worksheet, in unit of points. |
| [getStandardHeightInch()](#getStandardHeightInch--) | Gets the default row height in this worksheet, in unit of inches. |
| [getStandardHeightPixels()](#getStandardHeightPixels--) | Gets the default row height in this worksheet, in unit of pixels. |
| [getStandardWidth()](#getStandardWidth--) | Gets the default column width in the worksheet, in unit of characters. |
| [getStandardWidthInch()](#getStandardWidthInch--) | Gets the default column width in the worksheet, in unit of inches. |
| [getStandardWidthPixels()](#getStandardWidthPixels--) | Gets the default column width in the worksheet, in unit of pixels. |
| [getStyle()](#getStyle--) | Gets the default style of the worksheet. |
| [getViewColumnWidthPixel(int column)](#getViewColumnWidthPixel-int-) | Get the width in different view type. |
| [getViewRowHeight(int row)](#getViewRowHeight-int-) | Gets the height of a specified row. |
| [getViewRowHeightInch(int row)](#getViewRowHeightInch-int-) | Gets the height of a specified row in unit of inches. |
| [groupColumns(int firstIndex, int lastIndex)](#groupColumns-int-int-) | Groups columns. |
| [groupColumns(int firstIndex, int lastIndex, boolean isHidden)](#groupColumns-int-int-boolean-) | Groups columns. |
| [groupRows(int firstIndex, int lastIndex)](#groupRows-int-int-) | Groups rows. |
| [groupRows(int firstIndex, int lastIndex, boolean isHidden)](#groupRows-int-int-boolean-) | Groups rows. |
| [hashCode()](#hashCode--) |  |
| [hideColumn(int column)](#hideColumn-int-) | Hides a column. |
| [hideColumns(int column, int totalColumns)](#hideColumns-int-int-) | Hide multiple columns. |
| [hideGroupDetail(boolean isVertical, int index)](#hideGroupDetail-boolean-int-) | Collapses the grouped rows/columns. |
| [hideRow(int row)](#hideRow-int-) | Hides a row. |
| [hideRows(int row, int totalRows)](#hideRows-int-int-) | Hides multiple rows. |
| [importArray(double[] doubleArray, int firstRow, int firstColumn, boolean isVertical)](#importArray-double---int-int-boolean-) | Imports an array of double into a worksheet. |
| [importArray(double[][] doubleArray, int firstRow, int firstColumn)](#importArray-double-----int-int-) | Imports a two-dimension array of double into a worksheet. |
| [importArray(int[] intArray, int firstRow, int firstColumn, boolean isVertical)](#importArray-int---int-int-boolean-) | Imports an array of integer into a worksheet. |
| [importArray(int[][] intArray, int firstRow, int firstColumn)](#importArray-int-----int-int-) | Imports a two-dimension array of integer into a worksheet. |
| [importArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical)](#importArray-java.lang.String---int-int-boolean-) | Imports an array of string into a worksheet. |
| [importArray(String[][] stringArray, int firstRow, int firstColumn)](#importArray-java.lang.String-----int-int-) | Imports a two-dimension array of string into a worksheet. |
| [importArrayList(ArrayList arrayList, int firstRow, int firstColumn, boolean isVertical)](#importArrayList-java.util.ArrayList-int-int-boolean-) | Imports an arraylist of data into a worksheet. |
| [importCSV(InputStream stream, TxtLoadOptions options, int firstRow, int firstColumn)](#importCSV-java.io.InputStream-com.aspose.cells.TxtLoadOptions-int-int-) | Import a CSV file to the cells. |
| [importCSV(InputStream stream, String splitter, boolean convertNumericData, int firstRow, int firstColumn)](#importCSV-java.io.InputStream-java.lang.String-boolean-int-int-) | Import a CSV file to the cells. |
| [importCSV(String fileName, TxtLoadOptions options, int firstRow, int firstColumn)](#importCSV-java.lang.String-com.aspose.cells.TxtLoadOptions-int-int-) | Import a CSV file to the cells. |
| [importCSV(String fileName, String splitter, boolean convertNumericData, int firstRow, int firstColumn)](#importCSV-java.lang.String-java.lang.String-boolean-int-int-) | Import a CSV file to the cells. |
| [importCustomObjects(Collection list, int firstRow, int firstColumn, ImportTableOptions options)](#importCustomObjects-java.util.Collection-int-int-com.aspose.cells.ImportTableOptions-) | Imports custom objects. |
| [importCustomObjects(Collection list, String[] propertyNames, boolean isPropertyNameShown, int firstRow, int firstColumn, int rowNumber, boolean insertRows, String dateFormatString, boolean convertStringToNumber)](#importCustomObjects-java.util.Collection-java.lang.String---boolean-int-int-int-boolean-java.lang.String-boolean-) | Imports custom objects. |
| [importData(ICellsDataTable table, int firstRow, int firstColumn, ImportTableOptions options)](#importData-com.aspose.cells.ICellsDataTable-int-int-com.aspose.cells.ImportTableOptions-) | Import data from custom data table. |
| [importFormulaArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical)](#importFormulaArray-java.lang.String---int-int-boolean-) | Imports an array of formula into a worksheet. |
| [importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical)](#importObjectArray-java.lang.Object---int-int-boolean-) | Imports an array of data into a worksheet. |
| [importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical, int skip)](#importObjectArray-java.lang.Object---int-int-boolean-int-) | Imports an array of data into a worksheet. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown)](#importResultSet-java.sql.ResultSet-int-int-boolean-) | Imports data in a ResultSet object to the worksheet. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber)](#importResultSet-java.sql.ResultSet-int-int-boolean-java.lang.String-boolean-) | Imports data in a ResultSet object to the worksheet. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, ImportTableOptions options)](#importResultSet-java.sql.ResultSet-int-int-com.aspose.cells.ImportTableOptions-) | Imports data in a ResultSet object to the worksheet. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown)](#importResultSet-java.sql.ResultSet-int-int-int-int-boolean-) | Imports data in a ResultSet object to the worksheet. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber)](#importResultSet-java.sql.ResultSet-int-int-int-int-boolean-java.lang.String-boolean-) | Imports data in a ResultSet object to the worksheet. |
| [importResultSet(ResultSet rs, String startCell, boolean isFieldNameShown)](#importResultSet-java.sql.ResultSet-java.lang.String-boolean-) | Imports data in a ResultSet object to the worksheet. |
| [importResultSet(ResultSet rs, String startCell, ImportTableOptions options)](#importResultSet-java.sql.ResultSet-java.lang.String-com.aspose.cells.ImportTableOptions-) | Imports data in a ResultSet object to the worksheet. |
| [importResultSet(ResultSet rs, String startCell, int rowNum, int columnNum, boolean isFieldNameShown)](#importResultSet-java.sql.ResultSet-java.lang.String-int-int-boolean-) | Imports data in a ResultSet object to the worksheet. |
| [importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn)](#importTwoDimensionArray-java.lang.Object-----int-int-) | Imports a two-dimension array of data into a worksheet. |
| [importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn, boolean convertStringToNumber)](#importTwoDimensionArray-java.lang.Object-----int-int-boolean-) | Imports a two-dimension array of data into a worksheet. |
| [importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, boolean convertStringToNumber)](#importTwoDimensionArray-java.lang.Object-----java.lang.Object-----int-int-boolean-) | Imports a two-dimension array of data into a worksheet. |
| [importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, TxtLoadOptions opts)](#importTwoDimensionArray-java.lang.Object-----java.lang.Object-----int-int-com.aspose.cells.TxtLoadOptions-) | Imports a two-dimension array of data into a worksheet. |
| [insertColumn(int columnIndex)](#insertColumn-int-) | Inserts a new column into the worksheet. |
| [insertColumn(int columnIndex, boolean updateReference)](#insertColumn-int-boolean-) | Inserts a new column into the worksheet. |
| [insertColumns(int columnIndex, int totalColumns)](#insertColumns-int-int-) | Inserts some columns into the worksheet. |
| [insertColumns(int columnIndex, int totalColumns, boolean updateReference)](#insertColumns-int-int-boolean-) | Inserts some columns into the worksheet. |
| [insertColumns(int columnIndex, int totalColumns, InsertOptions options)](#insertColumns-int-int-com.aspose.cells.InsertOptions-) | Inserts some columns into the worksheet. |
| [insertCutCells(Range cutRange, int row, int column, int shiftType)](#insertCutCells-com.aspose.cells.Range-int-int-int-) | Insert cut range. |
| [insertRange(CellArea area, int shiftType)](#insertRange-com.aspose.cells.CellArea-int-) | Inserts a range of cells and shift cells according to the shift option. |
| [insertRange(CellArea area, int shiftNumber, int shiftType)](#insertRange-com.aspose.cells.CellArea-int-int-) | Inserts a range of cells and shift cells according to the shift option. |
| [insertRange(CellArea area, int shiftNumber, int shiftType, boolean updateReference)](#insertRange-com.aspose.cells.CellArea-int-int-boolean-) | Inserts a range of cells and shift cells according to the shift option. |
| [insertRow(int rowIndex)](#insertRow-int-) | Inserts a new row into the worksheet. |
| [insertRows(int rowIndex, int totalRows)](#insertRows-int-int-) | Inserts multiple rows into the worksheet. |
| [insertRows(int rowIndex, int totalRows, boolean updateReference)](#insertRows-int-int-boolean-) | Inserts multiple rows into the worksheet. |
| [insertRows(int rowIndex, int totalRows, InsertOptions options)](#insertRows-int-int-com.aspose.cells.InsertOptions-) | Inserts multiple rows into the worksheet. |
| [isBlankColumn(int columnIndex)](#isBlankColumn-int-) | Checks whether given column is blank(does not contain any data). |
| [isColumnHidden(int columnIndex)](#isColumnHidden-int-) | Checks whether a column at given index is hidden. |
| [isDefaultColumnHidden()](#isDefaultColumnHidden--) |  |
| [isDefaultRowHeightMatched()](#isDefaultRowHeightMatched--) | Indicates that row height and default font height matches |
| [isDefaultRowHidden()](#isDefaultRowHidden--) | Indicates whether the row is default hidden. |
| [isDeletingRangeEnabled(int startRow, int startColumn, int totalRows, int totalColumns)](#isDeletingRangeEnabled-int-int-int-int-) | Check whether the range could be deleted. |
| [isRowHidden(int rowIndex)](#isRowHidden-int-) | Checks whether a row at given index is hidden. |
| [iterator()](#iterator--) | Gets the cells enumerator. |
| [linkToXmlMap(String mapName, int row, int column, String path)](#linkToXmlMap-java.lang.String-int-int-java.lang.String-) | Link to a xml map. |
| [merge(int firstRow, int firstColumn, int totalRows, int totalColumns)](#merge-int-int-int-int-) | Merges a specified range of cells into a single cell. |
| [merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean mergeConflict)](#merge-int-int-int-int-boolean-) | Merges a specified range of cells into a single cell. |
| [merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean checkConflict, boolean mergeConflict)](#merge-int-int-int-int-boolean-boolean-) | Merges a specified range of cells into a single cell. |
| [moveRange(CellArea sourceArea, int destRow, int destColumn)](#moveRange-com.aspose.cells.CellArea-int-int-) | Moves the range. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeDuplicates()](#removeDuplicates--) | Removes duplicate rows in the sheet. |
| [removeDuplicates(int startRow, int startColumn, int endRow, int endColumn)](#removeDuplicates-int-int-int-int-) | Removes duplicate values in the range. |
| [removeDuplicates(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders, int[] columnOffsets)](#removeDuplicates-int-int-int-int-boolean-int---) | Removes duplicate data of the range. |
| [removeFormulas()](#removeFormulas--) | Removes all formula and replaces with the value of the formula. |
| [retrieveSubtotalSetting(CellArea ca)](#retrieveSubtotalSetting-com.aspose.cells.CellArea-) | Retrieves subtotals setting of the range. |
| [setColumnWidth(int column, double width)](#setColumnWidth-int-double-) | Sets the width of the specified column in normal view. |
| [setColumnWidthInch(int column, double inches)](#setColumnWidthInch-int-double-) | Sets column width in unit of inches in normal view. |
| [setColumnWidthPixel(int column, int pixels)](#setColumnWidthPixel-int-int-) | Sets column width in unit of pixels in normal view. |
| [setDefaultColumnHidden(boolean value)](#setDefaultColumnHidden-boolean-) |  |
| [setDefaultRowHeightMatched(boolean value)](#setDefaultRowHeightMatched-boolean-) | Indicates that row height and default font height matches |
| [setDefaultRowHidden(boolean value)](#setDefaultRowHidden-boolean-) | Indicates whether the row is default hidden. |
| [setMemorySetting(int value)](#setMemorySetting-int-) | Sets the memory usage option for this cells. |
| [setMultiThreadReading(boolean value)](#setMultiThreadReading-boolean-) | Sets whether the cells data model should support Multi-Thread reading. |
| [setPreserveString(boolean value)](#setPreserveString-boolean-) | Sets a value indicating whether all worksheet values are preserved as strings. |
| [setRowHeight(int row, double height)](#setRowHeight-int-double-) | Sets the height of the specified row. |
| [setRowHeightInch(int row, double inches)](#setRowHeightInch-int-double-) | Sets row height in unit of inches. |
| [setRowHeightPixel(int row, int pixels)](#setRowHeightPixel-int-int-) | Sets row height in unit of pixels. |
| [setStandardHeight(double value)](#setStandardHeight-double-) | Sets the default row height in this worksheet, in unit of points. |
| [setStandardHeightInch(double value)](#setStandardHeightInch-double-) | Sets the default row height in this worksheet, in unit of inches. |
| [setStandardHeightPixels(int value)](#setStandardHeightPixels-int-) | Sets the default row height in this worksheet, in unit of pixels. |
| [setStandardWidth(double value)](#setStandardWidth-double-) | Sets the default column width in the worksheet, in unit of characters. |
| [setStandardWidthInch(double value)](#setStandardWidthInch-double-) | Sets the default column width in the worksheet, in unit of inches. |
| [setStandardWidthPixels(int value)](#setStandardWidthPixels-int-) | Sets the default column width in the worksheet, in unit of pixels. |
| [setStyle(Style value)](#setStyle-com.aspose.cells.Style-) | Sets the default style of the worksheet. |
| [setViewColumnWidthPixel(int column, int pixels)](#setViewColumnWidthPixel-int-int-) | Sets the width of the column in different view. |
| [showGroupDetail(boolean isVertical, int index)](#showGroupDetail-boolean-int-) | Expands the grouped rows/columns. |
| [subtotal(CellArea ca, int groupBy, int function, int[] totalList)](#subtotal-com.aspose.cells.CellArea-int-int-int---) | Creates subtotals for the range. |
| [subtotal(CellArea ca, int groupBy, int function, int[] totalList, boolean replace, boolean pageBreaks, boolean summaryBelowData)](#subtotal-com.aspose.cells.CellArea-int-int-int---boolean-boolean-boolean-) | Creates subtotals for the range. |
| [textToColumns(int row, int column, int totalRows, TxtLoadOptions options)](#textToColumns-int-int-int-com.aspose.cells.TxtLoadOptions-) | Splits content in specified column into multiple columns.. |
| [toString()](#toString--) |  |
| [unMerge(int firstRow, int firstColumn, int totalRows, int totalColumns)](#unMerge-int-int-int-int-) | Unmerges a specified range of merged cells. |
| [ungroupColumns(int firstIndex, int lastIndex)](#ungroupColumns-int-int-) | Ungroups columns. |
| [ungroupRows(int firstIndex, int lastIndex)](#ungroupRows-int-int-) | Ungroups rows. |
| [ungroupRows(int firstIndex, int lastIndex, boolean isAll)](#ungroupRows-int-int-boolean-) | Ungroups rows. |
| [unhideColumn(int column, double width)](#unhideColumn-int-double-) | Unhides a column |
| [unhideColumns(int column, int totalColumns, double width)](#unhideColumns-int-int-double-) | Unhide multiple columns. |
| [unhideRow(int row, double height)](#unhideRow-int-double-) | Unhides a row. |
| [unhideRows(int row, int totalRows, double height)](#unhideRows-int-int-double-) | Unhides the hidden rows. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addRange(Range rangeObject) {#addRange-com.aspose.cells.Range-}
```
public void addRange(Range rangeObject)
```


Adds a range object reference to cells

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rangeObject | [Range](../../com.aspose.cells/range) | The range object will be contained in the cells |

### applyColumnStyle(int column, Style style, StyleFlag flag) {#applyColumnStyle-int-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyColumnStyle(int column, Style style, StyleFlag flag)
```


Applies formats for a whole column.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | int | The column index. |
| style | [Style](../../com.aspose.cells/style) | The style object which will be applied. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Flags which indicates applied formatting properties. |

### applyRowStyle(int row, Style style, StyleFlag flag) {#applyRowStyle-int-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyRowStyle(int row, Style style, StyleFlag flag)
```


Applies formats for a whole row.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | The row index. |
| style | [Style](../../com.aspose.cells/style) | The style object which will be applied. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Flags which indicates applied formatting properties. |

### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


Applies formats for a whole worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | The style object which will be applied. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Flags which indicates applied formatting properties. |

### checkCell(int row, int column) {#checkCell-int-int-}
```
public Cell checkCell(int row, int column)
```


Gets the [Cell](../../com.aspose.cells/cell) element or null at the specified cell row index and column index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Row index |
| column | int | Column index |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Return Cell object if a Cell object exists. Return null if the cell does not exist.
### checkColumn(int columnIndex) {#checkColumn-int-}
```
public Column checkColumn(int columnIndex)
```


Gets the [Column](../../com.aspose.cells/column) element or null at the specified column index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | int | The column index. |

**Returns:**
[Column](../../com.aspose.cells/column) - The Column object.
### checkRow(int row) {#checkRow-int-}
```
public Row checkRow(int row)
```


Gets the [Row](../../com.aspose.cells/row) element or null at the specified cell row index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Row index |

**Returns:**
[Row](../../com.aspose.cells/row) - Returns [Row](../../com.aspose.cells/row) object If the row object does exist, otherwise returns null.
### clear() {#clear--}
```
public void clear()
```


Clears all data of the worksheet.

### clearContents(CellArea range) {#clearContents-com.aspose.cells.CellArea-}
```
public void clearContents(CellArea range)
```


Clears contents of a range.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| range | [CellArea](../../com.aspose.cells/cellarea) | Range to be cleared. |

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

### clearFormats(CellArea range) {#clearFormats-com.aspose.cells.CellArea-}
```
public void clearFormats(CellArea range)
```


Clears formatting of a range.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| range | [CellArea](../../com.aspose.cells/cellarea) | Range to be cleared. |

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

### clearMergedCells() {#clearMergedCells--}
```
public void clearMergedCells()
```


Clears all merged ranges.

### clearRange(CellArea range) {#clearRange-com.aspose.cells.CellArea-}
```
public void clearRange(CellArea range)
```


Clears contents and formatting of a range.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| range | [CellArea](../../com.aspose.cells/cellarea) | Range to be cleared. |

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

### convertStringToNumericValue() {#convertStringToNumericValue--}
```
public void convertStringToNumericValue()
```


Converts all string data in the worksheet to numeric value if possible.

### copyColumn(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex) {#copyColumn-com.aspose.cells.Cells-int-int-}
```
public void copyColumn(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex)
```


Copies data and formats of a whole column.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | Source Cells object contains data and formats to copy. |
| sourceColumnIndex | int | Source column index. |
| destinationColumnIndex | int | Destination column index. |

### copyColumns(Cells sourceCells0, int sourceColumnIndex, int destinationColumnIndex, int columnNumber) {#copyColumns-com.aspose.cells.Cells-int-int-int-}
```
public void copyColumns(Cells sourceCells0, int sourceColumnIndex, int destinationColumnIndex, int columnNumber)
```


Copies data and formats of a whole column.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells0 | [Cells](../../com.aspose.cells/cells) | Source Cells object contains data and formats to copy. |
| sourceColumnIndex | int | Source column index. |
| destinationColumnIndex | int | Destination column index. |
| columnNumber | int | The copied column number. |

### copyColumns(Cells sourceCells0, int sourceColumnIndex, int destinationColumnIndex, int columnNumber, PasteOptions pasteOptions) {#copyColumns-com.aspose.cells.Cells-int-int-int-com.aspose.cells.PasteOptions-}
```
public void copyColumns(Cells sourceCells0, int sourceColumnIndex, int destinationColumnIndex, int columnNumber, PasteOptions pasteOptions)
```


Copies data and formats of a whole column.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells0 | [Cells](../../com.aspose.cells/cells) | Source Cells object contains data and formats to copy. |
| sourceColumnIndex | int | Source column index. |
| destinationColumnIndex | int | Destination column index. |
| columnNumber | int | The copied column number. |
| pasteOptions | [PasteOptions](../../com.aspose.cells/pasteoptions) | the options of pasting. |

### copyColumns(Cells sourceCells, int sourceColumnIndex, int sourceTotalColumns, int destinationColumnIndex, int destinationTotalColumns) {#copyColumns-com.aspose.cells.Cells-int-int-int-int-}
```
public void copyColumns(Cells sourceCells, int sourceColumnIndex, int sourceTotalColumns, int destinationColumnIndex, int destinationTotalColumns)
```


Copies data and formats of the whole columns.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | Source Cells object contains data and formats to copy. |
| sourceColumnIndex | int | Source column index. |
| sourceTotalColumns | int | The number of the source columns. |
| destinationColumnIndex | int | Destination column index. |
| destinationTotalColumns | int | The number of the destination columns. |

### copyRow(Cells sourceCells, int sourceRowIndex, int destinationRowIndex) {#copyRow-com.aspose.cells.Cells-int-int-}
```
public void copyRow(Cells sourceCells, int sourceRowIndex, int destinationRowIndex)
```


Copies data and formats of a whole row.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | Source Cells object contains data and formats to copy. |
| sourceRowIndex | int | Source row index. |
| destinationRowIndex | int | Destination row index. |

### copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber) {#copyRows-com.aspose.cells.Cells-int-int-int-}
```
public void copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)
```


Copies data and formats of some whole rows.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | Source Cells object contains data and formats to copy. |
| sourceRowIndex | int | Source row index. |
| destinationRowIndex | int | Destination row index. |
| rowNumber | int | The copied row number. |

### copyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions) {#copyRows-com.aspose.cells.Cells-int-int-int-com.aspose.cells.CopyOptions-}
```
public void copyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions)
```


Copies data and formats of some whole rows.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells0 | [Cells](../../com.aspose.cells/cells) | Source Cells object contains data and formats to copy. |
| sourceRowIndex | int | Source row index. |
| destinationRowIndex | int | Destination row index. |
| rowNumber | int | The copied row number. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | The copy options. |

### copyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions) {#copyRows-com.aspose.cells.Cells-int-int-int-com.aspose.cells.CopyOptions-com.aspose.cells.PasteOptions-}
```
public void copyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions)
```


Copies data and formats of some whole rows.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells0 | [Cells](../../com.aspose.cells/cells) | Source Cells object contains data and formats to copy. |
| sourceRowIndex | int | Source row index. |
| destinationRowIndex | int | Destination row index. |
| rowNumber | int | The copied row number. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | The copy options. |
| pasteOptions | [PasteOptions](../../com.aspose.cells/pasteoptions) | the options of pasting. |

### createRange(int firstIndex, int number, boolean isVertical) {#createRange-int-int-boolean-}
```
public Range createRange(int firstIndex, int number, boolean isVertical)
```


Creates a [Range](../../com.aspose.cells/range) object from rows of cells or columns of cells.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | int | First row index or first column index, zero based. |
| number | int | Total number of rows or columns, one based. |
| isVertical | boolean | True - Range created from columns of cells. False - Range created from rows of cells. |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object.
### createRange(int firstRow, int firstColumn, int totalRows, int totalColumns) {#createRange-int-int-int-int-}
```
public Range createRange(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


Creates a [Range](../../com.aspose.cells/range) object from a range of cells.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | int | First row of this range |
| firstColumn | int | First column of this range |
| totalRows | int | Number of rows |
| totalColumns | int | Number of columns |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object
### createRange(String address) {#createRange-java.lang.String-}
```
public Range createRange(String address)
```


Creates a [Range](../../com.aspose.cells/range) object from an address of the range.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| address | java.lang.String | The address of the range. |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object
### createRange(String upperLeftCell, String lowerRightCell) {#createRange-java.lang.String-java.lang.String-}
```
public Range createRange(String upperLeftCell, String lowerRightCell)
```


Creates a [Range](../../com.aspose.cells/range) object from a range of cells.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftCell | java.lang.String | Upper left cell name. |
| lowerRightCell | java.lang.String | Lower right cell name. |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object
### deleteBlankColumns() {#deleteBlankColumns--}
```
public void deleteBlankColumns()
```


Delete all blank columns which do not contain any data.

### deleteBlankColumns(DeleteOptions options) {#deleteBlankColumns-com.aspose.cells.DeleteOptions-}
```
public void deleteBlankColumns(DeleteOptions options)
```


Delete all blank columns which do not contain any data.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [DeleteOptions](../../com.aspose.cells/deleteoptions) | The options of deleting range. |

### deleteBlankRows() {#deleteBlankRows--}
```
public void deleteBlankRows()
```


Delete all blank rows which do not contain any data or other object.

### deleteBlankRows(DeleteOptions options) {#deleteBlankRows-com.aspose.cells.DeleteOptions-}
```
public void deleteBlankRows(DeleteOptions options)
```


Delete all blank rows which do not contain any data or some special objects such as visible comment, pivot table.

**Remarks**

For blank rows that will be deleted, it is not only required that [Row.isBlank()](../../com.aspose.cells/row\#isBlank--) should be true, but also there should be no visible comment defined for any cell in those rows, and no pivot table whose range intersects with them.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [DeleteOptions](../../com.aspose.cells/deleteoptions) | The options of deleting range. |

### deleteColumn(int columnIndex) {#deleteColumn-int-}
```
public void deleteColumn(int columnIndex)
```


Deletes a column.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | int | Index of the column to be deleted. |

### deleteColumn(int columnIndex, boolean updateReference) {#deleteColumn-int-boolean-}
```
public void deleteColumn(int columnIndex, boolean updateReference)
```


Deletes a column.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | int | Index of the column to be deleted. |
| updateReference | boolean | Indicates whether update references in other worksheets. |

### deleteColumns(int columnIndex, int totalColumns, boolean updateReference) {#deleteColumns-int-int-boolean-}
```
public void deleteColumns(int columnIndex, int totalColumns, boolean updateReference)
```


Deletes several columns.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | int | Index of the first column to be deleted. |
| totalColumns | int | Count of columns to be deleted. |
| updateReference | boolean | Indicates whether update references in other worksheets. |

### deleteColumns(int columnIndex, int totalColumns, DeleteOptions options) {#deleteColumns-int-int-com.aspose.cells.DeleteOptions-}
```
public void deleteColumns(int columnIndex, int totalColumns, DeleteOptions options)
```


Deletes several columns.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | int | Index of the first column to be deleted. |
| totalColumns | int | Count of columns to be deleted. |
| options | [DeleteOptions](../../com.aspose.cells/deleteoptions) | Options for the deleting operation |

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
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). Shift cells option. |

### deleteRow(int rowIndex) {#deleteRow-int-}
```
public void deleteRow(int rowIndex)
```


Deletes a row.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | int | Index of the row to be deleted. |

### deleteRow(int rowIndex, boolean updateReference) {#deleteRow-int-boolean-}
```
public void deleteRow(int rowIndex, boolean updateReference)
```


Deletes a row.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | int | Index of the row to be deleted. |
| updateReference | boolean | Indicates whether update references in other worksheets. |

### deleteRows(int rowIndex, int totalRows) {#deleteRows-int-int-}
```
public boolean deleteRows(int rowIndex, int totalRows)
```


Deletes multiple rows.

**Remarks**

If the deleted range contains the top part(not whole) of the table(ListObject), the ranged could not be deleted and nothing will be done. It works in the same way with MS Excel.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | int | The first row index to be deleted. |
| totalRows | int | Count of rows to be deleted. |

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
| rowIndex | int | Index of the first row to be deleted. |
| totalRows | int | Count of rows to be deleted. |
| updateReference | boolean | Indicates whether update references in other worksheets. |

**Returns:**
boolean - 
### deleteRows(int rowIndex, int totalRows, DeleteOptions options) {#deleteRows-int-int-com.aspose.cells.DeleteOptions-}
```
public boolean deleteRows(int rowIndex, int totalRows, DeleteOptions options)
```


Deletes multiple rows in the worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | int | Index of the first row to be deleted. |
| totalRows | int | Count of rows to be deleted. |
| options | [DeleteOptions](../../com.aspose.cells/deleteoptions) | Options for the deleting operation |

**Returns:**
boolean - 
### dispose() {#dispose--}
```
public void dispose()
```


Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources.

### endCellInColumn(int columnIndex) {#endCellInColumn-int-}
```
public Cell endCellInColumn(int columnIndex)
```


Gets the last cell in this column.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | int | Column index. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### endCellInColumn(int startRow, int endRow, int startColumn, int endColumn) {#endCellInColumn-int-int-int-int-}
```
public Cell endCellInColumn(int startRow, int endRow, int startColumn, int endColumn)
```


Gets the last cell with maximum column index in this range.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | int | Start row index. |
| endRow | int | End row index. |
| startColumn | int | Start column index. |
| endColumn | int | End column index. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### endCellInRow(int rowIndex) {#endCellInRow-int-}
```
public Cell endCellInRow(int rowIndex)
```


Gets the last cell in this row.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | int | Row index. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### endCellInRow(int startRow, int endRow, int startColumn, int endColumn) {#endCellInRow-int-int-int-int-}
```
public Cell endCellInRow(int startRow, int endRow, int startColumn, int endColumn)
```


Gets the last cell with maximum row index in this range.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | int | Start row index. |
| endRow | int | End row index. |
| startColumn | int | Start column index. |
| endColumn | int | End column index. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
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


Exports data in the [Cells](../../com.aspose.cells/cells) collection to a two-dimension array object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | int | The row number of the first cell to export out. |
| firstColumn | int | The column number of the first cell to export out. |
| totalRows | int | Number of rows to be exported |
| totalColumns | int | Number of columns to be exported |

**Returns:**
java.lang.Object[][] - Exported cell value array object.
### exportTypeArray(int firstRow, int firstColumn, int totalRows, int totalColumns) {#exportTypeArray-int-int-int-int-}
```
public int[][] exportTypeArray(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


Exports cell value type in the [Cells](../../com.aspose.cells/cells) collection to a two-dimension array object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | int | The row number of the first cell to export out. |
| firstColumn | int | The column number of the first cell to export out. |
| totalRows | int | Number of rows to be exported. |
| totalColumns | int | Number of columns to be exported. |

**Returns:**
int[][] - [CellValueType](../../com.aspose.cells/cellvaluetype). Exported array object representing cell value types.
### find(Object what, Cell previousCell) {#find-java.lang.Object-com.aspose.cells.Cell-}
```
public Cell find(Object what, Cell previousCell)
```


Finds the cell containing with the input object.

**Remarks**

Returns null (Nothing) if no cell is found.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| what | java.lang.Object | The object to search for. The type should be int,double,DateTime,string,bool. |
| previousCell | [Cell](../../com.aspose.cells/cell) | Previous cell with the same object. This parameter can be set to null if searching from the start. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### find(Object what, Cell previousCell, FindOptions findOptions) {#find-java.lang.Object-com.aspose.cells.Cell-com.aspose.cells.FindOptions-}
```
public Cell find(Object what, Cell previousCell, FindOptions findOptions)
```


Finds the cell containing with the input object.

**Remarks**

Returns null (Nothing) if no cell is found.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| what | java.lang.Object | The object to search for. The type should be int,double,DateTime,string,bool. |
| previousCell | [Cell](../../com.aspose.cells/cell) | Previous cell with the same object. This parameter can be set to null if searching from the start. |
| findOptions | [FindOptions](../../com.aspose.cells/findoptions) | Find options |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### get(int row, int column) {#get-int-int-}
```
public Cell get(int row, int column)
```


Gets the [Cell](../../com.aspose.cells/cell) element at the specified cell row index and column index.

**Example**

```
         Workbook excel = new Workbook();
         Cells cells = excel.getWorksheets().get(0).getCells();
         Cell cell = cells.get(0, 0);	//Gets the cell at "A1"
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Row index. |
| column | int | Column index. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - The [Cell](../../com.aspose.cells/cell) object.
### get(String cellName) {#get-java.lang.String-}
```
public Cell get(String cellName)
```


Gets the [Cell](../../com.aspose.cells/cell) element at the specified cell name.

**Example**

```
         Workbook excel = new Workbook();
         Cells cells = excel.getWorksheets().get(0).getCells();
         Cell cell = cells.get("A1");	//Gets the cell at "A1"
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | java.lang.String | Cell name,including its column letter and row number, for example A5. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - A [Cell](../../com.aspose.cells/cell) object
### getCellDisplayStyle(int row, int column) {#getCellDisplayStyle-int-int-}
```
public Style getCellDisplayStyle(int row, int column)
```


Get the display style of given cell.

**Remarks**

Same with [Cell.getDisplayStyle()](../../com.aspose.cells/cell\#getDisplayStyle--), and same with using [BorderType.SIDE\_BORDERS](../../com.aspose.cells/bordertype\#SIDE-BORDERS) for [getCellDisplayStyle(int,int,int)](../../com.aspose.cells/cells\#getCellDisplayStyle-int-int-int-).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | row index of given cell |
| column | int | column of given cell |

**Returns:**
[Style](../../com.aspose.cells/style) - the display style of given cell.
### getCellDisplayStyle(int row, int column, int adjacentBorders) {#getCellDisplayStyle-int-int-int-}
```
public Style getCellDisplayStyle(int row, int column, int adjacentBorders)
```


Get the display style of given cell.

**Remarks**

If the cell is also affected by other settings such as conditional formatting, list objects, etc., then the display style may be different from [getCellStyle(int,int)](../../com.aspose.cells/cells\#getCellStyle-int-int-). And because those settings also may be applied to empty(non-existing) cells, using this method can avoid the instantiation of those empty cells so the performance will be better than getting the Cell instance from Cells and then calling [Cell.getDisplayStyle(int)](../../com.aspose.cells/cell\#getDisplayStyle-int-).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | row index of given cell |
| column | int | column of given cell |
| adjacentBorders | int | [BorderType](../../com.aspose.cells/bordertype). Indicates which borders need to be checked and adjusted according to the borders of adjacent cells. Please see the description for the same parameter of [Cell.getDisplayStyle(int)](../../com.aspose.cells/cell\#getDisplayStyle-int-). |

**Returns:**
[Style](../../com.aspose.cells/style) - the display style of given cell.
### getCellStyle(int row, int column) {#getCellStyle-int-int-}
```
public Style getCellStyle(int row, int column)
```


Get the style of given cell.

**Remarks**

The returned style is only the one set for the cell or inherited from the row/column of the cell, does not include the applied properties by other settings such as conditional formattings.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | row index |
| column | int | column |

**Returns:**
[Style](../../com.aspose.cells/style) - the style of given cell.
### getCellsWithPlaceInCellPicture() {#getCellsWithPlaceInCellPicture--}
```
public Iterator getCellsWithPlaceInCellPicture()
```


Gets all cells that contain embedded picture.

**Remarks**

If there is no picture which is set as "Place in Cell" in this worksheet, null will be returned.

**Returns:**
java.util.Iterator - Enumerator to enumerate all Cell objects that contain embedded picture
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnOriginalWidthPoint(int column) {#getColumnOriginalWidthPoint-int-}
```
public double getColumnOriginalWidthPoint(int column)
```


Gets original column's height in unit of point if the column is hidden

**Remarks**

NOTE: This method is now obsolete. Instead, please use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method. This method will be removed 12 months later since April 2024. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | int | The row index. |

**Returns:**
double - Width of column in normal view.
### getColumnWidth(int column) {#getColumnWidth-int-}
```
public double getColumnWidth(int column)
```


Gets the width(in unit of characters) of the specified column in normal view

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | int | Column index |

**Returns:**
double - Width of column. For spreadsheet, column width is measured as the number of characters of the maximum digit width of the numbers 0~9 as rendered in the normal style's font.
### getColumnWidth(int column, boolean isOriginal, int unitType) {#getColumnWidth-int-boolean-int-}
```
public double getColumnWidth(int column, boolean isOriginal, int unitType)
```


Gets the column width.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | int | The column index. |
| isOriginal | boolean | Indicates whether getting original width. |
| unitType | int | [CellsUnitType](../../com.aspose.cells/cellsunittype). |

**Returns:**
double - 
### getColumnWidthInch(int column) {#getColumnWidthInch-int-}
```
public double getColumnWidthInch(int column)
```


Gets the width of the specified column in normal view, in units of inches.

**Remarks**

NOTE: This method is now obsolete. Instead, please use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method. This method will be removed 12 months later since April 2024. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | int | Column index |

**Returns:**
double - Width of column in normal view.
### getColumnWidthPixel(int column) {#getColumnWidthPixel-int-}
```
public int getColumnWidthPixel(int column)
```


Gets the width of the specified column in normal view, in units of pixel.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | int | Column index |

**Returns:**
int - Width of column in normal view.
### getColumnWidthPixel(int column, boolean original) {#getColumnWidthPixel-int-boolean-}
```
public int getColumnWidthPixel(int column, boolean original)
```


Gets the width of the specified column in normal view, in units of pixel.

**Remarks**

NOTE: This method is now obsolete. Instead, please use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method. This method will be removed 12 months later since April 2024. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | int | Column index |
| original | boolean | Indicates whether returning original width even when the column is hidden |

**Returns:**
int - Width of column in normal view.
### getColumns() {#getColumns--}
```
public ColumnCollection getColumns()
```


Gets the collection of [Column](../../com.aspose.cells/column) objects that represents the individual columns in this worksheet.

**Returns:**
[ColumnCollection](../../com.aspose.cells/columncollection)
### getCount() {#getCount--}
```
public int getCount()
```


Gets the total count of instantiated Cell objects.

**Returns:**
int
### getCountLarge() {#getCountLarge--}
```
public long getCountLarge()
```


Gets the total count of instantiated Cell objects.

**Returns:**
long
### getDependents(boolean isAll, int row, int column) {#getDependents-boolean-int-int-}
```
public Cell[] getDependents(boolean isAll, int row, int column)
```


Get all cells which refer to the specific cell.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isAll | boolean | Indicates whether check other worksheets |
| row | int | The row index. |
| column | int | The column index. |

**Returns:**
com.aspose.cells.Cell[] - 
### getDependentsInCalculation(int row, int column, boolean recursive) {#getDependentsInCalculation-int-int-boolean-}
```
public Iterator getDependentsInCalculation(int row, int column, boolean recursive)
```


Gets all cells whose calculated result depends on specific cell.

**Remarks**

To use this method, please make sure the workbook has been set with true value for [FormulaSettings.getEnableCalculationChain()](../../com.aspose.cells/formulasettings\#getEnableCalculationChain--) and has been fully calculated with this setting. If there is no formula reference to this cell, null will be returned. For more details and example, please see [Cell.getDependentsInCalculation(boolean)](../../com.aspose.cells/cell\#getDependentsInCalculation-boolean-)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Row index of the specific cell |
| column | int | Column index of the specific cell. |
| recursive | boolean | Whether returns those dependents which do not reference to the specific cell directly but reference to other leafs of that cell. |

**Returns:**
java.util.Iterator - Enumerator to enumerate all dependents(Cell objects)
### getFirstCell() {#getFirstCell--}
```
public Cell getFirstCell()
```


Gets the first cell in this worksheet.

**Remarks**

Returns null if there is no data in the worksheet.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getFirstDataRow(int column) {#getFirstDataRow-int-}
```
public int getFirstDataRow(int column)
```


Gets the first row index of cell which contains data in the specified column.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | int | Column index. |

**Returns:**
int - first row index.
### getGroupedColumnOutlineLevel(int columnIndex) {#getGroupedColumnOutlineLevel-int-}
```
public int getGroupedColumnOutlineLevel(int columnIndex)
```


Gets the outline level (zero-based) of the column.

**Remarks**

If the column is not grouped, returns zero.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | int | The column index |

**Returns:**
int - The outline level of the column
### getGroupedRowOutlineLevel(int rowIndex) {#getGroupedRowOutlineLevel-int-}
```
public int getGroupedRowOutlineLevel(int rowIndex)
```


Gets the outline level (zero-based) of the row.

**Remarks**

If the row is not grouped, returns zero.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | int | The row index. |

**Returns:**
int - The outline level (zero-based) of the row.
### getLastCell() {#getLastCell--}
```
public Cell getLastCell()
```


Gets the last cell in this worksheet.

**Remarks**

Returns null if there is no data in the worksheet.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getLastDataRow(int column) {#getLastDataRow-int-}
```
public int getLastDataRow(int column)
```


Gets the last row index of cell which contains data in the specified column.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | int | Column index. |

**Returns:**
int - last row index.
### getMaxColumn() {#getMaxColumn--}
```
public int getMaxColumn()
```


Maximum column index of those cells that have been instantiated in the collection(does not include the column where style is defined for the whole column but no cell has been instantiated in it).

**Remarks**

Return -1 if there is no cell has been instantiated.

**Returns:**
int
### getMaxDataColumn() {#getMaxDataColumn--}
```
public int getMaxDataColumn()
```


Maximum column index of cell which contains data.

**Remarks**

\-1 will be returned if there is no cell which contains data. This property needs to iterate and check all cells in a worksheet dynamically, so it is a time-consumed progress and should not be invoked repeatedly, such as using it directly as condition in a loop.

**Returns:**
int
### getMaxDataRow() {#getMaxDataRow--}
```
public int getMaxDataRow()
```


Maximum row index of cell which contains data.

**Remarks**

Return -1 if there is no cell which contains data. This property needs to iterate and check cells and rows dynamically, so it is a time-consumed progress and should not be invoked repeatedly, such as using it directly as condition in a loop.

**Returns:**
int
### getMaxDisplayRange() {#getMaxDisplayRange--}
```
public Range getMaxDisplayRange()
```


Gets the max range which includes data, merged cells and shapes.

**Remarks**

Reutrns null if the worksheet is empty since Aspose.Cells 21.5.2.

**Returns:**
[Range](../../com.aspose.cells/range)
### getMaxGroupedColumnOutlineLevel() {#getMaxGroupedColumnOutlineLevel--}
```
public int getMaxGroupedColumnOutlineLevel()
```


Gets the max grouped column outline level (zero-based).

**Returns:**
int - The max grouped column outline level (zero-based)
### getMaxGroupedRowOutlineLevel() {#getMaxGroupedRowOutlineLevel--}
```
public int getMaxGroupedRowOutlineLevel()
```


Gets the max grouped row outline level (zero-based).

**Returns:**
int - The max grouped row outline level (zero-based)
### getMaxRow() {#getMaxRow--}
```
public int getMaxRow()
```


Maximum row index of cell which contains data or style.

**Remarks**

Return -1 if there is no cell which contains data or style in the worksheet. This property needs to iterate and check cells and rows dynamically, so it is a time-consumed progress and should not be invoked repeatedly, such as using it directly as condition in a loop.

**Returns:**
int
### getMemorySetting() {#getMemorySetting--}
```
public int getMemorySetting()
```


Gets the memory usage option for this cells.

See [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

Notable limits and recommended operations for some modes:

| Mode                                                                                       | Remarks                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             | Supported |
| ------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------- |
| [MemorySetting.MEMORY\_PREFERENCE](../../com.aspose.cells/memorysetting\#MEMORY-PREFERENCE) | Cells data will be maintained in compact format to decrease the memory cost. On other hand, the compact data also may cause higher time cost, especially when updating the cells data, or accessing cells/rows randomly                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             | v8.0.0    |
| [MemorySetting.FILE\_CACHE](../../com.aspose.cells/memorysetting\#FILE-CACHE)               | When this mode is used for any worksheet in one workbook, [Workbook.dispose()](../../com.aspose.cells/workbook\#dispose--) should be called at the end of work to release all resources such as the temporary files.  Randomly accessing cells will give poor performance because data needs to be read/updated randomly and repeatedly(so the pointer in the file will be changed accordingly and IO operations will be required repeatedly). If possible, please always access the data sequentially(row by row).  When the data of one row/cell be changed, data of other cells/rows may also be influenced(such as the data be shifted/moved to other places to allocated enough spaces for the changed data). So every change of every data requires synchronization of other existing objects( such as Row or Cell object). So, to get better performance, please do not maintain multiple Rows/Cells at the same time. Processing them one by one will reduce the data synchronization for them so the performance can be improved a bit. | v25.7     |

**Returns:**
int
### getMergedAreas() {#getMergedAreas--}
```
public CellArea[] getMergedAreas()
```


Gets all merged cells.

**Returns:**
com.aspose.cells.CellArea[]
### getMergedCells() {#getMergedCells--}
```
public ArrayList getMergedCells()
```


Gets the collection of merged cells.

**Remarks**

NOTE: This method is now obsolete. Instead, please use Cells.GetMergedAreas() method. This method will be removed 12 months later since November 2023. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
java.util.ArrayList
### getMinColumn() {#getMinColumn--}
```
public int getMinColumn()
```


Minimum column index of those cells that have been instantiated in the collection(does not include the column where style is defined for the whole column but no cell has been instantiated in it).

**Remarks**

This property needs to iterate and check cells and rows dynamically, so it is a time-consumed progress and should not be invoked repeatedly, such as using it directly as condition in a loop.

**Returns:**
int
### getMinDataColumn() {#getMinDataColumn--}
```
public int getMinDataColumn()
```


Minimum column index of cell which contains data.

**Remarks**

\-1 will be returned if there is no cell which contains data. This property needs to iterate and check all cells in a worksheet dynamically, so it is a time-consumed progress and should not be invoked repeatedly, such as using it directly as condition in a loop.

**Returns:**
int
### getMinDataRow() {#getMinDataRow--}
```
public int getMinDataRow()
```


Minimum row index of cell which contains data.

**Remarks**

Return -1 if there is no cell which contains data. This property needs to iterate and check cells and rows dynamically, so it is a time-consumed progress and should not be invoked repeatedly, such as using it directly as condition in a loop.

**Returns:**
int
### getMinRow() {#getMinRow--}
```
public int getMinRow()
```


Minimum row index of cell which contains data or style.

**Remarks**

This property needs to iterate and check cells and rows dynamically, so it is a time-consumed progress and should not be invoked repeatedly, such as using it directly as condition in a loop.

**Returns:**
int
### getMultiThreadReading() {#getMultiThreadReading--}
```
public boolean getMultiThreadReading()
```


Gets whether the cells data model should support Multi-Thread reading. Default value of this property is false.

**Remarks**

If there are multiple threads to read Row/Cell objects in this collection concurrently, this property should be set as true, otherwise unexpected result may be produced. Supporting Multi-Thread reading may degrade the performance for accessing Row/Cell objects from this collection. Please note, some features cannot support Multi-Thread reading, such as formatting values(by [Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--), [Cell.getDisplayStringValue()](../../com.aspose.cells/cell\#getDisplayStringValue--), .etc.). So, even with this property being set as true, those APIs still may give unexpected result for Multi-Thread reading.

**Returns:**
boolean
### getOdsCellFields() {#getOdsCellFields--}
```
public OdsCellFieldCollection getOdsCellFields()
```


Gets the list of fields of ods.

**Returns:**
[OdsCellFieldCollection](../../com.aspose.cells/odscellfieldcollection)
### getPreserveString() {#getPreserveString--}
```
public boolean getPreserveString()
```


Gets a value indicating whether all worksheet values are preserved as strings. Default is false.

**Returns:**
boolean
### getRanges() {#getRanges--}
```
public RangeCollection getRanges()
```


Gets the collection of [Range](../../com.aspose.cells/range) objects created at run time.

**Returns:**
[RangeCollection](../../com.aspose.cells/rangecollection)
### getRowEnumerator() {#getRowEnumerator--}
```
public Iterator getRowEnumerator()
```


Gets the rows enumerator.

**Remarks**

NOTE: This member is now obsolete. Instead, please use RowCollection.GetEnumerator() method. This method will be removed 12 months later since May 2023. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
java.util.Iterator - The rows enumerator.
### getRowHeight(int row) {#getRowHeight-int-}
```
public double getRowHeight(int row)
```


Gets the height of a specified row, in unit of points.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Row index |

**Returns:**
double - Height of row
### getRowHeight(int row, boolean isOriginal, int unitType) {#getRowHeight-int-boolean-int-}
```
public double getRowHeight(int row, boolean isOriginal, int unitType)
```


Gets row's height.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | The row index. |
| isOriginal | boolean | Whether returns the original row height or 0 for hidden row. |
| unitType | int | [CellsUnitType](../../com.aspose.cells/cellsunittype). Unit type of the returned height value |

**Returns:**
double - Row's height
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
### getRowOriginalHeightPoint(int row) {#getRowOriginalHeightPoint-int-}
```
public double getRowOriginalHeightPoint(int row)
```


Gets original row's height in unit of point if the row is hidden

**Remarks**

NOTE: This member is now obsolete. Instead, please use Cells.GetRowHeight(int,bool,CellsUnitType) method. This method will be removed 12 months later since April 2024. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | The row index. |

**Returns:**
double - 
### getRows() {#getRows--}
```
public RowCollection getRows()
```


Gets the collection of [Row](../../com.aspose.cells/row) objects that represents the individual rows in this worksheet.

**Returns:**
[RowCollection](../../com.aspose.cells/rowcollection)
### getStandardHeight() {#getStandardHeight--}
```
public double getStandardHeight()
```


Gets the default row height in this worksheet, in unit of points.

**Returns:**
double
### getStandardHeightInch() {#getStandardHeightInch--}
```
public double getStandardHeightInch()
```


Gets the default row height in this worksheet, in unit of inches.

**Returns:**
double
### getStandardHeightPixels() {#getStandardHeightPixels--}
```
public int getStandardHeightPixels()
```


Gets the default row height in this worksheet, in unit of pixels.

**Returns:**
int
### getStandardWidth() {#getStandardWidth--}
```
public double getStandardWidth()
```


Gets the default column width in the worksheet, in unit of characters.

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
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Gets the default style of the worksheet.

**Returns:**
[Style](../../com.aspose.cells/style)
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
### getViewRowHeight(int row) {#getViewRowHeight-int-}
```
public double getViewRowHeight(int row)
```


Gets the height of a specified row.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Row index. |

**Returns:**
double - Height of row.
### getViewRowHeightInch(int row) {#getViewRowHeightInch-int-}
```
public double getViewRowHeightInch(int row)
```


Gets the height of a specified row in unit of inches.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Row index |

**Returns:**
double - Height of row
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
### hideColumn(int column) {#hideColumn-int-}
```
public void hideColumn(int column)
```


Hides a column.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | int | Column index. |

### hideColumns(int column, int totalColumns) {#hideColumns-int-int-}
```
public void hideColumns(int column, int totalColumns)
```


Hide multiple columns.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | int | Column index. |
| totalColumns | int | Column number. |

### hideGroupDetail(boolean isVertical, int index) {#hideGroupDetail-boolean-int-}
```
public void hideGroupDetail(boolean isVertical, int index)
```


Collapses the grouped rows/columns.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isVertical | boolean | True, collapse the grouped rows. |
| index | int | The row/column index |

### hideRow(int row) {#hideRow-int-}
```
public void hideRow(int row)
```


Hides a row.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Row index. |

### hideRows(int row, int totalRows) {#hideRows-int-int-}
```
public void hideRows(int row, int totalRows)
```


Hides multiple rows.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | The row index. |
| totalRows | int | The row number. |

### importArray(double[] doubleArray, int firstRow, int firstColumn, boolean isVertical) {#importArray-double---int-int-boolean-}
```
public void importArray(double[] doubleArray, int firstRow, int firstColumn, boolean isVertical)
```


Imports an array of double into a worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| doubleArray | double[] | Double array. |
| firstRow | int | The row number of the first cell to import in. |
| firstColumn | int | The column number of the first cell to import in. |
| isVertical | boolean | Specifies to import data vertically or horizontally. |

### importArray(double[][] doubleArray, int firstRow, int firstColumn) {#importArray-double-----int-int-}
```
public void importArray(double[][] doubleArray, int firstRow, int firstColumn)
```


Imports a two-dimension array of double into a worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| doubleArray | double[][] | Two-dimension double array. |
| firstRow | int | The row number of the first cell to import in. |
| firstColumn | int | The column number of the first cell to import in. |

### importArray(int[] intArray, int firstRow, int firstColumn, boolean isVertical) {#importArray-int---int-int-boolean-}
```
public void importArray(int[] intArray, int firstRow, int firstColumn, boolean isVertical)
```


Imports an array of integer into a worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| intArray | int[] | Integer array. |
| firstRow | int | The row number of the first cell to import in. |
| firstColumn | int | The column number of the first cell to import in. |
| isVertical | boolean | Specifies to import data vertically or horizontally. |

### importArray(int[][] intArray, int firstRow, int firstColumn) {#importArray-int-----int-int-}
```
public void importArray(int[][] intArray, int firstRow, int firstColumn)
```


Imports a two-dimension array of integer into a worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| intArray | int[][] | Two-dimension integer array. |
| firstRow | int | The row number of the first cell to import in. |
| firstColumn | int | The column number of the first cell to import in. |

### importArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical) {#importArray-java.lang.String---int-int-boolean-}
```
public void importArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical)
```


Imports an array of string into a worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stringArray | java.lang.String[] | String array. |
| firstRow | int | The row number of the first cell to import in. |
| firstColumn | int | The column number of the first cell to import in. |
| isVertical | boolean | Specifies to import data vertically or horizontally. |

### importArray(String[][] stringArray, int firstRow, int firstColumn) {#importArray-java.lang.String-----int-int-}
```
public void importArray(String[][] stringArray, int firstRow, int firstColumn)
```


Imports a two-dimension array of string into a worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stringArray | java.lang.String[][] | Two-dimension string array. |
| firstRow | int | The row number of the first cell to import in. |
| firstColumn | int | The column number of the first cell to import in. |

### importArrayList(ArrayList arrayList, int firstRow, int firstColumn, boolean isVertical) {#importArrayList-java.util.ArrayList-int-int-boolean-}
```
public void importArrayList(ArrayList arrayList, int firstRow, int firstColumn, boolean isVertical)
```


Imports an arraylist of data into a worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arrayList | java.util.ArrayList | Data arraylist. |
| firstRow | int | The row number of the first cell to import in. |
| firstColumn | int | The column number of the first cell to import in. |
| isVertical | boolean | Specifies to import data vertically or horizontally. |

### importCSV(InputStream stream, TxtLoadOptions options, int firstRow, int firstColumn) {#importCSV-java.io.InputStream-com.aspose.cells.TxtLoadOptions-int-int-}
```
public void importCSV(InputStream stream, TxtLoadOptions options, int firstRow, int firstColumn)
```


Import a CSV file to the cells.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | The CSV file stream. |
| options | [TxtLoadOptions](../../com.aspose.cells/txtloadoptions) | The load options for reading text file |
| firstRow | int | The row number of the first cell to import in. |
| firstColumn | int | The column number of the first cell to import in. |

### importCSV(InputStream stream, String splitter, boolean convertNumericData, int firstRow, int firstColumn) {#importCSV-java.io.InputStream-java.lang.String-boolean-int-int-}
```
public void importCSV(InputStream stream, String splitter, boolean convertNumericData, int firstRow, int firstColumn)
```


Import a CSV file to the cells.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | The CSV file stream. |
| splitter | java.lang.String | The splitter |
| convertNumericData | boolean | Whether the string in text file is converted to numeric data. |
| firstRow | int | The row number of the first cell to import in. |
| firstColumn | int | The column number of the first cell to import in. |

### importCSV(String fileName, TxtLoadOptions options, int firstRow, int firstColumn) {#importCSV-java.lang.String-com.aspose.cells.TxtLoadOptions-int-int-}
```
public void importCSV(String fileName, TxtLoadOptions options, int firstRow, int firstColumn)
```


Import a CSV file to the cells.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | The CSV file name. |
| options | [TxtLoadOptions](../../com.aspose.cells/txtloadoptions) | The load options for reading text file |
| firstRow | int | The row number of the first cell to import in. |
| firstColumn | int | The column number of the first cell to import in. |

### importCSV(String fileName, String splitter, boolean convertNumericData, int firstRow, int firstColumn) {#importCSV-java.lang.String-java.lang.String-boolean-int-int-}
```
public void importCSV(String fileName, String splitter, boolean convertNumericData, int firstRow, int firstColumn)
```


Import a CSV file to the cells.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | The CSV file name. |
| splitter | java.lang.String | The splitter |
| convertNumericData | boolean | Whether the string in text file is converted to numeric data. |
| firstRow | int | The row number of the first cell to import in. |
| firstColumn | int | The column number of the first cell to import in. |

### importCustomObjects(Collection list, int firstRow, int firstColumn, ImportTableOptions options) {#importCustomObjects-java.util.Collection-int-int-com.aspose.cells.ImportTableOptions-}
```
public int importCustomObjects(Collection list, int firstRow, int firstColumn, ImportTableOptions options)
```


Imports custom objects.

**Remarks**

The custom objects should be the same type.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| list | java.util.Collection | The custom object |
| firstRow | int | The row number of the first cell to import in. |
| firstColumn | int | The column number of the first cell to import in. |
| options | [ImportTableOptions](../../com.aspose.cells/importtableoptions) | The import options. |

**Returns:**
int - Total number of rows imported.
### importCustomObjects(Collection list, String[] propertyNames, boolean isPropertyNameShown, int firstRow, int firstColumn, int rowNumber, boolean insertRows, String dateFormatString, boolean convertStringToNumber) {#importCustomObjects-java.util.Collection-java.lang.String---boolean-int-int-int-boolean-java.lang.String-boolean-}
```
public int importCustomObjects(Collection list, String[] propertyNames, boolean isPropertyNameShown, int firstRow, int firstColumn, int rowNumber, boolean insertRows, String dateFormatString, boolean convertStringToNumber)
```


Imports custom objects.

**Remarks**

The custom objects should be the same type.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| list | java.util.Collection | The custom object |
| propertyNames | java.lang.String[] | The property names.If it is null,we will import all properties of the object. |
| isPropertyNameShown | boolean | Indicates whether the property name will be imported to the first row. |
| firstRow | int | The row number of the first cell to import in. |
| firstColumn | int | The column number of the first cell to import in. |
| rowNumber | int | Number of rows to be imported. |
| insertRows | boolean | Indicates whether extra rows are added to fit data. |
| dateFormatString | java.lang.String | Date format string for cells. |
| convertStringToNumber | boolean | Indicates if this method will try to convert string to number. |

**Returns:**
int - Total number of rows imported.
### importData(ICellsDataTable table, int firstRow, int firstColumn, ImportTableOptions options) {#importData-com.aspose.cells.ICellsDataTable-int-int-com.aspose.cells.ImportTableOptions-}
```
public int importData(ICellsDataTable table, int firstRow, int firstColumn, ImportTableOptions options)
```


Import data from custom data table.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| table | [ICellsDataTable](../../com.aspose.cells/icellsdatatable) | The custom data table. |
| firstRow | int | First row index. |
| firstColumn | int | First column index. |
| options | [ImportTableOptions](../../com.aspose.cells/importtableoptions) | The import options |

**Returns:**
int - 
### importFormulaArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical) {#importFormulaArray-java.lang.String---int-int-boolean-}
```
public void importFormulaArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical)
```


Imports an array of formula into a worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stringArray | java.lang.String[] | Formula array. |
| firstRow | int | The row number of the first cell to import in. |
| firstColumn | int | The column number of the first cell to import in. |
| isVertical | boolean | Specifies to import data vertically or horizontally. |

### importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical) {#importObjectArray-java.lang.Object---int-int-boolean-}
```
public void importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical)
```


Imports an array of data into a worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| objArray | java.lang.Object[] | Data array. |
| firstRow | int | The row number of the first cell to import in. |
| firstColumn | int | The column number of the first cell to import in. |
| isVertical | boolean | Specifies to import data vertically or horizontally. |

### importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical, int skip) {#importObjectArray-java.lang.Object---int-int-boolean-int-}
```
public void importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical, int skip)
```


Imports an array of data into a worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| objArray | java.lang.Object[] | Data array. |
| firstRow | int | The row number of the first cell to import in. |
| firstColumn | int | The column number of the first cell to import in. |
| isVertical | boolean | Specifies to import data vertically or horizontally. |
| skip | int | Skipped number of rows or columns. |

### importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown) {#importResultSet-java.sql.ResultSet-int-int-boolean-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown)
```


Imports data in a ResultSet object to the worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rs | java.sql.ResultSet | the ResultSet object to import from. |
| rowIndex | int | start row index in the worksheet. |
| columnIndex | int | start column index in the worksheet. |
| isFieldNameShown | boolean | Indicates whether the field name of the resultset will be imported to the first row. |

**Returns:**
int - how many rows actually imported.
### importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber) {#importResultSet-java.sql.ResultSet-int-int-boolean-java.lang.String-boolean-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber)
```


Imports data in a ResultSet object to the worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rs | java.sql.ResultSet | the ResultSet object to import from. |
| rowIndex | int | start row index in the worksheet. |
| columnIndex | int | start column index in the worksheet. |
| isFieldNameShown | boolean | Indicates whether the field name of the resultset will be imported to the first row. |
| customDateFormatString | java.lang.String | Date format string for cells which contain date value. |
| convertStringToNumber | boolean | Indicates if this method will try to convert string to number. |

**Returns:**
int - how many rows actually imported.
### importResultSet(ResultSet rs, int rowIndex, int columnIndex, ImportTableOptions options) {#importResultSet-java.sql.ResultSet-int-int-com.aspose.cells.ImportTableOptions-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, ImportTableOptions options)
```


Imports data in a ResultSet object to the worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rs | java.sql.ResultSet | the ResultSet object to import from. |
| rowIndex | int | start row index in the worksheet. |
| columnIndex | int | start column index in the worksheet. |
| options | [ImportTableOptions](../../com.aspose.cells/importtableoptions) | The import options |

**Returns:**
int - how many rows actually imported.
### importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown) {#importResultSet-java.sql.ResultSet-int-int-int-int-boolean-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown)
```


Imports data in a ResultSet object to the worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rs | java.sql.ResultSet | the ResultSet object to import from. |
| rowIndex | int | start row index in the worksheet. |
| columnIndex | int | start column index in the worksheet. |
| rowNum | int | number of rows to import. -1 to import all records in given resultset. |
| columnNum | int | number of columns to import. -1 to import all columns in given resultset. |
| isFieldNameShown | boolean | Indicates whether the field name of the resultset will be imported to the first row. |

**Returns:**
int - how many rows actually imported.
### importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber) {#importResultSet-java.sql.ResultSet-int-int-int-int-boolean-java.lang.String-boolean-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber)
```


Imports data in a ResultSet object to the worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rs | java.sql.ResultSet | the ResultSet object to import from. |
| rowIndex | int | start row index in the worksheet. |
| columnIndex | int | start column index in the worksheet. |
| rowNum | int | number of rows to import. -1 to import all records in given resultset. |
| columnNum | int | number of columns to import. -1 to import all columns in given resultset. |
| isFieldNameShown | boolean | Indicates whether the field name of the resultset will be imported to the first row. |
| customDateFormatString | java.lang.String | Date format string for cells which contain date value. |
| convertStringToNumber | boolean | Indicates if this method will try to convert string to number. |

**Returns:**
int - how many rows actually imported.
### importResultSet(ResultSet rs, String startCell, boolean isFieldNameShown) {#importResultSet-java.sql.ResultSet-java.lang.String-boolean-}
```
public int importResultSet(ResultSet rs, String startCell, boolean isFieldNameShown)
```


Imports data in a ResultSet object to the worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rs | java.sql.ResultSet | the ResultSet object to import from. |
| startCell | java.lang.String | name of start cell to insert the resultset, such as "A1". |
| isFieldNameShown | boolean | Indicates whether the field name of the resultset will be imported to the first row. |

**Returns:**
int - how many rows actually imported.
### importResultSet(ResultSet rs, String startCell, ImportTableOptions options) {#importResultSet-java.sql.ResultSet-java.lang.String-com.aspose.cells.ImportTableOptions-}
```
public int importResultSet(ResultSet rs, String startCell, ImportTableOptions options)
```


Imports data in a ResultSet object to the worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rs | java.sql.ResultSet | the ResultSet object to import from. |
| startCell | java.lang.String | name of start cell to insert the resultset, such as "A1". |
| options | [ImportTableOptions](../../com.aspose.cells/importtableoptions) | The import options |

**Returns:**
int - how many rows actually imported.
### importResultSet(ResultSet rs, String startCell, int rowNum, int columnNum, boolean isFieldNameShown) {#importResultSet-java.sql.ResultSet-java.lang.String-int-int-boolean-}
```
public int importResultSet(ResultSet rs, String startCell, int rowNum, int columnNum, boolean isFieldNameShown)
```


Imports data in a ResultSet object to the worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rs | java.sql.ResultSet | the ResultSet object to import from. |
| startCell | java.lang.String | name of start cell to insert the resultset, such as "A1". |
| rowNum | int | number of rows to import. -1 to import all records in given resultset. |
| columnNum | int | number of columns to import. -1 to import all columns in given resultset. |
| isFieldNameShown | boolean | Indicates whether the field name of the resultset will be imported to the first row. |

**Returns:**
int - how many rows actually imported.
### importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn) {#importTwoDimensionArray-java.lang.Object-----int-int-}
```
public void importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn)
```


Imports a two-dimension array of data into a worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| objArray | java.lang.Object[][] | Two-dimension data array. |
| firstRow | int | The row number of the first cell to import in. |
| firstColumn | int | The column number of the first cell to import in. |

### importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn, boolean convertStringToNumber) {#importTwoDimensionArray-java.lang.Object-----int-int-boolean-}
```
public void importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn, boolean convertStringToNumber)
```


Imports a two-dimension array of data into a worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| objArray | java.lang.Object[][] | Two-dimension data array. |
| firstRow | int | The row number of the first cell to import in. |
| firstColumn | int | The column number of the first cell to import in. |
| convertStringToNumber | boolean | Indicates if this method will try to convert string to number. |

### importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, boolean convertStringToNumber) {#importTwoDimensionArray-java.lang.Object-----java.lang.Object-----int-int-boolean-}
```
public void importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, boolean convertStringToNumber)
```


Imports a two-dimension array of data into a worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| objArray | java.lang.Object[][] | Two-dimension data array. |
| styles | java.lang.Object[][] | Two-dimension data style. |
| firstRow | int | The row number of the first cell to import in. |
| firstColumn | int | The column number of the first cell to import in. |
| convertStringToNumber | boolean | Indicates if this method will try to convert string to number. |

### importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, TxtLoadOptions opts) {#importTwoDimensionArray-java.lang.Object-----java.lang.Object-----int-int-com.aspose.cells.TxtLoadOptions-}
```
public void importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, TxtLoadOptions opts)
```


Imports a two-dimension array of data into a worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| objArray | java.lang.Object[][] | Two-dimension data array. |
| styles | java.lang.Object[][] | Two-dimension data style. |
| firstRow | int | The row number of the first cell to import in. |
| firstColumn | int | The column number of the first cell to import in. |
| opts | [TxtLoadOptions](../../com.aspose.cells/txtloadoptions) | Options for converting string values |

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

### insertColumns(int columnIndex, int totalColumns, InsertOptions options) {#insertColumns-int-int-com.aspose.cells.InsertOptions-}
```
public void insertColumns(int columnIndex, int totalColumns, InsertOptions options)
```


Inserts some columns into the worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | int | Column index. |
| totalColumns | int | The number of columns. |
| options | [InsertOptions](../../com.aspose.cells/insertoptions) | The options for inserting operation. |

### insertCutCells(Range cutRange, int row, int column, int shiftType) {#insertCutCells-com.aspose.cells.Range-int-int-int-}
```
public void insertCutCells(Range cutRange, int row, int column, int shiftType)
```


Insert cut range.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cutRange | [Range](../../com.aspose.cells/range) | The cut range. |
| row | int | The row. |
| column | int | The column. |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). Indicates how to shift other objects of the target range when inserting cut range. |

### insertRange(CellArea area, int shiftType) {#insertRange-com.aspose.cells.CellArea-int-}
```
public void insertRange(CellArea area, int shiftType)
```


Inserts a range of cells and shift cells according to the shift option.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| area | [CellArea](../../com.aspose.cells/cellarea) | Shift area. |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). Shift cells option. |

### insertRange(CellArea area, int shiftNumber, int shiftType) {#insertRange-com.aspose.cells.CellArea-int-int-}
```
public void insertRange(CellArea area, int shiftNumber, int shiftType)
```


Inserts a range of cells and shift cells according to the shift option.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| area | [CellArea](../../com.aspose.cells/cellarea) | Shift area. |
| shiftNumber | int | Number of rows or columns to be inserted. |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). Shift cells option. |

### insertRange(CellArea area, int shiftNumber, int shiftType, boolean updateReference) {#insertRange-com.aspose.cells.CellArea-int-int-boolean-}
```
public void insertRange(CellArea area, int shiftNumber, int shiftType, boolean updateReference)
```


Inserts a range of cells and shift cells according to the shift option.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| area | [CellArea](../../com.aspose.cells/cellarea) | Shift area. |
| shiftNumber | int | Number of rows or columns to be inserted. |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). Shift cells option. |
| updateReference | boolean | Indicates whether update references in other worksheets. |

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

### insertRows(int rowIndex, int totalRows, InsertOptions options) {#insertRows-int-int-com.aspose.cells.InsertOptions-}
```
public void insertRows(int rowIndex, int totalRows, InsertOptions options)
```


Inserts multiple rows into the worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | int | Row index. |
| totalRows | int | Number of rows to be inserted. |
| options | [InsertOptions](../../com.aspose.cells/insertoptions) | Options for inserting operation. |

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
### isDefaultColumnHidden() {#isDefaultColumnHidden--}
```
public boolean isDefaultColumnHidden()
```




**Returns:**
boolean
### isDefaultRowHeightMatched() {#isDefaultRowHeightMatched--}
```
public boolean isDefaultRowHeightMatched()
```


Indicates that row height and default font height matches

**Returns:**
boolean
### isDefaultRowHidden() {#isDefaultRowHidden--}
```
public boolean isDefaultRowHidden()
```


Indicates whether the row is default hidden.

**Returns:**
boolean
### isDeletingRangeEnabled(int startRow, int startColumn, int totalRows, int totalColumns) {#isDeletingRangeEnabled-int-int-int-int-}
```
public boolean isDeletingRangeEnabled(int startRow, int startColumn, int totalRows, int totalColumns)
```


Check whether the range could be deleted.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | int | The start row index of the range. |
| startColumn | int | The start column index of the range. |
| totalRows | int | The number of the rows in the range. |
| totalColumns | int | The number of the columns in the range. |

**Returns:**
boolean - 
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


Gets the cells enumerator.

**Remarks**

When traversing elements by the returned Enumerator, the cells collection should not be modified(such as operations that will cause new Cell/Row be instantiated or existing Cell/Row be deleted). Otherwise the enumerator may not be able to traverse all cells correctly(some elements may be traversed repeatedly or skipped).

**Example**

```
         Workbook workbook = new Workbook("template.xlsx");
         	Cells cells = workbook.getWorksheets().get(0).getCells();
 
         	Iterator en = cells.iterator();
         	while (en.hasNext())
         	{
         	    Cell cell = (Cell)en.next();
         	    System.out.println(cell.getName() + ": " + cell.getValue());
         	}
```

**Returns:**
java.util.Iterator - The cells enumerator
### linkToXmlMap(String mapName, int row, int column, String path) {#linkToXmlMap-java.lang.String-int-int-java.lang.String-}
```
public void linkToXmlMap(String mapName, int row, int column, String path)
```


Link to a xml map.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| mapName | java.lang.String | name of xml map |
| row | int | row of the destination cell |
| column | int | column of the destination cell |
| path | java.lang.String | path of xml element in xml map |

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

### merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean mergeConflict) {#merge-int-int-int-int-boolean-}
```
public void merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean mergeConflict)
```


Merges a specified range of cells into a single cell.

**Remarks**

Reference the merged cell via the address of the upper-left cell in the range. If mergeConflict is true and the merged range conflicts with other merged cells, other merged cells will be automatically removed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | int | First row of this range(zero based) |
| firstColumn | int | First column of this range(zero based) |
| totalRows | int | Number of rows(one based) |
| totalColumns | int | Number of columns(one based) |
| mergeConflict | boolean | Merge conflict merged ranges. |

### merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean checkConflict, boolean mergeConflict) {#merge-int-int-int-int-boolean-boolean-}
```
public void merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean checkConflict, boolean mergeConflict)
```


Merges a specified range of cells into a single cell.

**Remarks**

Reference the merged cell via the address of the upper-left cell in the range. If mergeConflict is true and the merged range conflicts with other merged cells, other merged cells will be automatically removed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | int | First row of this range(zero based) |
| firstColumn | int | First column of this range(zero based) |
| totalRows | int | Number of rows(one based) |
| totalColumns | int | Number of columns(one based) |
| checkConflict | boolean | Indicates whether check the merged cells intersects other merged cells |
| mergeConflict | boolean | Merge conflict merged ranges. |

### moveRange(CellArea sourceArea, int destRow, int destColumn) {#moveRange-com.aspose.cells.CellArea-int-int-}
```
public void moveRange(CellArea sourceArea, int destRow, int destColumn)
```


Moves the range.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceArea | [CellArea](../../com.aspose.cells/cellarea) | The range which should be moved. |
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




### removeDuplicates() {#removeDuplicates--}
```
public void removeDuplicates()
```


Removes duplicate rows in the sheet.

### removeDuplicates(int startRow, int startColumn, int endRow, int endColumn) {#removeDuplicates-int-int-int-int-}
```
public void removeDuplicates(int startRow, int startColumn, int endRow, int endColumn)
```


Removes duplicate values in the range.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | int | The start row. |
| startColumn | int | The start column |
| endRow | int | The end row index. |
| endColumn | int | The end column index. |

### removeDuplicates(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders, int[] columnOffsets) {#removeDuplicates-int-int-int-int-boolean-int---}
```
public void removeDuplicates(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders, int[] columnOffsets)
```


Removes duplicate data of the range.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | int | The start row. |
| startColumn | int | The start column |
| endRow | int | The end row index. |
| endColumn | int | The end column index. |
| hasHeaders | boolean | Indicates whether the range contains headers. |
| columnOffsets | int[] | The column offsets. |

### removeFormulas() {#removeFormulas--}
```
public void removeFormulas()
```


Removes all formula and replaces with the value of the formula.

### retrieveSubtotalSetting(CellArea ca) {#retrieveSubtotalSetting-com.aspose.cells.CellArea-}
```
public SubtotalSetting retrieveSubtotalSetting(CellArea ca)
```


Retrieves subtotals setting of the range.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | The range |

**Returns:**
[SubtotalSetting](../../com.aspose.cells/subtotalsetting) - 
### setColumnWidth(int column, double width) {#setColumnWidth-int-double-}
```
public void setColumnWidth(int column, double width)
```


Sets the width of the specified column in normal view.

**Remarks**

For spreadsheet, column width is measured as the number of characters of the maximum digit width of the numbers 0~9 as rendered in the normal style's font.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | int | Column index. |
| width | double | Width of column in unit of characters.Column width must be between 0 and 255. |

### setColumnWidthInch(int column, double inches) {#setColumnWidthInch-int-double-}
```
public void setColumnWidthInch(int column, double inches)
```


Sets column width in unit of inches in normal view.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | int | Column index. |
| inches | double | Number of inches. |

### setColumnWidthPixel(int column, int pixels) {#setColumnWidthPixel-int-int-}
```
public void setColumnWidthPixel(int column, int pixels)
```


Sets column width in unit of pixels in normal view.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | int | Column index. |
| pixels | int | Number of pixels. |

### setDefaultColumnHidden(boolean value) {#setDefaultColumnHidden-boolean-}
```
public void setDefaultColumnHidden(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDefaultRowHeightMatched(boolean value) {#setDefaultRowHeightMatched-boolean-}
```
public void setDefaultRowHeightMatched(boolean value)
```


Indicates that row height and default font height matches

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDefaultRowHidden(boolean value) {#setDefaultRowHidden-boolean-}
```
public void setDefaultRowHidden(boolean value)
```


Indicates whether the row is default hidden.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setMemorySetting(int value) {#setMemorySetting-int-}
```
public void setMemorySetting(int value)
```


Sets the memory usage option for this cells.

See [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

Notable limits and recommended operations for some modes:

| Mode                                                                                       | Remarks                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             | Supported |
| ------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------- |
| [MemorySetting.MEMORY\_PREFERENCE](../../com.aspose.cells/memorysetting\#MEMORY-PREFERENCE) | Cells data will be maintained in compact format to decrease the memory cost. On other hand, the compact data also may cause higher time cost, especially when updating the cells data, or accessing cells/rows randomly                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             | v8.0.0    |
| [MemorySetting.FILE\_CACHE](../../com.aspose.cells/memorysetting\#FILE-CACHE)               | When this mode is used for any worksheet in one workbook, [Workbook.dispose()](../../com.aspose.cells/workbook\#dispose--) should be called at the end of work to release all resources such as the temporary files.  Randomly accessing cells will give poor performance because data needs to be read/updated randomly and repeatedly(so the pointer in the file will be changed accordingly and IO operations will be required repeatedly). If possible, please always access the data sequentially(row by row).  When the data of one row/cell be changed, data of other cells/rows may also be influenced(such as the data be shifted/moved to other places to allocated enough spaces for the changed data). So every change of every data requires synchronization of other existing objects( such as Row or Cell object). So, to get better performance, please do not maintain multiple Rows/Cells at the same time. Processing them one by one will reduce the data synchronization for them so the performance can be improved a bit. | v25.7     |

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setMultiThreadReading(boolean value) {#setMultiThreadReading-boolean-}
```
public void setMultiThreadReading(boolean value)
```


Sets whether the cells data model should support Multi-Thread reading. Default value of this property is false.

**Remarks**

If there are multiple threads to read Row/Cell objects in this collection concurrently, this property should be set as true, otherwise unexpected result may be produced. Supporting Multi-Thread reading may degrade the performance for accessing Row/Cell objects from this collection. Please note, some features cannot support Multi-Thread reading, such as formatting values(by [Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--), [Cell.getDisplayStringValue()](../../com.aspose.cells/cell\#getDisplayStringValue--), .etc.). So, even with this property being set as true, those APIs still may give unexpected result for Multi-Thread reading.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setPreserveString(boolean value) {#setPreserveString-boolean-}
```
public void setPreserveString(boolean value)
```


Sets a value indicating whether all worksheet values are preserved as strings. Default is false.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setRowHeight(int row, double height) {#setRowHeight-int-double-}
```
public void setRowHeight(int row, double height)
```


Sets the height of the specified row.

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
| inches | double | Number of inches. It should be between 0 and 409.5/72. |

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

### setStandardHeight(double value) {#setStandardHeight-double-}
```
public void setStandardHeight(double value)
```


Sets the default row height in this worksheet, in unit of points.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setStandardHeightInch(double value) {#setStandardHeightInch-double-}
```
public void setStandardHeightInch(double value)
```


Sets the default row height in this worksheet, in unit of inches.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setStandardHeightPixels(int value) {#setStandardHeightPixels-int-}
```
public void setStandardHeightPixels(int value)
```


Sets the default row height in this worksheet, in unit of pixels.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setStandardWidth(double value) {#setStandardWidth-double-}
```
public void setStandardWidth(double value)
```


Sets the default column width in the worksheet, in unit of characters.

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

### setStyle(Style value) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style value)
```


Sets the default style of the worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Style](../../com.aspose.cells/style) |  |

### setViewColumnWidthPixel(int column, int pixels) {#setViewColumnWidthPixel-int-int-}
```
public void setViewColumnWidthPixel(int column, int pixels)
```


Sets the width of the column in different view.

**Remarks**

If the current view type is [ViewType.PAGE\_LAYOUT\_VIEW](../../com.aspose.cells/viewtype\#PAGE-LAYOUT-VIEW), the column's width is same as printed width.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | int | The column index. |
| pixels | int | The width in unit of pixels. |

### showGroupDetail(boolean isVertical, int index) {#showGroupDetail-boolean-int-}
```
public void showGroupDetail(boolean isVertical, int index)
```


Expands the grouped rows/columns.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isVertical | boolean | True, expands the grouped rows. |
| index | int | The row/column index |

### subtotal(CellArea ca, int groupBy, int function, int[] totalList) {#subtotal-com.aspose.cells.CellArea-int-int-int---}
```
public void subtotal(CellArea ca, int groupBy, int function, int[] totalList)
```


Creates subtotals for the range.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | The range |
| groupBy | int | The field to group by, as a zero-based integer offset |
| function | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). The subtotal function. |
| totalList | int[] | An array of zero-based field offsets, indicating the fields to which the subtotals are added. |

### subtotal(CellArea ca, int groupBy, int function, int[] totalList, boolean replace, boolean pageBreaks, boolean summaryBelowData) {#subtotal-com.aspose.cells.CellArea-int-int-int---boolean-boolean-boolean-}
```
public void subtotal(CellArea ca, int groupBy, int function, int[] totalList, boolean replace, boolean pageBreaks, boolean summaryBelowData)
```


Creates subtotals for the range.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | The range |
| groupBy | int | The field to group by, as a zero-based integer offset |
| function | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). The subtotal function. |
| totalList | int[] | An array of zero-based field offsets, indicating the fields to which the subtotals are added. |
| replace | boolean | Indicates whether replace the current subtotals |
| pageBreaks | boolean | Indicates whether add page break between groups |
| summaryBelowData | boolean | Indicates whether add summary below data. |

### textToColumns(int row, int column, int totalRows, TxtLoadOptions options) {#textToColumns-int-int-int-com.aspose.cells.TxtLoadOptions-}
```
public int textToColumns(int row, int column, int totalRows, TxtLoadOptions options)
```


Splits content in specified column into multiple columns..

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | The row index. |
| column | int | The column index. |
| totalRows | int | The number of rows. |
| options | [TxtLoadOptions](../../com.aspose.cells/txtloadoptions) | The split options. |

**Returns:**
int - Total column count of the split values.
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

Only removes outer group info.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | int | The first row index to be ungrouped. |
| lastIndex | int | The last row index to be ungrouped. |

### ungroupRows(int firstIndex, int lastIndex, boolean isAll) {#ungroupRows-int-int-boolean-}
```
public void ungroupRows(int firstIndex, int lastIndex, boolean isAll)
```


Ungroups rows.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | int | The first row index to be ungrouped. |
| lastIndex | int | The last row index to be ungrouped. |
| isAll | boolean | True, removes all grouped info.Otherwise, remove the outer group info. |

### unhideColumn(int column, double width) {#unhideColumn-int-double-}
```
public void unhideColumn(int column, double width)
```


Unhides a column

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | int | Column index. |
| width | double | Column width. |

### unhideColumns(int column, int totalColumns, double width) {#unhideColumns-int-int-double-}
```
public void unhideColumns(int column, int totalColumns, double width)
```


Unhide multiple columns.

**Remarks**

Only applies the column width to the hidden columns.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | int | Column index. |
| totalColumns | int | Column number |
| width | double | Column width. |

### unhideRow(int row, double height) {#unhideRow-int-double-}
```
public void unhideRow(int row, double height)
```


Unhides a row.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Row index. |
| height | double | Row height. The row's height will be changed only when the row is hidden and given height value is positive. |

### unhideRows(int row, int totalRows, double height) {#unhideRows-int-int-double-}
```
public void unhideRows(int row, int totalRows, double height)
```


Unhides the hidden rows.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | The row index. |
| totalRows | int | The row number. |
| height | double | Row height. The row's height will be changed only when the row is hidden and given height value is positive. |

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

