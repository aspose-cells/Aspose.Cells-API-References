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
| [addHyperlink(address, textToDisplay, screenTip)](#addhyperlink) | Adds a hyperlink to a specified cell or a range of cells. |
| [applyStyle(style, flag)](#applystyle) | Applies formats for a whole range. Each cell in this range will contains a Style object. So this is a memory-consuming m |
| [autoFill(target)](#autofill) | Automaticall fill the target range. |
| [autoFill(target, autoFillType)](#autofill-1) | Automaticall fill the target range. |
| [clear()](#clear) |  |
| [clearComments()](#clearcomments) |  |
| [clearContents()](#clearcontents) |  |
| [clearFormats()](#clearformats) |  |
| [clearHyperlinks()](#clearhyperlinks) |  |
| [copy(range, options)](#copy) | Copying the range with paste special options. |
| [copy(range)](#copy-1) | Copies data (including formulas), formatting, drawing objects etc. from a source range. |
| [copyData(range)](#copydata) | Copies cell data (including formulas) from a source range. |
| [copyStyle(range)](#copystyle) | Copies style settings from a source range. |
| [copyValue(range)](#copyvalue) | Copies cell value from a source range. |
| [get(rowOffset, columnOffset)](#get) | Gets Cell object in this range. |
| [getAddress()](#getaddress) | Gets address of the range. |
| [getCellOrNull(rowOffset, columnOffset)](#getcellornull) | Gets Cell object or null in this range. |
| [getColumnCount()](#getcolumncount) | Gets the count of columns in the range. |
| [getColumnWidth()](#getcolumnwidth) | Sets or gets the column width of this range |
| [getCurrentRegion()](#getcurrentregion) | Returns a Range object that represents the current region. The current region is a range bounded by any combination of b |
| [getEntireColumn()](#getentirecolumn) | Gets a Range object that represents the entire column (or columns) that contains the specified range. |
| [getEntireRow()](#getentirerow) | Gets a Range object that represents the entire row (or rows) that contains the specified range. |
| [getFirstColumn()](#getfirstcolumn) | Gets the index of the first column of the range. |
| [getFirstRow()](#getfirstrow) | Gets the index of the first row of the range. |
| [getHeight()](#getheight) | Gets the width of a range in points. |
| [getHyperlinks()](#gethyperlinks) | Gets all hyperlink in the range. |
| [getLeft()](#getleft) | Gets the distance, in points, from the left edge of column A to the left edge of the range. |
| [getName()](#getname) | Gets or sets the name of the range. Named range is supported. For example, range.Name = "Sheet1!MyRange"; |
| [getOffset(rowOffset, columnOffset)](#getoffset) | Gets Range range by offset. |
| [getRefersTo()](#getrefersto) | Gets the range's refers to. |
| [getRowCount()](#getrowcount) | Gets the count of rows in the range. |
| [getRowHeight()](#getrowheight) | Sets or gets the height of rows in this range |
| [getTop()](#gettop) | Gets the distance, in points, from the top edge of row 1 to the top edge of the range. |
| [getValue()](#getvalue) | Gets and sets the value of the range. If the range contains multiple cells, the returned/applied object should be Object |
| [getWidth()](#getwidth) | Gets the width of a range in points. |
| [getWorksheet()](#getworksheet) | Gets the Worksheetobject which contains this range. |
| [intersect(range)](#intersect) | Returns a Range object that represents the rectangular intersection of two ranges. If the two ranges are not intersected |
| [isBlank()](#isblank) | Indicates whether the range contains values. |
| [isIntersect(range)](#isintersect) | Indicates whether the range is intersect. If the two ranges area not in the same worksheet ,return false. |
| [iterator()](#iterator) | Gets the enumerator for cells in this Range. When traversing elements by the returned Enumerator, the cells collection s |
| [merge()](#merge) | Combines a range of cells into a single cell. Reference the merged cell via the address of the upper-left cell in the ra |
| [moveTo(destRow, destColumn)](#moveto) | Move the current range to the dest range. |
| [putValue(stringValue, isConverted, setStyle)](#putvalue) | Puts a value into the range, if appropriate the value will be converted to other data type and cell's number format will |
| [setColumnWidth()](#setcolumnwidth) | Sets or gets the column width of this range |
| [setInsideBorders(borderEdge, lineStyle, borderColor)](#setinsideborders) | Set inside borders of the range. |
| [setName()](#setname) | Gets or sets the name of the range. Named range is supported. For example, range.Name = "Sheet1!MyRange"; |
| [setOutlineBorder(borderEdge, borderStyle, borderColor)](#setoutlineborder) | Sets outline border around a range of cells. |
| [setOutlineBorder(borderEdge, borderStyle, borderColor)](#setoutlineborder-1) | Sets outline border around a range of cells. |
| [setOutlineBorders(borderStyle, borderColor)](#setoutlineborders) | Sets the outline borders around a range of cells with same border style and color. |
| [setOutlineBorders(borderStyle, borderColor)](#setoutlineborders-1) | Sets the outline borders around a range of cells with same border style and color. |
| [setOutlineBorders(borderStyles, borderColors)](#setoutlineborders-2) | Sets out line borders around a range of cells. Both the length of borderStyles and borderStyles must be 4. The order of  |
| [setRowHeight()](#setrowheight) | Sets or gets the height of rows in this range |
| [setStyle(style, explicitFlag)](#setstyle) | Apply the cell style. |
| [setStyle(style)](#setstyle-1) | Sets the style of the range. |
| [setValue()](#setvalue) | Gets and sets the value of the range. If the range contains multiple cells, the returned/applied object should be Object |
| [toHtml(saveOptions)](#tohtml) | Convert the range to html . |
| [toImage(options)](#toimage) | Converts the range to image. |
| [toJson(options)](#tojson) | Convert the range to JSON value. |
| [toString()](#tostring) | Returns a string represents the current Range object. |
| [transpose()](#transpose) | Transpose (rotate) data from rows to columns or vice versa. |
| [unMerge()](#unmerge) | Unmerges merged cells of this range. |
| [union(range)](#union) | Returns the union of two ranges. NOTE: This method is now obsolete. Instead, please use Range.UnionRanges() method. This |
| [unionRang(range)](#unionrang) | Returns the union result of two ranges. NOTE: This method is now obsolete. Instead, please use Range.UnionRanges() metho |
| [unionRanges(ranges)](#unionranges) | Returns the union result of two ranges. |

### addHyperlink(address, textToDisplay, screenTip) {#addhyperlink}

Adds a hyperlink to a specified cell or a range of cells.

| Parameter | Type | Description |
| --- | --- | --- |
| address | String | Address of the hyperlink. |
| textToDisplay | String | The text to be displayed for the specified hyperlink. |
| screenTip | String | The screenTip text for the specified hyperlink. |

**Returns:** Hyperlink — `Hyperlink` Hyperlink object.

### applyStyle(style, flag) {#applystyle}

Applies formats for a whole range. Each cell in this range will contains a Style object. So this is a memory-consuming method. Please use it carefully.

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The style object which will be applied. |
| flag | StyleFlag | Flags which indicates applied formatting properties. |

### autoFill(target) {#autofill}

Automaticall fill the target range.

| Parameter | Type | Description |
| --- | --- | --- |
| target | Range | the target range. |

### autoFill(target, autoFillType) {#autofill-1}

Automaticall fill the target range.

| Parameter | Type | Description |
| --- | --- | --- |
| target | Range | The targed range. |
| autoFillType | Number | AutoFillType |

### clear() {#clear}

### clearComments() {#clearcomments}

### clearContents() {#clearcontents}

### clearFormats() {#clearformats}

### clearHyperlinks() {#clearhyperlinks}

### copy(range, options) {#copy}

Copying the range with paste special options.

| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | The source range. |
| options | PasteOptions | The paste special options. |

### copy(range) {#copy-1}

Copies data (including formulas), formatting, drawing objects etc. from a source range.

| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | Source |

### copyData(range) {#copydata}

Copies cell data (including formulas) from a source range.

| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | Source |

### copyStyle(range) {#copystyle}

Copies style settings from a source range.

| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | Source |

### copyValue(range) {#copyvalue}

Copies cell value from a source range.

| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | Source |

### get(rowOffset, columnOffset) {#get}

Gets Cell object in this range.

| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | Number | Row offset in this range, zero based. |
| columnOffset | Number | Column offset in this range, zero based. |

**Returns:** Cell — `Cell` Cell object.

### getAddress() {#getaddress}

Gets address of the range.

### getCellOrNull(rowOffset, columnOffset) {#getcellornull}

Gets Cell object or null in this range.

| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | Number | Row offset in this range, zero based. |
| columnOffset | Number | Column offset in this range, zero based. |

**Returns:** Cell — `Cell` Cell object.

### getColumnCount() {#getcolumncount}

Gets the count of columns in the range.

### getColumnWidth() {#getcolumnwidth}

Sets or gets the column width of this range

### getCurrentRegion() {#getcurrentregion}

Returns a Range object that represents the current region. The current region is a range bounded by any combination of blank rows and blank columns.

### getEntireColumn() {#getentirecolumn}

Gets a Range object that represents the entire column (or columns) that contains the specified range.

### getEntireRow() {#getentirerow}

Gets a Range object that represents the entire row (or rows) that contains the specified range.

### getFirstColumn() {#getfirstcolumn}

Gets the index of the first column of the range.

### getFirstRow() {#getfirstrow}

Gets the index of the first row of the range.

### getHeight() {#getheight}

Gets the width of a range in points.

### getHyperlinks() {#gethyperlinks}

Gets all hyperlink in the range.

### getLeft() {#getleft}

Gets the distance, in points, from the left edge of column A to the left edge of the range.

### getName() {#getname}

Gets or sets the name of the range. Named range is supported. For example, range.Name = "Sheet1!MyRange";

### getOffset(rowOffset, columnOffset) {#getoffset}

Gets Range range by offset.

| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | Number | Row offset in this range, zero based. |
| columnOffset | Number | Column offset in this range, zero based. |

**Returns:** Range — `Range`

### getRefersTo() {#getrefersto}

Gets the range's refers to.

### getRowCount() {#getrowcount}

Gets the count of rows in the range.

### getRowHeight() {#getrowheight}

Sets or gets the height of rows in this range

### getTop() {#gettop}

Gets the distance, in points, from the top edge of row 1 to the top edge of the range.

### getValue() {#getvalue}

Gets and sets the value of the range. If the range contains multiple cells, the returned/applied object should be Object[][].

### getWidth() {#getwidth}

Gets the width of a range in points.

### getWorksheet() {#getworksheet}

Gets the Worksheetobject which contains this range.

### intersect(range) {#intersect}

Returns a Range object that represents the rectangular intersection of two ranges. If the two ranges are not intersected, returns null.

| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | The intersecting range. |

**Returns:** Range — `Range` Returns a Range object

### isBlank() {#isblank}

Indicates whether the range contains values.

**Returns:** boolean — `boolean`

### isIntersect(range) {#isintersect}

Indicates whether the range is intersect. If the two ranges area not in the same worksheet ,return false.

| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | The range. |

**Returns:** boolean — `boolean` Whether the range is intersect.

### iterator() {#iterator}

Gets the enumerator for cells in this Range. When traversing elements by the returned Enumerator, the cells collection should not be modified(such as operations that will cause new Cell/Row be instantiated or existing Cell/Row be deleted). Otherwise the enumerator may not be able to traverse all cells correctly(some elements may be traversed repeatedly or skipped).@return {Iterator} The cells enumerator

### merge() {#merge}

Combines a range of cells into a single cell. Reference the merged cell via the address of the upper-left cell in the range.

### moveTo(destRow, destColumn) {#moveto}

Move the current range to the dest range.

| Parameter | Type | Description |
| --- | --- | --- |
| destRow | Number | The start row of the dest range. |
| destColumn | Number | The start column of the dest range. |

### putValue(stringValue, isConverted, setStyle) {#putvalue}

Puts a value into the range, if appropriate the value will be converted to other data type and cell's number format will be reset.

| Parameter | Type | Description |
| --- | --- | --- |
| stringValue | String | Input value |
| isConverted | boolean | True: converted to other data type if appropriate. |
| setStyle | boolean | True: set the number format to cell's style when converting to other data type |

### setColumnWidth() {#setcolumnwidth}

Sets or gets the column width of this range

### setInsideBorders(borderEdge, lineStyle, borderColor) {#setinsideborders}

Set inside borders of the range.

| Parameter | Type | Description |
| --- | --- | --- |
| borderEdge | Number | BorderType |
| lineStyle | Number | CellBorderType |
| borderColor | CellsColor | The color of the border. |

### setName() {#setname}

Gets or sets the name of the range. Named range is supported. For example, range.Name = "Sheet1!MyRange";

### setOutlineBorder(borderEdge, borderStyle, borderColor) {#setoutlineborder}

Sets outline border around a range of cells.

| Parameter | Type | Description |
| --- | --- | --- |
| borderEdge | Number | BorderType |
| borderStyle | Number | CellBorderType |
| borderColor | CellsColor | Border color. |

### setOutlineBorder(borderEdge, borderStyle, borderColor) {#setoutlineborder-1}

Sets outline border around a range of cells.

| Parameter | Type | Description |
| --- | --- | --- |
| borderEdge | Number | BorderType |
| borderStyle | Number | CellBorderType |
| borderColor | Color | Border color. |

### setOutlineBorders(borderStyle, borderColor) {#setoutlineborders}

Sets the outline borders around a range of cells with same border style and color.

| Parameter | Type | Description |
| --- | --- | --- |
| borderStyle | Number | CellBorderType |
| borderColor | CellsColor | Border color. |

### setOutlineBorders(borderStyle, borderColor) {#setoutlineborders-1}

Sets the outline borders around a range of cells with same border style and color.

| Parameter | Type | Description |
| --- | --- | --- |
| borderStyle | Number | CellBorderType |
| borderColor | Color | Border color. |

### setOutlineBorders(borderStyles, borderColors) {#setoutlineborders-2}

Sets out line borders around a range of cells. Both the length of borderStyles and borderStyles must be 4. The order of borderStyles and borderStyles must be top,bottom,left,right

| Parameter | Type | Description |
| --- | --- | --- |
| borderStyles | Array of Number | Border styles. |
| borderColors | Array ofColor | Border colors. |

### setRowHeight() {#setrowheight}

Sets or gets the height of rows in this range

### setStyle(style, explicitFlag) {#setstyle}

Apply the cell style.

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The cell style. |
| explicitFlag | boolean | True, only overwriting formatting which is explicitly set. |

### setStyle(style) {#setstyle-1}

Sets the style of the range.

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The Style object. |

### setValue() {#setvalue}

Gets and sets the value of the range. If the range contains multiple cells, the returned/applied object should be Object[][].

### toHtml(saveOptions) {#tohtml}

Convert the range to html .

| Parameter | Type | Description |
| --- | --- | --- |
| saveOptions | HtmlSaveOptions | Options for coverting range to html. |

**Returns:** Array of byte — `Array of byte`

### toImage(options) {#toimage}

Converts the range to image.

| Parameter | Type | Description |
| --- | --- | --- |
| options | ImageOrPrintOptions | The options for converting this range to image |

**Returns:** Array of byte — `Array of byte`

### toJson(options) {#tojson}

Convert the range to JSON value.

| Parameter | Type | Description |
| --- | --- | --- |
| options | JsonSaveOptions | The options of converting |

**Returns:** String — `String`

### toString() {#tostring}

Returns a string represents the current Range object.

**Returns:** String — `String`

### transpose() {#transpose}

Transpose (rotate) data from rows to columns or vice versa.

### unMerge() {#unmerge}

Unmerges merged cells of this range.

### union(range) {#union}

Returns the union of two ranges. NOTE: This method is now obsolete. Instead, please use Range.UnionRanges() method. This method will be removed 12 months later since November 2023. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | The range |

**Returns:** ArrayList — `ArrayList` The union of two ranges.

### unionRang(range) {#unionrang}

Returns the union result of two ranges. NOTE: This method is now obsolete. Instead, please use Range.UnionRanges() method. This method will be removed 12 months later since May 2024. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | The range |

**Returns:** Array ofRange — `Array ofRange` The union of two ranges.

### unionRanges(ranges) {#unionranges}

Returns the union result of two ranges.

| Parameter | Type | Description |
| --- | --- | --- |
| ranges | Array ofRange | The range |

**Returns:** UnionRange — `UnionRange` The union of two ranges.
