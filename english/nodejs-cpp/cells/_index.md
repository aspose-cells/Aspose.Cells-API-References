---
title: Cells
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Encapsulates a collection of cell relevant objects such as Cell..cell Row..row ...etc.
type: docs
url: /nodejs-cpp/cells/
---

## Cells class

Encapsulates a collection of cell relevant objects, such as [Cell](../cell/), [Row](../row/), ...etc.

```javascript
class Cells;
```


### Example
```javascript
const { Workbook } = require("aspose.cells.node");

var excel = new Workbook();
var cells = excel.getWorksheets().get(0).getCells();
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
```
## Methods

| Method | Description |
| --- | --- |
| [get(number, number)](#get-number-number-)| Gets the [Cell](../cell/) element at the specified cell row index and column index. |
| [get(string)](#get-string-)| Gets the [Cell](../cell/) element at the specified cell name. |
| [getOdsCellFields()](#getOdsCellFields--)| Gets the list of fields of ods. |
| [getCount()](#getCount--)| Gets the total count of instantiated Cell objects. |
| [getCountLarge()](#getCountLarge--)| Gets the total count of instantiated Cell objects. |
| [getRows()](#getRows--)| Gets the collection of [Row](../row/) objects that represents the individual rows in this worksheet. |
| [getMultiThreadReading()](#getMultiThreadReading--)| Gets or sets whether the cells data model should support Multi-Thread reading. Default value of this property is false. |
| [setMultiThreadReading(boolean)](#setMultiThreadReading-boolean-)| Gets or sets whether the cells data model should support Multi-Thread reading. Default value of this property is false. |
| [getMemorySetting()](#getMemorySetting--)| Gets or sets the memory usage option for this cells. |
| [setMemorySetting(MemorySetting)](#setMemorySetting-memorysetting-)| Gets or sets the memory usage option for this cells. |
| [getStyle()](#getStyle--)| Gets and sets the default style of the worksheet. |
| [setStyle(Style)](#setStyle-style-)| Gets and sets the default style of the worksheet. |
| [getStandardWidthInch()](#getStandardWidthInch--)| Gets or sets the default column width in the worksheet, in unit of inches. |
| [setStandardWidthInch(number)](#setStandardWidthInch-number-)| Gets or sets the default column width in the worksheet, in unit of inches. |
| [getStandardWidthPixels()](#getStandardWidthPixels--)| Gets or sets the default column width in the worksheet, in unit of pixels. |
| [setStandardWidthPixels(number)](#setStandardWidthPixels-number-)| Gets or sets the default column width in the worksheet, in unit of pixels. |
| [getStandardWidth()](#getStandardWidth--)| Gets or sets the default column width in the worksheet, in unit of characters. |
| [setStandardWidth(number)](#setStandardWidth-number-)| Gets or sets the default column width in the worksheet, in unit of characters. |
| [getStandardHeight()](#getStandardHeight--)| Gets or sets the default row height in this worksheet, in unit of points. |
| [setStandardHeight(number)](#setStandardHeight-number-)| Gets or sets the default row height in this worksheet, in unit of points. |
| [getStandardHeightPixels()](#getStandardHeightPixels--)| Gets or sets the default row height in this worksheet, in unit of pixels. |
| [setStandardHeightPixels(number)](#setStandardHeightPixels-number-)| Gets or sets the default row height in this worksheet, in unit of pixels. |
| [getStandardHeightInch()](#getStandardHeightInch--)| Gets or sets the default row height in this worksheet, in unit of inches. |
| [setStandardHeightInch(number)](#setStandardHeightInch-number-)| Gets or sets the default row height in this worksheet, in unit of inches. |
| [getPreserveString()](#getPreserveString--)| Gets or sets a value indicating whether all worksheet values are preserved as strings. Default is false. |
| [setPreserveString(boolean)](#setPreserveString-boolean-)| Gets or sets a value indicating whether all worksheet values are preserved as strings. Default is false. |
| [getMinRow()](#getMinRow--)| Minimum row index of cell which contains data or style. |
| [getMaxRow()](#getMaxRow--)| Maximum row index of cell which contains data or style. |
| [getMinColumn()](#getMinColumn--)| Minimum column index of those cells that have been instantiated in the collection(does not include the column where style is defined for the whole column but no cell has been instantiated in it). |
| [getMaxColumn()](#getMaxColumn--)| Maximum column index of those cells that have been instantiated in the collection(does not include the column where style is defined for the whole column but no cell has been instantiated in it). |
| [getMinDataRow()](#getMinDataRow--)| Minimum row index of cell which contains data. |
| [getMaxDataRow()](#getMaxDataRow--)| Maximum row index of cell which contains data. |
| [getMinDataColumn()](#getMinDataColumn--)| Minimum column index of cell which contains data. |
| [getMaxDataColumn()](#getMaxDataColumn--)| Maximum column index of cell which contains data. |
| [isDefaultRowHeightMatched()](#isDefaultRowHeightMatched--)| Indicates that row height and default font height matches |
| [setIsDefaultRowHeightMatched(boolean)](#setIsDefaultRowHeightMatched-boolean-)| Indicates that row height and default font height matches |
| [isDefaultRowHidden()](#isDefaultRowHidden--)| Indicates whether the row is default hidden. |
| [setIsDefaultRowHidden(boolean)](#setIsDefaultRowHidden-boolean-)| Indicates whether the row is default hidden. |
| [getColumns()](#getColumns--)| Gets the collection of [Column](../column/) objects that represents the individual columns in this worksheet. |
| [getRanges()](#getRanges--)| Gets the collection of [Range](../range/) objects created at run time. |
| [getLastCell()](#getLastCell--)| Gets the last cell in this worksheet. |
| [getMaxDisplayRange()](#getMaxDisplayRange--)| Gets the max range which includes data, merged cells and shapes. |
| [getFirstCell()](#getFirstCell--)| Gets the first cell in this worksheet. |
| [dispose()](#dispose--)| Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [getEnumerator()](#getEnumerator--)| Gets the cells enumerator. |
| [getMergedAreas()](#getMergedAreas--)| Gets all merged cells. |
| [getCell(number, number)](#getCell-number-number-)| Gets the [Cell](../cell/) element or null at the specified cell row index and column index. |
| [getRow(number)](#getRow-number-)| Gets the [Row](../row/) element at the specified cell row index. |
| [checkCell(number, number)](#checkCell-number-number-)| Gets the [Cell](../cell/) element or null at the specified cell row index and column index. |
| [checkRow(number)](#checkRow-number-)| Gets the [Row](../row/) element or null at the specified cell row index. |
| [checkColumn(number)](#checkColumn-number-)| Gets the [Column](../column/) element or null at the specified column index. |
| [isRowHidden(number)](#isRowHidden-number-)| Checks whether a row at given index is hidden. |
| [isColumnHidden(number)](#isColumnHidden-number-)| Checks whether a column at given index is hidden. |
| [addRange(Range)](#addRange-range-)| Adds a range object reference to cells |
| [createRange(string, string)](#createRange-string-string-)| Creates a [Range](../range/) object from a range of cells. |
| [createRange(number, number, number, number)](#createRange-number-number-number-number-)| Creates a [Range](../range/) object from a range of cells. |
| [createRange(string)](#createRange-string-)| Creates a [Range](../range/) object from an address of the range. |
| [createRange(number, number, boolean)](#createRange-number-number-boolean-)| Creates a [Range](../range/) object from rows of cells or columns of cells. |
| [clear()](#clear--)| Clears all data of the worksheet. |
| [importObjectArray(object[], number, number, boolean, number)](#importObjectArray-objectarray-number-number-boolean-number-)| Imports an array of data into a worksheet. |
| [importFormulaArray(string[], number, number, boolean)](#importFormulaArray-stringarray-number-number-boolean-)| Imports an array of formula into a worksheet. |
| [textToColumns(number, number, number, TxtLoadOptions)](#textToColumns-number-number-number-txtloadoptions-)| Splits content in specified column into multiple columns.. |
| [importCSV(string, string, boolean, number, number)](#importCSV-string-string-boolean-number-number-)| Import a CSV file to the cells. |
| [importCSV(Uint8Array, string, boolean, number, number)](#importCSV-uint8array-string-boolean-number-number-)| Import a CSV file to the cells. |
| [importCSV(string, TxtLoadOptions, number, number)](#importCSV-string-txtloadoptions-number-number-)| Import a CSV file to the cells. |
| [importCSV(Uint8Array, TxtLoadOptions, number, number)](#importCSV-uint8array-txtloadoptions-number-number-)| Import a CSV file to the cells. |
| [merge(number, number, number, number)](#merge-number-number-number-number-)| Merges a specified range of cells into a single cell. |
| [merge(number, number, number, number, boolean)](#merge-number-number-number-number-boolean-)| Merges a specified range of cells into a single cell. |
| [merge(number, number, number, number, boolean, boolean)](#merge-number-number-number-number-boolean-boolean-)| Merges a specified range of cells into a single cell. |
| [unMerge(number, number, number, number)](#unMerge-number-number-number-number-)| Unmerges a specified range of merged cells. |
| [clearMergedCells()](#clearMergedCells--)| Clears all merged ranges. |
| [hideRow(number)](#hideRow-number-)| Hides a row. |
| [unhideRow(number, number)](#unhideRow-number-number-)| Unhides a row. |
| [hideRows(number, number)](#hideRows-number-number-)| Hides multiple rows. |
| [unhideRows(number, number, number)](#unhideRows-number-number-number-)| Unhides the hidden rows. |
| [setRowHeightPixel(number, number)](#setRowHeightPixel-number-number-)| Sets row height in unit of pixels. |
| [setRowHeightInch(number, number)](#setRowHeightInch-number-number-)| Sets row height in unit of inches. |
| [setRowHeight(number, number)](#setRowHeight-number-number-)| Sets the height of the specified row. |
| [getRowHeight(number, boolean, CellsUnitType)](#getRowHeight-number-boolean-cellsunittype-)| Gets row's height. |
| [getRowHeight(number)](#getRowHeight-number-)| Gets the height of a specified row, in unit of points. |
| [getRowOriginalHeightPoint(number)](#getRowOriginalHeightPoint-number-)| Gets original row's height in unit of point if the row is hidden |
| [getColumnWidth(number, boolean, CellsUnitType)](#getColumnWidth-number-boolean-cellsunittype-)| Gets the column width. |
| [getColumnWidth(number)](#getColumnWidth-number-)| Gets the width(in unit of characters) of the specified column in normal view |
| [getColumnOriginalWidthPoint(number)](#getColumnOriginalWidthPoint-number-)| Gets original column's height in unit of point if the column is hidden |
| [hideColumn(number)](#hideColumn-number-)| Hides a column. |
| [unhideColumn(number, number)](#unhideColumn-number-number-)| Unhides a column |
| [hideColumns(number, number)](#hideColumns-number-number-)| Hide multiple columns. |
| [unhideColumns(number, number, number)](#unhideColumns-number-number-number-)| Unhide multiple columns. |
| [getViewRowHeight(number)](#getViewRowHeight-number-)| Gets the height of a specified row. |
| [getRowHeightInch(number)](#getRowHeightInch-number-)| Gets the height of a specified row in unit of inches. |
| [getViewRowHeightInch(number)](#getViewRowHeightInch-number-)| Gets the height of a specified row in unit of inches. |
| [getRowHeightPixel(number)](#getRowHeightPixel-number-)| Gets the height of a specified row in unit of pixel. |
| [setColumnWidthPixel(number, number)](#setColumnWidthPixel-number-number-)| Sets column width in unit of pixels in normal view. |
| [setColumnWidthInch(number, number)](#setColumnWidthInch-number-number-)| Sets column width in unit of inches  in normal view. |
| [setColumnWidth(number, number)](#setColumnWidth-number-number-)| Sets the width of the specified column in normal view. |
| [getColumnWidthPixel(number)](#getColumnWidthPixel-number-)| Gets the width of the specified column in normal view, in units of pixel. |
| [getColumnWidthPixel(number, boolean)](#getColumnWidthPixel-number-boolean-)| Gets the width of the specified column in normal view, in units of pixel. |
| [getColumnWidthInch(number)](#getColumnWidthInch-number-)| Gets the width of the specified column in normal view, in units of inches. |
| [getViewColumnWidthPixel(number)](#getViewColumnWidthPixel-number-)| Get the width in different view type. |
| [setViewColumnWidthPixel(number, number)](#setViewColumnWidthPixel-number-number-)| Sets the width of the column in different view. |
| [getLastDataRow(number)](#getLastDataRow-number-)| Gets the last row index of cell which contains data in the specified column. |
| [applyColumnStyle(number, Style, StyleFlag)](#applyColumnStyle-number-style-styleflag-)| Applies formats for a whole column. |
| [applyRowStyle(number, Style, StyleFlag)](#applyRowStyle-number-style-styleflag-)| Applies formats for a whole row. |
| [applyStyle(Style, StyleFlag)](#applyStyle-style-styleflag-)| Applies formats for a whole worksheet. |
| [copyColumns(Cells, number, number, number, PasteOptions)](#copyColumns-cells-number-number-number-pasteoptions-)| Copies data and formats of a whole column. |
| [copyColumns(Cells, number, number, number)](#copyColumns-cells-number-number-number-)| Copies data and formats of a whole column. |
| [copyColumns(Cells, number, number, number, number)](#copyColumns-cells-number-number-number-number-)| Copies data and formats of the whole columns. |
| [copyColumn(Cells, number, number)](#copyColumn-cells-number-number-)| Copies data and formats of a whole column. |
| [copyRow(Cells, number, number)](#copyRow-cells-number-number-)| Copies data and formats of a whole row. |
| [copyRows(Cells, number, number, number)](#copyRows-cells-number-number-number-)| Copies data and formats of some whole rows. |
| [copyRows(Cells, number, number, number, CopyOptions)](#copyRows-cells-number-number-number-copyoptions-)| Copies data and formats of some whole rows. |
| [copyRows(Cells, number, number, number, CopyOptions, PasteOptions)](#copyRows-cells-number-number-number-copyoptions-pasteoptions-)| Copies data and formats of some whole rows. |
| [getGroupedRowOutlineLevel(number)](#getGroupedRowOutlineLevel-number-)| Gets the outline level (zero-based) of the row. |
| [getGroupedColumnOutlineLevel(number)](#getGroupedColumnOutlineLevel-number-)| Gets the outline level (zero-based) of the column. |
| [getMaxGroupedColumnOutlineLevel()](#getMaxGroupedColumnOutlineLevel--)| Gets the max grouped column outline level (zero-based). |
| [getMaxGroupedRowOutlineLevel()](#getMaxGroupedRowOutlineLevel--)| Gets the max grouped row outline level (zero-based). |
| [showGroupDetail(boolean, number)](#showGroupDetail-boolean-number-)| Expands the grouped rows/columns. |
| [hideGroupDetail(boolean, number)](#hideGroupDetail-boolean-number-)| Collapses the grouped rows/columns. |
| [ungroupColumns(number, number)](#ungroupColumns-number-number-)| Ungroups columns. |
| [groupColumns(number, number)](#groupColumns-number-number-)| Groups columns. |
| [groupColumns(number, number, boolean)](#groupColumns-number-number-boolean-)| Groups columns. |
| [ungroupRows(number, number, boolean)](#ungroupRows-number-number-boolean-)| Ungroups rows. |
| [ungroupRows(number, number)](#ungroupRows-number-number-)| Ungroups rows. |
| [groupRows(number, number, boolean)](#groupRows-number-number-boolean-)| Groups rows. |
| [groupRows(number, number)](#groupRows-number-number-)| Groups rows. |
| [deleteColumn(number, boolean)](#deleteColumn-number-boolean-)| Deletes a column. |
| [deleteColumn(number)](#deleteColumn-number-)| Deletes a column. |
| [deleteColumns(number, number, boolean)](#deleteColumns-number-number-boolean-)| Deletes several columns. |
| [deleteColumns(number, number, DeleteOptions)](#deleteColumns-number-number-deleteoptions-)| Deletes several columns. |
| [isDeletingRangeEnabled(number, number, number, number)](#isDeletingRangeEnabled-number-number-number-number-)| Check whether the range could be deleted. |
| [deleteRow(number)](#deleteRow-number-)| Deletes a row. |
| [deleteRow(number, boolean)](#deleteRow-number-boolean-)| Deletes a row. |
| [deleteRows(number, number)](#deleteRows-number-number-)| Deletes multiple rows. |
| [deleteRows(number, number, boolean)](#deleteRows-number-number-boolean-)| Deletes multiple rows in the worksheet. |
| [deleteRows(number, number, DeleteOptions)](#deleteRows-number-number-deleteoptions-)| Deletes multiple rows in the worksheet. |
| [deleteBlankColumns()](#deleteBlankColumns--)| Delete all blank columns which do not contain any data. |
| [deleteBlankColumns(DeleteOptions)](#deleteBlankColumns-deleteoptions-)| Delete all blank columns which do not contain any data. |
| [isBlankColumn(number)](#isBlankColumn-number-)| Checks whether given column is blank(does not contain any data). |
| [deleteBlankRows()](#deleteBlankRows--)| Delete all blank rows which do not contain any data or other object. |
| [deleteBlankRows(DeleteOptions)](#deleteBlankRows-deleteoptions-)| Delete all blank rows which do not contain any data or some special objects such as visible comment, pivot table. |
| [insertColumns(number, number)](#insertColumns-number-number-)| Inserts some columns into the worksheet. |
| [insertColumns(number, number, boolean)](#insertColumns-number-number-boolean-)| Inserts some columns into the worksheet. |
| [insertColumns(number, number, InsertOptions)](#insertColumns-number-number-insertoptions-)| Inserts some columns into the worksheet. |
| [insertColumn(number, boolean)](#insertColumn-number-boolean-)| Inserts a new column into the worksheet. |
| [insertColumn(number)](#insertColumn-number-)| Inserts a new column into the worksheet. |
| [insertRows(number, number, boolean)](#insertRows-number-number-boolean-)| Inserts multiple rows into the worksheet. |
| [insertRows(number, number, InsertOptions)](#insertRows-number-number-insertoptions-)| Inserts multiple rows into the worksheet. |
| [insertRows(number, number)](#insertRows-number-number-)| Inserts multiple rows into the worksheet. |
| [insertRow(number)](#insertRow-number-)| Inserts a new row into the worksheet. |
| [clearRange(CellArea)](#clearRange-cellarea-)| Clears contents and formatting of a range. |
| [clearRange(number, number, number, number)](#clearRange-number-number-number-number-)| Clears contents and formatting of a range. |
| [clearContents(CellArea)](#clearContents-cellarea-)| Clears contents of a range. |
| [clearContents(number, number, number, number)](#clearContents-number-number-number-number-)| Clears contents of a range. |
| [clearFormats(CellArea)](#clearFormats-cellarea-)| Clears formatting of a range. |
| [clearFormats(number, number, number, number)](#clearFormats-number-number-number-number-)| Clears formatting of a range. |
| [linkToXmlMap(string, number, number, string)](#linkToXmlMap-string-number-number-string-)| Link to a xml map. |
| [find(object, Cell)](#find-object-cell-)| Finds the cell containing with the input object. |
| [find(object, Cell, FindOptions)](#find-object-cell-findoptions-)| Finds the cell containing with the input object. |
| [endCellInRow(number)](#endCellInRow-number-)| Gets the last cell in this row. |
| [endCellInRow(number, number, number, number)](#endCellInRow-number-number-number-number-)| Gets the last cell with maximum row index in this range. |
| [endCellInColumn(number)](#endCellInColumn-number-)| Gets the last cell in this column. |
| [endCellInColumn(number, number, number, number)](#endCellInColumn-number-number-number-number-)| Gets the last cell with maximum column index in this range. |
| [moveRange(CellArea, number, number)](#moveRange-cellarea-number-number-)| Moves the range. |
| [insertCutCells(Range, number, number, ShiftType)](#insertCutCells-range-number-number-shifttype-)| Insert cut range. |
| [insertRange(CellArea, number, ShiftType, boolean)](#insertRange-cellarea-number-shifttype-boolean-)| Inserts a range of cells and shift cells according to the shift option. |
| [insertRange(CellArea, ShiftType)](#insertRange-cellarea-shifttype-)| Inserts a range of cells and shift cells according to the shift option. |
| [insertRange(CellArea, number, ShiftType)](#insertRange-cellarea-number-shifttype-)| Inserts a range of cells and shift cells according to the shift option. |
| [deleteRange(number, number, number, number, ShiftType)](#deleteRange-number-number-number-number-shifttype-)| Deletes a range of cells and shift cells according to the shift option. |
| [exportArray(number, number, number, number)](#exportArray-number-number-number-number-)| Exports data in the [Cells](../cells/) collection to a two-dimension array object. |
| [retrieveSubtotalSetting(CellArea)](#retrieveSubtotalSetting-cellarea-)| Retrieves subtotals setting of the range. |
| [subtotal(CellArea, number, ConsolidationFunction, number[])](#subtotal-cellarea-number-consolidationfunction-numberarray-)| Creates subtotals for the range. |
| [subtotal(CellArea, number, ConsolidationFunction, number[], boolean, boolean, boolean)](#subtotal-cellarea-number-consolidationfunction-numberarray-boolean-boolean-boolean-)| Creates subtotals for the range. |
| [removeFormulas()](#removeFormulas--)| Removes all formula and replaces with the value of the formula. |
| [removeDuplicates()](#removeDuplicates--)| Removes duplicate rows in the sheet. |
| [removeDuplicates(number, number, number, number)](#removeDuplicates-number-number-number-number-)| Removes duplicate values in the range. |
| [removeDuplicates(number, number, number, number, boolean, number[])](#removeDuplicates-number-number-number-number-boolean-numberarray-)| Removes duplicate data of the range. |
| [convertStringToNumericValue()](#convertStringToNumericValue--)| Converts all string data in the worksheet to numeric value if possible. |
| [getDependents(boolean, number, number)](#getDependents-boolean-number-number-)| Get all cells which refer to the specific cell. |
| [getDependentsInCalculation(number, number, boolean)](#getDependentsInCalculation-number-number-boolean-)| Gets all cells whose calculated result depends on specific cell. |
| [getCellsWithPlaceInCellPicture()](#getCellsWithPlaceInCellPicture--)| Gets all cells that contain embedded picture. |
| [getCellStyle(number, number)](#getCellStyle-number-number-)| Get the style of given cell. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### get(number, number) {#get-number-number-}

Gets the [Cell](../cell/) element at the specified cell row index and column index.

```javascript
get(row: number, column: number) : Cell;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | Row index. |
| column | number | Column index. |

**Returns**

The [Cell](../cell/) object.

**Example**
```javascript
const { Workbook } = require("aspose.cells.node");

var excel = new Workbook();
var cells = excel.getWorksheets().get(0).getCells();
var cell = cells.get(0, 0);    //Gets the cell at "A1"
```

### get(string) {#get-string-}

Gets the [Cell](../cell/) element at the specified cell name.

```javascript
get(cellName: string) : Cell;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | string | Cell name,including its column letter and row number, for example A5. |

**Returns**

A [Cell](../cell/) object

**Example**
```javascript
const { Workbook } = require("aspose.cells.node");

var excel = new Workbook();
var cells = excel.getWorksheets().get(0).getCells();
var cell = cells.get("A1");    //Gets the cell at "A1"
```

### getOdsCellFields() {#getOdsCellFields--}

Gets the list of fields of ods.

```javascript
getOdsCellFields() : OdsCellFieldCollection;
```


**Returns**

[OdsCellFieldCollection](../odscellfieldcollection/)

### getCount() {#getCount--}

Gets the total count of instantiated Cell objects.

```javascript
getCount() : number;
```


### getCountLarge() {#getCountLarge--}

Gets the total count of instantiated Cell objects.

```javascript
getCountLarge() : number;
```


### getRows() {#getRows--}

Gets the collection of [Row](../row/) objects that represents the individual rows in this worksheet.

```javascript
getRows() : RowCollection;
```


**Returns**

[RowCollection](../rowcollection/)

### getMultiThreadReading() {#getMultiThreadReading--}

Gets or sets whether the cells data model should support Multi-Thread reading. Default value of this property is false.

```javascript
getMultiThreadReading() : boolean;
```


**Remarks**

If there are multiple threads to read Row/Cell objects in this collection concurrently, this property should be set as true, otherwise unexpected result may be produced. Supporting Multi-Thread reading may degrade the performance for accessing Row/Cell objects from this collection. Please note, some features cannot support Multi-Thread reading, such as formatting values(by [Cell.StringValue](../cell.stringvalue/), [Cell.DisplayStringValue](../cell.displaystringvalue/), .etc.). So, even with this property being set as true, those APIs still may give unexpected result for Multi-Thread reading.

### setMultiThreadReading(boolean) {#setMultiThreadReading-boolean-}

Gets or sets whether the cells data model should support Multi-Thread reading. Default value of this property is false.

```javascript
setMultiThreadReading(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

If there are multiple threads to read Row/Cell objects in this collection concurrently, this property should be set as true, otherwise unexpected result may be produced. Supporting Multi-Thread reading may degrade the performance for accessing Row/Cell objects from this collection. Please note, some features cannot support Multi-Thread reading, such as formatting values(by [Cell.StringValue](../cell.stringvalue/), [Cell.DisplayStringValue](../cell.displaystringvalue/), .etc.). So, even with this property being set as true, those APIs still may give unexpected result for Multi-Thread reading.

### getMemorySetting() {#getMemorySetting--}

Gets or sets the memory usage option for this cells.

```javascript
getMemorySetting() : MemorySetting;
```


**Returns**

[MemorySetting](../memorysetting/)

### setMemorySetting(MemorySetting) {#setMemorySetting-memorysetting-}

Gets or sets the memory usage option for this cells.

```javascript
setMemorySetting(value: MemorySetting) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MemorySetting](../memorysetting/) | The value to set. |

### getStyle() {#getStyle--}

Gets and sets the default style of the worksheet.

```javascript
getStyle() : Style;
```


**Returns**

[Style](../style/)

### setStyle(Style) {#setStyle-style-}

Gets and sets the default style of the worksheet.

```javascript
setStyle(value: Style) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Style](../style/) | The value to set. |

### getStandardWidthInch() {#getStandardWidthInch--}

Gets or sets the default column width in the worksheet, in unit of inches.

```javascript
getStandardWidthInch() : number;
```


### setStandardWidthInch(number) {#setStandardWidthInch-number-}

Gets or sets the default column width in the worksheet, in unit of inches.

```javascript
setStandardWidthInch(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getStandardWidthPixels() {#getStandardWidthPixels--}

Gets or sets the default column width in the worksheet, in unit of pixels.

```javascript
getStandardWidthPixels() : number;
```


### setStandardWidthPixels(number) {#setStandardWidthPixels-number-}

Gets or sets the default column width in the worksheet, in unit of pixels.

```javascript
setStandardWidthPixels(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getStandardWidth() {#getStandardWidth--}

Gets or sets the default column width in the worksheet, in unit of characters.

```javascript
getStandardWidth() : number;
```


### setStandardWidth(number) {#setStandardWidth-number-}

Gets or sets the default column width in the worksheet, in unit of characters.

```javascript
setStandardWidth(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getStandardHeight() {#getStandardHeight--}

Gets or sets the default row height in this worksheet, in unit of points.

```javascript
getStandardHeight() : number;
```


### setStandardHeight(number) {#setStandardHeight-number-}

Gets or sets the default row height in this worksheet, in unit of points.

```javascript
setStandardHeight(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getStandardHeightPixels() {#getStandardHeightPixels--}

Gets or sets the default row height in this worksheet, in unit of pixels.

```javascript
getStandardHeightPixels() : number;
```


### setStandardHeightPixels(number) {#setStandardHeightPixels-number-}

Gets or sets the default row height in this worksheet, in unit of pixels.

```javascript
setStandardHeightPixels(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getStandardHeightInch() {#getStandardHeightInch--}

Gets or sets the default row height in this worksheet, in unit of inches.

```javascript
getStandardHeightInch() : number;
```


### setStandardHeightInch(number) {#setStandardHeightInch-number-}

Gets or sets the default row height in this worksheet, in unit of inches.

```javascript
setStandardHeightInch(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getPreserveString() {#getPreserveString--}

Gets or sets a value indicating whether all worksheet values are preserved as strings. Default is false.

```javascript
getPreserveString() : boolean;
```


### setPreserveString(boolean) {#setPreserveString-boolean-}

Gets or sets a value indicating whether all worksheet values are preserved as strings. Default is false.

```javascript
setPreserveString(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getMinRow() {#getMinRow--}

Minimum row index of cell which contains data or style.

```javascript
getMinRow() : number;
```


### getMaxRow() {#getMaxRow--}

Maximum row index of cell which contains data or style.

```javascript
getMaxRow() : number;
```


**Remarks**

Return -1 if there is no cell which contains data or style in the worksheet.

### getMinColumn() {#getMinColumn--}

Minimum column index of those cells that have been instantiated in the collection(does not include the column where style is defined for the whole column but no cell has been instantiated in it).

```javascript
getMinColumn() : number;
```


### getMaxColumn() {#getMaxColumn--}

Maximum column index of those cells that have been instantiated in the collection(does not include the column where style is defined for the whole column but no cell has been instantiated in it).

```javascript
getMaxColumn() : number;
```


**Remarks**

Return -1 if there is no cell.

### getMinDataRow() {#getMinDataRow--}

Minimum row index of cell which contains data.

```javascript
getMinDataRow() : number;
```


### getMaxDataRow() {#getMaxDataRow--}

Maximum row index of cell which contains data.

```javascript
getMaxDataRow() : number;
```


**Remarks**

Return -1 if there is no cell which contains data.

### getMinDataColumn() {#getMinDataColumn--}

Minimum column index of cell which contains data.

```javascript
getMinDataColumn() : number;
```


**Remarks**

-1 will be returned if there is no cell which contains data. This property needs to iterate and check all cells in a worksheet, so it is a time-consumed progress and should not be invoked repeatedly.

### getMaxDataColumn() {#getMaxDataColumn--}

Maximum column index of cell which contains data.

```javascript
getMaxDataColumn() : number;
```


**Remarks**

-1 will be returned if there is no cell which contains data. This property needs to iterate and check all cells in a worksheet, so it is a time-consumed progress and should not be invoked repeatedly.

### isDefaultRowHeightMatched() {#isDefaultRowHeightMatched--}

Indicates that row height and default font height matches

```javascript
isDefaultRowHeightMatched() : boolean;
```


### setIsDefaultRowHeightMatched(boolean) {#setIsDefaultRowHeightMatched-boolean-}

Indicates that row height and default font height matches

```javascript
setIsDefaultRowHeightMatched(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isDefaultRowHidden() {#isDefaultRowHidden--}

Indicates whether the row is default hidden.

```javascript
isDefaultRowHidden() : boolean;
```


### setIsDefaultRowHidden(boolean) {#setIsDefaultRowHidden-boolean-}

Indicates whether the row is default hidden.

```javascript
setIsDefaultRowHidden(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getColumns() {#getColumns--}

Gets the collection of [Column](../column/) objects that represents the individual columns in this worksheet.

```javascript
getColumns() : ColumnCollection;
```


**Returns**

[ColumnCollection](../columncollection/)

### getRanges() {#getRanges--}

Gets the collection of [Range](../range/) objects created at run time.

```javascript
getRanges() : RangeCollection;
```


**Returns**

[RangeCollection](../rangecollection/)

### getLastCell() {#getLastCell--}

Gets the last cell in this worksheet.

```javascript
getLastCell() : Cell;
```


**Returns**

[Cell](../cell/)

**Remarks**

Returns null if there is no data in the worksheet.

### getMaxDisplayRange() {#getMaxDisplayRange--}

Gets the max range which includes data, merged cells and shapes.

```javascript
getMaxDisplayRange() : Range;
```


**Returns**

[Range](../range/)

**Remarks**

Reutrns null if the worksheet is empty since Aspose.Cells 21.5.2.

### getFirstCell() {#getFirstCell--}

Gets the first cell in this worksheet.

```javascript
getFirstCell() : Cell;
```


**Returns**

[Cell](../cell/)

**Remarks**

Returns null if there is no data in the worksheet.

### dispose() {#dispose--}

Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources.

```javascript
dispose() : void;
```


### getEnumerator() {#getEnumerator--}

Gets the cells enumerator.

```javascript
getEnumerator() : CellEnumerator;
```


**Returns**

The cells enumerator

**Remarks**

When traversing elements by the returned Enumerator, the cells collection should not be modified(such as operations that will cause new Cell/Row be instantiated or existing Cell/Row be deleted). Otherwise the enumerator may not be able to traverse all cells correctly(some elements may be traversed repeatedly or skipped).

### getMergedAreas() {#getMergedAreas--}

Gets all merged cells.

```javascript
getMergedAreas() : CellArea[];
```


**Returns**

[CellArea](../cellarea/)[]

### getCell(number, number) {#getCell-number-number-}

Gets the [Cell](../cell/) element or null at the specified cell row index and column index.

```javascript
getCell(row: number, column: number) : Cell;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | Row index |
| column | number | Column index |

**Returns**

Return Cell object if a Cell object exists. Return null if the cell does not exist.

**Remarks**

NOTE: This member is now obsolete. Instead, please use CheckCell(int row, int column) method. This method will be removed 12 months later since February 2024. Aspose apologizes for any inconvenience you may have experienced.

### getRow(number) {#getRow-number-}

Gets the [Row](../row/) element at the specified cell row index.

```javascript
getRow(row: number) : Row;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | Row index |

**Returns**

If the row object does exist return Row object, otherwise return null.

**Remarks**

NOTE: This member is now obsolete. Instead, please use Cells.CheckRow(int row) method. This method will be removed 12 months later since February 2024. Aspose apologizes for any inconvenience you may have experienced.

### checkCell(number, number) {#checkCell-number-number-}

Gets the [Cell](../cell/) element or null at the specified cell row index and column index.

```javascript
checkCell(row: number, column: number) : Cell;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | Row index |
| column | number | Column index |

**Returns**

Return Cell object if a Cell object exists. Return null if the cell does not exist.

### checkRow(number) {#checkRow-number-}

Gets the [Row](../row/) element or null at the specified cell row index.

```javascript
checkRow(row: number) : Row;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | Row index |

**Returns**

Returns [Row](../row/) object If the row object does exist, otherwise returns null.

### checkColumn(number) {#checkColumn-number-}

Gets the [Column](../column/) element or null at the specified column index.

```javascript
checkColumn(columnIndex: number) : Column;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | number | The column index. |

**Returns**

The Column object.

### isRowHidden(number) {#isRowHidden-number-}

Checks whether a row at given index is hidden.

```javascript
isRowHidden(rowIndex: number) : boolean;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | number | row index |

**Returns**

true if the row is hidden

### isColumnHidden(number) {#isColumnHidden-number-}

Checks whether a column at given index is hidden.

```javascript
isColumnHidden(columnIndex: number) : boolean;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | number | column index |

**Returns**

true if the column is hidden.

### addRange(Range) {#addRange-range-}

Adds a range object reference to cells

```javascript
addRange(rangeObject: Range) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rangeObject | [Range](../range/) | The range object will be contained in the cells |

### createRange(string, string) {#createRange-string-string-}

Creates a [Range](../range/) object from a range of cells.

```javascript
createRange(upperLeftCell: string, lowerRightCell: string) : Range;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftCell | string | Upper left cell name. |
| lowerRightCell | string | Lower right cell name. |

**Returns**

A [Range](../range/) object

### createRange(number, number, number, number) {#createRange-number-number-number-number-}

Creates a [Range](../range/) object from a range of cells.

```javascript
createRange(firstRow: number, firstColumn: number, totalRows: number, totalColumns: number) : Range;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | number | First row of this range |
| firstColumn | number | First column of this range |
| totalRows | number | Number of rows |
| totalColumns | number | Number of columns |

**Returns**

A [Range](../range/) object

### createRange(string) {#createRange-string-}

Creates a [Range](../range/) object from an address of the range.

```javascript
createRange(address: string) : Range;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| address | string | The address of the range. |

**Returns**

A [Range](../range/) object

### createRange(number, number, boolean) {#createRange-number-number-boolean-}

Creates a [Range](../range/) object from rows of cells or columns of cells.

```javascript
createRange(firstIndex: number, number: number, isVertical: boolean) : Range;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | number | First row index or first column index, zero based. |
| number | number | Total number of rows or columns, one based. |
| isVertical | boolean | True - Range created from columns of cells. False - Range created from rows of cells. |

**Returns**

A [Range](../range/) object.

### clear() {#clear--}

Clears all data of the worksheet.

```javascript
clear() : void;
```


### importObjectArray(object[], number, number, boolean, number) {#importObjectArray-objectarray-number-number-boolean-number-}

Imports an array of data into a worksheet.

```javascript
importObjectArray(objArray: object[], firstRow: number, firstColumn: number, isVertical: boolean, skip: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| objArray | object[] | Data array. |
| firstRow | number | The row number of the first cell to import in. |
| firstColumn | number | The column number of the first cell to import in. |
| isVertical | boolean | Specifies to import data vertically or horizontally. |
| skip | number | Skipped number of rows or columns. |

### importFormulaArray(string[], number, number, boolean) {#importFormulaArray-stringarray-number-number-boolean-}

Imports an array of formula into a worksheet.

```javascript
importFormulaArray(stringArray: string[], firstRow: number, firstColumn: number, isVertical: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stringArray | string[] | Formula array. |
| firstRow | number | The row number of the first cell to import in. |
| firstColumn | number | The column number of the first cell to import in. |
| isVertical | boolean | Specifies to import data vertically or horizontally. |

### textToColumns(number, number, number, TxtLoadOptions) {#textToColumns-number-number-number-txtloadoptions-}

Splits content in specified column into multiple columns..

```javascript
textToColumns(row: number, column: number, totalRows: number, options: TxtLoadOptions) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | The row index. |
| column | number | The column index. |
| totalRows | number | The number of rows. |
| options | [TxtLoadOptions](../txtloadoptions/) | The split options. |

**Returns**

Total column count of the split values.

### importCSV(string, string, boolean, number, number) {#importCSV-string-string-boolean-number-number-}

Import a CSV file to the cells.

```javascript
importCSV(fileName: string, splitter: string, convertNumericData: boolean, firstRow: number, firstColumn: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | string | The CSV file name. |
| splitter | string | The splitter |
| convertNumericData | boolean | Whether the string in text file is converted to numeric data. |
| firstRow | number | The row number of the first cell to import in. |
| firstColumn | number | The column number of the first cell to import in. |

### importCSV(Uint8Array, string, boolean, number, number) {#importCSV-uint8array-string-boolean-number-number-}

Import a CSV file to the cells.

```javascript
importCSV(stream: Uint8Array, splitter: string, convertNumericData: boolean, firstRow: number, firstColumn: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | Uint8Array | The CSV file stream. |
| splitter | string | The splitter |
| convertNumericData | boolean | Whether the string in text file is converted to numeric data. |
| firstRow | number | The row number of the first cell to import in. |
| firstColumn | number | The column number of the first cell to import in. |

### importCSV(string, TxtLoadOptions, number, number) {#importCSV-string-txtloadoptions-number-number-}

Import a CSV file to the cells.

```javascript
importCSV(fileName: string, options: TxtLoadOptions, firstRow: number, firstColumn: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | string | The CSV file name. |
| options | [TxtLoadOptions](../txtloadoptions/) | The load options for reading text file |
| firstRow | number | The row number of the first cell to import in. |
| firstColumn | number | The column number of the first cell to import in. |

### importCSV(Uint8Array, TxtLoadOptions, number, number) {#importCSV-uint8array-txtloadoptions-number-number-}

Import a CSV file to the cells.

```javascript
importCSV(stream: Uint8Array, options: TxtLoadOptions, firstRow: number, firstColumn: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | Uint8Array | The CSV file stream. |
| options | [TxtLoadOptions](../txtloadoptions/) | The load options for reading text file |
| firstRow | number | The row number of the first cell to import in. |
| firstColumn | number | The column number of the first cell to import in. |

### merge(number, number, number, number) {#merge-number-number-number-number-}

Merges a specified range of cells into a single cell.

```javascript
merge(firstRow: number, firstColumn: number, totalRows: number, totalColumns: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | number | First row of this range(zero based) |
| firstColumn | number | First column of this range(zero based) |
| totalRows | number | Number of rows(one based) |
| totalColumns | number | Number of columns(one based) |

**Remarks**

Reference the merged cell via the address of the upper-left cell in the range.

### merge(number, number, number, number, boolean) {#merge-number-number-number-number-boolean-}

Merges a specified range of cells into a single cell.

```javascript
merge(firstRow: number, firstColumn: number, totalRows: number, totalColumns: number, mergeConflict: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | number | First row of this range(zero based) |
| firstColumn | number | First column of this range(zero based) |
| totalRows | number | Number of rows(one based) |
| totalColumns | number | Number of columns(one based) |
| mergeConflict | boolean | Merge conflict merged ranges. |

**Remarks**

Reference the merged cell via the address of the upper-left cell in the range. If mergeConflict is true and the merged range conflicts with other merged cells, other merged cells will be  automatically removed.

### merge(number, number, number, number, boolean, boolean) {#merge-number-number-number-number-boolean-boolean-}

Merges a specified range of cells into a single cell.

```javascript
merge(firstRow: number, firstColumn: number, totalRows: number, totalColumns: number, checkConflict: boolean, mergeConflict: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | number | First row of this range(zero based) |
| firstColumn | number | First column of this range(zero based) |
| totalRows | number | Number of rows(one based) |
| totalColumns | number | Number of columns(one based) |
| checkConflict | boolean | Indicates whether check the merged cells intersects other merged cells |
| mergeConflict | boolean | Merge conflict merged ranges. |

**Remarks**

Reference the merged cell via the address of the upper-left cell in the range. If mergeConflict is true and the merged range conflicts with other merged cells, other merged cells will be  automatically removed.

### unMerge(number, number, number, number) {#unMerge-number-number-number-number-}

Unmerges a specified range of merged cells.

```javascript
unMerge(firstRow: number, firstColumn: number, totalRows: number, totalColumns: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | number | First row of this range(zero based) |
| firstColumn | number | First column of this range(zero based) |
| totalRows | number | Number of rows(one based) |
| totalColumns | number | Number of columns(one based) |

### clearMergedCells() {#clearMergedCells--}

Clears all merged ranges.

```javascript
clearMergedCells() : void;
```


### hideRow(number) {#hideRow-number-}

Hides a row.

```javascript
hideRow(row: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | Row index. |

### unhideRow(number, number) {#unhideRow-number-number-}

Unhides a row.

```javascript
unhideRow(row: number, height: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | Row index. |
| height | number | Row height. The row's height will be changed only when the row is hidden and given height value is positive. |

### hideRows(number, number) {#hideRows-number-number-}

Hides multiple rows.

```javascript
hideRows(row: number, totalRows: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | The row index. |
| totalRows | number | The row number. |

### unhideRows(number, number, number) {#unhideRows-number-number-number-}

Unhides the hidden rows.

```javascript
unhideRows(row: number, totalRows: number, height: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | The row index. |
| totalRows | number | The row number. |
| height | number | Row height. The row's height will be changed only when the row is hidden and given height value is positive. |

### setRowHeightPixel(number, number) {#setRowHeightPixel-number-number-}

Sets row height in unit of pixels.

```javascript
setRowHeightPixel(row: number, pixels: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | Row index. |
| pixels | number | Number of pixels. |

### setRowHeightInch(number, number) {#setRowHeightInch-number-number-}

Sets row height in unit of inches.

```javascript
setRowHeightInch(row: number, inches: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | Row index. |
| inches | number | Number of inches. It should be between 0 and 409.5/72. |

### setRowHeight(number, number) {#setRowHeight-number-number-}

Sets the height of the specified row.

```javascript
setRowHeight(row: number, height: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | Row index. |
| height | number | Height of row.In unit of point It should be between 0 and 409.5. |

### getRowHeight(number, boolean, CellsUnitType) {#getRowHeight-number-boolean-cellsunittype-}

Gets row's height.

```javascript
getRowHeight(row: number, isOriginal: boolean, unitType: CellsUnitType) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | The row index. |
| isOriginal | boolean | Whether returns the original row height or 0 for hidden row. |
| unitType | [CellsUnitType](../cellsunittype/) | Unit type of the returned height value |

**Returns**

Row's height

### getRowHeight(number) {#getRowHeight-number-}

Gets the height of a specified row, in unit of points.

```javascript
getRowHeight(row: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | Row index |

**Returns**

Height of row

### getRowOriginalHeightPoint(number) {#getRowOriginalHeightPoint-number-}

Gets original row's height in unit of point if the row is hidden

```javascript
getRowOriginalHeightPoint(row: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | The row index. |

**Remarks**

NOTE: This member is now obsolete. Instead, please use Cells.GetRowHeight(int,bool,CellsUnitType) method. This method will be removed 12 months later since April 2024. Aspose apologizes for any inconvenience you may have experienced.

### getColumnWidth(number, boolean, CellsUnitType) {#getColumnWidth-number-boolean-cellsunittype-}

Gets the column width.

```javascript
getColumnWidth(column: number, isOriginal: boolean, unitType: CellsUnitType) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | number | The column index. |
| isOriginal | boolean | Indicates whether getting original width. |
| unitType | [CellsUnitType](../cellsunittype/) |  |

### getColumnWidth(number) {#getColumnWidth-number-}

Gets the width(in unit of characters) of the specified column in normal view

```javascript
getColumnWidth(column: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | number | Column index |

**Returns**

Width of column. For spreadsheet, column width is measured as the number of characters of the maximum digit width of the numbers 0~9 as rendered in the normal style's font.

### getColumnOriginalWidthPoint(number) {#getColumnOriginalWidthPoint-number-}

Gets original column's height in unit of point if the column is hidden

```javascript
getColumnOriginalWidthPoint(column: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | number | The row index. |

**Remarks**

NOTE: This method is now obsolete. Instead, please use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method. This method will be removed 12 months later since April 2024. Aspose apologizes for any inconvenience you may have experienced.

### hideColumn(number) {#hideColumn-number-}

Hides a column.

```javascript
hideColumn(column: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | number | Column index. |

### unhideColumn(number, number) {#unhideColumn-number-number-}

Unhides a column

```javascript
unhideColumn(column: number, width: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | number | Column index. |
| width | number | Column width. |

### hideColumns(number, number) {#hideColumns-number-number-}

Hide multiple columns.

```javascript
hideColumns(column: number, totalColumns: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | number | Column index. |
| totalColumns | number | Column number. |

### unhideColumns(number, number, number) {#unhideColumns-number-number-number-}

Unhide multiple columns.

```javascript
unhideColumns(column: number, totalColumns: number, width: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | number | Column index. |
| totalColumns | number | Column number |
| width | number | Column width. |

**Remarks**

Only applies the column width to the hidden columns.

### getViewRowHeight(number) {#getViewRowHeight-number-}

Gets the height of a specified row.

```javascript
getViewRowHeight(row: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | Row index. |

**Returns**

Height of row.

### getRowHeightInch(number) {#getRowHeightInch-number-}

Gets the height of a specified row in unit of inches.

```javascript
getRowHeightInch(row: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | Row index |

**Returns**

Height of row

### getViewRowHeightInch(number) {#getViewRowHeightInch-number-}

Gets the height of a specified row in unit of inches.

```javascript
getViewRowHeightInch(row: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | Row index |

**Returns**

Height of row

### getRowHeightPixel(number) {#getRowHeightPixel-number-}

Gets the height of a specified row in unit of pixel.

```javascript
getRowHeightPixel(row: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | Row index |

**Returns**

Height of row

### setColumnWidthPixel(number, number) {#setColumnWidthPixel-number-number-}

Sets column width in unit of pixels in normal view.

```javascript
setColumnWidthPixel(column: number, pixels: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | number | Column index. |
| pixels | number | Number of pixels. |

### setColumnWidthInch(number, number) {#setColumnWidthInch-number-number-}

Sets column width in unit of inches  in normal view.

```javascript
setColumnWidthInch(column: number, inches: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | number | Column index. |
| inches | number | Number of inches. |

### setColumnWidth(number, number) {#setColumnWidth-number-number-}

Sets the width of the specified column in normal view.

```javascript
setColumnWidth(column: number, width: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | number | Column index. |
| width | number | Width of column.Column width must be between 0 and 255. |

**Remarks**

To hide a column, sets column width to zero.

### getColumnWidthPixel(number) {#getColumnWidthPixel-number-}

Gets the width of the specified column in normal view, in units of pixel.

```javascript
getColumnWidthPixel(column: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | number | Column index |

**Returns**

Width of column in normal view.

### getColumnWidthPixel(number, boolean) {#getColumnWidthPixel-number-boolean-}

Gets the width of the specified column in normal view, in units of pixel.

```javascript
getColumnWidthPixel(column: number, original: boolean) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | number | Column index |
| original | boolean | Indicates whether returning original width even when the column is hidden |

**Returns**

Width of column in normal view.

**Remarks**

NOTE: This method is now obsolete. Instead, please use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method. This method will be removed 12 months later since April 2024. Aspose apologizes for any inconvenience you may have experienced.

### getColumnWidthInch(number) {#getColumnWidthInch-number-}

Gets the width of the specified column in normal view, in units of inches.

```javascript
getColumnWidthInch(column: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | number | Column index |

**Returns**

Width of column

**Remarks**

NOTE: This method is now obsolete. Instead, please use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method. This method will be removed 12 months later since April 2024. Aspose apologizes for any inconvenience you may have experienced.

### getViewColumnWidthPixel(number) {#getViewColumnWidthPixel-number-}

Get the width in different view type.

```javascript
getViewColumnWidthPixel(column: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | number | The column index. |

**Returns**

the column width in unit of pixels

### setViewColumnWidthPixel(number, number) {#setViewColumnWidthPixel-number-number-}

Sets the width of the column in different view.

```javascript
setViewColumnWidthPixel(column: number, pixels: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | number | The column index. |
| pixels | number | The width in unit of pixels. |

**Remarks**

If the current view type is [ViewType.PageLayoutView](../viewtype.pagelayoutview/), the column's width is same as printed width.

### getLastDataRow(number) {#getLastDataRow-number-}

Gets the last row index of cell which contains data in the specified column.

```javascript
getLastDataRow(column: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | number | Column index. |

**Returns**

last row index.

### applyColumnStyle(number, Style, StyleFlag) {#applyColumnStyle-number-style-styleflag-}

Applies formats for a whole column.

```javascript
applyColumnStyle(column: number, style: Style, flag: StyleFlag) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | number | The column index. |
| style | [Style](../style/) | The style object which will be applied. |
| flag | [StyleFlag](../styleflag/) | Flags which indicates applied formatting properties. |

### applyRowStyle(number, Style, StyleFlag) {#applyRowStyle-number-style-styleflag-}

Applies formats for a whole row.

```javascript
applyRowStyle(row: number, style: Style, flag: StyleFlag) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | The row index. |
| style | [Style](../style/) | The style object which will be applied. |
| flag | [StyleFlag](../styleflag/) | Flags which indicates applied formatting properties. |

### applyStyle(Style, StyleFlag) {#applyStyle-style-styleflag-}

Applies formats for a whole worksheet.

```javascript
applyStyle(style: Style, flag: StyleFlag) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [Style](../style/) | The style object which will be applied. |
| flag | [StyleFlag](../styleflag/) | Flags which indicates applied formatting properties. |

### copyColumns(Cells, number, number, number, PasteOptions) {#copyColumns-cells-number-number-number-pasteoptions-}

Copies data and formats of a whole column.

```javascript
copyColumns(sourceCells0: Cells, sourceColumnIndex: number, destinationColumnIndex: number, columnNumber: number, pasteOptions: PasteOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells0 | [Cells](../cells/) | Source Cells object contains data and formats to copy. |
| sourceColumnIndex | number | Source column index. |
| destinationColumnIndex | number | Destination column index. |
| columnNumber | number | The copied column number. |
| pasteOptions | [PasteOptions](../pasteoptions/) | the options of pasting. |

### copyColumns(Cells, number, number, number) {#copyColumns-cells-number-number-number-}

Copies data and formats of a whole column.

```javascript
copyColumns(sourceCells0: Cells, sourceColumnIndex: number, destinationColumnIndex: number, columnNumber: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells0 | [Cells](../cells/) | Source Cells object contains data and formats to copy. |
| sourceColumnIndex | number | Source column index. |
| destinationColumnIndex | number | Destination column index. |
| columnNumber | number | The copied column number. |

### copyColumns(Cells, number, number, number, number) {#copyColumns-cells-number-number-number-number-}

Copies data and formats of the whole columns.

```javascript
copyColumns(sourceCells: Cells, sourceColumnIndex: number, sourceTotalColumns: number, destinationColumnIndex: number, destinationTotalColumns: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells | [Cells](../cells/) | Source Cells object contains data and formats to copy. |
| sourceColumnIndex | number | Source column index. |
| sourceTotalColumns | number | The number of the source columns. |
| destinationColumnIndex | number | Destination column index. |
| destinationTotalColumns | number | The number of the destination columns. |

### copyColumn(Cells, number, number) {#copyColumn-cells-number-number-}

Copies data and formats of a whole column.

```javascript
copyColumn(sourceCells: Cells, sourceColumnIndex: number, destinationColumnIndex: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells | [Cells](../cells/) | Source Cells object contains data and formats to copy. |
| sourceColumnIndex | number | Source column index. |
| destinationColumnIndex | number | Destination column index. |

### copyRow(Cells, number, number) {#copyRow-cells-number-number-}

Copies data and formats of a whole row.

```javascript
copyRow(sourceCells: Cells, sourceRowIndex: number, destinationRowIndex: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells | [Cells](../cells/) | Source Cells object contains data and formats to copy. |
| sourceRowIndex | number | Source row index. |
| destinationRowIndex | number | Destination row index. |

### copyRows(Cells, number, number, number) {#copyRows-cells-number-number-number-}

Copies data and formats of some whole rows.

```javascript
copyRows(sourceCells: Cells, sourceRowIndex: number, destinationRowIndex: number, rowNumber: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells | [Cells](../cells/) | Source Cells object contains data and formats to copy. |
| sourceRowIndex | number | Source row index. |
| destinationRowIndex | number | Destination row index. |
| rowNumber | number | The copied row number. |

### copyRows(Cells, number, number, number, CopyOptions) {#copyRows-cells-number-number-number-copyoptions-}

Copies data and formats of some whole rows.

```javascript
copyRows(sourceCells0: Cells, sourceRowIndex: number, destinationRowIndex: number, rowNumber: number, copyOptions: CopyOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells0 | [Cells](../cells/) | Source Cells object contains data and formats to copy. |
| sourceRowIndex | number | Source row index. |
| destinationRowIndex | number | Destination row index. |
| rowNumber | number | The copied row number. |
| copyOptions | [CopyOptions](../copyoptions/) | The copy options. |

### copyRows(Cells, number, number, number, CopyOptions, PasteOptions) {#copyRows-cells-number-number-number-copyoptions-pasteoptions-}

Copies data and formats of some whole rows.

```javascript
copyRows(sourceCells0: Cells, sourceRowIndex: number, destinationRowIndex: number, rowNumber: number, copyOptions: CopyOptions, pasteOptions: PasteOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells0 | [Cells](../cells/) | Source Cells object contains data and formats to copy. |
| sourceRowIndex | number | Source row index. |
| destinationRowIndex | number | Destination row index. |
| rowNumber | number | The copied row number. |
| copyOptions | [CopyOptions](../copyoptions/) | The copy options. |
| pasteOptions | [PasteOptions](../pasteoptions/) | the options of pasting. |

### getGroupedRowOutlineLevel(number) {#getGroupedRowOutlineLevel-number-}

Gets the outline level (zero-based) of the row.

```javascript
getGroupedRowOutlineLevel(rowIndex: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | number | The row index. |

**Returns**

The outline level (zero-based) of the row.

**Remarks**

If the row is not grouped, returns zero.

### getGroupedColumnOutlineLevel(number) {#getGroupedColumnOutlineLevel-number-}

Gets the outline level (zero-based) of the column.

```javascript
getGroupedColumnOutlineLevel(columnIndex: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | number | The column index |

**Returns**

The outline level of the column

**Remarks**

If the column is not grouped, returns zero.

### getMaxGroupedColumnOutlineLevel() {#getMaxGroupedColumnOutlineLevel--}

Gets the max grouped column outline level (zero-based).

```javascript
getMaxGroupedColumnOutlineLevel() : number;
```


**Returns**

The max grouped column outline level (zero-based)

### getMaxGroupedRowOutlineLevel() {#getMaxGroupedRowOutlineLevel--}

Gets the max grouped row outline level (zero-based).

```javascript
getMaxGroupedRowOutlineLevel() : number;
```


**Returns**

The max grouped row outline level (zero-based)

### showGroupDetail(boolean, number) {#showGroupDetail-boolean-number-}

Expands the grouped rows/columns.

```javascript
showGroupDetail(isVertical: boolean, index: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isVertical | boolean | True, expands the grouped rows. |
| index | number | The row/column index |

### hideGroupDetail(boolean, number) {#hideGroupDetail-boolean-number-}

Collapses the grouped rows/columns.

```javascript
hideGroupDetail(isVertical: boolean, index: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isVertical | boolean | True, collapse the grouped rows. |
| index | number | The row/column index |

### ungroupColumns(number, number) {#ungroupColumns-number-number-}

Ungroups columns.

```javascript
ungroupColumns(firstIndex: number, lastIndex: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | number | The first column index to be ungrouped. |
| lastIndex | number | The last column index to be ungrouped. |

### groupColumns(number, number) {#groupColumns-number-number-}

Groups columns.

```javascript
groupColumns(firstIndex: number, lastIndex: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | number | The first column index to be grouped. |
| lastIndex | number | The last column index to be grouped. |

### groupColumns(number, number, boolean) {#groupColumns-number-number-boolean-}

Groups columns.

```javascript
groupColumns(firstIndex: number, lastIndex: number, isHidden: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | number | The first column index to be grouped. |
| lastIndex | number | The last column index to be grouped. |
| isHidden | boolean | Specifies if the grouped columns are hidden. |

### ungroupRows(number, number, boolean) {#ungroupRows-number-number-boolean-}

Ungroups rows.

```javascript
ungroupRows(firstIndex: number, lastIndex: number, isAll: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | number | The first row index to be ungrouped. |
| lastIndex | number | The last row index to be ungrouped. |
| isAll | boolean | True, removes all grouped info.Otherwise, remove the outer group info. |

### ungroupRows(number, number) {#ungroupRows-number-number-}

Ungroups rows.

```javascript
ungroupRows(firstIndex: number, lastIndex: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | number | The first row index to be ungrouped. |
| lastIndex | number | The last row index to be ungrouped. |

**Remarks**

Only removes outer group info.

### groupRows(number, number, boolean) {#groupRows-number-number-boolean-}

Groups rows.

```javascript
groupRows(firstIndex: number, lastIndex: number, isHidden: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | number | The first row index to be grouped. |
| lastIndex | number | The last row index to be grouped. |
| isHidden | boolean | Specifies if the grouped rows are hidden. |

### groupRows(number, number) {#groupRows-number-number-}

Groups rows.

```javascript
groupRows(firstIndex: number, lastIndex: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | number | The first row index to be grouped. |
| lastIndex | number | The last row index to be grouped. |

### deleteColumn(number, boolean) {#deleteColumn-number-boolean-}

Deletes a column.

```javascript
deleteColumn(columnIndex: number, updateReference: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | number | Index of the column to be deleted. |
| updateReference | boolean | Indicates whether update references in other worksheets. |

### deleteColumn(number) {#deleteColumn-number-}

Deletes a column.

```javascript
deleteColumn(columnIndex: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | number | Index of the column to be deleted. |

### deleteColumns(number, number, boolean) {#deleteColumns-number-number-boolean-}

Deletes several columns.

```javascript
deleteColumns(columnIndex: number, totalColumns: number, updateReference: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | number | Index of the first column to be deleted. |
| totalColumns | number | Count of columns to be deleted. |
| updateReference | boolean | Indicates whether update references in other worksheets. |

### deleteColumns(number, number, DeleteOptions) {#deleteColumns-number-number-deleteoptions-}

Deletes several columns.

```javascript
deleteColumns(columnIndex: number, totalColumns: number, options: DeleteOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | number | Index of the first column to be deleted. |
| totalColumns | number | Count of columns to be deleted. |
| options | [DeleteOptions](../deleteoptions/) | Options for the deleting operation |

### isDeletingRangeEnabled(number, number, number, number) {#isDeletingRangeEnabled-number-number-number-number-}

Check whether the range could be deleted.

```javascript
isDeletingRangeEnabled(startRow: number, startColumn: number, totalRows: number, totalColumns: number) : boolean;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | number | The start row index of the range. |
| startColumn | number | The start column index of the range. |
| totalRows | number | The number of the rows in the range. |
| totalColumns | number | The number of the columns in the range. |

### deleteRow(number) {#deleteRow-number-}

Deletes a row.

```javascript
deleteRow(rowIndex: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | number | Index of the row to be deleted. |

### deleteRow(number, boolean) {#deleteRow-number-boolean-}

Deletes a row.

```javascript
deleteRow(rowIndex: number, updateReference: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | number | Index of the row to be deleted. |
| updateReference | boolean | Indicates whether update references in other worksheets. |

### deleteRows(number, number) {#deleteRows-number-number-}

Deletes multiple rows.

```javascript
deleteRows(rowIndex: number, totalRows: number) : boolean;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | number | The first row index to be deleted. |
| totalRows | number | Count of rows to be deleted. |

**Remarks**

If the deleted range contains the top part(not whole) of the table(ListObject), the ranged could not be deleted and nothing will be done. It works in the same way with MS Excel.

### deleteRows(number, number, boolean) {#deleteRows-number-number-boolean-}

Deletes multiple rows in the worksheet.

```javascript
deleteRows(rowIndex: number, totalRows: number, updateReference: boolean) : boolean;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | number | Index of the first row to be deleted. |
| totalRows | number | Count of rows to be deleted. |
| updateReference | boolean | Indicates whether update references in other worksheets. |

### deleteRows(number, number, DeleteOptions) {#deleteRows-number-number-deleteoptions-}

Deletes multiple rows in the worksheet.

```javascript
deleteRows(rowIndex: number, totalRows: number, options: DeleteOptions) : boolean;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | number | Index of the first row to be deleted. |
| totalRows | number | Count of rows to be deleted. |
| options | [DeleteOptions](../deleteoptions/) | Options for the deleting operation |

### deleteBlankColumns() {#deleteBlankColumns--}

Delete all blank columns which do not contain any data.

```javascript
deleteBlankColumns() : void;
```


### deleteBlankColumns(DeleteOptions) {#deleteBlankColumns-deleteoptions-}

Delete all blank columns which do not contain any data.

```javascript
deleteBlankColumns(options: DeleteOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [DeleteOptions](../deleteoptions/) | The options of deleting range. |

### isBlankColumn(number) {#isBlankColumn-number-}

Checks whether given column is blank(does not contain any data).

```javascript
isBlankColumn(columnIndex: number) : boolean;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | number | the column index |

**Returns**

true if given column does not contain any data

### deleteBlankRows() {#deleteBlankRows--}

Delete all blank rows which do not contain any data or other object.

```javascript
deleteBlankRows() : void;
```


### deleteBlankRows(DeleteOptions) {#deleteBlankRows-deleteoptions-}

Delete all blank rows which do not contain any data or some special objects such as visible comment, pivot table.

```javascript
deleteBlankRows(options: DeleteOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [DeleteOptions](../deleteoptions/) | The options of deleting range. |

**Remarks**

For blank rows that will be deleted, it is not only required that [Row.IsBlank](../row.isblank/) should be true, but also there should be no visible comment defined for any cell in those rows, and no pivot table whose range intersects with them.

### insertColumns(number, number) {#insertColumns-number-number-}

Inserts some columns into the worksheet.

```javascript
insertColumns(columnIndex: number, totalColumns: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | number | Column index. |
| totalColumns | number | The number of columns. |

### insertColumns(number, number, boolean) {#insertColumns-number-number-boolean-}

Inserts some columns into the worksheet.

```javascript
insertColumns(columnIndex: number, totalColumns: number, updateReference: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | number | Column index. |
| totalColumns | number | The number of columns. |
| updateReference | boolean | Indicates if references in other worksheets will be updated. |

### insertColumns(number, number, InsertOptions) {#insertColumns-number-number-insertoptions-}

Inserts some columns into the worksheet.

```javascript
insertColumns(columnIndex: number, totalColumns: number, options: InsertOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | number | Column index. |
| totalColumns | number | The number of columns. |
| options | [InsertOptions](../insertoptions/) | The options for inserting operation. |

### insertColumn(number, boolean) {#insertColumn-number-boolean-}

Inserts a new column into the worksheet.

```javascript
insertColumn(columnIndex: number, updateReference: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | number | Column index. |
| updateReference | boolean | Indicates if references in other worksheets will be updated. |

### insertColumn(number) {#insertColumn-number-}

Inserts a new column into the worksheet.

```javascript
insertColumn(columnIndex: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | number | Column index. |

### insertRows(number, number, boolean) {#insertRows-number-number-boolean-}

Inserts multiple rows into the worksheet.

```javascript
insertRows(rowIndex: number, totalRows: number, updateReference: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | number | Row index. |
| totalRows | number | Number of rows to be inserted. |
| updateReference | boolean | Indicates if references in other worksheets will be updated. |

### insertRows(number, number, InsertOptions) {#insertRows-number-number-insertoptions-}

Inserts multiple rows into the worksheet.

```javascript
insertRows(rowIndex: number, totalRows: number, options: InsertOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | number | Row index. |
| totalRows | number | Number of rows to be inserted. |
| options | [InsertOptions](../insertoptions/) | Options for inserting operation. |

### insertRows(number, number) {#insertRows-number-number-}

Inserts multiple rows into the worksheet.

```javascript
insertRows(rowIndex: number, totalRows: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | number | Row index. |
| totalRows | number | Number of rows to be inserted. |

### insertRow(number) {#insertRow-number-}

Inserts a new row into the worksheet.

```javascript
insertRow(rowIndex: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | number | Row index. |

### clearRange(CellArea) {#clearRange-cellarea-}

Clears contents and formatting of a range.

```javascript
clearRange(range: CellArea) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| range | [CellArea](../cellarea/) | Range to be cleared. |

### clearRange(number, number, number, number) {#clearRange-number-number-number-number-}

Clears contents and formatting of a range.

```javascript
clearRange(startRow: number, startColumn: number, endRow: number, endColumn: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | number | Start row index. |
| startColumn | number | Start column index. |
| endRow | number | End row index. |
| endColumn | number | End column index. |

### clearContents(CellArea) {#clearContents-cellarea-}

Clears contents of a range.

```javascript
clearContents(range: CellArea) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| range | [CellArea](../cellarea/) | Range to be cleared. |

### clearContents(number, number, number, number) {#clearContents-number-number-number-number-}

Clears contents of a range.

```javascript
clearContents(startRow: number, startColumn: number, endRow: number, endColumn: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | number | Start row index. |
| startColumn | number | Start column index. |
| endRow | number | End row index. |
| endColumn | number | End column index. |

### clearFormats(CellArea) {#clearFormats-cellarea-}

Clears formatting of a range.

```javascript
clearFormats(range: CellArea) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| range | [CellArea](../cellarea/) | Range to be cleared. |

### clearFormats(number, number, number, number) {#clearFormats-number-number-number-number-}

Clears formatting of a range.

```javascript
clearFormats(startRow: number, startColumn: number, endRow: number, endColumn: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | number | Start row index. |
| startColumn | number | Start column index. |
| endRow | number | End row index. |
| endColumn | number | End column index. |

### linkToXmlMap(string, number, number, string) {#linkToXmlMap-string-number-number-string-}

Link to a xml map.

```javascript
linkToXmlMap(mapName: string, row: number, column: number, path: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| mapName | string | name of xml map |
| row | number | row of the destination cell |
| column | number | column of the destination cell |
| path | string | path of xml element in xml map |

### find(object, Cell) {#find-object-cell-}

Finds the cell containing with the input object.

```javascript
find(what: object, previousCell: Cell) : Cell;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| what | object | The object to search for.         /// The type should be int,double,DateTime,string,bool. |
| previousCell | [Cell](../cell/) | Previous cell with the same object.          /// This parameter can be set to null if searching from the start. |

**Returns**

Cell object.

**Remarks**

Returns null (Nothing) if no cell is found.

### find(object, Cell, FindOptions) {#find-object-cell-findoptions-}

Finds the cell containing with the input object.

```javascript
find(what: object, previousCell: Cell, findOptions: FindOptions) : Cell;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| what | object | The object to search for.         /// The type should be int,double,DateTime,string,bool. |
| previousCell | [Cell](../cell/) | Previous cell with the same object.          /// This parameter can be set to null if searching from the start. |
| findOptions | [FindOptions](../findoptions/) | Find options |

**Returns**

Cell object.

**Remarks**

Returns null (Nothing) if no cell is found.

### endCellInRow(number) {#endCellInRow-number-}

Gets the last cell in this row.

```javascript
endCellInRow(rowIndex: number) : Cell;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | number | Row index. |

**Returns**

Cell object.

### endCellInRow(number, number, number, number) {#endCellInRow-number-number-number-number-}

Gets the last cell with maximum row index in this range.

```javascript
endCellInRow(startRow: number, endRow: number, startColumn: number, endColumn: number) : Cell;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | number | Start row index. |
| endRow | number | End row index. |
| startColumn | number | Start column index. |
| endColumn | number | End column index. |

**Returns**

Cell object.

### endCellInColumn(number) {#endCellInColumn-number-}

Gets the last cell in this column.

```javascript
endCellInColumn(columnIndex: number) : Cell;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | number | Column index. |

**Returns**

Cell object.

### endCellInColumn(number, number, number, number) {#endCellInColumn-number-number-number-number-}

Gets the last cell with maximum column index in this range.

```javascript
endCellInColumn(startRow: number, endRow: number, startColumn: number, endColumn: number) : Cell;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | number | Start row index. |
| endRow | number | End row index. |
| startColumn | number | Start column index. |
| endColumn | number | End column index. |

**Returns**

Cell object.

### moveRange(CellArea, number, number) {#moveRange-cellarea-number-number-}

Moves the range.

```javascript
moveRange(sourceArea: CellArea, destRow: number, destColumn: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceArea | [CellArea](../cellarea/) | The range which should be moved. |
| destRow | number | The dest row. |
| destColumn | number | The dest column. |

### insertCutCells(Range, number, number, ShiftType) {#insertCutCells-range-number-number-shifttype-}

Insert cut range.

```javascript
insertCutCells(cutRange: Range, row: number, column: number, shiftType: ShiftType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cutRange | [Range](../range/) | The cut range. |
| row | number | The row. |
| column | number | The column. |
| shiftType | [ShiftType](../shifttype/) | The shift type . |

### insertRange(CellArea, number, ShiftType, boolean) {#insertRange-cellarea-number-shifttype-boolean-}

Inserts a range of cells and shift cells according to the shift option.

```javascript
insertRange(area: CellArea, shiftNumber: number, shiftType: ShiftType, updateReference: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| area | [CellArea](../cellarea/) | Shift area. |
| shiftNumber | number | Number of rows or columns to be inserted. |
| shiftType | [ShiftType](../shifttype/) | Shift cells option. |
| updateReference | boolean | Indicates whether update references in other worksheets. |

### insertRange(CellArea, ShiftType) {#insertRange-cellarea-shifttype-}

Inserts a range of cells and shift cells according to the shift option.

```javascript
insertRange(area: CellArea, shiftType: ShiftType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| area | [CellArea](../cellarea/) | Shift area. |
| shiftType | [ShiftType](../shifttype/) | Shift cells option. |

### insertRange(CellArea, number, ShiftType) {#insertRange-cellarea-number-shifttype-}

Inserts a range of cells and shift cells according to the shift option.

```javascript
insertRange(area: CellArea, shiftNumber: number, shiftType: ShiftType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| area | [CellArea](../cellarea/) | Shift area. |
| shiftNumber | number | Number of rows or columns to be inserted. |
| shiftType | [ShiftType](../shifttype/) | Shift cells option. |

### deleteRange(number, number, number, number, ShiftType) {#deleteRange-number-number-number-number-shifttype-}

Deletes a range of cells and shift cells according to the shift option.

```javascript
deleteRange(startRow: number, startColumn: number, endRow: number, endColumn: number, shiftType: ShiftType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | number | Start row index. |
| startColumn | number | Start column index. |
| endRow | number | End row index. |
| endColumn | number | End column index. |
| shiftType | [ShiftType](../shifttype/) | Shift cells option. |

### exportArray(number, number, number, number) {#exportArray-number-number-number-number-}

Exports data in the [Cells](../cells/) collection to a two-dimension array object.

```javascript
exportArray(firstRow: number, firstColumn: number, totalRows: number, totalColumns: number) : object[][];
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | number | The row number of the first cell to export out. |
| firstColumn | number | The column number of the first cell to export out. |
| totalRows | number | Number of rows to be exported |
| totalColumns | number | Number of columns to be exported |

**Returns**

Exported cell value array object.

### retrieveSubtotalSetting(CellArea) {#retrieveSubtotalSetting-cellarea-}

Retrieves subtotals setting of the range.

```javascript
retrieveSubtotalSetting(ca: CellArea) : SubtotalSetting;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| ca | [CellArea](../cellarea/) | The range |

**Returns**

[SubtotalSetting](../subtotalsetting/)

### subtotal(CellArea, number, ConsolidationFunction, number[]) {#subtotal-cellarea-number-consolidationfunction-numberarray-}

Creates subtotals for the range.

```javascript
subtotal(ca: CellArea, groupBy: number, consolidationFunction: ConsolidationFunction, totalList: number[]) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| ca | [CellArea](../cellarea/) | The range |
| groupBy | number | The field to group by, as a zero-based integer offset |
| consolidationFunction | [ConsolidationFunction](../consolidationfunction/) | The subtotal function. |
| totalList | number[] | An array of zero-based field offsets, indicating the fields to which the subtotals are added. |

### subtotal(CellArea, number, ConsolidationFunction, number[], boolean, boolean, boolean) {#subtotal-cellarea-number-consolidationfunction-numberarray-boolean-boolean-boolean-}

Creates subtotals for the range.

```javascript
subtotal(ca: CellArea, groupBy: number, consolidationFunction: ConsolidationFunction, totalList: number[], replace: boolean, pageBreaks: boolean, summaryBelowData: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| ca | [CellArea](../cellarea/) | The range |
| groupBy | number | The field to group by, as a zero-based integer offset |
| consolidationFunction | [ConsolidationFunction](../consolidationfunction/) | The subtotal function. |
| totalList | number[] | An array of zero-based field offsets, indicating the fields to which the subtotals are added. |
| replace | boolean | Indicates whether replace the current subtotals |
| pageBreaks | boolean | Indicates whether add page break between groups |
| summaryBelowData | boolean | Indicates whether add summary below data. |

### removeFormulas() {#removeFormulas--}

Removes all formula and replaces with the value of the formula.

```javascript
removeFormulas() : void;
```


### removeDuplicates() {#removeDuplicates--}

Removes duplicate rows in the sheet.

```javascript
removeDuplicates() : void;
```


### removeDuplicates(number, number, number, number) {#removeDuplicates-number-number-number-number-}

Removes duplicate values in the range.

```javascript
removeDuplicates(startRow: number, startColumn: number, endRow: number, endColumn: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | number | The start row. |
| startColumn | number | The start column |
| endRow | number | The end row index. |
| endColumn | number | The end column index. |

### removeDuplicates(number, number, number, number, boolean, number[]) {#removeDuplicates-number-number-number-number-boolean-numberarray-}

Removes duplicate data of the range.

```javascript
removeDuplicates(startRow: number, startColumn: number, endRow: number, endColumn: number, hasHeaders: boolean, columnOffsets: number[]) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | number | The start row. |
| startColumn | number | The start column |
| endRow | number | The end row index. |
| endColumn | number | The end column index. |
| hasHeaders | boolean | Indicates whether the range contains headers. |
| columnOffsets | number[] | The column offsets. |

### convertStringToNumericValue() {#convertStringToNumericValue--}

Converts all string data in the worksheet to numeric value if possible.

```javascript
convertStringToNumericValue() : void;
```


### getDependents(boolean, number, number) {#getDependents-boolean-number-number-}

Get all cells which refer to the specific cell.

```javascript
getDependents(isAll: boolean, row: number, column: number) : Cell[];
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isAll | boolean | Indicates whether check other worksheets |
| row | number | The row index. |
| column | number | The column index. |

**Returns**

[Cell](../cell/)[]

### getDependentsInCalculation(number, number, boolean) {#getDependentsInCalculation-number-number-boolean-}

Gets all cells whose calculated result depends on specific cell.

```javascript
getDependentsInCalculation(row: number, column: number, recursive: boolean) : CellEnumerator;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | Row index of the specific cell |
| column | number | Column index of the specific cell. |
| recursive | boolean | Whether returns those dependents which do not reference to the specific cell directly         /// but reference to other leafs of that cell. |

**Returns**

Enumerator to enumerate all dependents(Cell objects)

**Remarks**

To use this method, please make sure the workbook has been set with true value for [FormulaSettings.EnableCalculationChain](../formulasettings.enablecalculationchain/) and has been fully calculated with this setting. If there is no formula reference to this cell, null will be returned. For more details and example, please see [Cell.GetDependentsInCalculation(bool)](../cell.getdependentsincalculation(bool)/)

### getCellsWithPlaceInCellPicture() {#getCellsWithPlaceInCellPicture--}

Gets all cells that contain embedded picture.

```javascript
getCellsWithPlaceInCellPicture() : CellEnumerator;
```


**Returns**

Enumerator to enumerate all Cell objects that contain embedded picture

**Remarks**

If there is no picture which is set as "Place in Cell" in this worksheet, null will be returned.

### getCellStyle(number, number) {#getCellStyle-number-number-}

Get the style of given cell.

```javascript
getCellStyle(row: number, column: number) : Style;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | row index |
| column | number | column |

**Returns**

the style of given cell.

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



