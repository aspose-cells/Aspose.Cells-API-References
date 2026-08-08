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
| [addRange(rangeObject)](./addrange/) | Adds a range object reference to cells |
| [applyColumnStyle(column, style, flag)](./applycolumnstyle/) | Applies formats for a whole column. |
| [applyRowStyle(row, style, flag)](./applyrowstyle/) | Applies formats for a whole row. |
| [applyStyle(style, flag)](./applystyle/) | Applies formats for a whole worksheet. |
| [checkCell(row, column)](./checkcell/) | Gets the Cell element or null at the specified cell row index and column index. |
| [checkColumn(columnIndex)](./checkcolumn/) | Gets the Column element or null at the specified column index. |
| [checkRow(row)](./checkrow/) | Gets the Row element or null at the specified cell row index. |
| [clear()](./clear/) | Clears all data of the worksheet. |
| [clearContents(range)](./clearcontents/) | Clears contents of a range. |
| [clearContents(startRow, startColumn, endRow, endColumn)](./clearcontents-1/) | Clears contents of a range. |
| [clearFormats(range)](./clearformats/) | Clears formatting of a range. |
| [clearFormats(startRow, startColumn, endRow, endColumn)](./clearformats-1/) | Clears formatting of a range. |
| [clearMergedCells()](./clearmergedcells/) | Clears all merged ranges. |
| [clearRange(range)](./clearrange/) | Clears contents and formatting of a range. |
| [clearRange(startRow, startColumn, endRow, endColumn)](./clearrange-1/) | Clears contents and formatting of a range. |
| [convertStringToNumericValue()](./convertstringtonumericvalue/) | Converts all string data in the worksheet to numeric value if possible. |
| [copyColumn(sourceCells, sourceColumnIndex, destinationColumnIndex)](./copycolumn/) | Copies data and formats of a whole column. |
| [copyColumns(sourceCells0, sourceColumnIndex, destinationColumnIndex, columnNumber, pasteOptions)](./copycolumns/) | Copies data and formats of a whole column. |
| [copyColumns(sourceCells0, sourceColumnIndex, destinationColumnIndex, columnNumber)](./copycolumns-1/) | Copies data and formats of a whole column. |
| [copyColumns(sourceCells, sourceColumnIndex, sourceTotalColumns, destinationColumnIndex, destinationTotalColumns)](./copycolumns-2/) | Copies data and formats of the whole columns. |
| [copyRow(sourceCells, sourceRowIndex, destinationRowIndex)](./copyrow/) | Copies data and formats of a whole row. |
| [copyRows(sourceCells, sourceRowIndex, destinationRowIndex, rowNumber)](./copyrows/) | Copies data and formats of some whole rows. |
| [copyRows(sourceCells0, sourceRowIndex, destinationRowIndex, rowNumber, copyOptions)](./copyrows-1/) | Copies data and formats of some whole rows. |
| [copyRows(sourceCells0, sourceRowIndex, destinationRowIndex, rowNumber, copyOptions, pasteOptions)](./copyrows-2/) | Copies data and formats of some whole rows. |
| [createRange(upperLeftCell, lowerRightCell)](./createrange/) | Creates a Range object from a range of cells. |
| [createRange(firstRow, firstColumn, totalRows, totalColumns)](./createrange-1/) | Creates a Range object from a range of cells. |
| [createRange(address)](./createrange-2/) | Creates a Range object from an address of the range. |
| [createRange(firstIndex, number, isVertical)](./createrange-3/) | Creates a Range object from rows of cells or columns of cells. |
| [deleteBlankColumns()](./deleteblankcolumns/) | Delete all blank columns which do not contain any data. |
| [deleteBlankColumns(options)](./deleteblankcolumns-1/) | Delete all blank columns which do not contain any data. |
| [deleteBlankRows()](./deleteblankrows/) | Delete all blank rows which do not contain any data or other object. |
| [deleteBlankRows(options)](./deleteblankrows-1/) | Delete all blank rows which do not contain any data or other object. For blank rows that will be deleted, it is not only |
| [deleteColumn(columnIndex, updateReference)](./deletecolumn/) | Deletes a column. |
| [deleteColumn(columnIndex)](./deletecolumn-1/) | Deletes a column. |
| [deleteColumns(columnIndex, totalColumns, updateReference)](./deletecolumns/) | Deletes several columns. |
| [deleteColumns()](./deletecolumns-1/) |  |
| [deleteRange(startRow, startColumn, endRow, endColumn, shiftType)](./deleterange/) | Deletes a range of cells and shift cells according to the shift option. |
| [deleteRow(rowIndex)](./deleterow/) | Deletes a row. |
| [deleteRow(rowIndex, updateReference)](./deleterow-1/) | Deletes a row. |
| [deleteRows(rowIndex, totalRows)](./deleterows/) | Deletes several rows. If the deleted range contains the top part(not whole) of the table(ListObject), the ranged could n |
| [deleteRows(rowIndex, totalRows, updateReference)](./deleterows-1/) | Deletes multiple rows in the worksheet. |
| [deleteRows()](./deleterows-2/) |  |
| [dispose()](./dispose/) | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [endCellInColumn()](./endcellincolumn/) |  |
| [endCellInColumn()](./endcellincolumn-1/) |  |
| [endCellInRow(rowIndex)](./endcellinrow/) | Gets the last cell in this row. |
| [endCellInRow(startRow, endRow, startColumn, endColumn)](./endcellinrow-1/) | Gets the last cell with maximum row index in this range. |
| [find(what, previousCell)](./find/) | Finds the cell containing with the input object. Returns null (Nothing) if no cell is found. |
| [find(what, previousCell, findOptions)](./find-1/) | Finds the cell containing with the input object. Returns null (Nothing) if no cell is found. |
| [get(row, column)](./get/) | Gets the Cell element at the specified cell row index and column index. |
| [get(cellName)](./get-1/) | Gets the Cell element at the specified cell name. |
| [getCellDisplayStyle()](./getcelldisplaystyle/) |  |
| [getCellDisplayStyle()](./getcelldisplaystyle-1/) |  |
| [getCellStyle(row, column)](./getcellstyle/) | Get the style of given cell. |
| [getCellsWithPlaceInCellPicture()](./getcellswithplaceincellpicture/) |  |
| [getColumnOriginalWidthPoint(column)](./getcolumnoriginalwidthpoint/) | Gets original column's height in unit of point if the column is hidden Width of column in normal view.NOTE: This method  |
| [getColumnWidth(column)](./getcolumnwidth/) | Gets the width(in unit of characters) of the specified column in normal view |
| [getColumnWidth(column, isOriginal, unitType)](./getcolumnwidth-1/) | Gets the column width. |
| [getColumnWidthInch(column)](./getcolumnwidthinch/) | Gets the width of the specified column in normal view, in units of inches. Width of column in normal view.NOTE: This met |
| [getColumnWidthPixel(column)](./getcolumnwidthpixel/) | Gets the width of the specified column in normal view, in units of pixel. |
| [getColumnWidthPixel(column, original)](./getcolumnwidthpixel-1/) | Gets the width of the specified column in normal view, in units of pixel. NOTE: This method is now obsolete. Instead, pl |
| [getColumns()](./getcolumns/) | Gets the collection of Column objects that represents the individual columns in this worksheet. |
| [getCount()](./getcount/) | Gets the total count of instantiated Cell objects. |
| [getCountLarge()](./getcountlarge/) | Gets the total count of instantiated Cell objects. |
| [getDependents(isAll, row, column)](./getdependents/) | Get all cells which refer to the specific cell. |
| [getDependentsInCalculation(row, column, recursive)](./getdependentsincalculation/) | Gets all cells whose calculated result depends on specific cell. To use this method, please make sure the workbook has b |
| [getFirstCell()](./getfirstcell/) | Gets the first cell in this worksheet. Returns null if there is no data in the worksheet. |
| [getFirstDataRow()](./getfirstdatarow/) |  |
| [getGroupedColumnOutlineLevel(columnIndex)](./getgroupedcolumnoutlinelevel/) | Gets the outline level (zero-based) of the column. If the column is not grouped, returns zero. |
| [getGroupedRowOutlineLevel(rowIndex)](./getgroupedrowoutlinelevel/) | Gets the outline level (zero-based) of the row. If the row is not grouped, returns zero. |
| [getLastCell()](./getlastcell/) | Gets the last cell in this worksheet. Returns null if there is no data in the worksheet. |
| [getLastDataRow(column)](./getlastdatarow/) | Gets the last row index of cell which contains data in the specified column. |
| [getMaxColumn()](./getmaxcolumn/) | Maximum column index of those cells that have been instantiated in the collection(does not include the column where styl |
| [getMaxDataColumn()](./getmaxdatacolumn/) | Maximum column index of cell which contains data. -1 will be returned if there is no cell which contains data. This prop |
| [getMaxDataRow()](./getmaxdatarow/) | Maximum row index of cell which contains data. Return -1 if there is no cell which contains data. |
| [getMaxDisplayRange()](./getmaxdisplayrange/) | Gets the max range which includes data, merged cells and shapes. Reutrns null if the worksheet is empty since Aspose.Cel |
| [getMaxGroupedColumnOutlineLevel()](./getmaxgroupedcolumnoutlinelevel/) | Gets the max grouped column outline level (zero-based). |
| [getMaxGroupedRowOutlineLevel()](./getmaxgroupedrowoutlinelevel/) | Gets the max grouped row outline level (zero-based). |
| [getMaxRow()](./getmaxrow/) | Maximum row index of cell which contains data or style. Return -1 if there is no cell which contains data or style in th |
| [getMemorySetting()](./getmemorysetting/) | Gets or sets the memory usage option for this cells. The value of the property is MemorySetting integer constant. |
| [getMergedAreas()](./getmergedareas/) | Gets all merged cells. |
| [getMergedCells()](./getmergedcells/) | Gets the collection of merged cells. In this collection, each item is a CellArea structure which represents an area of m |
| [getMinColumn()](./getmincolumn/) | Minimum column index of those cells that have been instantiated in the collection(does not include the column where styl |
| [getMinDataColumn()](./getmindatacolumn/) | Minimum column index of cell which contains data. -1 will be returned if there is no cell which contains data. This prop |
| [getMinDataRow()](./getmindatarow/) | Minimum row index of cell which contains data. |
| [getMinRow()](./getminrow/) | Minimum row index of cell which contains data or style. |
| [getMultiThreadReading()](./getmultithreadreading/) | Gets or sets whether the cells data model should support Multi-Thread reading. Default value of this property is false.  |
| [getOdsCellFields()](./getodscellfields/) | Gets the list of fields of ods. |
| [getPreserveString()](./getpreservestring/) | Gets or sets a value indicating whether all worksheet values are preserved as strings. Default is false. |
| [getRanges()](./getranges/) | Gets the collection of Range objects created at run time. |
| [getRowEnumerator()](./getrowenumerator/) | Gets the rows enumerator. NOTE: This member is now obsolete. Instead, please use RowCollection.GetEnumerator() method. T |
| [getRowHeight(row, isOriginal, unitType)](./getrowheight/) | Gets row's height. |
| [getRowHeight(row)](./getrowheight-1/) | Gets the height of a specified row, in unit of points. |
| [getRowHeightInch(row)](./getrowheightinch/) | Gets the height of a specified row in unit of inches. |
| [getRowHeightPixel(row)](./getrowheightpixel/) | Gets the height of a specified row in unit of pixel. |
| [getRowOriginalHeightPoint(row)](./getroworiginalheightpoint/) | Gets original row's height in unit of point if the row is hidden NOTE: This member is now obsolete. Instead, please use  |
| [getRows()](./getrows/) | Gets the collection of Row objects that represents the individual rows in this worksheet. |
| [getStandardHeight()](./getstandardheight/) | Gets or sets the default row height in this worksheet, in unit of points. |
| [getStandardHeightInch()](./getstandardheightinch/) | Gets or sets the default row height in this worksheet, in unit of inches. |
| [getStandardHeightPixels()](./getstandardheightpixels/) | Gets or sets the default row height in this worksheet, in unit of pixels. |
| [getStandardWidth()](./getstandardwidth/) | Gets or sets the default column width in the worksheet, in unit of characters. |
| [getStandardWidthInch()](./getstandardwidthinch/) | Gets or sets the default column width in the worksheet, in unit of inches. |
| [getStandardWidthPixels()](./getstandardwidthpixels/) | Gets or sets the default column width in the worksheet, in unit of pixels. |
| [getStyle()](./getstyle/) | Gets and sets the default style of the worksheet. |
| [getViewColumnWidthPixel(column)](./getviewcolumnwidthpixel/) | Get the width in different view type. |
| [getViewRowHeight(row)](./getviewrowheight/) | Gets the height of a specified row. |
| [getViewRowHeightInch(row)](./getviewrowheightinch/) | Gets the height of a specified row in unit of inches. |
| [groupColumns(firstIndex, lastIndex)](./groupcolumns/) | Groups columns. |
| [groupColumns(firstIndex, lastIndex, isHidden)](./groupcolumns-1/) | Groups columns. |
| [groupRows(firstIndex, lastIndex, isHidden)](./grouprows/) | Groups rows. |
| [groupRows(firstIndex, lastIndex)](./grouprows-1/) | Groups rows. |
| [hideColumn(column)](./hidecolumn/) | Hides a column. |
| [hideColumns(column, totalColumns)](./hidecolumns/) | Hide multiple columns. |
| [hideGroupDetail(isVertical, index)](./hidegroupdetail/) | Collapses the grouped rows/columns. |
| [hideRow(row)](./hiderow/) | Hides a row. |
| [hideRows(row, totalRows)](./hiderows/) | Hides multiple rows. |
| [importCSV(fileName, splitter, convertNumericData, firstRow, firstColumn)](./importcsv/) | Import a CSV file to the cells. |
| [importCSV(fileName, options, firstRow, firstColumn)](./importcsv-1/) | Import a CSV file to the cells. |
| [importFormulaArray(stringArray, firstRow, firstColumn, isVertical)](./importformulaarray/) | Imports an array of formula into a worksheet. |
| [insertColumn(columnIndex, updateReference)](./insertcolumn/) | Inserts a new column into the worksheet. |
| [insertColumn(columnIndex)](./insertcolumn-1/) | Inserts a new column into the worksheet. |
| [insertColumns(columnIndex, totalColumns)](./insertcolumns/) | Inserts some columns into the worksheet. |
| [insertColumns(columnIndex, totalColumns, updateReference)](./insertcolumns-1/) | Inserts some columns into the worksheet. |
| [insertColumns()](./insertcolumns-2/) |  |
| [insertCutCells(cutRange, row, column, shiftType)](./insertcutcells/) | Insert cut range. |
| [insertRange(area, shiftNumber, shiftType, updateReference)](./insertrange/) | Inserts a range of cells and shift cells according to the shift option. |
| [insertRange(area, shiftType)](./insertrange-1/) | Inserts a range of cells and shift cells according to the shift option. |
| [insertRange(area, shiftNumber, shiftType)](./insertrange-2/) | Inserts a range of cells and shift cells according to the shift option. |
| [insertRow(rowIndex)](./insertrow/) | Inserts a new row into the worksheet. |
| [insertRows(rowIndex, totalRows, updateReference)](./insertrows/) | Inserts multiple rows into the worksheet. |
| [insertRows(rowIndex, totalRows, options)](./insertrows-1/) | Inserts multiple rows into the worksheet. |
| [insertRows(rowIndex, totalRows)](./insertrows-2/) | Inserts multiple rows into the worksheet. |
| [isBlankColumn(columnIndex)](./isblankcolumn/) | Checks whether given column is blank(does not contain any data). |
| [isColumnHidden(columnIndex)](./iscolumnhidden/) | Checks whether a column at given index is hidden. |
| [isDefaultColumnHidden()](./isdefaultcolumnhidden/) |  |
| [isDefaultRowHeightMatched()](./isdefaultrowheightmatched/) | Indicates that row height and default font height matches |
| [isDefaultRowHidden()](./isdefaultrowhidden/) | Indicates whether the row is default hidden. |
| [isDeletingRangeEnabled(startRow, startColumn, totalRows, totalColumns)](./isdeletingrangeenabled/) | Check whether the range could be deleted. |
| [isRowHidden(rowIndex)](./isrowhidden/) | Checks whether a row at given index is hidden. |
| [iterator()](./iterator/) | Gets the cells enumerator. When traversing elements by the returned Enumerator, the cells collection should not be modif |
| [linkToXmlMap(mapName, row, column, path)](./linktoxmlmap/) | Link to a xml map. e.g. A xml map element structure: -RootElement \|-Attribute1 \|-SubElement \|-Attribute2 \|-Attribute3 To |
| [merge(firstRow, firstColumn, totalRows, totalColumns)](./merge/) | Merges a specified range of cells into a single cell. Reference the merged cell via the address of the upper-left cell i |
| [merge(firstRow, firstColumn, totalRows, totalColumns, mergeConflict)](./merge-1/) | Merges a specified range of cells into a single cell. Reference the merged cell via the address of the upper-left cell i |
| [merge(firstRow, firstColumn, totalRows, totalColumns, checkConflict, mergeConflict)](./merge-2/) | Merges a specified range of cells into a single cell. Reference the merged cell via the address of the upper-left cell i |
| [moveRange(sourceArea, destRow, destColumn)](./moverange/) | Moves the range. |
| [removeDuplicates()](./removeduplicates/) | Removes duplicate rows in the sheet. |
| [removeDuplicates(startRow, startColumn, endRow, endColumn)](./removeduplicates-1/) | Removes duplicate values in the range. |
| [removeDuplicates(startRow, startColumn, endRow, endColumn, hasHeaders, columnOffsets)](./removeduplicates-2/) | Removes duplicate data of the range. |
| [removeFormulas()](./removeformulas/) | Removes all formula and replaces with the value of the formula. |
| [retrieveSubtotalSetting(ca)](./retrievesubtotalsetting/) | Retrieves subtotals setting of the range. |
| [setColumnWidth(column, width)](./setcolumnwidth/) | Sets the width of the specified column in normal view. To hide a column, sets column width to zero. |
| [setColumnWidthInch(column, inches)](./setcolumnwidthinch/) | Sets column width in unit of inches in normal view. |
| [setColumnWidthPixel(column, pixels)](./setcolumnwidthpixel/) | Sets column width in unit of pixels in normal view. |
| [setDefaultColumnHidden()](./setdefaultcolumnhidden/) |  |
| [setDefaultRowHeightMatched()](./setdefaultrowheightmatched/) | Indicates that row height and default font height matches |
| [setDefaultRowHidden()](./setdefaultrowhidden/) | Indicates whether the row is default hidden. |
| [setMemorySetting()](./setmemorysetting/) | Gets or sets the memory usage option for this cells. The value of the property is MemorySetting integer constant. |
| [setMultiThreadReading()](./setmultithreadreading/) | Gets or sets whether the cells data model should support Multi-Thread reading. Default value of this property is false.  |
| [setPreserveString()](./setpreservestring/) | Gets or sets a value indicating whether all worksheet values are preserved as strings. Default is false. |
| [setRowHeight(row, height)](./setrowheight/) | Sets the height of the specified row. |
| [setRowHeightInch(row, inches)](./setrowheightinch/) | Sets row height in unit of inches. |
| [setRowHeightPixel(row, pixels)](./setrowheightpixel/) | Sets row height in unit of pixels. |
| [setStandardHeight()](./setstandardheight/) | Gets or sets the default row height in this worksheet, in unit of points. |
| [setStandardHeightInch()](./setstandardheightinch/) | Gets or sets the default row height in this worksheet, in unit of inches. |
| [setStandardHeightPixels()](./setstandardheightpixels/) | Gets or sets the default row height in this worksheet, in unit of pixels. |
| [setStandardWidth()](./setstandardwidth/) | Gets or sets the default column width in the worksheet, in unit of characters. |
| [setStandardWidthInch()](./setstandardwidthinch/) | Gets or sets the default column width in the worksheet, in unit of inches. |
| [setStandardWidthPixels()](./setstandardwidthpixels/) | Gets or sets the default column width in the worksheet, in unit of pixels. |
| [setStyle()](./setstyle/) | Gets and sets the default style of the worksheet. |
| [setViewColumnWidthPixel(column, pixels)](./setviewcolumnwidthpixel/) | Sets the width of the column in different view. If the current view type is ViewType.PAGE_LAYOUT_VIEW, the column's widt |
| [showGroupDetail(isVertical, index)](./showgroupdetail/) | Expands the grouped rows/columns. |
| [subtotal(ca, groupBy, function, totalList)](./subtotal/) | Creates subtotals for the range. |
| [subtotal(ca, groupBy, function, totalList, replace, pageBreaks, summaryBelowData)](./subtotal-1/) | Creates subtotals for the range. |
| [textToColumns(row, column, totalRows, options)](./texttocolumns/) | Splits the text in the column to columns. |
| [unMerge(firstRow, firstColumn, totalRows, totalColumns)](./unmerge/) | Unmerges a specified range of merged cells. |
| [ungroupColumns(firstIndex, lastIndex)](./ungroupcolumns/) | Ungroups columns. |
| [ungroupRows(firstIndex, lastIndex, isAll)](./ungrouprows/) | Ungroups rows. |
| [ungroupRows(firstIndex, lastIndex)](./ungrouprows-1/) | Ungroups rows. Only removes outer group info. |
| [unhideColumn(column, width)](./unhidecolumn/) | Unhides a column |
| [unhideColumns(column, totalColumns, width)](./unhidecolumns/) | Unhide multiple columns. Only applies the column width to the hidden columns. |
| [unhideRow(row, height)](./unhiderow/) | Unhides a row. |
| [unhideRows(row, totalRows, height)](./unhiderows/) | Unhides the hidden rows. |
| [importCSVFromStream(cells, stream, spliter, convertNumericData, firstRow, firstColumn, callback)](./importcsvfromstream/) *(static)* | Import a CSV file to the cells. |
| [importCSVFromStream(cells, stream, options, firstRow, firstColumn, callback)](./importcsvfromstream-1/) *(static)* | Import a CSV file to the cells. |
