---
title: "Range Class"
linktitle: "Range"
articleTitle: "Range"
second_title: "Aspose.Cells for Python via Java"
description: "Encapsulates the object that represents a range of cells within a spreadsheet."
type: docs
weight: 5270
url: /python-java/asposecells.api/range/
---

## Range class

Encapsulates the object that represents a range of cells within a spreadsheet.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [CurrentRegion](#currentregion) | Range | Returns a Range object that represents the current region. The current region is a range bounded by any combination of b |
| [Hyperlinks](#hyperlinks) | Hyperlink[] | Gets all hyperlink in the range. |
| [RowCount](#rowcount) | int | Gets the count of rows in the range. |
| [ColumnCount](#columncount) | int | Gets the count of columns in the range. |
| [Name](#name) | String | Gets or sets the name of the range. Named range is supported. For example, range.Name = "Sheet1!MyRange"; |
| [RefersTo](#refersto) | String | Gets the range's refers to. |
| [Address](#address) | String | Gets address of the range. |
| [Left](#left) | float | Gets the distance, in points, from the left edge of column A to the left edge of the range. |
| [Top](#top) | float | Gets the distance, in points, from the top edge of row 1 to the top edge of the range. |
| [Width](#width) | float | Gets the width of a range in points. |
| [Height](#height) | float | Gets the width of a range in points. |
| [FirstRow](#firstrow) | int | Gets the index of the first row of the range. |
| [FirstColumn](#firstcolumn) | int | Gets the index of the first column of the range. |
| [Value](#value) | Object | Gets and sets the value of the range. If the range contains multiple cells, the returned/applied object should be Object |
| [ColumnWidth](#columnwidth) | float | Sets or gets the column width of this range |
| [RowHeight](#rowheight) | float | Sets or gets the height of rows in this range |
| [EntireColumn](#entirecolumn) | Range | Gets a Range object that represents the entire column (or columns) that contains the specified range. |
| [EntireRow](#entirerow) | Range | Gets a Range object that represents the entire row (or rows) that contains the specified range. |
| [Worksheet](#worksheet) | Worksheet | Gets the Worksheet object which contains this range. |
| [Item (int, int)](#itemintint) | Cell | Gets Cell object in this range. |

## Methods

| Name | Description |
| --- | --- |
| [autoFill](#autofill) | Automaticall fill the target range. |
| [addHyperlink](#addhyperlink) | Adds a hyperlink to a specified cell or a range of cells. |
| [iterator](#iterator) | Gets the enumerator for cells in this Range.

When traversing elements by the returned Enumerator, the cells collection  |
| [isIntersect](#isintersect) | Indicates whether the range is intersect.

If the two ranges area not in the same worksheet ,return false. |
| [intersect](#intersect) | Returns a Range object that represents the rectangular intersection of two ranges.

If the two ranges are not intersecte |
| [unionRang](#unionrang) | Returns the union result of two ranges.

NOTE: This method is now obsolete. Instead, please use Range.UnionRanges() meth |
| [unionRanges](#unionranges) | Returns the union result of two ranges. |
| [union](#union) | Returns the union of two ranges.

NOTE: This method is now obsolete. Instead, please use Range.UnionRanges() method. Thi |
| [isBlank](#isblank) | Indicates whether the range contains values. |
| [merge](#merge) | Combines a range of cells into a single cell.

Reference the merged cell via the address of the upper-left cell in the r |
| [unMerge](#unmerge) | Unmerges merged cells of this range. |
| [putValue](#putvalue) | Puts a value into the range, if appropriate the value will be converted to other data type and cell's number format will |
| [setStyle](#setstyle) | Apply the cell style. |
| [applyStyle](#applystyle) | Applies formats for a whole range.

Each cell in this range will contains a Style object. So this is a memory-consuming  |
| [setOutlineBorders](#setoutlineborders) | Sets the outline borders around a range of cells with same border style and color. |
| [setOutlineBorder](#setoutlineborder) | Sets outline border around a range of cells. |
| [setInsideBorders](#setinsideborders) | Set inside borders of the range. |
| [moveTo](#moveto) | Move the current range to the dest range. |
| [copyData](#copydata) | Copies cell data (including formulas) from a source range. |
| [copyValue](#copyvalue) | Copies cell value from a source range. |
| [copyStyle](#copystyle) | Copies style settings from a source range. |
| [copy](#copy) | Copying the range with paste special options. |
| [transpose](#transpose) | Transpose (rotate) data from rows to columns or vice versa. |
| [getCellOrNull](#getcellornull) | Gets Cell object or null in this range. |
| [getOffset](#getoffset) | Gets Range range by offset. |
| [toString](#tostring) | Returns a string represents the current Range object. |
| [toImage](#toimage) | Converts the range to image. |
| [toJson](#tojson) | Convert the range to JSON value. |
| [toHtml](#tohtml) | Convert the range to html . |
| [clear](#clear) |  |
| [clearContents](#clearcontents) |  |
| [clearFormats](#clearformats) |  |
| [clearComments](#clearcomments) |  |
| [clearHyperlinks](#clearhyperlinks) |  |

### Range.CurrentRegion property {#currentregion}

Returns a Range object that represents the current region. The current region is a range bounded by any combination of blank rows and blank columns.

**Type:** Range

### Range.Hyperlinks property {#hyperlinks}

Gets all hyperlink in the range.

**Type:** Hyperlink[]

### Range.RowCount property {#rowcount}

Gets the count of rows in the range.

**Type:** int

### Range.ColumnCount property {#columncount}

Gets the count of columns in the range.

**Type:** int

### Range.Name property {#name}

Gets or sets the name of the range. Named range is supported. For example, range.Name = "Sheet1!MyRange";

**Type:** String

### Range.RefersTo property {#refersto}

Gets the range's refers to.

**Type:** String

### Range.Address property {#address}

Gets address of the range.

**Type:** String

### Range.Left property {#left}

Gets the distance, in points, from the left edge of column A to the left edge of the range.

**Type:** float

### Range.Top property {#top}

Gets the distance, in points, from the top edge of row 1 to the top edge of the range.

**Type:** float

### Range.Width property {#width}

Gets the width of a range in points.

**Type:** float

### Range.Height property {#height}

Gets the width of a range in points.

**Type:** float

### Range.FirstRow property {#firstrow}

Gets the index of the first row of the range.

**Type:** int

### Range.FirstColumn property {#firstcolumn}

Gets the index of the first column of the range.

**Type:** int

### Range.Value property {#value}

Gets and sets the value of the range. If the range contains multiple cells, the returned/applied object should be Object[][].

**Type:** Object

### Range.ColumnWidth property {#columnwidth}

Sets or gets the column width of this range

**Type:** float

### Range.RowHeight property {#rowheight}

Sets or gets the height of rows in this range

**Type:** float

### Range.EntireColumn property {#entirecolumn}

Gets a Range object that represents the entire column (or columns) that contains the specified range.

**Type:** Range

### Range.EntireRow property {#entirerow}

Gets a Range object that represents the entire row (or rows) that contains the specified range.

**Type:** Range

### Range.Worksheet property {#worksheet}

Gets the Worksheet object which contains this range.

**Type:** Worksheet

### Range.Item (int, int) property {#itemintint}

Gets Cell object in this range.

**Type:** Cell

### autoFill(target) (1 of 2) {#autofill}

Automaticall fill the target range.

| Parameter | Type | Description |
| --- | --- | --- |
| target | Range | the target range. |

---

### autoFill(target, autoFillType) (2 of 2) {#autofill-1}

Automaticall fill the target range.

| Parameter | Type | Description |
| --- | --- | --- |
| target | Range | The targed range. |
| autoFillType | int | A AutoFillType value. The auto fill type. |

### addHyperlink(address, textToDisplay, screenTip) {#addhyperlink}

Adds a hyperlink to a specified cell or a range of cells.

| Parameter | Type | Description |
| --- | --- | --- |
| address | String | Address of the hyperlink. |
| textToDisplay | String | The text to be displayed for the specified hyperlink. |
| screenTip | String | The screenTip text for the specified hyperlink. |

**Returns:** Hyperlink object.

### iterator() {#iterator}

Gets the enumerator for cells in this Range.

When traversing elements by the returned Enumerator, the cells collection should not be modified(such as operations that will cause new Cell/Row be instantiated or existing Cell/Row be deleted). Otherwise the enumerator may not be able to traverse all cells correctly(some elements may be traversed repeatedly or skipped).

**Returns:** The cells enumerator

### isIntersect(range) {#isintersect}

Indicates whether the range is intersect.

If the two ranges area not in the same worksheet ,return false.

| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | The range. |

**Returns:** Whether the range is intersect.

### intersect(range) {#intersect}

Returns a Range object that represents the rectangular intersection of two ranges.

If the two ranges are not intersected, returns null.

| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | The intersecting range. |

**Returns:** Returns a Range object

### unionRang(range) {#unionrang}

Returns the union result of two ranges.

NOTE: This method is now obsolete. Instead, please use Range.UnionRanges() method. This method will be removed 12 months later since May 2024. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | The range |

**Returns:** The union of two ranges.

### unionRanges(ranges) {#unionranges}

Returns the union result of two ranges.

| Parameter | Type | Description |
| --- | --- | --- |
| ranges | Range[] | The range |

**Returns:** The union of two ranges.

### union(range) {#union}

Returns the union of two ranges.

NOTE: This method is now obsolete. Instead, please use Range.UnionRanges() method. This method will be removed 12 months later since November 2023. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | The range |

**Returns:** The union of two ranges.

### isBlank() {#isblank}

Indicates whether the range contains values.

### merge() {#merge}

Combines a range of cells into a single cell.

Reference the merged cell via the address of the upper-left cell in the range.

### unMerge() {#unmerge}

Unmerges merged cells of this range.

### putValue(stringValue, isConverted, setStyle) {#putvalue}

Puts a value into the range, if appropriate the value will be converted to other data type and cell's number format will be reset.

| Parameter | Type | Description |
| --- | --- | --- |
| stringValue | String | Input value |
| isConverted | boolean | True: converted to other data type if appropriate. |
| setStyle | boolean | True: set the number format to cell's style when converting to other data type |

### setStyle(style, explicitFlag) (1 of 2) {#setstyle}

Apply the cell style.

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The cell style. |
| explicitFlag | boolean | True, only overwriting formatting which is explicitly set. |

---

### setStyle(style) (2 of 2) {#setstyle-1}

Sets the style of the range.

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The Style object. |

### applyStyle(style, flag) {#applystyle}

Applies formats for a whole range.

Each cell in this range will contains a Style object. So this is a memory-consuming method. Please use it carefully.

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The style object which will be applied. |
| flag | StyleFlag | Flags which indicates applied formatting properties. |

### setOutlineBorders(borderStyle, borderColor) (1 of 3) {#setoutlineborders}

Sets the outline borders around a range of cells with same border style and color.

| Parameter | Type | Description |
| --- | --- | --- |
| borderStyle | int | A CellBorderType value. Border style. |
| borderColor | CellsColor | Border color. |

---

### setOutlineBorders(borderStyle, borderColor) (2 of 3) {#setoutlineborders-1}

Sets the outline borders around a range of cells with same border style and color.

| Parameter | Type | Description |
| --- | --- | --- |
| borderStyle | int | A CellBorderType value. Border style. |
| borderColor | Color | Border color. |

---

### setOutlineBorders(borderStyles, borderColors) (3 of 3) {#setoutlineborders-2}

Sets out line borders around a range of cells.

Both the length of borderStyles and borderStyles must be 4. The order of borderStyles and borderStyles must be top,bottom,left,right

| Parameter | Type | Description |
| --- | --- | --- |
| borderStyles | Number Array | Border styles. |
| borderColors | Color[] | Border colors. |

### setOutlineBorder(borderEdge, borderStyle, borderColor) (1 of 2) {#setoutlineborder}

Sets outline border around a range of cells.

| Parameter | Type | Description |
| --- | --- | --- |
| borderEdge | int | A BorderType value. Border edge. |
| borderStyle | int | A CellBorderType value. Border style. |
| borderColor | CellsColor | Border color. |

---

### setOutlineBorder(borderEdge, borderStyle, borderColor) (2 of 2) {#setoutlineborder-1}

Sets outline border around a range of cells.

| Parameter | Type | Description |
| --- | --- | --- |
| borderEdge | int | A BorderType value. Border edge. |
| borderStyle | int | A CellBorderType value. Border style. |
| borderColor | Color | Border color. |

### setInsideBorders(borderEdge, lineStyle, borderColor) {#setinsideborders}

Set inside borders of the range.

| Parameter | Type | Description |
| --- | --- | --- |
| borderEdge | int | A BorderType value. Inside borde type, only can be BorderType.VERTICAL and BorderType.HORIZONTAL . |
| lineStyle | int | A CellBorderType value. The border style. |
| borderColor | CellsColor | The color of the border. |

### moveTo(destRow, destColumn) {#moveto}

Move the current range to the dest range.

| Parameter | Type | Description |
| --- | --- | --- |
| destRow | int | The start row of the dest range. |
| destColumn | int | The start column of the dest range. |

### copyData(range) {#copydata}

Copies cell data (including formulas) from a source range.

| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | Source Range object. |

### copyValue(range) {#copyvalue}

Copies cell value from a source range.

| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | Source Range object. |

### copyStyle(range) {#copystyle}

Copies style settings from a source range.

| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | Source Range object. |

### copy(range, options) (1 of 2) {#copy}

Copying the range with paste special options.

| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | The source range. |
| options | PasteOptions | The paste special options. |

---

### copy(range) (2 of 2) {#copy-1}

Copies data (including formulas), formatting, drawing objects etc. from a source range.

| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | Source Range object. |

### transpose() {#transpose}

Transpose (rotate) data from rows to columns or vice versa.

### getCellOrNull(rowOffset, columnOffset) {#getcellornull}

Gets Cell object or null in this range.

| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | int | Row offset in this range, zero based. |
| columnOffset | int | Column offset in this range, zero based. |

**Returns:** Cell object.

### getOffset(rowOffset, columnOffset) {#getoffset}

Gets Range range by offset.

| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | int | Row offset in this range, zero based. |
| columnOffset | int | Column offset in this range, zero based. |

### toString() {#tostring}

Returns a string represents the current Range object.

### toImage(options) {#toimage}

Converts the range to image.

| Parameter | Type | Description |
| --- | --- | --- |
| options | ImageOrPrintOptions | The options for converting this range to image |

### toJson(options) {#tojson}

Convert the range to JSON value.

| Parameter | Type | Description |
| --- | --- | --- |
| options | JsonSaveOptions | The options of converting |

### toHtml(saveOptions) {#tohtml}

Convert the range to html .

| Parameter | Type | Description |
| --- | --- | --- |
| saveOptions | HtmlSaveOptions | Options for coverting range to html. |

### clear() {#clear}

### clearContents() {#clearcontents}

### clearFormats() {#clearformats}

### clearComments() {#clearcomments}

### clearHyperlinks(clearFormat) {#clearhyperlinks}
