---
title: "Cells Class"
linktitle: "Cells"
articleTitle: "Cells"
second_title: "Aspose.Cells for PHP via Java"
description: "Encapsulates a collection of cell relevant objects, such as Cell , Row , ...etc."
type: docs
weight: 620
url: /php/aspose.cells/cells/
---

## Cells class

Encapsulates a collection of cell relevant objects, such as Cell , Row , ...etc.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [OdsCellFields](#odscellfields) | OdsCellFieldCollection | Gets the list of fields of ods. |
| [Count](#count) | Number | Gets the total count of instantiated Cell objects. |
| [CountLarge](#countlarge) | long | Gets the total count of instantiated Cell objects. |
| [Rows](#rows) | RowCollection | Gets the collection of Row objects that represents the individual rows in this worksheet. |
| [MergedCells](#mergedcells) | ArrayList | Gets the collection of merged cells. In this collection, each item is a CellArea structure which represents an area of m |
| [MultiThreadReading](#multithreadreading) | boolean | Gets or sets whether the cells data model should support Multi-Thread reading. Default value of this property is false.  |
| [MemorySetting](#memorysetting) | Number | Gets or sets the memory usage option for this cells. The value of the property is MemorySetting integer constant. |
| [Style](#style) | Style | Gets and sets the default style of the worksheet. |
| [IsDefaultColumnHidden](#isdefaultcolumnhidden) | boolean |  |
| [StandardWidthInch](#standardwidthinch) | Number | Gets or sets the default column width in the worksheet, in unit of inches. |
| [StandardWidthPixels](#standardwidthpixels) | Number | Gets or sets the default column width in the worksheet, in unit of pixels. |
| [StandardWidth](#standardwidth) | Number | Gets or sets the default column width in the worksheet, in unit of characters. |
| [StandardHeight](#standardheight) | Number | Gets or sets the default row height in this worksheet, in unit of points. |
| [StandardHeightPixels](#standardheightpixels) | Number | Gets or sets the default row height in this worksheet, in unit of pixels. |
| [StandardHeightInch](#standardheightinch) | Number | Gets or sets the default row height in this worksheet, in unit of inches. |
| [PreserveString](#preservestring) | boolean | Gets or sets a value indicating whether all worksheet values are preserved as strings. Default is false. |
| [MinRow](#minrow) | Number | Minimum row index of cell which contains data or style. |
| [MaxRow](#maxrow) | Number | Maximum row index of cell which contains data or style. Return -1 if there is no cell which contains data or style in th |
| [MinColumn](#mincolumn) | Number | Minimum column index of those cells that have been instantiated in the collection(does not include the column where styl |
| [MaxColumn](#maxcolumn) | Number | Maximum column index of those cells that have been instantiated in the collection(does not include the column where styl |
| [MinDataRow](#mindatarow) | Number | Minimum row index of cell which contains data. |
| [MaxDataRow](#maxdatarow) | Number | Maximum row index of cell which contains data. Return -1 if there is no cell which contains data. |
| [MinDataColumn](#mindatacolumn) | Number | Minimum column index of cell which contains data. -1 will be returned if there is no cell which contains data. This prop |
| [MaxDataColumn](#maxdatacolumn) | Number | Maximum column index of cell which contains data. -1 will be returned if there is no cell which contains data. This prop |
| [IsDefaultRowHeightMatched](#isdefaultrowheightmatched) | boolean | Indicates that row height and default font height matches |
| [IsDefaultRowHidden](#isdefaultrowhidden) | boolean | Indicates whether the row is default hidden. |
| [Columns](#columns) | ColumnCollection | Gets the collection of Column objects that represents the individual columns in this worksheet. |
| [Ranges](#ranges) | RangeCollection | Gets the collection of Range objects created at run time. |
| [LastCell](#lastcell) | Cell | Gets the last cell in this worksheet. Returns null if there is no data in the worksheet. |
| [MaxDisplayRange](#maxdisplayrange) | Range | Gets the max range which includes data, merged cells and shapes. Reutrns null if the worksheet is empty since Aspose.Cel |
| [FirstCell](#firstcell) | Cell | Gets the first cell in this worksheet. Returns null if there is no data in the worksheet. |
| [Item (int, int)](#itemintint) | Cell | Gets the Cell element at the specified cell row index and column index. |
| [Item (java.lang.String)](#itemjavalangstring) | Cell | Gets the Cell element at the specified cell name. |

## Methods

| Name | Description |
| --- | --- |
| [insertRange](#insertrange) | Inserts a range of cells and shift cells according to the shift option. |
| [deleteRange](#deleterange) | Deletes a range of cells and shift cells according to the shift option. |
| [retrieveSubtotalSetting](#retrievesubtotalsetting) | Retrieves subtotals setting of the range. |
| [subtotal](#subtotal) | Creates subtotals for the range. |
| [removeFormulas](#removeformulas) | Removes all formula and replaces with the value of the formula. |
| [removeDuplicates](#removeduplicates) | Removes duplicate rows in the sheet. |
| [convertStringToNumericValue](#convertstringtonumericvalue) | Converts all string data in the worksheet to numeric value if possible. |
| [getDependents](#getdependents) | Get all cells which refer to the specific cell. |
| [getDependentsInCalculation](#getdependentsincalculation) | Gets all cells whose calculated result depends on specific cell.

To use this method, please make sure the workbook has  |
| [getCellsWithPlaceInCellPicture](#getcellswithplaceincellpicture) | Gets all cells that contain embedded picture.

If there is no picture which is set as "Place in Cell" in this worksheet, |
| [getCellStyle](#getcellstyle) | Get the style of given cell. |
| [getCellDisplayStyle](#getcelldisplaystyle) |  |
| [getColumnWidth](#getcolumnwidth) | Gets the width(in unit of characters) of the specified column in normal view |
| [getViewColumnWidthPixel](#getviewcolumnwidthpixel) | Get the width in different view type. |
| [setViewColumnWidthPixel](#setviewcolumnwidthpixel) | Sets the width of the column in different view.

If the current view type is ViewType.PAGE_LAYOUT_VIEW , the column's wi |
| [getLastDataRow](#getlastdatarow) | Gets the last row index of cell which contains data in the specified column. |
| [getFirstDataRow](#getfirstdatarow) |  |
| [applyColumnStyle](#applycolumnstyle) | Applies formats for a whole column. |
| [applyRowStyle](#applyrowstyle) | Applies formats for a whole row. |
| [applyStyle](#applystyle) | Applies formats for a whole worksheet. |
| [copyColumns](#copycolumns) | Copies data and formats of a whole column. |
| [copyColumn](#copycolumn) | Copies data and formats of a whole column. |
| [copyRow](#copyrow) | Copies data and formats of a whole row. |
| [copyRows](#copyrows) | Copies data and formats of some whole rows. |
| [getGroupedRowOutlineLevel](#getgroupedrowoutlinelevel) | Gets the outline level (zero-based) of the row.

If the row is not grouped, returns zero. |
| [getGroupedColumnOutlineLevel](#getgroupedcolumnoutlinelevel) | Gets the outline level (zero-based) of the column.

If the column is not grouped, returns zero. |
| [getMaxGroupedColumnOutlineLevel](#getmaxgroupedcolumnoutlinelevel) | Gets the max grouped column outline level (zero-based). |
| [getMaxGroupedRowOutlineLevel](#getmaxgroupedrowoutlinelevel) | Gets the max grouped row outline level (zero-based). |
| [showGroupDetail](#showgroupdetail) | Expands the grouped rows/columns. |
| [hideGroupDetail](#hidegroupdetail) | Collapses the grouped rows/columns. |
| [ungroupColumns](#ungroupcolumns) | Ungroups columns. |
| [groupColumns](#groupcolumns) | Groups columns. |
| [ungroupRows](#ungrouprows) | Ungroups rows. |
| [groupRows](#grouprows) | Groups rows. |
| [deleteColumn](#deletecolumn) | Deletes a column. |
| [deleteColumns](#deletecolumns) | Deletes several columns. |
| [isDeletingRangeEnabled](#isdeletingrangeenabled) | Check whether the range could be deleted. |
| [deleteRow](#deleterow) | Deletes a row. |
| [deleteRows](#deleterows) | Deletes several rows.

If the deleted range contains the top part(not whole) of the table(ListObject), the ranged could  |
| [deleteBlankColumns](#deleteblankcolumns) | Delete all blank columns which do not contain any data. |
| [isBlankColumn](#isblankcolumn) | Checks whether given column is blank(does not contain any data). |
| [deleteBlankRows](#deleteblankrows) | Delete all blank rows which do not contain any data or other object. |
| [insertColumns](#insertcolumns) | Inserts some columns into the worksheet. |
| [insertColumn](#insertcolumn) | Inserts a new column into the worksheet. |
| [insertRows](#insertrows) | Inserts multiple rows into the worksheet. |
| [insertRow](#insertrow) | Inserts a new row into the worksheet. |
| [clearRange](#clearrange) | Clears contents and formatting of a range. |
| [clearContents](#clearcontents) | Clears contents of a range. |
| [clearFormats](#clearformats) | Clears formatting of a range. |
| [linkToXmlMap](#linktoxmlmap) | Link to a xml map. |
| [find](#find) | Finds the cell containing with the input object.

Returns null (Nothing) if no cell is found. |
| [endCellInRow](#endcellinrow) | Gets the last cell in this row. |
| [endCellInColumn](#endcellincolumn) |  |
| [moveRange](#moverange) | Moves the range. |
| [insertCutCells](#insertcutcells) | Insert cut range. |
| [dispose](#dispose) | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [iterator](#iterator) | Gets the cells enumerator.

When traversing elements by the returned Enumerator, the cells collection should not be modi |
| [getRowEnumerator](#getrowenumerator) | Gets the rows enumerator.

NOTE: This member is now obsolete. Instead, please use RowCollection.GetEnumerator() method.  |
| [getMergedAreas](#getmergedareas) | Gets all merged cells. |
| [checkCell](#checkcell) | Gets the Cell element or null at the specified cell row index and column index. |
| [checkRow](#checkrow) | Gets the Row element or null at the specified cell row index. |
| [checkColumn](#checkcolumn) | Gets the Column element or null at the specified column index. |
| [isRowHidden](#isrowhidden) | Checks whether a row at given index is hidden. |
| [isColumnHidden](#iscolumnhidden) | Checks whether a column at given index is hidden. |
| [addRange](#addrange) | Adds a range object reference to cells |
| [createRange](#createrange) | Creates a Range object from a range of cells. |
| [clear](#clear) | Clears all data of the worksheet. |
| [importFormulaArray](#importformulaarray) | Imports an array of formula into a worksheet. |
| [textToColumns](#texttocolumns) | Splits the text in the column to columns. |
| [importCSV](#importcsv) | Import a CSV file to the cells. |
| [merge](#merge) | Merges a specified range of cells into a single cell.

Reference the merged cell via the address of the upper-left cell  |
| [unMerge](#unmerge) | Unmerges a specified range of merged cells. |
| [clearMergedCells](#clearmergedcells) | Clears all merged ranges. |
| [hideRow](#hiderow) | Hides a row. |
| [unhideRow](#unhiderow) | Unhides a row. |
| [hideRows](#hiderows) | Hides multiple rows. |
| [unhideRows](#unhiderows) | Unhides the hidden rows. |
| [setRowHeightPixel](#setrowheightpixel) | Sets row height in unit of pixels. |
| [setRowHeightInch](#setrowheightinch) | Sets row height in unit of inches. |
| [setRowHeight](#setrowheight) | Sets the height of the specified row. |
| [getRowHeight](#getrowheight) | Gets row's height. |
| [getRowOriginalHeightPoint](#getroworiginalheightpoint) | Gets original row's height in unit of point if the row is hidden

NOTE: This member is now obsolete. Instead, please use |
| [getColumnOriginalWidthPoint](#getcolumnoriginalwidthpoint) | Gets original column's height in unit of point if the column is hidden

NOTE: This method is now obsolete. Instead, plea |
| [hideColumn](#hidecolumn) | Hides a column. |
| [unhideColumn](#unhidecolumn) | Unhides a column |
| [hideColumns](#hidecolumns) | Hide multiple columns. |
| [unhideColumns](#unhidecolumns) | Unhide multiple columns.

Only applies the column width to the hidden columns. |
| [getViewRowHeight](#getviewrowheight) | Gets the height of a specified row. |
| [getRowHeightInch](#getrowheightinch) | Gets the height of a specified row in unit of inches. |
| [getViewRowHeightInch](#getviewrowheightinch) | Gets the height of a specified row in unit of inches. |
| [getRowHeightPixel](#getrowheightpixel) | Gets the height of a specified row in unit of pixel. |
| [setColumnWidthPixel](#setcolumnwidthpixel) | Sets column width in unit of pixels in normal view. |
| [setColumnWidthInch](#setcolumnwidthinch) | Sets column width in unit of inches in normal view. |
| [setColumnWidth](#setcolumnwidth) | Sets the width of the specified column in normal view.

To hide a column, sets column width to zero. |
| [getColumnWidthPixel](#getcolumnwidthpixel) | Gets the width of the specified column in normal view, in units of pixel. |
| [getColumnWidthInch](#getcolumnwidthinch) | Gets the width of the specified column in normal view, in units of inches.

NOTE: This method is now obsolete. Instead,  |

### Cells.OdsCellFields property {#odscellfields}

Gets the list of fields of ods.

**Type:** OdsCellFieldCollection

### Cells.Count property {#count}

Gets the total count of instantiated Cell objects.

**Type:** Number

### Cells.CountLarge property {#countlarge}

Gets the total count of instantiated Cell objects.

**Type:** long

### Cells.Rows property {#rows}

Gets the collection of Row objects that represents the individual rows in this worksheet.

**Type:** RowCollection

### Cells.MergedCells property {#mergedcells}

Gets the collection of merged cells. In this collection, each item is a CellArea structure which represents an area of merged cells.

**Type:** ArrayList

### Cells.MultiThreadReading property {#multithreadreading}

Gets or sets whether the cells data model should support Multi-Thread reading. Default value of this property is false. If there are multiple threads to read Row/Cell objects in this collection concurrently, this property should be set as true, otherwise unexpected result may be produced. Supporting Multi-Thread reading may degrade the performance for accessing Row/Cell objects from this collection. Please note, some features cannot support Multi-Thread reading, such as formatting values(by Cell.StringValue , Cell.DisplayStringValue , .etc.). So, even with this property being set as true, those APIs still may give unexpected result for Multi-Thread reading.

**Type:** boolean

### Cells.MemorySetting property {#memorysetting}

Gets or sets the memory usage option for this cells. The value of the property is MemorySetting integer constant.

**Type:** Number

### Cells.Style property {#style}

Gets and sets the default style of the worksheet.

**Type:** Style

### Cells.IsDefaultColumnHidden property {#isdefaultcolumnhidden}

**Type:** boolean

### Cells.StandardWidthInch property {#standardwidthinch}

Gets or sets the default column width in the worksheet, in unit of inches.

**Type:** Number

### Cells.StandardWidthPixels property {#standardwidthpixels}

Gets or sets the default column width in the worksheet, in unit of pixels.

**Type:** Number

### Cells.StandardWidth property {#standardwidth}

Gets or sets the default column width in the worksheet, in unit of characters.

**Type:** Number

### Cells.StandardHeight property {#standardheight}

Gets or sets the default row height in this worksheet, in unit of points.

**Type:** Number

### Cells.StandardHeightPixels property {#standardheightpixels}

Gets or sets the default row height in this worksheet, in unit of pixels.

**Type:** Number

### Cells.StandardHeightInch property {#standardheightinch}

Gets or sets the default row height in this worksheet, in unit of inches.

**Type:** Number

### Cells.PreserveString property {#preservestring}

Gets or sets a value indicating whether all worksheet values are preserved as strings. Default is false.

**Type:** boolean

### Cells.MinRow property {#minrow}

Minimum row index of cell which contains data or style.

**Type:** Number

### Cells.MaxRow property {#maxrow}

Maximum row index of cell which contains data or style. Return -1 if there is no cell which contains data or style in the worksheet.

**Type:** Number

### Cells.MinColumn property {#mincolumn}

Minimum column index of those cells that have been instantiated in the collection(does not include the column where style is defined for the whole column but no cell has been instantiated in it).

**Type:** Number

### Cells.MaxColumn property {#maxcolumn}

Maximum column index of those cells that have been instantiated in the collection(does not include the column where style is defined for the whole column but no cell has been instantiated in it). Return -1 if there is no cell.

**Type:** Number

### Cells.MinDataRow property {#mindatarow}

Minimum row index of cell which contains data.

**Type:** Number

### Cells.MaxDataRow property {#maxdatarow}

Maximum row index of cell which contains data. Return -1 if there is no cell which contains data.

**Type:** Number

### Cells.MinDataColumn property {#mindatacolumn}

Minimum column index of cell which contains data. -1 will be returned if there is no cell which contains data. This property needs to iterate and check all cells in a worksheet, so it is a time-consumed progress and should not be invoked repeatedly.

**Type:** Number

### Cells.MaxDataColumn property {#maxdatacolumn}

Maximum column index of cell which contains data. -1 will be returned if there is no cell which contains data. This property needs to iterate and check all cells in a worksheet, so it is a time-consumed progress and should not be invoked repeatedly.

**Type:** Number

### Cells.IsDefaultRowHeightMatched property {#isdefaultrowheightmatched}

Indicates that row height and default font height matches

**Type:** boolean

### Cells.IsDefaultRowHidden property {#isdefaultrowhidden}

Indicates whether the row is default hidden.

**Type:** boolean

### Cells.Columns property {#columns}

Gets the collection of Column objects that represents the individual columns in this worksheet.

**Type:** ColumnCollection

### Cells.Ranges property {#ranges}

Gets the collection of Range objects created at run time.

**Type:** RangeCollection

### Cells.LastCell property {#lastcell}

Gets the last cell in this worksheet. Returns null if there is no data in the worksheet.

**Type:** Cell

### Cells.MaxDisplayRange property {#maxdisplayrange}

Gets the max range which includes data, merged cells and shapes. Reutrns null if the worksheet is empty since Aspose.Cells 21.5.2.

**Type:** Range

### Cells.FirstCell property {#firstcell}

Gets the first cell in this worksheet. Returns null if there is no data in the worksheet.

**Type:** Cell

### Cells.Item (int, int) property {#itemintint}

Gets the Cell element at the specified cell row index and column index.

**Type:** Cell

### Cells.Item (java.lang.String) property {#itemjavalangstring}

Gets the Cell element at the specified cell name.

**Type:** Cell

### insertRange(area, shiftNumber, shiftType, updateReference) (1 of 3) {#insertrange}

Inserts a range of cells and shift cells according to the shift option.

| Parameter | Type | Description |
| --- | --- | --- |
| area | CellArea | Shift area. |
| shiftNumber | Number | Number of rows or columns to be inserted. |
| shiftType | Number | A ShiftType value. Shift cells option. |
| updateReference | boolean | Indicates whether update references in other worksheets. |

---

### insertRange(area, shiftType) (2 of 3) {#insertrange-1}

Inserts a range of cells and shift cells according to the shift option.

| Parameter | Type | Description |
| --- | --- | --- |
| area | CellArea | Shift area. |
| shiftType | Number | A ShiftType value. Shift cells option. |

---

### insertRange(area, shiftNumber, shiftType) (3 of 3) {#insertrange-2}

Inserts a range of cells and shift cells according to the shift option.

| Parameter | Type | Description |
| --- | --- | --- |
| area | CellArea | Shift area. |
| shiftNumber | Number | Number of rows or columns to be inserted. |
| shiftType | Number | A ShiftType value. Shift cells option. |

### deleteRange(startRow, startColumn, endRow, endColumn, shiftType) {#deleterange}

Deletes a range of cells and shift cells according to the shift option.

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Number | Start row index. |
| startColumn | Number | Start column index. |
| endRow | Number | End row index. |
| endColumn | Number | End column index. |
| shiftType | Number | A ShiftType value. Shift cells option. |

### retrieveSubtotalSetting(ca) {#retrievesubtotalsetting}

Retrieves subtotals setting of the range.

| Parameter | Type | Description |
| --- | --- | --- |
| ca | CellArea | The range |

### subtotal(ca, groupBy, function, totalList) (1 of 2) {#subtotal}

Creates subtotals for the range.

| Parameter | Type | Description |
| --- | --- | --- |
| ca | CellArea | The range |
| groupBy | Number | The field to group by, as a zero-based integer offset |
| function | Number | A ConsolidationFunction value. The subtotal function. |
| totalList | Number Array | An array of zero-based field offsets, indicating the fields to which the subtotals are added. |

---

### subtotal(ca, groupBy, function, totalList, replace, pageBreaks, summaryBelowData) (2 of 2) {#subtotal-1}

Creates subtotals for the range.

| Parameter | Type | Description |
| --- | --- | --- |
| ca | CellArea | The range |
| groupBy | Number | The field to group by, as a zero-based integer offset |
| function | Number | A ConsolidationFunction value. The subtotal function. |
| totalList | Number Array | An array of zero-based field offsets, indicating the fields to which the subtotals are added. |
| replace | boolean | Indicates whether replace the current subtotals |
| pageBreaks | boolean | Indicates whether add page break between groups |
| summaryBelowData | boolean | Indicates whether add summary below data. |

### removeFormulas() {#removeformulas}

Removes all formula and replaces with the value of the formula.

### removeDuplicates() (1 of 3) {#removeduplicates}

Removes duplicate rows in the sheet.

---

### removeDuplicates(startRow, startColumn, endRow, endColumn) (2 of 3) {#removeduplicates-1}

Removes duplicate values in the range.

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Number | The start row. |
| startColumn | Number | The start column |
| endRow | Number | The end row index. |
| endColumn | Number | The end column index. |

---

### removeDuplicates(startRow, startColumn, endRow, endColumn, hasHeaders, columnOffsets) (3 of 3) {#removeduplicates-2}

Removes duplicate data of the range.

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Number | The start row. |
| startColumn | Number | The start column |
| endRow | Number | The end row index. |
| endColumn | Number | The end column index. |
| hasHeaders | boolean | Indicates whether the range contains headers. |
| columnOffsets | Number Array | The column offsets. |

### convertStringToNumericValue() {#convertstringtonumericvalue}

Converts all string data in the worksheet to numeric value if possible.

### getDependents(isAll, row, column) {#getdependents}

Get all cells which refer to the specific cell.

| Parameter | Type | Description |
| --- | --- | --- |
| isAll | boolean | Indicates whether check other worksheets |
| row | Number | The row index. |
| column | Number | The column index. |

### getDependentsInCalculation(row, column, recursive) {#getdependentsincalculation}

Gets all cells whose calculated result depends on specific cell.

To use this method, please make sure the workbook has been set with true value for FormulaSettings.EnableCalculationChain and has been fully calculated with this setting. If there is no formula reference to this cell, null will be returned. For more details and example, please see Cell.getDependentsInCalculation(boolean)

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Row index of the specific cell |
| column | Number | Column index of the specific cell. |
| recursive | boolean | Whether returns those dependents which do not reference to the specific cell directly but reference to other leafs of that cell. |

**Returns:** Enumerator to enumerate all dependents(Cell objects)

### getCellsWithPlaceInCellPicture() {#getcellswithplaceincellpicture}

Gets all cells that contain embedded picture.

If there is no picture which is set as "Place in Cell" in this worksheet, null will be returned. />

**Returns:** Enumerator to enumerate all Cell objects that contain embedded picture

### getCellStyle(row, column) {#getcellstyle}

Get the style of given cell.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | row index |
| column | Number | column |

**Returns:** the style of given cell.

### getCellDisplayStyle(row, column) (1 of 2) {#getcelldisplaystyle}

---

### getCellDisplayStyle(row, column, adjacentBorders) (2 of 2) {#getcelldisplaystyle-1}

### getColumnWidth(column) (1 of 2) {#getcolumnwidth}

Gets the width(in unit of characters) of the specified column in normal view

| Parameter | Type | Description |
| --- | --- | --- |
| column | Number | Column index |

**Returns:** Width of column. For spreadsheet, column width is measured as the number of characters of the maximum digit width of the numbers 0~9 as rendered in the normal style's font.

---

### getColumnWidth(column, isOriginal, unitType) (2 of 2) {#getcolumnwidth-1}

Gets the column width.

| Parameter | Type | Description |
| --- | --- | --- |
| column | Number | The column index. |
| isOriginal | boolean | Indicates whether getting original width. |
| unitType | Number | A CellsUnitType value. |

### getViewColumnWidthPixel(column) {#getviewcolumnwidthpixel}

Get the width in different view type.

| Parameter | Type | Description |
| --- | --- | --- |
| column | Number | The column index. |

**Returns:** the column width in unit of pixels

### setViewColumnWidthPixel(column, pixels) {#setviewcolumnwidthpixel}

Sets the width of the column in different view.

If the current view type is ViewType.PAGE_LAYOUT_VIEW , the column's width is same as printed width.

| Parameter | Type | Description |
| --- | --- | --- |
| column | Number | The column index. |
| pixels | Number | The width in unit of pixels. |

### getLastDataRow(column) {#getlastdatarow}

Gets the last row index of cell which contains data in the specified column.

| Parameter | Type | Description |
| --- | --- | --- |
| column | Number | Column index. |

**Returns:** last row index.

### getFirstDataRow(column) {#getfirstdatarow}

### applyColumnStyle(column, style, flag) {#applycolumnstyle}

Applies formats for a whole column.

| Parameter | Type | Description |
| --- | --- | --- |
| column | Number | The column index. |
| style | Style | The style object which will be applied. |
| flag | StyleFlag | Flags which indicates applied formatting properties. |

### applyRowStyle(row, style, flag) {#applyrowstyle}

Applies formats for a whole row.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | The row index. |
| style | Style | The style object which will be applied. |
| flag | StyleFlag | Flags which indicates applied formatting properties. |

### applyStyle(style, flag) {#applystyle}

Applies formats for a whole worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The style object which will be applied. |
| flag | StyleFlag | Flags which indicates applied formatting properties. |

### copyColumns(sourceCells, sourceColumnIndex, destinationColumnIndex, columnNumber, pasteOptions) (1 of 3) {#copycolumns}

Copies data and formats of a whole column.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells0 |  | Source Cells object contains data and formats to copy. |
| sourceColumnIndex | Number | Source column index. |
| destinationColumnIndex | Number | Destination column index. |
| columnNumber | Number | The copied column number. |
| pasteOptions | PasteOptions | the options of pasting. |

---

### copyColumns(sourceCells, sourceColumnIndex, destinationColumnIndex, columnNumber) (2 of 3) {#copycolumns-1}

Copies data and formats of a whole column.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells0 |  | Source Cells object contains data and formats to copy. |
| sourceColumnIndex | Number | Source column index. |
| destinationColumnIndex | Number | Destination column index. |
| columnNumber | Number | The copied column number. |

---

### copyColumns(sourceCells, sourceColumnIndex, sourceTotalColumns, destinationColumnIndex, destinationTotalColumns) (3 of 3) {#copycolumns-2}

Copies data and formats of the whole columns.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells | Cells | Source Cells object contains data and formats to copy. |
| sourceColumnIndex | Number | Source column index. |
| sourceTotalColumns | Number | The number of the source columns. |
| destinationColumnIndex | Number | Destination column index. |
| destinationTotalColumns | Number | The number of the destination columns. |

### copyColumn(sourceCells, sourceColumnIndex, destinationColumnIndex) {#copycolumn}

Copies data and formats of a whole column.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells | Cells | Source Cells object contains data and formats to copy. |
| sourceColumnIndex | Number | Source column index. |
| destinationColumnIndex | Number | Destination column index. |

### copyRow(sourceCells, sourceRowIndex, destinationRowIndex) {#copyrow}

Copies data and formats of a whole row.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells | Cells | Source Cells object contains data and formats to copy. |
| sourceRowIndex | Number | Source row index. |
| destinationRowIndex | Number | Destination row index. |

### copyRows(sourceCells, sourceRowIndex, destinationRowIndex, rowNumber) (1 of 3) {#copyrows}

Copies data and formats of some whole rows.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells | Cells | Source Cells object contains data and formats to copy. |
| sourceRowIndex | Number | Source row index. |
| destinationRowIndex | Number | Destination row index. |
| rowNumber | Number | The copied row number. |

---

### copyRows(sourceCells, sourceRowIndex, destinationRowIndex, rowNumber, copyOptions) (2 of 3) {#copyrows-1}

Copies data and formats of some whole rows.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells0 |  | Source Cells object contains data and formats to copy. |
| sourceRowIndex | Number | Source row index. |
| destinationRowIndex | Number | Destination row index. |
| rowNumber | Number | The copied row number. |
| copyOptions | CopyOptions | The copy options. |

---

### copyRows(sourceCells0, sourceRowIndex, destinationRowIndex, rowNumber, copyOptions, pasteOptions) (3 of 3) {#copyrows-2}

Copies data and formats of some whole rows.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells0 | Cells | Source Cells object contains data and formats to copy. |
| sourceRowIndex | Number | Source row index. |
| destinationRowIndex | Number | Destination row index. |
| rowNumber | Number | The copied row number. |
| copyOptions | CopyOptions | The copy options. |
| pasteOptions | PasteOptions | the options of pasting. |

### getGroupedRowOutlineLevel(rowIndex) {#getgroupedrowoutlinelevel}

Gets the outline level (zero-based) of the row.

If the row is not grouped, returns zero.

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Number | The row index. |

**Returns:** The outline level (zero-based) of the row.

### getGroupedColumnOutlineLevel(columnIndex) {#getgroupedcolumnoutlinelevel}

Gets the outline level (zero-based) of the column.

If the column is not grouped, returns zero.

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Number | The column index |

**Returns:** The outline level of the column

### getMaxGroupedColumnOutlineLevel() {#getmaxgroupedcolumnoutlinelevel}

Gets the max grouped column outline level (zero-based).

**Returns:** The max grouped column outline level (zero-based)

### getMaxGroupedRowOutlineLevel() {#getmaxgroupedrowoutlinelevel}

Gets the max grouped row outline level (zero-based).

**Returns:** The max grouped row outline level (zero-based)

### showGroupDetail(isVertical, index) {#showgroupdetail}

Expands the grouped rows/columns.

| Parameter | Type | Description |
| --- | --- | --- |
| isVertical | boolean | True, expands the grouped rows. |
| index | Number | The row/column index |

### hideGroupDetail(isVertical, index) {#hidegroupdetail}

Collapses the grouped rows/columns.

| Parameter | Type | Description |
| --- | --- | --- |
| isVertical | boolean | True, collapse the grouped rows. |
| index | Number | The row/column index |

### ungroupColumns(firstIndex, lastIndex) {#ungroupcolumns}

Ungroups columns.

| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | Number | The first column index to be ungrouped. |
| lastIndex | Number | The last column index to be ungrouped. |

### groupColumns(firstIndex, lastIndex) (1 of 2) {#groupcolumns}

Groups columns.

| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | Number | The first column index to be grouped. |
| lastIndex | Number | The last column index to be grouped. |

---

### groupColumns(firstIndex, lastIndex, isHidden) (2 of 2) {#groupcolumns-1}

Groups columns.

| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | Number | The first column index to be grouped. |
| lastIndex | Number | The last column index to be grouped. |
| isHidden | boolean | Specifies if the grouped columns are hidden. |

### ungroupRows(firstIndex, lastIndex, isAll) (1 of 2) {#ungrouprows}

Ungroups rows.

| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | Number | The first row index to be ungrouped. |
| lastIndex | Number | The last row index to be ungrouped. |
| isAll | boolean | True, removes all grouped info.Otherwise, remove the outer group info. |

---

### ungroupRows(firstIndex, lastIndex) (2 of 2) {#ungrouprows-1}

Ungroups rows.

Only removes outer group info.

| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | Number | The first row index to be ungrouped. |
| lastIndex | Number | The last row index to be ungrouped. |

### groupRows(firstIndex, lastIndex, isHidden) (1 of 2) {#grouprows}

Groups rows.

| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | Number | The first row index to be grouped. |
| lastIndex | Number | The last row index to be grouped. |
| isHidden | boolean | Specifies if the grouped rows are hidden. |

---

### groupRows(firstIndex, lastIndex) (2 of 2) {#grouprows-1}

Groups rows.

| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | Number | The first row index to be grouped. |
| lastIndex | Number | The last row index to be grouped. |

### deleteColumn(columnIndex, updateReference) (1 of 2) {#deletecolumn}

Deletes a column.

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Number | Index of the column to be deleted. |
| updateReference | boolean | Indicates whether update references in other worksheets. |

---

### deleteColumn(columnIndex) (2 of 2) {#deletecolumn-1}

Deletes a column.

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Number | Index of the column to be deleted. |

### deleteColumns(columnIndex, totalColumns, updateReference) (1 of 2) {#deletecolumns}

Deletes several columns.

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Number | Index of the first column to be deleted. |
| totalColumns | Number | Count of columns to be deleted. |
| updateReference | boolean | Indicates whether update references in other worksheets. |

---

### deleteColumns(columnIndex, totalColumns, options) (2 of 2) {#deletecolumns-1}

### isDeletingRangeEnabled(startRow, startColumn, totalRows, totalColumns) {#isdeletingrangeenabled}

Check whether the range could be deleted.

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Number | The start row index of the range. |
| startColumn | Number | The start column index of the range. |
| totalRows | Number | The number of the rows in the range. |
| totalColumns | Number | The number of the columns in the range. |

### deleteRow(rowIndex) (1 of 2) {#deleterow}

Deletes a row.

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Number | Index of the row to be deleted. |

---

### deleteRow(rowIndex, updateReference) (2 of 2) {#deleterow-1}

Deletes a row.

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Number | Index of the row to be deleted. |
| updateReference | boolean | Indicates whether update references in other worksheets. |

### deleteRows(rowIndex, totalRows) (1 of 3) {#deleterows}

Deletes several rows.

If the deleted range contains the top part(not whole) of the table(ListObject), the ranged could not be deleted and nothing will be done. It works in the same way with MS Excel.

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Number | The first row index to be deleted. |
| totalRows | Number | Count of rows to be deleted. |

---

### deleteRows(rowIndex, totalRows, updateReference) (2 of 3) {#deleterows-1}

Deletes multiple rows in the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Number | Index of the first row to be deleted. |
| totalRows | Number | Count of rows to be deleted. |
| updateReference | boolean | Indicates whether update references in other worksheets. |

---

### deleteRows(rowIndex, totalRows, options) (3 of 3) {#deleterows-2}

### deleteBlankColumns() (1 of 2) {#deleteblankcolumns}

Delete all blank columns which do not contain any data.

---

### deleteBlankColumns(options) (2 of 2) {#deleteblankcolumns-1}

Delete all blank columns which do not contain any data.

| Parameter | Type | Description |
| --- | --- | --- |
| options | DeleteOptions | The options of deleting range. |

### isBlankColumn(columnIndex) {#isblankcolumn}

Checks whether given column is blank(does not contain any data).

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Number | the column index |

**Returns:** true if given column does not contain any data

### deleteBlankRows() (1 of 2) {#deleteblankrows}

Delete all blank rows which do not contain any data or other object.

---

### deleteBlankRows(options) (2 of 2) {#deleteblankrows-1}

Delete all blank rows which do not contain any data or other object.

For blank rows that will be deleted, it is not only required that Row.IsBlank should be true, but also there should be no visible comment defined for any cell in those rows, and no pivot table whose range intersects with them.

| Parameter | Type | Description |
| --- | --- | --- |
| options | DeleteOptions | The options of deleting range. |

### insertColumns(columnIndex, totalColumns) (1 of 3) {#insertcolumns}

Inserts some columns into the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Number | Column index. |
| totalColumns | Number | The number of columns. |

---

### insertColumns(columnIndex, totalColumns, updateReference) (2 of 3) {#insertcolumns-1}

Inserts some columns into the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Number | Column index. |
| totalColumns | Number | The number of columns. |
| updateReference | boolean | Indicates if references in other worksheets will be updated. |

---

### insertColumns(columnIndex, totalColumns, options) (3 of 3) {#insertcolumns-2}

### insertColumn(columnIndex, updateReference) (1 of 2) {#insertcolumn}

Inserts a new column into the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Number | Column index. |
| updateReference | boolean | Indicates if references in other worksheets will be updated. |

---

### insertColumn(columnIndex) (2 of 2) {#insertcolumn-1}

Inserts a new column into the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Number | Column index. |

### insertRows(rowIndex, totalRows, updateReference) (1 of 3) {#insertrows}

Inserts multiple rows into the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Number | Row index. |
| totalRows | Number | Number of rows to be inserted. |
| updateReference | boolean | Indicates if references in other worksheets will be updated. |

---

### insertRows(rowIndex, totalRows, options) (2 of 3) {#insertrows-1}

Inserts multiple rows into the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Number | Row index. |
| totalRows | Number | Number of rows to be inserted. |
| options | InsertOptions | Indicates if references in other worksheets will be updated. |

---

### insertRows(rowIndex, totalRows) (3 of 3) {#insertrows-2}

Inserts multiple rows into the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Number | Row index. |
| totalRows | Number | Number of rows to be inserted. |

### insertRow(rowIndex) {#insertrow}

Inserts a new row into the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Number | Row index. |

### clearRange(range) (1 of 2) {#clearrange}

Clears contents and formatting of a range.

| Parameter | Type | Description |
| --- | --- | --- |
| range | CellArea | Range to be cleared. |

---

### clearRange(startRow, startColumn, endRow, endColumn) (2 of 2) {#clearrange-1}

Clears contents and formatting of a range.

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Number | Start row index. |
| startColumn | Number | Start column index. |
| endRow | Number | End row index. |
| endColumn | Number | End column index. |

### clearContents(range) (1 of 2) {#clearcontents}

Clears contents of a range.

| Parameter | Type | Description |
| --- | --- | --- |
| range | CellArea | Range to be cleared. |

---

### clearContents(startRow, startColumn, endRow, endColumn) (2 of 2) {#clearcontents-1}

Clears contents of a range.

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Number | Start row index. |
| startColumn | Number | Start column index. |
| endRow | Number | End row index. |
| endColumn | Number | End column index. |

### clearFormats(range) (1 of 2) {#clearformats}

Clears formatting of a range.

| Parameter | Type | Description |
| --- | --- | --- |
| range | CellArea | Range to be cleared. |

---

### clearFormats(startRow, startColumn, endRow, endColumn) (2 of 2) {#clearformats-1}

Clears formatting of a range.

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Number | Start row index. |
| startColumn | Number | Start column index. |
| endRow | Number | End row index. |
| endColumn | Number | End column index. |

### linkToXmlMap(mapName, row, column, path) {#linktoxmlmap}

Link to a xml map.

| Parameter | Type | Description |
| --- | --- | --- |
| mapName | String | name of xml map |
| row | Number | row of the destination cell |
| column | Number | column of the destination cell |
| path | String | path of xml element in xml map |

### find(what, previousCell) (1 of 2) {#find}

Finds the cell containing with the input object.

Returns null (Nothing) if no cell is found.

| Parameter | Type | Description |
| --- | --- | --- |
| what | Object | The object to search for. The type should be int,double,DateTime,string,bool. |
| previousCell | Cell | Previous cell with the same object. This parameter can be set to null if searching from the start. |

**Returns:** Cell object.

---

### find(what, previousCell, findOptions) (2 of 2) {#find-1}

Finds the cell containing with the input object.

Returns null (Nothing) if no cell is found.

| Parameter | Type | Description |
| --- | --- | --- |
| what | Object | The object to search for. The type should be int,double,DateTime,string,bool. |
| previousCell | Cell | Previous cell with the same object. This parameter can be set to null if searching from the start. |
| findOptions | FindOptions | Find options |

**Returns:** Cell object.

### endCellInRow(rowIndex) (1 of 2) {#endcellinrow}

Gets the last cell in this row.

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Number | Row index. |

**Returns:** Cell object.

---

### endCellInRow(startRow, endRow, startColumn, endColumn) (2 of 2) {#endcellinrow-1}

Gets the last cell with maximum row index in this range.

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Number | Start row index. |
| endRow | Number | End row index. |
| startColumn | Number | Start column index. |
| endColumn | Number | End column index. |

**Returns:** Cell object.

### endCellInColumn(columnIndex) (1 of 2) {#endcellincolumn}

---

### endCellInColumn(startRow, endRow, startColumn, endColumn) (2 of 2) {#endcellincolumn-1}

### moveRange(sourceArea, destRow, destColumn) {#moverange}

Moves the range.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceArea | CellArea | The range which should be moved. |
| destRow | Number | The dest row. |
| destColumn | Number | The dest column. |

### insertCutCells(cutRange, row, column, shiftType) {#insertcutcells}

Insert cut range.

| Parameter | Type | Description |
| --- | --- | --- |
| cutRange | Range | The cut range. |
| row | Number | The row. |
| column | Number | The column. |
| shiftType | Number | A ShiftType value. The shift type . |

### dispose() {#dispose}

Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources.

### iterator() {#iterator}

Gets the cells enumerator.

When traversing elements by the returned Enumerator, the cells collection should not be modified(such as operations that will cause new Cell/Row be instantiated or existing Cell/Row be deleted). Otherwise the enumerator may not be able to traverse all cells correctly(some elements may be traversed repeatedly or skipped).

**Returns:** The cells enumerator

### getRowEnumerator() {#getrowenumerator}

Gets the rows enumerator.

NOTE: This member is now obsolete. Instead, please use RowCollection.GetEnumerator() method. This method will be removed 12 months later since May 2023. Aspose apologizes for any inconvenience you may have experienced.

**Returns:** The rows enumerator.


**See Also:**

- RowCollection.iterator()

### getMergedAreas() {#getmergedareas}

Gets all merged cells.

### checkCell(row, column) {#checkcell}

Gets the Cell element or null at the specified cell row index and column index.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Row index |
| column | Number | Column index |

**Returns:** Return Cell object if a Cell object exists. Return null if the cell does not exist.

### checkRow(row) {#checkrow}

Gets the Row element or null at the specified cell row index.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Row index |

**Returns:** Returns Row object If the row object does exist, otherwise returns null.

### checkColumn(columnIndex) {#checkcolumn}

Gets the Column element or null at the specified column index.

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Number | The column index. |

**Returns:** The Column object.

### isRowHidden(rowIndex) {#isrowhidden}

Checks whether a row at given index is hidden.

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Number | row index |

**Returns:** true if the row is hidden

### isColumnHidden(columnIndex) {#iscolumnhidden}

Checks whether a column at given index is hidden.

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Number | column index |

**Returns:** true if the column is hidden.

### addRange(rangeObject) {#addrange}

Adds a range object reference to cells

| Parameter | Type | Description |
| --- | --- | --- |
| rangeObject | Range | The range object will be contained in the cells |

### createRange(upperLeftCell, lowerRightCell) (1 of 4) {#createrange}

Creates a Range object from a range of cells.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftCell | String | Upper left cell name. |
| lowerRightCell | String | Lower right cell name. |

**Returns:** A Range object

---

### createRange(firstRow, firstColumn, totalRows, totalColumns) (2 of 4) {#createrange-1}

Creates a Range object from a range of cells.

| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Number | First row of this range |
| firstColumn | Number | First column of this range |
| totalRows | Number | Number of rows |
| totalColumns | Number | Number of columns |

**Returns:** A Range object

---

### createRange(address) (3 of 4) {#createrange-2}

Creates a Range object from an address of the range.

| Parameter | Type | Description |
| --- | --- | --- |
| address | String | The address of the range. |

**Returns:** A Range object

---

### createRange(firstIndex, number, isVertical) (4 of 4) {#createrange-3}

Creates a Range object from rows of cells or columns of cells.

| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | Number | First row index or first column index, zero based. |
| number | Number | Total number of rows or columns, one based. |
| isVertical | boolean | True - Range created from columns of cells. False - Range created from rows of cells. |

**Returns:** A Range object.

### clear() {#clear}

Clears all data of the worksheet.

### importFormulaArray(stringArray, firstRow, firstColumn, isVertical) {#importformulaarray}

Imports an array of formula into a worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| stringArray | String[] | Formula array. |
| firstRow | Number | The row number of the first cell to import in. |
| firstColumn | Number | The column number of the first cell to import in. |
| isVertical | boolean | Specifies to import data vertically or horizontally. |

### textToColumns(row, column, totalRows, options) {#texttocolumns}

Splits the text in the column to columns.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | The row index. |
| column | Number | The column index. |
| totalRows | Number | The number of rows. |
| options | TxtLoadOptions | The split options. |

### importCSV(fileName, splitter, convertNumericData, firstRow, firstColumn) (1 of 2) {#importcsv}

Import a CSV file to the cells.

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | The CSV file name. |
| splitter | String | The splitter |
| convertNumericData | boolean | Whether the string in text file is converted to numeric data. |
| firstRow | Number | The row number of the first cell to import in. |
| firstColumn | Number | The column number of the first cell to import in. |

---

### importCSV(fileName, options, firstRow, firstColumn) (2 of 2) {#importcsv-1}

Import a CSV file to the cells.

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | The CSV file name. |
| options | TxtLoadOptions | The load options for reading text file |
| firstRow | Number | The row number of the first cell to import in. |
| firstColumn | Number | The column number of the first cell to import in. |

### merge(firstRow, firstColumn, totalRows, totalColumns) (1 of 3) {#merge}

Merges a specified range of cells into a single cell.

Reference the merged cell via the address of the upper-left cell in the range.

| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Number | First row of this range(zero based) |
| firstColumn | Number | First column of this range(zero based) |
| totalRows | Number | Number of rows(one based) |
| totalColumns | Number | Number of columns(one based) |

---

### merge(firstRow, firstColumn, totalRows, totalColumns, mergeConflict) (2 of 3) {#merge-1}

Merges a specified range of cells into a single cell.

Reference the merged cell via the address of the upper-left cell in the range. If mergeConflict is true and the merged range conflicts with other merged cells, other merged cells will be automatically removed.

| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Number | First row of this range(zero based) |
| firstColumn | Number | First column of this range(zero based) |
| totalRows | Number | Number of rows(one based) |
| totalColumns | Number | Number of columns(one based) |
| mergeConflict | boolean | Merge conflict merged ranges. |

---

### merge(firstRow, firstColumn, totalRows, totalColumns, checkConflict, mergeConflict) (3 of 3) {#merge-2}

Merges a specified range of cells into a single cell.

Reference the merged cell via the address of the upper-left cell in the range. If mergeConflict is true and the merged range conflicts with other merged cells, other merged cells will be automatically removed.

| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Number | First row of this range(zero based) |
| firstColumn | Number | First column of this range(zero based) |
| totalRows | Number | Number of rows(one based) |
| totalColumns | Number | Number of columns(one based) |
| checkConflict | boolean | Indicates whether check the merged cells intersects other merged cells |
| mergeConflict | boolean | Merge conflict merged ranges. |

### unMerge(firstRow, firstColumn, totalRows, totalColumns) {#unmerge}

Unmerges a specified range of merged cells.

| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Number | First row of this range(zero based) |
| firstColumn | Number | First column of this range(zero based) |
| totalRows | Number | Number of rows(one based) |
| totalColumns | Number | Number of columns(one based) |

### clearMergedCells() {#clearmergedcells}

Clears all merged ranges.

### hideRow(row) {#hiderow}

Hides a row.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Row index. |

### unhideRow(row, height) {#unhiderow}

Unhides a row.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Row index. |
| height | Number | Row height. The row's height will be changed only when the row is hidden and given height value is positive. |

### hideRows(row, totalRows) {#hiderows}

Hides multiple rows.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | The row index. |
| totalRows | Number | The row number. |

### unhideRows(row, totalRows, height) {#unhiderows}

Unhides the hidden rows.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | The row index. |
| totalRows | Number | The row number. |
| height | Number | Row height. The row's height will be changed only when the row is hidden and given height value is positive. |

### setRowHeightPixel(row, pixels) {#setrowheightpixel}

Sets row height in unit of pixels.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Row index. |
| pixels | Number | Number of pixels. |

### setRowHeightInch(row, inches) {#setrowheightinch}

Sets row height in unit of inches.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Row index. |
| inches | Number | Number of inches. It should be between 0 and 409.5/72. |

### setRowHeight(row, height) {#setrowheight}

Sets the height of the specified row.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Row index. |
| height | Number | Height of row.In unit of point It should be between 0 and 409.5. |

### getRowHeight(row, isOriginal, unitType) (1 of 2) {#getrowheight}

Gets row's height.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | The row index. |
| isOriginal | boolean | Whether returns the original row height or 0 for hidden row. |
| unitType | Number | A CellsUnitType value. Unit type of the returned height value |

**Returns:** Row's height

---

### getRowHeight(row) (2 of 2) {#getrowheight-1}

Gets the height of a specified row, in unit of points.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Row index |

**Returns:** Height of row

### getRowOriginalHeightPoint(row) {#getroworiginalheightpoint}

Gets original row's height in unit of point if the row is hidden

NOTE: This member is now obsolete. Instead, please use Cells.GetRowHeight(int,bool,CellsUnitType) method. This method will be removed 12 months later since April 2024. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | The row index. |

### getColumnOriginalWidthPoint(column) {#getcolumnoriginalwidthpoint}

Gets original column's height in unit of point if the column is hidden

NOTE: This method is now obsolete. Instead, please use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method. This method will be removed 12 months later since April 2024. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| column | Number | The row index. |

### hideColumn(column) {#hidecolumn}

Hides a column.

| Parameter | Type | Description |
| --- | --- | --- |
| column | Number | Column index. |

### unhideColumn(column, width) {#unhidecolumn}

Unhides a column

| Parameter | Type | Description |
| --- | --- | --- |
| column | Number | Column index. |
| width | Number | Column width. |

### hideColumns(column, totalColumns) {#hidecolumns}

Hide multiple columns.

| Parameter | Type | Description |
| --- | --- | --- |
| column | Number | Column index. |
| totalColumns | Number | Column number. |

### unhideColumns(column, totalColumns, width) {#unhidecolumns}

Unhide multiple columns.

Only applies the column width to the hidden columns.

| Parameter | Type | Description |
| --- | --- | --- |
| column | Number | Column index. |
| totalColumns | Number | Column number |
| width | Number | Column width. |

### getViewRowHeight(row) {#getviewrowheight}

Gets the height of a specified row.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Row index. |

**Returns:** Height of row.

### getRowHeightInch(row) {#getrowheightinch}

Gets the height of a specified row in unit of inches.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Row index |

**Returns:** Height of row

### getViewRowHeightInch(row) {#getviewrowheightinch}

Gets the height of a specified row in unit of inches.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Row index |

**Returns:** Height of row

### getRowHeightPixel(row) {#getrowheightpixel}

Gets the height of a specified row in unit of pixel.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Row index |

**Returns:** Height of row

### setColumnWidthPixel(column, pixels) {#setcolumnwidthpixel}

Sets column width in unit of pixels in normal view.

| Parameter | Type | Description |
| --- | --- | --- |
| column | Number | Column index. |
| pixels | Number | Number of pixels. |

### setColumnWidthInch(column, inches) {#setcolumnwidthinch}

Sets column width in unit of inches in normal view.

| Parameter | Type | Description |
| --- | --- | --- |
| column | Number | Column index. |
| inches | Number | Number of inches. |

### setColumnWidth(column, width) {#setcolumnwidth}

Sets the width of the specified column in normal view.

To hide a column, sets column width to zero.

| Parameter | Type | Description |
| --- | --- | --- |
| column | Number | Column index. |
| width | Number | Width of column.Column width must be between 0 and 255. |

### getColumnWidthPixel(column) (1 of 2) {#getcolumnwidthpixel}

Gets the width of the specified column in normal view, in units of pixel.

| Parameter | Type | Description |
| --- | --- | --- |
| column | Number | Column index |

**Returns:** Width of column in normal view.

---

### getColumnWidthPixel(column, original) (2 of 2) {#getcolumnwidthpixel-1}

Gets the width of the specified column in normal view, in units of pixel.

NOTE: This method is now obsolete. Instead, please use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method. This method will be removed 12 months later since April 2024. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| column | Number | Column index |
| original | boolean | Indicates whether returning original width even when the column is hidden |

**Returns:** Width of column in normal view.

### getColumnWidthInch(column) {#getcolumnwidthinch}

Gets the width of the specified column in normal view, in units of inches.

NOTE: This method is now obsolete. Instead, please use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method. This method will be removed 12 months later since April 2024. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| column | Number | Column index |

**Returns:** Width of column
