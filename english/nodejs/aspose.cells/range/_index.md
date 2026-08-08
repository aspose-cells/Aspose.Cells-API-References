---
title: "Range"
linktitle: "Range"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Encapsulates the object that represents a range of cells within a spreadsheet."
type: docs
weight: 3130
url: /nodejs/aspose.cells/range/
---

## Range class

Encapsulates the object that represents a range of cells within a spreadsheet. The Range class denotes a region of Excel spreadsheet. With this, you can format and set value of the range. And you can simply copy range of Excel too.

## Methods

| Name | Description |
| --- | --- |
| [addHyperlink(address, textToDisplay, screenTip)](./addhyperlink/) | Adds a hyperlink to a specified cell or a range of cells. |
| [applyStyle(style, flag)](./applystyle/) | Applies formats for a whole range. Each cell in this range will contains a Style object. So this is a memory-consuming m |
| [autoFill(target)](./autofill/) | Automaticall fill the target range. |
| [autoFill(target, autoFillType)](./autofill-1/) | Automaticall fill the target range. |
| [clear()](./clear/) |  |
| [clearComments()](./clearcomments/) |  |
| [clearContents()](./clearcontents/) |  |
| [clearFormats()](./clearformats/) |  |
| [clearHyperlinks()](./clearhyperlinks/) |  |
| [copy(range, options)](./copy/) | Copying the range with paste special options. |
| [copy(range)](./copy-1/) | Copies data (including formulas), formatting, drawing objects etc. from a source range. |
| [copyData(range)](./copydata/) | Copies cell data (including formulas) from a source range. |
| [copyStyle(range)](./copystyle/) | Copies style settings from a source range. |
| [copyValue(range)](./copyvalue/) | Copies cell value from a source range. |
| [get(rowOffset, columnOffset)](./get/) | Gets Cell object in this range. |
| [getAddress()](./getaddress/) | Gets address of the range. |
| [getCellOrNull(rowOffset, columnOffset)](./getcellornull/) | Gets Cell object or null in this range. |
| [getColumnCount()](./getcolumncount/) | Gets the count of columns in the range. |
| [getColumnWidth()](./getcolumnwidth/) | Sets or gets the column width of this range |
| [getCurrentRegion()](./getcurrentregion/) | Returns a Range object that represents the current region. The current region is a range bounded by any combination of b |
| [getEntireColumn()](./getentirecolumn/) | Gets a Range object that represents the entire column (or columns) that contains the specified range. |
| [getEntireRow()](./getentirerow/) | Gets a Range object that represents the entire row (or rows) that contains the specified range. |
| [getFirstColumn()](./getfirstcolumn/) | Gets the index of the first column of the range. |
| [getFirstRow()](./getfirstrow/) | Gets the index of the first row of the range. |
| [getHeight()](./getheight/) | Gets the width of a range in points. |
| [getHyperlinks()](./gethyperlinks/) | Gets all hyperlink in the range. |
| [getLeft()](./getleft/) | Gets the distance, in points, from the left edge of column A to the left edge of the range. |
| [getName()](./getname/) | Gets or sets the name of the range. Named range is supported. For example, range.Name = "Sheet1!MyRange"; |
| [getOffset(rowOffset, columnOffset)](./getoffset/) | Gets Range range by offset. |
| [getRefersTo()](./getrefersto/) | Gets the range's refers to. |
| [getRowCount()](./getrowcount/) | Gets the count of rows in the range. |
| [getRowHeight()](./getrowheight/) | Sets or gets the height of rows in this range |
| [getTop()](./gettop/) | Gets the distance, in points, from the top edge of row 1 to the top edge of the range. |
| [getValue()](./getvalue/) | Gets and sets the value of the range. If the range contains multiple cells, the returned/applied object should be Object |
| [getWidth()](./getwidth/) | Gets the width of a range in points. |
| [getWorksheet()](./getworksheet/) | Gets the Worksheetobject which contains this range. |
| [intersect(range)](./intersect/) | Returns a Range object that represents the rectangular intersection of two ranges. If the two ranges are not intersected |
| [isBlank()](./isblank/) | Indicates whether the range contains values. |
| [isIntersect(range)](./isintersect/) | Indicates whether the range is intersect. If the two ranges area not in the same worksheet ,return false. |
| [iterator()](./iterator/) | Gets the enumerator for cells in this Range. When traversing elements by the returned Enumerator, the cells collection s |
| [merge()](./merge/) | Combines a range of cells into a single cell. Reference the merged cell via the address of the upper-left cell in the ra |
| [moveTo(destRow, destColumn)](./moveto/) | Move the current range to the dest range. |
| [putValue(stringValue, isConverted, setStyle)](./putvalue/) | Puts a value into the range, if appropriate the value will be converted to other data type and cell's number format will |
| [setColumnWidth()](./setcolumnwidth/) | Sets or gets the column width of this range |
| [setInsideBorders(borderEdge, lineStyle, borderColor)](./setinsideborders/) | Set inside borders of the range. |
| [setName()](./setname/) | Gets or sets the name of the range. Named range is supported. For example, range.Name = "Sheet1!MyRange"; |
| [setOutlineBorder(borderEdge, borderStyle, borderColor)](./setoutlineborder/) | Sets outline border around a range of cells. |
| [setOutlineBorder(borderEdge, borderStyle, borderColor)](./setoutlineborder-1/) | Sets outline border around a range of cells. |
| [setOutlineBorders(borderStyle, borderColor)](./setoutlineborders/) | Sets the outline borders around a range of cells with same border style and color. |
| [setOutlineBorders(borderStyle, borderColor)](./setoutlineborders-1/) | Sets the outline borders around a range of cells with same border style and color. |
| [setOutlineBorders(borderStyles, borderColors)](./setoutlineborders-2/) | Sets out line borders around a range of cells. Both the length of borderStyles and borderStyles must be 4. The order of  |
| [setRowHeight()](./setrowheight/) | Sets or gets the height of rows in this range |
| [setStyle(style, explicitFlag)](./setstyle/) | Apply the cell style. |
| [setStyle(style)](./setstyle-1/) | Sets the style of the range. |
| [setValue()](./setvalue/) | Gets and sets the value of the range. If the range contains multiple cells, the returned/applied object should be Object |
| [toHtml(saveOptions)](./tohtml/) | Convert the range to html . |
| [toImage(options)](./toimage/) | Converts the range to image. |
| [toJson(options)](./tojson/) | Convert the range to JSON value. |
| [toString()](./tostring/) | Returns a string represents the current Range object. |
| [transpose()](./transpose/) | Transpose (rotate) data from rows to columns or vice versa. |
| [unMerge()](./unmerge/) | Unmerges merged cells of this range. |
| [union(range)](./union/) | Returns the union of two ranges. NOTE: This method is now obsolete. Instead, please use Range.UnionRanges() method. This |
| [unionRang(range)](./unionrang/) | Returns the union result of two ranges. NOTE: This method is now obsolete. Instead, please use Range.UnionRanges() metho |
| [unionRanges(ranges)](./unionranges/) | Returns the union result of two ranges. |
