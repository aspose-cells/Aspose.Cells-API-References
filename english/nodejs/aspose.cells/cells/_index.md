---
title: "Cells"
linktitle: "Cells"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Encapsulates a collection of cell relevant objects, such as Cell, Row, ...etc."
type: docs
weight: 400
url: /nodejs/aspose.cells/cells/
---

## Cells class

Encapsulates a collection of cell relevant objects, such as Cell, Row, ...etc.

## Methods

| Name | Description |
| --- | --- |
| [addRange(rangeObject)](#addrange) | Adds a range object reference to cells |
| [applyColumnStyle(column, style, flag)](#applycolumnstyle) | Applies formats for a whole column. |
| [applyRowStyle(row, style, flag)](#applyrowstyle) | Applies formats for a whole row. |
| [applyStyle(style, flag)](#applystyle) | Applies formats for a whole worksheet. |
| [checkCell(row, column)](#checkcell) | Gets the Cell element or null at the specified cell row index and column index. |
| [checkColumn(columnIndex)](#checkcolumn) | Gets the Column element or null at the specified column index. |
| [checkRow(row)](#checkrow) | Gets the Row element or null at the specified cell row index. |
| [clear()](#clear) | Clears all data of the worksheet. |
| [clearContents(range)](#clearcontents) | Clears contents of a range. |
| [clearContents(startRow, startColumn, endRow, endColumn)](#clearcontents-1) | Clears contents of a range. |
| [clearFormats(range)](#clearformats) | Clears formatting of a range. |
| [clearFormats(startRow, startColumn, endRow, endColumn)](#clearformats-1) | Clears formatting of a range. |
| [clearMergedCells()](#clearmergedcells) | Clears all merged ranges. |
| [clearRange(range)](#clearrange) | Clears contents and formatting of a range. |
| [clearRange(startRow, startColumn, endRow, endColumn)](#clearrange-1) | Clears contents and formatting of a range. |
| [convertStringToNumericValue()](#convertstringtonumericvalue) | Converts all string data in the worksheet to numeric value if possible. |
| [copyColumn(sourceCells, sourceColumnIndex, destinationColumnIndex)](#copycolumn) | Copies data and formats of a whole column. |
| [copyColumns(sourceCells0, sourceColumnIndex, destinationColumnIndex, columnNumber, pasteOptions)](#copycolumns) | Copies data and formats of a whole column. |
| [copyColumns(sourceCells0, sourceColumnIndex, destinationColumnIndex, columnNumber)](#copycolumns-1) | Copies data and formats of a whole column. |
| [copyColumns(sourceCells, sourceColumnIndex, sourceTotalColumns, destinationColumnIndex, destinationTotalColumns)](#copycolumns-2) | Copies data and formats of the whole columns. |
| [copyRow(sourceCells, sourceRowIndex, destinationRowIndex)](#copyrow) | Copies data and formats of a whole row. |
| [copyRows(sourceCells, sourceRowIndex, destinationRowIndex, rowNumber)](#copyrows) | Copies data and formats of some whole rows. |
| [copyRows(sourceCells0, sourceRowIndex, destinationRowIndex, rowNumber, copyOptions)](#copyrows-1) | Copies data and formats of some whole rows. |
| [copyRows(sourceCells0, sourceRowIndex, destinationRowIndex, rowNumber, copyOptions, pasteOptions)](#copyrows-2) | Copies data and formats of some whole rows. |
| [createRange(upperLeftCell, lowerRightCell)](#createrange) | Creates a Range object from a range of cells. |
| [createRange(firstRow, firstColumn, totalRows, totalColumns)](#createrange-1) | Creates a Range object from a range of cells. |
| [createRange(address)](#createrange-2) | Creates a Range object from an address of the range. |
| [createRange(firstIndex, number, isVertical)](#createrange-3) | Creates a Range object from rows of cells or columns of cells. |
| [deleteBlankColumns()](#deleteblankcolumns) | Delete all blank columns which do not contain any data. |
| [deleteBlankColumns(options)](#deleteblankcolumns-1) | Delete all blank columns which do not contain any data. |
| [deleteBlankRows()](#deleteblankrows) | Delete all blank rows which do not contain any data or other object. |
| [deleteBlankRows(options)](#deleteblankrows-1) | Delete all blank rows which do not contain any data or other object. For blank rows that will be deleted, it is not only |
| [deleteColumn(columnIndex, updateReference)](#deletecolumn) | Deletes a column. |
| [deleteColumn(columnIndex)](#deletecolumn-1) | Deletes a column. |
| [deleteColumns(columnIndex, totalColumns, updateReference)](#deletecolumns) | Deletes several columns. |
| [deleteColumns()](#deletecolumns-1) |  |
| [deleteRange(startRow, startColumn, endRow, endColumn, shiftType)](#deleterange) | Deletes a range of cells and shift cells according to the shift option. |
| [deleteRow(rowIndex)](#deleterow) | Deletes a row. |
| [deleteRow(rowIndex, updateReference)](#deleterow-1) | Deletes a row. |
| [deleteRows(rowIndex, totalRows)](#deleterows) | Deletes several rows. If the deleted range contains the top part(not whole) of the table(ListObject), the ranged could n |
| [deleteRows(rowIndex, totalRows, updateReference)](#deleterows-1) | Deletes multiple rows in the worksheet. |
| [deleteRows()](#deleterows-2) |  |
| [dispose()](#dispose) | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [endCellInColumn()](#endcellincolumn) |  |
| [endCellInColumn()](#endcellincolumn-1) |  |
| [endCellInRow(rowIndex)](#endcellinrow) | Gets the last cell in this row. |
| [endCellInRow(startRow, endRow, startColumn, endColumn)](#endcellinrow-1) | Gets the last cell with maximum row index in this range. |
| [find(what, previousCell)](#find) | Finds the cell containing with the input object. Returns null (Nothing) if no cell is found. |
| [find(what, previousCell, findOptions)](#find-1) | Finds the cell containing with the input object. Returns null (Nothing) if no cell is found. |
| [get(row, column)](#get) | Gets the Cell element at the specified cell row index and column index. |
| [get(cellName)](#get-1) | Gets the Cell element at the specified cell name. |
| [getCellDisplayStyle()](#getcelldisplaystyle) |  |
| [getCellDisplayStyle()](#getcelldisplaystyle-1) |  |
| [getCellStyle(row, column)](#getcellstyle) | Get the style of given cell. |
| [getCellsWithPlaceInCellPicture()](#getcellswithplaceincellpicture) |  |
| [getColumnOriginalWidthPoint(column)](#getcolumnoriginalwidthpoint) | Gets original column's height in unit of point if the column is hidden Width of column in normal view.NOTE: This method  |
| [getColumnWidth(column)](#getcolumnwidth) | Gets the width(in unit of characters) of the specified column in normal view |
| [getColumnWidth(column, isOriginal, unitType)](#getcolumnwidth-1) | Gets the column width. |
| [getColumnWidthInch(column)](#getcolumnwidthinch) | Gets the width of the specified column in normal view, in units of inches. Width of column in normal view.NOTE: This met |
| [getColumnWidthPixel(column)](#getcolumnwidthpixel) | Gets the width of the specified column in normal view, in units of pixel. |
| [getColumnWidthPixel(column, original)](#getcolumnwidthpixel-1) | Gets the width of the specified column in normal view, in units of pixel. NOTE: This method is now obsolete. Instead, pl |
| [getColumns()](#getcolumns) | Gets the collection of Column objects that represents the individual columns in this worksheet. |
| [getCount()](#getcount) | Gets the total count of instantiated Cell objects. |
| [getCountLarge()](#getcountlarge) | Gets the total count of instantiated Cell objects. |
| [getDependents(isAll, row, column)](#getdependents) | Get all cells which refer to the specific cell. |
| [getDependentsInCalculation(row, column, recursive)](#getdependentsincalculation) | Gets all cells whose calculated result depends on specific cell. To use this method, please make sure the workbook has b |
| [getFirstCell()](#getfirstcell) | Gets the first cell in this worksheet. Returns null if there is no data in the worksheet. |
| [getFirstDataRow()](#getfirstdatarow) |  |
| [getGroupedColumnOutlineLevel(columnIndex)](#getgroupedcolumnoutlinelevel) | Gets the outline level (zero-based) of the column. If the column is not grouped, returns zero. |
| [getGroupedRowOutlineLevel(rowIndex)](#getgroupedrowoutlinelevel) | Gets the outline level (zero-based) of the row. If the row is not grouped, returns zero. |
| [getLastCell()](#getlastcell) | Gets the last cell in this worksheet. Returns null if there is no data in the worksheet. |
| [getLastDataRow(column)](#getlastdatarow) | Gets the last row index of cell which contains data in the specified column. |
| [getMaxColumn()](#getmaxcolumn) | Maximum column index of those cells that have been instantiated in the collection(does not include the column where styl |
| [getMaxDataColumn()](#getmaxdatacolumn) | Maximum column index of cell which contains data. -1 will be returned if there is no cell which contains data. This prop |
| [getMaxDataRow()](#getmaxdatarow) | Maximum row index of cell which contains data. Return -1 if there is no cell which contains data. |
| [getMaxDisplayRange()](#getmaxdisplayrange) | Gets the max range which includes data, merged cells and shapes. Reutrns null if the worksheet is empty since Aspose.Cel |
| [getMaxGroupedColumnOutlineLevel()](#getmaxgroupedcolumnoutlinelevel) | Gets the max grouped column outline level (zero-based). |
| [getMaxGroupedRowOutlineLevel()](#getmaxgroupedrowoutlinelevel) | Gets the max grouped row outline level (zero-based). |
| [getMaxRow()](#getmaxrow) | Maximum row index of cell which contains data or style. Return -1 if there is no cell which contains data or style in th |
| [getMemorySetting()](#getmemorysetting) | Gets or sets the memory usage option for this cells. The value of the property is MemorySetting integer constant. |
| [getMergedAreas()](#getmergedareas) | Gets all merged cells. |
| [getMergedCells()](#getmergedcells) | Gets the collection of merged cells. In this collection, each item is a CellArea structure which represents an area of m |
| [getMinColumn()](#getmincolumn) | Minimum column index of those cells that have been instantiated in the collection(does not include the column where styl |
| [getMinDataColumn()](#getmindatacolumn) | Minimum column index of cell which contains data. -1 will be returned if there is no cell which contains data. This prop |
| [getMinDataRow()](#getmindatarow) | Minimum row index of cell which contains data. |
| [getMinRow()](#getminrow) | Minimum row index of cell which contains data or style. |
| [getMultiThreadReading()](#getmultithreadreading) | Gets or sets whether the cells data model should support Multi-Thread reading. Default value of this property is false.  |
| [getOdsCellFields()](#getodscellfields) | Gets the list of fields of ods. |
| [getPreserveString()](#getpreservestring) | Gets or sets a value indicating whether all worksheet values are preserved as strings. Default is false. |
| [getRanges()](#getranges) | Gets the collection of Range objects created at run time. |
| [getRowEnumerator()](#getrowenumerator) | Gets the rows enumerator. NOTE: This member is now obsolete. Instead, please use RowCollection.GetEnumerator() method. T |
| [getRowHeight(row, isOriginal, unitType)](#getrowheight) | Gets row's height. |
| [getRowHeight(row)](#getrowheight-1) | Gets the height of a specified row, in unit of points. |
| [getRowHeightInch(row)](#getrowheightinch) | Gets the height of a specified row in unit of inches. |
| [getRowHeightPixel(row)](#getrowheightpixel) | Gets the height of a specified row in unit of pixel. |
| [getRowOriginalHeightPoint(row)](#getroworiginalheightpoint) | Gets original row's height in unit of point if the row is hidden NOTE: This member is now obsolete. Instead, please use  |
| [getRows()](#getrows) | Gets the collection of Row objects that represents the individual rows in this worksheet. |
| [getStandardHeight()](#getstandardheight) | Gets or sets the default row height in this worksheet, in unit of points. |
| [getStandardHeightInch()](#getstandardheightinch) | Gets or sets the default row height in this worksheet, in unit of inches. |
| [getStandardHeightPixels()](#getstandardheightpixels) | Gets or sets the default row height in this worksheet, in unit of pixels. |
| [getStandardWidth()](#getstandardwidth) | Gets or sets the default column width in the worksheet, in unit of characters. |
| [getStandardWidthInch()](#getstandardwidthinch) | Gets or sets the default column width in the worksheet, in unit of inches. |
| [getStandardWidthPixels()](#getstandardwidthpixels) | Gets or sets the default column width in the worksheet, in unit of pixels. |
| [getStyle()](#getstyle) | Gets and sets the default style of the worksheet. |
| [getViewColumnWidthPixel(column)](#getviewcolumnwidthpixel) | Get the width in different view type. |
| [getViewRowHeight(row)](#getviewrowheight) | Gets the height of a specified row. |
| [getViewRowHeightInch(row)](#getviewrowheightinch) | Gets the height of a specified row in unit of inches. |
| [groupColumns(firstIndex, lastIndex)](#groupcolumns) | Groups columns. |
| [groupColumns(firstIndex, lastIndex, isHidden)](#groupcolumns-1) | Groups columns. |
| [groupRows(firstIndex, lastIndex, isHidden)](#grouprows) | Groups rows. |
| [groupRows(firstIndex, lastIndex)](#grouprows-1) | Groups rows. |
| [hideColumn(column)](#hidecolumn) | Hides a column. |
| [hideColumns(column, totalColumns)](#hidecolumns) | Hide multiple columns. |
| [hideGroupDetail(isVertical, index)](#hidegroupdetail) | Collapses the grouped rows/columns. |
| [hideRow(row)](#hiderow) | Hides a row. |
| [hideRows(row, totalRows)](#hiderows) | Hides multiple rows. |
| [importCSV(fileName, splitter, convertNumericData, firstRow, firstColumn)](#importcsv) | Import a CSV file to the cells. |
| [importCSV(fileName, options, firstRow, firstColumn)](#importcsv-1) | Import a CSV file to the cells. |
| [importFormulaArray(stringArray, firstRow, firstColumn, isVertical)](#importformulaarray) | Imports an array of formula into a worksheet. |
| [insertColumn(columnIndex, updateReference)](#insertcolumn) | Inserts a new column into the worksheet. |
| [insertColumn(columnIndex)](#insertcolumn-1) | Inserts a new column into the worksheet. |
| [insertColumns(columnIndex, totalColumns)](#insertcolumns) | Inserts some columns into the worksheet. |
| [insertColumns(columnIndex, totalColumns, updateReference)](#insertcolumns-1) | Inserts some columns into the worksheet. |
| [insertColumns()](#insertcolumns-2) |  |
| [insertCutCells(cutRange, row, column, shiftType)](#insertcutcells) | Insert cut range. |
| [insertRange(area, shiftNumber, shiftType, updateReference)](#insertrange) | Inserts a range of cells and shift cells according to the shift option. |
| [insertRange(area, shiftType)](#insertrange-1) | Inserts a range of cells and shift cells according to the shift option. |
| [insertRange(area, shiftNumber, shiftType)](#insertrange-2) | Inserts a range of cells and shift cells according to the shift option. |
| [insertRow(rowIndex)](#insertrow) | Inserts a new row into the worksheet. |
| [insertRows(rowIndex, totalRows, updateReference)](#insertrows) | Inserts multiple rows into the worksheet. |
| [insertRows(rowIndex, totalRows, options)](#insertrows-1) | Inserts multiple rows into the worksheet. |
| [insertRows(rowIndex, totalRows)](#insertrows-2) | Inserts multiple rows into the worksheet. |
| [isBlankColumn(columnIndex)](#isblankcolumn) | Checks whether given column is blank(does not contain any data). |
| [isColumnHidden(columnIndex)](#iscolumnhidden) | Checks whether a column at given index is hidden. |
| [isDefaultColumnHidden()](#isdefaultcolumnhidden) |  |
| [isDefaultRowHeightMatched()](#isdefaultrowheightmatched) | Indicates that row height and default font height matches |
| [isDefaultRowHidden()](#isdefaultrowhidden) | Indicates whether the row is default hidden. |
| [isDeletingRangeEnabled(startRow, startColumn, totalRows, totalColumns)](#isdeletingrangeenabled) | Check whether the range could be deleted. |
| [isRowHidden(rowIndex)](#isrowhidden) | Checks whether a row at given index is hidden. |
| [iterator()](#iterator) | Gets the cells enumerator. When traversing elements by the returned Enumerator, the cells collection should not be modif |
| [linkToXmlMap(mapName, row, column, path)](#linktoxmlmap) | Link to a xml map. e.g. A xml map element structure: -RootElement \|-Attribute1 \|-SubElement \|-Attribute2 \|-Attribute3 To |
| [merge(firstRow, firstColumn, totalRows, totalColumns)](#merge) | Merges a specified range of cells into a single cell. Reference the merged cell via the address of the upper-left cell i |
| [merge(firstRow, firstColumn, totalRows, totalColumns, mergeConflict)](#merge-1) | Merges a specified range of cells into a single cell. Reference the merged cell via the address of the upper-left cell i |
| [merge(firstRow, firstColumn, totalRows, totalColumns, checkConflict, mergeConflict)](#merge-2) | Merges a specified range of cells into a single cell. Reference the merged cell via the address of the upper-left cell i |
| [moveRange(sourceArea, destRow, destColumn)](#moverange) | Moves the range. |
| [removeDuplicates()](#removeduplicates) | Removes duplicate rows in the sheet. |
| [removeDuplicates(startRow, startColumn, endRow, endColumn)](#removeduplicates-1) | Removes duplicate values in the range. |
| [removeDuplicates(startRow, startColumn, endRow, endColumn, hasHeaders, columnOffsets)](#removeduplicates-2) | Removes duplicate data of the range. |
| [removeFormulas()](#removeformulas) | Removes all formula and replaces with the value of the formula. |
| [retrieveSubtotalSetting(ca)](#retrievesubtotalsetting) | Retrieves subtotals setting of the range. |
| [setColumnWidth(column, width)](#setcolumnwidth) | Sets the width of the specified column in normal view. To hide a column, sets column width to zero. |
| [setColumnWidthInch(column, inches)](#setcolumnwidthinch) | Sets column width in unit of inches in normal view. |
| [setColumnWidthPixel(column, pixels)](#setcolumnwidthpixel) | Sets column width in unit of pixels in normal view. |
| [setDefaultColumnHidden()](#setdefaultcolumnhidden) |  |
| [setDefaultRowHeightMatched()](#setdefaultrowheightmatched) | Indicates that row height and default font height matches |
| [setDefaultRowHidden()](#setdefaultrowhidden) | Indicates whether the row is default hidden. |
| [setMemorySetting()](#setmemorysetting) | Gets or sets the memory usage option for this cells. The value of the property is MemorySetting integer constant. |
| [setMultiThreadReading()](#setmultithreadreading) | Gets or sets whether the cells data model should support Multi-Thread reading. Default value of this property is false.  |
| [setPreserveString()](#setpreservestring) | Gets or sets a value indicating whether all worksheet values are preserved as strings. Default is false. |
| [setRowHeight(row, height)](#setrowheight) | Sets the height of the specified row. |
| [setRowHeightInch(row, inches)](#setrowheightinch) | Sets row height in unit of inches. |
| [setRowHeightPixel(row, pixels)](#setrowheightpixel) | Sets row height in unit of pixels. |
| [setStandardHeight()](#setstandardheight) | Gets or sets the default row height in this worksheet, in unit of points. |
| [setStandardHeightInch()](#setstandardheightinch) | Gets or sets the default row height in this worksheet, in unit of inches. |
| [setStandardHeightPixels()](#setstandardheightpixels) | Gets or sets the default row height in this worksheet, in unit of pixels. |
| [setStandardWidth()](#setstandardwidth) | Gets or sets the default column width in the worksheet, in unit of characters. |
| [setStandardWidthInch()](#setstandardwidthinch) | Gets or sets the default column width in the worksheet, in unit of inches. |
| [setStandardWidthPixels()](#setstandardwidthpixels) | Gets or sets the default column width in the worksheet, in unit of pixels. |
| [setStyle()](#setstyle) | Gets and sets the default style of the worksheet. |
| [setViewColumnWidthPixel(column, pixels)](#setviewcolumnwidthpixel) | Sets the width of the column in different view. If the current view type is ViewType.PAGE_LAYOUT_VIEW, the column's widt |
| [showGroupDetail(isVertical, index)](#showgroupdetail) | Expands the grouped rows/columns. |
| [subtotal(ca, groupBy, function, totalList)](#subtotal) | Creates subtotals for the range. |
| [subtotal(ca, groupBy, function, totalList, replace, pageBreaks, summaryBelowData)](#subtotal-1) | Creates subtotals for the range. |
| [textToColumns(row, column, totalRows, options)](#texttocolumns) | Splits the text in the column to columns. |
| [unMerge(firstRow, firstColumn, totalRows, totalColumns)](#unmerge) | Unmerges a specified range of merged cells. |
| [ungroupColumns(firstIndex, lastIndex)](#ungroupcolumns) | Ungroups columns. |
| [ungroupRows(firstIndex, lastIndex, isAll)](#ungrouprows) | Ungroups rows. |
| [ungroupRows(firstIndex, lastIndex)](#ungrouprows-1) | Ungroups rows. Only removes outer group info. |
| [unhideColumn(column, width)](#unhidecolumn) | Unhides a column |
| [unhideColumns(column, totalColumns, width)](#unhidecolumns) | Unhide multiple columns. Only applies the column width to the hidden columns. |
| [unhideRow(row, height)](#unhiderow) | Unhides a row. |
| [unhideRows(row, totalRows, height)](#unhiderows) | Unhides the hidden rows. |
| [importCSVFromStream(cells, stream, spliter, convertNumericData, firstRow, firstColumn, callback)](#importcsvfromstream) *(static)* | Import a CSV file to the cells. |
| [importCSVFromStream(cells, stream, options, firstRow, firstColumn, callback)](#importcsvfromstream-1) *(static)* | Import a CSV file to the cells. |

### addRange(rangeObject) {#addrange}

Adds a range object reference to cells

| Parameter | Type | Description |
| --- | --- | --- |
| rangeObject | Range | The range object will be contained in the cells |

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

### checkCell(row, column) {#checkcell}

Gets the Cell element or null at the specified cell row index and column index.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Row index |
| column | Number | Column index |

**Returns:** Cell — `Cell` Return Cell object if a Cell object exists. Return null if the cell does not exist.

### checkColumn(columnIndex) {#checkcolumn}

Gets the Column element or null at the specified column index.

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Number | The column index. |

**Returns:** Column — `Column` The Column object.

### checkRow(row) {#checkrow}

Gets the Row element or null at the specified cell row index.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Row index |

**Returns:** Row — `Row` Returns Row object If the row object does exist, otherwise returns null.

### clear() {#clear}

Clears all data of the worksheet.

### clearContents(range) {#clearcontents}

Clears contents of a range.

| Parameter | Type | Description |
| --- | --- | --- |
| range | CellArea | Range to be cleared. |

### clearContents(startRow, startColumn, endRow, endColumn) {#clearcontents-1}

Clears contents of a range.

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Number | Start row index. |
| startColumn | Number | Start column index. |
| endRow | Number | End row index. |
| endColumn | Number | End column index. |

### clearFormats(range) {#clearformats}

Clears formatting of a range.

| Parameter | Type | Description |
| --- | --- | --- |
| range | CellArea | Range to be cleared. |

### clearFormats(startRow, startColumn, endRow, endColumn) {#clearformats-1}

Clears formatting of a range.

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Number | Start row index. |
| startColumn | Number | Start column index. |
| endRow | Number | End row index. |
| endColumn | Number | End column index. |

### clearMergedCells() {#clearmergedcells}

Clears all merged ranges.

### clearRange(range) {#clearrange}

Clears contents and formatting of a range.

| Parameter | Type | Description |
| --- | --- | --- |
| range | CellArea | Range to be cleared. |

### clearRange(startRow, startColumn, endRow, endColumn) {#clearrange-1}

Clears contents and formatting of a range.

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Number | Start row index. |
| startColumn | Number | Start column index. |
| endRow | Number | End row index. |
| endColumn | Number | End column index. |

### convertStringToNumericValue() {#convertstringtonumericvalue}

Converts all string data in the worksheet to numeric value if possible.

### copyColumn(sourceCells, sourceColumnIndex, destinationColumnIndex) {#copycolumn}

Copies data and formats of a whole column.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells | Cells | Source Cells object contains data and formats to copy. |
| sourceColumnIndex | Number | Source column index. |
| destinationColumnIndex | Number | Destination column index. |

### copyColumns(sourceCells0, sourceColumnIndex, destinationColumnIndex, columnNumber, pasteOptions) {#copycolumns}

Copies data and formats of a whole column.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells0 |  | Source Cells object contains data and formats to copy. |
| sourceColumnIndex | Number | Source column index. |
| destinationColumnIndex | Number | Destination column index. |
| columnNumber | Number | The copied column number. |
| pasteOptions | PasteOptions | the options of pasting. |

### copyColumns(sourceCells0, sourceColumnIndex, destinationColumnIndex, columnNumber) {#copycolumns-1}

Copies data and formats of a whole column.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells0 |  | Source Cells object contains data and formats to copy. |
| sourceColumnIndex | Number | Source column index. |
| destinationColumnIndex | Number | Destination column index. |
| columnNumber | Number | The copied column number. |

### copyColumns(sourceCells, sourceColumnIndex, sourceTotalColumns, destinationColumnIndex, destinationTotalColumns) {#copycolumns-2}

Copies data and formats of the whole columns.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells | Cells | Source Cells object contains data and formats to copy. |
| sourceColumnIndex | Number | Source column index. |
| sourceTotalColumns | Number | The number of the source columns. |
| destinationColumnIndex | Number | Destination column index. |
| destinationTotalColumns | Number | The number of the destination columns. |

### copyRow(sourceCells, sourceRowIndex, destinationRowIndex) {#copyrow}

Copies data and formats of a whole row.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells | Cells | Source Cells object contains data and formats to copy. |
| sourceRowIndex | Number | Source row index. |
| destinationRowIndex | Number | Destination row index. |

### copyRows(sourceCells, sourceRowIndex, destinationRowIndex, rowNumber) {#copyrows}

Copies data and formats of some whole rows.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells | Cells | Source Cells object contains data and formats to copy. |
| sourceRowIndex | Number | Source row index. |
| destinationRowIndex | Number | Destination row index. |
| rowNumber | Number | The copied row number. |

### copyRows(sourceCells0, sourceRowIndex, destinationRowIndex, rowNumber, copyOptions) {#copyrows-1}

Copies data and formats of some whole rows.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells0 |  | Source Cells object contains data and formats to copy. |
| sourceRowIndex | Number | Source row index. |
| destinationRowIndex | Number | Destination row index. |
| rowNumber | Number | The copied row number. |
| copyOptions | CopyOptions | The copy options. |

### copyRows(sourceCells0, sourceRowIndex, destinationRowIndex, rowNumber, copyOptions, pasteOptions) {#copyrows-2}

Copies data and formats of some whole rows.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells0 | Cells | Source Cells object contains data and formats to copy. |
| sourceRowIndex | Number | Source row index. |
| destinationRowIndex | Number | Destination row index. |
| rowNumber | Number | The copied row number. |
| copyOptions | CopyOptions | The copy options. |
| pasteOptions | PasteOptions | the options of pasting. |

### createRange(upperLeftCell, lowerRightCell) {#createrange}

Creates a Range object from a range of cells.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftCell | String | Upper left cell name. |
| lowerRightCell | String | Lower right cell name. |

**Returns:** Range — `Range` A Range object

### createRange(firstRow, firstColumn, totalRows, totalColumns) {#createrange-1}

Creates a Range object from a range of cells.

| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Number | First row of this range |
| firstColumn | Number | First column of this range |
| totalRows | Number | Number of rows |
| totalColumns | Number | Number of columns |

**Returns:** Range — `Range` A Range object

### createRange(address) {#createrange-2}

Creates a Range object from an address of the range.

| Parameter | Type | Description |
| --- | --- | --- |
| address | String | The address of the range. |

**Returns:** Range — `Range` A Range object

### createRange(firstIndex, number, isVertical) {#createrange-3}

Creates a Range object from rows of cells or columns of cells.

| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | Number | First row index or first column index, zero based. |
| number | Number | Total number of rows or columns, one based. |
| isVertical | boolean | True - Range created from columns of cells. False - Range created from rows of cells. |

**Returns:** Range — `Range` A Range object.

### deleteBlankColumns() {#deleteblankcolumns}

Delete all blank columns which do not contain any data.

### deleteBlankColumns(options) {#deleteblankcolumns-1}

Delete all blank columns which do not contain any data.

| Parameter | Type | Description |
| --- | --- | --- |
| options | DeleteOptions | The options of deleting range. |

### deleteBlankRows() {#deleteblankrows}

Delete all blank rows which do not contain any data or other object.

### deleteBlankRows(options) {#deleteblankrows-1}

Delete all blank rows which do not contain any data or other object. For blank rows that will be deleted, it is not only required that Row.IsBlank should be true, but also there should be no visible comment defined for any cell in those rows, and no pivot table whose range intersects with them.

| Parameter | Type | Description |
| --- | --- | --- |
| options | DeleteOptions | The options of deleting range. |

### deleteColumn(columnIndex, updateReference) {#deletecolumn}

Deletes a column.

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Number | Index of the column to be deleted. |
| updateReference | boolean | Indicates whether update references in other worksheets. |

### deleteColumn(columnIndex) {#deletecolumn-1}

Deletes a column.

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Number | Index of the column to be deleted. |

### deleteColumns(columnIndex, totalColumns, updateReference) {#deletecolumns}

Deletes several columns.

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Number | Index of the first column to be deleted. |
| totalColumns | Number | Count of columns to be deleted. |
| updateReference | boolean | Indicates whether update references in other worksheets. |

### deleteColumns() {#deletecolumns-1}

### deleteRange(startRow, startColumn, endRow, endColumn, shiftType) {#deleterange}

Deletes a range of cells and shift cells according to the shift option.

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Number | Start row index. |
| startColumn | Number | Start column index. |
| endRow | Number | End row index. |
| endColumn | Number | End column index. |
| shiftType | Number | ShiftType |

### deleteRow(rowIndex) {#deleterow}

Deletes a row.

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Number | Index of the row to be deleted. |

### deleteRow(rowIndex, updateReference) {#deleterow-1}

Deletes a row.

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Number | Index of the row to be deleted. |
| updateReference | boolean | Indicates whether update references in other worksheets. |

### deleteRows(rowIndex, totalRows) {#deleterows}

Deletes several rows. If the deleted range contains the top part(not whole) of the table(ListObject), the ranged could not be deleted and nothing will be done. It works in the same way with MS Excel.

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Number | The first row index to be deleted. |
| totalRows | Number | Count of rows to be deleted. |

### deleteRows(rowIndex, totalRows, updateReference) {#deleterows-1}

Deletes multiple rows in the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Number | Index of the first row to be deleted. |
| totalRows | Number | Count of rows to be deleted. |
| updateReference | boolean | Indicates whether update references in other worksheets. |

**Returns:** boolean — `boolean`

### deleteRows() {#deleterows-2}

### dispose() {#dispose}

Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources.

### endCellInColumn() {#endcellincolumn}

### endCellInColumn() {#endcellincolumn-1}

### endCellInRow(rowIndex) {#endcellinrow}

Gets the last cell in this row.

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Number | Row index. |

**Returns:** Cell — `Cell` Cell object.

### endCellInRow(startRow, endRow, startColumn, endColumn) {#endcellinrow-1}

Gets the last cell with maximum row index in this range.

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Number | Start row index. |
| endRow | Number | End row index. |
| startColumn | Number | Start column index. |
| endColumn | Number | End column index. |

**Returns:** Cell — `Cell` Cell object.

### find(what, previousCell) {#find}

Finds the cell containing with the input object. Returns null (Nothing) if no cell is found.

| Parameter | Type | Description |
| --- | --- | --- |
| what | Object | The object to search for. The type should be int,double,DateTime,string,bool. |
| previousCell | Cell | Previous cell with the same object. This parameter can be set to null if searching from the start. |

**Returns:** Cell — `Cell` Cell object.

### find(what, previousCell, findOptions) {#find-1}

Finds the cell containing with the input object. Returns null (Nothing) if no cell is found.

| Parameter | Type | Description |
| --- | --- | --- |
| what | Object | The object to search for. The type should be int,double,DateTime,string,bool. |
| previousCell | Cell | Previous cell with the same object. This parameter can be set to null if searching from the start. |
| findOptions | FindOptions | Find options |

**Returns:** Cell — `Cell` Cell object.

### get(row, column) {#get}

Gets the Cell element at the specified cell row index and column index.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Row index. |
| column | Number | Column index. |

**Returns:** Cell — `Cell` The Cell object.

**Example:**

```js
var cells = excel.getWorksheets().get(0).getCells();
var cell = cells.get(0, 0);    //Gets the cell at "A1"
```

### get(cellName) {#get-1}

Gets the Cell element at the specified cell name.

| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | Cell name,including its column letter and row number, for example A5. |

**Returns:** Cell — `Cell` A Cell object

**Example:**

```js
var cells = excel.getWorksheets().get(0).getCells();
var cell = cells.get("A1");    //Gets the cell at "A1"
```

### getCellDisplayStyle() {#getcelldisplaystyle}

### getCellDisplayStyle() {#getcelldisplaystyle-1}

### getCellStyle(row, column) {#getcellstyle}

Get the style of given cell.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | row index |
| column | Number | column |

**Returns:** Style — `Style` the style of given cell.

### getCellsWithPlaceInCellPicture() {#getcellswithplaceincellpicture}

### getColumnOriginalWidthPoint(column) {#getcolumnoriginalwidthpoint}

Gets original column's height in unit of point if the column is hidden Width of column in normal view.NOTE: This method is now obsolete. Instead, please use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method. This method will be removed 12 months later since April 2024. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| column | Number | The row index. |

**Returns:** Number — `Number`

### getColumnWidth(column) {#getcolumnwidth}

Gets the width(in unit of characters) of the specified column in normal view

| Parameter | Type | Description |
| --- | --- | --- |
| column | Number | Column index |

**Returns:** Number — `Number` Width of column. For spreadsheet, column width is measured as the number of characters of the maximum digit width of the numbers 0~9 as rendered in the normal style's font.

### getColumnWidth(column, isOriginal, unitType) {#getcolumnwidth-1}

Gets the column width.

| Parameter | Type | Description |
| --- | --- | --- |
| column | Number | The column index. |
| isOriginal | boolean | Indicates whether getting original width. |
| unitType | Number | CellsUnitType |

**Returns:** Number — `Number`

### getColumnWidthInch(column) {#getcolumnwidthinch}

Gets the width of the specified column in normal view, in units of inches. Width of column in normal view.NOTE: This method is now obsolete. Instead, please use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method. This method will be removed 12 months later since April 2024. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| column | Number | Column index |

**Returns:** Number — `Number` Width of column

### getColumnWidthPixel(column) {#getcolumnwidthpixel}

Gets the width of the specified column in normal view, in units of pixel.

| Parameter | Type | Description |
| --- | --- | --- |
| column | Number | Column index |

**Returns:** Number — `Number` Width of column in normal view.

### getColumnWidthPixel(column, original) {#getcolumnwidthpixel-1}

Gets the width of the specified column in normal view, in units of pixel. NOTE: This method is now obsolete. Instead, please use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method. This method will be removed 12 months later since April 2024. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| column | Number | Column index |
| original | boolean | Indicates whether returning original width even when the column is hidden |

**Returns:** Number — `Number` Width of column in normal view.

### getColumns() {#getcolumns}

Gets the collection of Column objects that represents the individual columns in this worksheet.

### getCount() {#getcount}

Gets the total count of instantiated Cell objects.

### getCountLarge() {#getcountlarge}

Gets the total count of instantiated Cell objects.

### getDependents(isAll, row, column) {#getdependents}

Get all cells which refer to the specific cell.

| Parameter | Type | Description |
| --- | --- | --- |
| isAll | boolean | Indicates whether check other worksheets |
| row | Number | The row index. |
| column | Number | The column index. |

**Returns:** Array ofCell — `Array ofCell`

### getDependentsInCalculation(row, column, recursive) {#getdependentsincalculation}

Gets all cells whose calculated result depends on specific cell. To use this method, please make sure the workbook has been set with true value for FormulaSettings.EnableCalculationChain and has been fully calculated with this setting. If there is no formula reference to this cell, null will be returned. For more details and example, please see Cell.getDependentsInCalculation(boolean)

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Row index of the specific cell |
| column | Number | Column index of the specific cell. |
| recursive | boolean | Whether returns those dependents which do not reference to the specific cell directly but reference to other leafs of that cell. |

**Returns:** Iterator — `Iterator` Enumerator to enumerate all dependents(Cell objects)

### getFirstCell() {#getfirstcell}

Gets the first cell in this worksheet. Returns null if there is no data in the worksheet.

### getFirstDataRow() {#getfirstdatarow}

### getGroupedColumnOutlineLevel(columnIndex) {#getgroupedcolumnoutlinelevel}

Gets the outline level (zero-based) of the column. If the column is not grouped, returns zero.

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Number | The column index |

**Returns:** Number — `Number` The outline level of the column

### getGroupedRowOutlineLevel(rowIndex) {#getgroupedrowoutlinelevel}

Gets the outline level (zero-based) of the row. If the row is not grouped, returns zero.

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Number | The row index. |

**Returns:** Number — `Number` The outline level (zero-based) of the row.

### getLastCell() {#getlastcell}

Gets the last cell in this worksheet. Returns null if there is no data in the worksheet.

### getLastDataRow(column) {#getlastdatarow}

Gets the last row index of cell which contains data in the specified column.

| Parameter | Type | Description |
| --- | --- | --- |
| column | Number | Column index. |

**Returns:** Number — `Number` last row index.

### getMaxColumn() {#getmaxcolumn}

Maximum column index of those cells that have been instantiated in the collection(does not include the column where style is defined for the whole column but no cell has been instantiated in it). Return -1 if there is no cell.

### getMaxDataColumn() {#getmaxdatacolumn}

Maximum column index of cell which contains data. -1 will be returned if there is no cell which contains data. This property needs to iterate and check all cells in a worksheet, so it is a time-consumed progress and should not be invoked repeatedly.

### getMaxDataRow() {#getmaxdatarow}

Maximum row index of cell which contains data. Return -1 if there is no cell which contains data.

### getMaxDisplayRange() {#getmaxdisplayrange}

Gets the max range which includes data, merged cells and shapes. Reutrns null if the worksheet is empty since Aspose.Cells 21.5.2.

### getMaxGroupedColumnOutlineLevel() {#getmaxgroupedcolumnoutlinelevel}

Gets the max grouped column outline level (zero-based).

**Returns:** Number — `Number` The max grouped column outline level (zero-based)

### getMaxGroupedRowOutlineLevel() {#getmaxgroupedrowoutlinelevel}

Gets the max grouped row outline level (zero-based).

**Returns:** Number — `Number` The max grouped row outline level (zero-based)

### getMaxRow() {#getmaxrow}

Maximum row index of cell which contains data or style. Return -1 if there is no cell which contains data or style in the worksheet.

### getMemorySetting() {#getmemorysetting}

Gets or sets the memory usage option for this cells. The value of the property is MemorySetting integer constant.

### getMergedAreas() {#getmergedareas}

Gets all merged cells.

### getMergedCells() {#getmergedcells}

Gets the collection of merged cells. In this collection, each item is a CellArea structure which represents an area of merged cells. NOTE: This method is now obsolete. Instead, please use Cells.GetMergedAreas() method. This method will be removed 12 months later since November 2023. Aspose apologizes for any inconvenience you may have experienced.

### getMinColumn() {#getmincolumn}

Minimum column index of those cells that have been instantiated in the collection(does not include the column where style is defined for the whole column but no cell has been instantiated in it).

### getMinDataColumn() {#getmindatacolumn}

Minimum column index of cell which contains data. -1 will be returned if there is no cell which contains data. This property needs to iterate and check all cells in a worksheet, so it is a time-consumed progress and should not be invoked repeatedly.

### getMinDataRow() {#getmindatarow}

Minimum row index of cell which contains data.

### getMinRow() {#getminrow}

Minimum row index of cell which contains data or style.

### getMultiThreadReading() {#getmultithreadreading}

Gets or sets whether the cells data model should support Multi-Thread reading. Default value of this property is false. If there are multiple threads to read Row/Cell objects in this collection concurrently, this property should be set as true, otherwise unexpected result may be produced. Supporting Multi-Thread reading may degrade the performance for accessing Row/Cell objects from this collection. Please note, some features cannot support Multi-Thread reading, such as formatting values(by Cell.StringValue, Cell.DisplayStringValue, .etc.). So, even with this property being set as true, those APIs still may give unexpected result for Multi-Thread reading.

### getOdsCellFields() {#getodscellfields}

Gets the list of fields of ods.

### getPreserveString() {#getpreservestring}

Gets or sets a value indicating whether all worksheet values are preserved as strings. Default is false.

### getRanges() {#getranges}

Gets the collection of Range objects created at run time.

### getRowEnumerator() {#getrowenumerator}

Gets the rows enumerator. NOTE: This member is now obsolete. Instead, please use RowCollection.GetEnumerator() method. This method will be removed 12 months later since May 2023. Aspose apologizes for any inconvenience you may have experienced.@return {Iterator} The rows enumerator.See Also:RowCollection.iterator()

### getRowHeight(row, isOriginal, unitType) {#getrowheight}

Gets row's height.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | The row index. |
| isOriginal | boolean | Whether returns the original row height or 0 for hidden row. |
| unitType | Number | CellsUnitType |

**Returns:** Number — `Number` Row's height

### getRowHeight(row) {#getrowheight-1}

Gets the height of a specified row, in unit of points.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Row index |

**Returns:** Number — `Number` Height of row

### getRowHeightInch(row) {#getrowheightinch}

Gets the height of a specified row in unit of inches.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Row index |

**Returns:** Number — `Number` Height of row

### getRowHeightPixel(row) {#getrowheightpixel}

Gets the height of a specified row in unit of pixel.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Row index |

**Returns:** Number — `Number` Height of row

### getRowOriginalHeightPoint(row) {#getroworiginalheightpoint}

Gets original row's height in unit of point if the row is hidden NOTE: This member is now obsolete. Instead, please use Cells.GetRowHeight(int,bool,CellsUnitType) method. This method will be removed 12 months later since April 2024. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | The row index. |

**Returns:** Number — `Number`

### getRows() {#getrows}

Gets the collection of Row objects that represents the individual rows in this worksheet.

### getStandardHeight() {#getstandardheight}

Gets or sets the default row height in this worksheet, in unit of points.

### getStandardHeightInch() {#getstandardheightinch}

Gets or sets the default row height in this worksheet, in unit of inches.

### getStandardHeightPixels() {#getstandardheightpixels}

Gets or sets the default row height in this worksheet, in unit of pixels.

### getStandardWidth() {#getstandardwidth}

Gets or sets the default column width in the worksheet, in unit of characters.

### getStandardWidthInch() {#getstandardwidthinch}

Gets or sets the default column width in the worksheet, in unit of inches.

### getStandardWidthPixels() {#getstandardwidthpixels}

Gets or sets the default column width in the worksheet, in unit of pixels.

### getStyle() {#getstyle}

Gets and sets the default style of the worksheet.

### getViewColumnWidthPixel(column) {#getviewcolumnwidthpixel}

Get the width in different view type.

| Parameter | Type | Description |
| --- | --- | --- |
| column | Number | The column index. |

**Returns:** Number — `Number` the column width in unit of pixels

### getViewRowHeight(row) {#getviewrowheight}

Gets the height of a specified row.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Row index. |

**Returns:** Number — `Number` Height of row.

### getViewRowHeightInch(row) {#getviewrowheightinch}

Gets the height of a specified row in unit of inches.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Row index |

**Returns:** Number — `Number` Height of row

### groupColumns(firstIndex, lastIndex) {#groupcolumns}

Groups columns.

| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | Number | The first column index to be grouped. |
| lastIndex | Number | The last column index to be grouped. |

### groupColumns(firstIndex, lastIndex, isHidden) {#groupcolumns-1}

Groups columns.

| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | Number | The first column index to be grouped. |
| lastIndex | Number | The last column index to be grouped. |
| isHidden | boolean | Specifies if the grouped columns are hidden. |

### groupRows(firstIndex, lastIndex, isHidden) {#grouprows}

Groups rows.

| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | Number | The first row index to be grouped. |
| lastIndex | Number | The last row index to be grouped. |
| isHidden | boolean | Specifies if the grouped rows are hidden. |

### groupRows(firstIndex, lastIndex) {#grouprows-1}

Groups rows.

| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | Number | The first row index to be grouped. |
| lastIndex | Number | The last row index to be grouped. |

### hideColumn(column) {#hidecolumn}

Hides a column.

| Parameter | Type | Description |
| --- | --- | --- |
| column | Number | Column index. |

### hideColumns(column, totalColumns) {#hidecolumns}

Hide multiple columns.

| Parameter | Type | Description |
| --- | --- | --- |
| column | Number | Column index. |
| totalColumns | Number | Column number. |

### hideGroupDetail(isVertical, index) {#hidegroupdetail}

Collapses the grouped rows/columns.

| Parameter | Type | Description |
| --- | --- | --- |
| isVertical | boolean | True, collapse the grouped rows. |
| index | Number | The row/column index |

### hideRow(row) {#hiderow}

Hides a row.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Row index. |

### hideRows(row, totalRows) {#hiderows}

Hides multiple rows.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | The row index. |
| totalRows | Number | The row number. |

### importCSV(fileName, splitter, convertNumericData, firstRow, firstColumn) {#importcsv}

Import a CSV file to the cells.

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | The CSV file name. |
| splitter | String | The splitter |
| convertNumericData | boolean | Whether the string in text file is converted to numeric data. |
| firstRow | Number | The row number of the first cell to import in. |
| firstColumn | Number | The column number of the first cell to import in. |

### importCSV(fileName, options, firstRow, firstColumn) {#importcsv-1}

Import a CSV file to the cells.

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | The CSV file name. |
| options | TxtLoadOptions | The load options for reading text file |
| firstRow | Number | The row number of the first cell to import in. |
| firstColumn | Number | The column number of the first cell to import in. |

### importFormulaArray(stringArray, firstRow, firstColumn, isVertical) {#importformulaarray}

Imports an array of formula into a worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| stringArray | Array of String | Formula array. |
| firstRow | Number | The row number of the first cell to import in. |
| firstColumn | Number | The column number of the first cell to import in. |
| isVertical | boolean | Specifies to import data vertically or horizontally. |

### insertColumn(columnIndex, updateReference) {#insertcolumn}

Inserts a new column into the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Number | Column index. |
| updateReference | boolean | Indicates if references in other worksheets will be updated. |

### insertColumn(columnIndex) {#insertcolumn-1}

Inserts a new column into the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Number | Column index. |

### insertColumns(columnIndex, totalColumns) {#insertcolumns}

Inserts some columns into the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Number | Column index. |
| totalColumns | Number | The number of columns. |

### insertColumns(columnIndex, totalColumns, updateReference) {#insertcolumns-1}

Inserts some columns into the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Number | Column index. |
| totalColumns | Number | The number of columns. |
| updateReference | boolean | Indicates if references in other worksheets will be updated. |

### insertColumns() {#insertcolumns-2}

### insertCutCells(cutRange, row, column, shiftType) {#insertcutcells}

Insert cut range.

| Parameter | Type | Description |
| --- | --- | --- |
| cutRange | Range | The cut range. |
| row | Number | The row. |
| column | Number | The column. |
| shiftType | Number | ShiftType |

### insertRange(area, shiftNumber, shiftType, updateReference) {#insertrange}

Inserts a range of cells and shift cells according to the shift option.

| Parameter | Type | Description |
| --- | --- | --- |
| area | CellArea | Shift area. |
| shiftNumber | Number | Number of rows or columns to be inserted. |
| shiftType | Number | ShiftType |
| updateReference | boolean | Indicates whether update references in other worksheets. |

### insertRange(area, shiftType) {#insertrange-1}

Inserts a range of cells and shift cells according to the shift option.

| Parameter | Type | Description |
| --- | --- | --- |
| area | CellArea | Shift area. |
| shiftType | Number | ShiftType |

### insertRange(area, shiftNumber, shiftType) {#insertrange-2}

Inserts a range of cells and shift cells according to the shift option.

| Parameter | Type | Description |
| --- | --- | --- |
| area | CellArea | Shift area. |
| shiftNumber | Number | Number of rows or columns to be inserted. |
| shiftType | Number | ShiftType |

### insertRow(rowIndex) {#insertrow}

Inserts a new row into the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Number | Row index. |

### insertRows(rowIndex, totalRows, updateReference) {#insertrows}

Inserts multiple rows into the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Number | Row index. |
| totalRows | Number | Number of rows to be inserted. |
| updateReference | boolean | Indicates if references in other worksheets will be updated. |

### insertRows(rowIndex, totalRows, options) {#insertrows-1}

Inserts multiple rows into the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Number | Row index. |
| totalRows | Number | Number of rows to be inserted. |
| options | InsertOptions | Indicates if references in other worksheets will be updated. |

### insertRows(rowIndex, totalRows) {#insertrows-2}

Inserts multiple rows into the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Number | Row index. |
| totalRows | Number | Number of rows to be inserted. |

### isBlankColumn(columnIndex) {#isblankcolumn}

Checks whether given column is blank(does not contain any data).

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Number | the column index |

**Returns:** boolean — `boolean` true if given column does not contain any data

### isColumnHidden(columnIndex) {#iscolumnhidden}

Checks whether a column at given index is hidden.

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Number | column index |

**Returns:** boolean — `boolean` true if the column is hidden.

### isDefaultColumnHidden() {#isdefaultcolumnhidden}

### isDefaultRowHeightMatched() {#isdefaultrowheightmatched}

Indicates that row height and default font height matches

### isDefaultRowHidden() {#isdefaultrowhidden}

Indicates whether the row is default hidden.

### isDeletingRangeEnabled(startRow, startColumn, totalRows, totalColumns) {#isdeletingrangeenabled}

Check whether the range could be deleted.

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Number | The start row index of the range. |
| startColumn | Number | The start column index of the range. |
| totalRows | Number | The number of the rows in the range. |
| totalColumns | Number | The number of the columns in the range. |

**Returns:** boolean — `boolean`

### isRowHidden(rowIndex) {#isrowhidden}

Checks whether a row at given index is hidden.

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Number | row index |

**Returns:** boolean — `boolean` true if the row is hidden

### iterator() {#iterator}

Gets the cells enumerator. When traversing elements by the returned Enumerator, the cells collection should not be modified(such as operations that will cause new Cell/Row be instantiated or existing Cell/Row be deleted). Otherwise the enumerator may not be able to traverse all cells correctly(some elements may be traversed repeatedly or skipped).@return {Iterator} The cells enumerator

### linkToXmlMap(mapName, row, column, path) {#linktoxmlmap}

Link to a xml map. e.g. A xml map element structure: -RootElement |-Attribute1 |-SubElement |-Attribute2 |-Attribute3 To link "Attribute1", path is "/RootElement/Attribute1" To link "Attribute2", path is "/RootElement/SubElement/Attribute2" To link whole "SubElement", path is "/RootElement/SubElement"

| Parameter | Type | Description |
| --- | --- | --- |
| mapName | String | name of xml map |
| row | Number | row of the destination cell |
| column | Number | column of the destination cell |
| path | String | path of xml element in xml map |

### merge(firstRow, firstColumn, totalRows, totalColumns) {#merge}

Merges a specified range of cells into a single cell. Reference the merged cell via the address of the upper-left cell in the range.

| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Number | First row of this range(zero based) |
| firstColumn | Number | First column of this range(zero based) |
| totalRows | Number | Number of rows(one based) |
| totalColumns | Number | Number of columns(one based) |

### merge(firstRow, firstColumn, totalRows, totalColumns, mergeConflict) {#merge-1}

Merges a specified range of cells into a single cell. Reference the merged cell via the address of the upper-left cell in the range. If mergeConflict is true and the merged range conflicts with other merged cells, other merged cells will be automatically removed.

| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Number | First row of this range(zero based) |
| firstColumn | Number | First column of this range(zero based) |
| totalRows | Number | Number of rows(one based) |
| totalColumns | Number | Number of columns(one based) |
| mergeConflict | boolean | Merge conflict merged ranges. |

### merge(firstRow, firstColumn, totalRows, totalColumns, checkConflict, mergeConflict) {#merge-2}

Merges a specified range of cells into a single cell. Reference the merged cell via the address of the upper-left cell in the range. If mergeConflict is true and the merged range conflicts with other merged cells, other merged cells will be automatically removed.

| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Number | First row of this range(zero based) |
| firstColumn | Number | First column of this range(zero based) |
| totalRows | Number | Number of rows(one based) |
| totalColumns | Number | Number of columns(one based) |
| checkConflict | boolean | Indicates whether check the merged cells intersects other merged cells |
| mergeConflict | boolean | Merge conflict merged ranges. |

### moveRange(sourceArea, destRow, destColumn) {#moverange}

Moves the range.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceArea | CellArea | The range which should be moved. |
| destRow | Number | The dest row. |
| destColumn | Number | The dest column. |

### removeDuplicates() {#removeduplicates}

Removes duplicate rows in the sheet.

### removeDuplicates(startRow, startColumn, endRow, endColumn) {#removeduplicates-1}

Removes duplicate values in the range.

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Number | The start row. |
| startColumn | Number | The start column |
| endRow | Number | The end row index. |
| endColumn | Number | The end column index. |

### removeDuplicates(startRow, startColumn, endRow, endColumn, hasHeaders, columnOffsets) {#removeduplicates-2}

Removes duplicate data of the range.

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Number | The start row. |
| startColumn | Number | The start column |
| endRow | Number | The end row index. |
| endColumn | Number | The end column index. |
| hasHeaders | boolean | Indicates whether the range contains headers. |
| columnOffsets | Array of Number | The column offsets. |

### removeFormulas() {#removeformulas}

Removes all formula and replaces with the value of the formula.

### retrieveSubtotalSetting(ca) {#retrievesubtotalsetting}

Retrieves subtotals setting of the range.

| Parameter | Type | Description |
| --- | --- | --- |
| ca | CellArea | The range |

**Returns:** SubtotalSetting — `SubtotalSetting`

### setColumnWidth(column, width) {#setcolumnwidth}

Sets the width of the specified column in normal view. To hide a column, sets column width to zero.

| Parameter | Type | Description |
| --- | --- | --- |
| column | Number | Column index. |
| width | Number | Width of column.Column width must be between 0 and 255. |

### setColumnWidthInch(column, inches) {#setcolumnwidthinch}

Sets column width in unit of inches in normal view.

| Parameter | Type | Description |
| --- | --- | --- |
| column | Number | Column index. |
| inches | Number | Number of inches. |

### setColumnWidthPixel(column, pixels) {#setcolumnwidthpixel}

Sets column width in unit of pixels in normal view.

| Parameter | Type | Description |
| --- | --- | --- |
| column | Number | Column index. |
| pixels | Number | Number of pixels. |

### setDefaultColumnHidden() {#setdefaultcolumnhidden}

### setDefaultRowHeightMatched() {#setdefaultrowheightmatched}

Indicates that row height and default font height matches

### setDefaultRowHidden() {#setdefaultrowhidden}

Indicates whether the row is default hidden.

### setMemorySetting() {#setmemorysetting}

Gets or sets the memory usage option for this cells. The value of the property is MemorySetting integer constant.

### setMultiThreadReading() {#setmultithreadreading}

Gets or sets whether the cells data model should support Multi-Thread reading. Default value of this property is false. If there are multiple threads to read Row/Cell objects in this collection concurrently, this property should be set as true, otherwise unexpected result may be produced. Supporting Multi-Thread reading may degrade the performance for accessing Row/Cell objects from this collection. Please note, some features cannot support Multi-Thread reading, such as formatting values(by Cell.StringValue, Cell.DisplayStringValue, .etc.). So, even with this property being set as true, those APIs still may give unexpected result for Multi-Thread reading.

### setPreserveString() {#setpreservestring}

Gets or sets a value indicating whether all worksheet values are preserved as strings. Default is false.

### setRowHeight(row, height) {#setrowheight}

Sets the height of the specified row.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Row index. |
| height | Number | Height of row.In unit of point It should be between 0 and 409.5. |

### setRowHeightInch(row, inches) {#setrowheightinch}

Sets row height in unit of inches.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Row index. |
| inches | Number | Number of inches. It should be between 0 and 409.5/72. |

### setRowHeightPixel(row, pixels) {#setrowheightpixel}

Sets row height in unit of pixels.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Row index. |
| pixels | Number | Number of pixels. |

### setStandardHeight() {#setstandardheight}

Gets or sets the default row height in this worksheet, in unit of points.

### setStandardHeightInch() {#setstandardheightinch}

Gets or sets the default row height in this worksheet, in unit of inches.

### setStandardHeightPixels() {#setstandardheightpixels}

Gets or sets the default row height in this worksheet, in unit of pixels.

### setStandardWidth() {#setstandardwidth}

Gets or sets the default column width in the worksheet, in unit of characters.

### setStandardWidthInch() {#setstandardwidthinch}

Gets or sets the default column width in the worksheet, in unit of inches.

### setStandardWidthPixels() {#setstandardwidthpixels}

Gets or sets the default column width in the worksheet, in unit of pixels.

### setStyle() {#setstyle}

Gets and sets the default style of the worksheet.

### setViewColumnWidthPixel(column, pixels) {#setviewcolumnwidthpixel}

Sets the width of the column in different view. If the current view type is ViewType.PAGE_LAYOUT_VIEW, the column's width is same as printed width.

| Parameter | Type | Description |
| --- | --- | --- |
| column | Number | The column index. |
| pixels | Number | The width in unit of pixels. |

### showGroupDetail(isVertical, index) {#showgroupdetail}

Expands the grouped rows/columns.

| Parameter | Type | Description |
| --- | --- | --- |
| isVertical | boolean | True, expands the grouped rows. |
| index | Number | The row/column index |

### subtotal(ca, groupBy, function, totalList) {#subtotal}

Creates subtotals for the range.

| Parameter | Type | Description |
| --- | --- | --- |
| ca | CellArea | The range |
| groupBy | Number | The field to group by, as a zero-based integer offset |
| function | Number | ConsolidationFunction |
| totalList | Array of Number | An array of zero-based field offsets, indicating the fields to which the subtotals are added. |

### subtotal(ca, groupBy, function, totalList, replace, pageBreaks, summaryBelowData) {#subtotal-1}

Creates subtotals for the range.

| Parameter | Type | Description |
| --- | --- | --- |
| ca | CellArea | The range |
| groupBy | Number | The field to group by, as a zero-based integer offset |
| function | Number | ConsolidationFunction |
| totalList | Array of Number | An array of zero-based field offsets, indicating the fields to which the subtotals are added. |
| replace | boolean | Indicates whether replace the current subtotals |
| pageBreaks | boolean | Indicates whether add page break between groups |
| summaryBelowData | boolean | Indicates whether add summary below data. |

### textToColumns(row, column, totalRows, options) {#texttocolumns}

Splits the text in the column to columns.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | The row index. |
| column | Number | The column index. |
| totalRows | Number | The number of rows. |
| options | TxtLoadOptions | The split options. |

### unMerge(firstRow, firstColumn, totalRows, totalColumns) {#unmerge}

Unmerges a specified range of merged cells.

| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Number | First row of this range(zero based) |
| firstColumn | Number | First column of this range(zero based) |
| totalRows | Number | Number of rows(one based) |
| totalColumns | Number | Number of columns(one based) |

### ungroupColumns(firstIndex, lastIndex) {#ungroupcolumns}

Ungroups columns.

| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | Number | The first column index to be ungrouped. |
| lastIndex | Number | The last column index to be ungrouped. |

### ungroupRows(firstIndex, lastIndex, isAll) {#ungrouprows}

Ungroups rows.

| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | Number | The first row index to be ungrouped. |
| lastIndex | Number | The last row index to be ungrouped. |
| isAll | boolean | True, removes all grouped info.Otherwise, remove the outer group info. |

### ungroupRows(firstIndex, lastIndex) {#ungrouprows-1}

Ungroups rows. Only removes outer group info.

| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | Number | The first row index to be ungrouped. |
| lastIndex | Number | The last row index to be ungrouped. |

### unhideColumn(column, width) {#unhidecolumn}

Unhides a column

| Parameter | Type | Description |
| --- | --- | --- |
| column | Number | Column index. |
| width | Number | Column width. |

### unhideColumns(column, totalColumns, width) {#unhidecolumns}

Unhide multiple columns. Only applies the column width to the hidden columns.

| Parameter | Type | Description |
| --- | --- | --- |
| column | Number | Column index. |
| totalColumns | Number | Column number |
| width | Number | Column width. |

### unhideRow(row, height) {#unhiderow}

Unhides a row.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Row index. |
| height | Number | Row height. The row's height will be changed only when the row is hidden and given height value is positive. |

### unhideRows(row, totalRows, height) {#unhiderows}

Unhides the hidden rows.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | The row index. |
| totalRows | Number | The row number. |
| height | Number | Row height. The row's height will be changed only when the row is hidden and given height value is positive. |

### importCSVFromStream(cells, stream, spliter, convertNumericData, firstRow, firstColumn, callback) (static) {#importcsvfromstream}

Import a CSV file to the cells.

| Parameter | Type | Description |
| --- | --- | --- |
| cells | Cells | The Cells object |
| stream | ReadableStream | The CSV file stream |
| spliter | String | The spliter |
| convertNumericData | boolean | Whether the string in text file is converted to numeric data |
| firstRow | Number | The row number of the first cell to import in |
| firstColumn | Number | The column number of the first cell to import in |
| callback | Callback | The callback function |

**Example:**

```js
var aspose = aspose || {};
aspose.cells = require("aspose.cells");
var fs = require("fs");
var workbook = new aspose.cells.Workbook();
var cells = workbook.getWorksheets().get(0).getCells();
var readStream = fs.createReadStream("EmployeeList.csv");
aspose.cells.Cells.importCSVFromStream(cells, readStream, ",", false, 0, 1,
function(err) {
workbook.save('result.xlsx');
}
);
```

### importCSVFromStream(cells, stream, options, firstRow, firstColumn, callback) (static) {#importcsvfromstream-1}

Import a CSV file to the cells.

| Parameter | Type | Description |
| --- | --- | --- |
| cells | Cells | The Cells object |
| stream | ReadableStream | The CSV file stream |
| options | TxtLoadOptions | The load options for reading text file |
| firstRow | Number | The row number of the first cell to import in |
| firstColumn | Number | The column number of the first cell to import in |
| callback | Callback | The callback function |

**Example:**

```js
var aspose = aspose || {};
aspose.cells = require("aspose.cells");
var fs = require("fs");
var workbook = new aspose.cells.Workbook();
var cells = workbook.getWorksheets().get(0).getCells();
var loadOptions = new aspose.cells.TxtLoadOptions();
var readStream = fs.createReadStream("EmployeeList.csv");
aspose.cells.Cells.importCSVFromStream(cells, readStream, loadOptions, 0, 1,
function(err) {
workbook.save('result.xlsx');
}
);
```
