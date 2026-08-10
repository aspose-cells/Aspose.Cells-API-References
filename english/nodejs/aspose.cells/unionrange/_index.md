---
title: "UnionRange"
linktitle: "UnionRange"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents union range."
type: docs
weight: 4410
url: /nodejs/aspose.cells/unionrange/
---

## UnionRange class

Represents union range.

## Methods

| Name | Description |
| --- | --- |
| [applyStyle(style, flag)](#applystyle) | Applies formats for a whole range. Each cell in this range will contains a Style object. So this is a memory-consuming m |
| [copy(range, options)](#copy) | Copying the range with paste special options. |
| [getCellCount()](#getcellcount) | Gets all cell count in the range. |
| [getColumnCount()](#getcolumncount) | Gets the count of rows in the range. Only effects when it only contains one range. |
| [getFirstColumn()](#getfirstcolumn) | Gets the index of the first column of the range. Only effects when it only contains one range. |
| [getFirstRow()](#getfirstrow) | Gets the index of the first row of the range. Only effects when it only contains one range. |
| [getHyperlinks()](#gethyperlinks) | Gets all hyperlink in the range. |
| [getName()](#getname) | Gets or sets the name of the range. Named range is supported. For example, range.Name = "Sheet1!MyRange"; |
| [getRangeCount()](#getrangecount) | Gets the count of the ranges. |
| [getRanges()](#getranges) | Gets all union ranges. |
| [getRefersTo()](#getrefersto) | Gets the range's refers to. |
| [getRowCount()](#getrowcount) | Gets the count of rows in the range. Only effects when it only contains one range. |
| [getValue()](#getvalue) | Gets and sets the values of the range. |
| [hasRange()](#hasrange) | Indicates whether this has range. |
| [intersect(range)](#intersect) | Intersects another range. If the two union ranges are not intersected, returns null. |
| [intersect(unionRange)](#intersect-1) | Intersects another range. If the two union ranges are not intersected, returns null. |
| [intersect(ranges)](#intersect-2) | Intersects another range. If the two union ranges are not intersected, returns null. |
| [iterator()](#iterator) | Gets the enumerator for cells in this Range. When traversing elements by the returned Enumerator, the cells collection s |
| [merge()](#merge) | Combines a range of cells into a single cell. Reference the merged cell via the address of the upper-left cell in the ra |
| [putValue(stringValue, isConverted, setStyle)](#putvalue) | Puts a value into the range, if appropriate the value will be converted to other data type and cell's number format will |
| [setName()](#setname) | Gets or sets the name of the range. Named range is supported. For example, range.Name = "Sheet1!MyRange"; |
| [setOutlineBorders(borderStyles, borderColors)](#setoutlineborders) | Sets out line borders around a range of cells. Both the length of borderStyles and borderStyles must be 4. The order of  |
| [setOutlineBorders(borderStyle, borderColor)](#setoutlineborders-1) | Sets the outline borders around a range of cells with same border style and color. |
| [setStyle(style)](#setstyle) | Sets the style of the range. |
| [setValue()](#setvalue) | Gets and sets the values of the range. |
| [unMerge()](#unmerge) | Unmerges merged cells of this range. |
| [union(range)](#union) | Union another range. |
| [union(unionRange)](#union-1) | Union another range. |
| [union(ranges)](#union-2) | Union the ranges. |

### applyStyle(style, flag) {#applystyle}

Applies formats for a whole range. Each cell in this range will contains a Style object. So this is a memory-consuming method. Please use it carefully.

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The style object which will be applied. |
| flag | StyleFlag | Flags which indicates applied formatting properties. |

### copy(range, options) {#copy}

Copying the range with paste special options.

| Parameter | Type | Description |
| --- | --- | --- |
| range | UnionRange | The source range. |
| options | PasteOptions | The paste special options. |

### getCellCount() {#getcellcount}

Gets all cell count in the range.

### getColumnCount() {#getcolumncount}

Gets the count of rows in the range. Only effects when it only contains one range.

### getFirstColumn() {#getfirstcolumn}

Gets the index of the first column of the range. Only effects when it only contains one range.

### getFirstRow() {#getfirstrow}

Gets the index of the first row of the range. Only effects when it only contains one range.

### getHyperlinks() {#gethyperlinks}

Gets all hyperlink in the range.

### getName() {#getname}

Gets or sets the name of the range. Named range is supported. For example, range.Name = "Sheet1!MyRange";

### getRangeCount() {#getrangecount}

Gets the count of the ranges.

### getRanges() {#getranges}

Gets all union ranges.

### getRefersTo() {#getrefersto}

Gets the range's refers to.

### getRowCount() {#getrowcount}

Gets the count of rows in the range. Only effects when it only contains one range.

### getValue() {#getvalue}

Gets and sets the values of the range.

### hasRange() {#hasrange}

Indicates whether this has range.

### intersect(range) {#intersect}

Intersects another range. If the two union ranges are not intersected, returns null.

| Parameter | Type | Description |
| --- | --- | --- |
| range | String | The range. |

### intersect(unionRange) {#intersect-1}

Intersects another range. If the two union ranges are not intersected, returns null.

| Parameter | Type | Description |
| --- | --- | --- |
| unionRange | UnionRange | The range. |

### intersect(ranges) {#intersect-2}

Intersects another range. If the two union ranges are not intersected, returns null.

| Parameter | Type | Description |
| --- | --- | --- |
| ranges | Array ofRange | The range. |

### iterator() {#iterator}

Gets the enumerator for cells in this Range. When traversing elements by the returned Enumerator, the cells collection should not be modified(such as operations that will cause new Cell/Row be instantiated or existing Cell/Row be deleted). Otherwise the enumerator may not be able to traverse all cells correctly(some elements may be traversed repeatedly or skipped).@return {Iterator} The cells enumerator

### merge() {#merge}

Combines a range of cells into a single cell. Reference the merged cell via the address of the upper-left cell in the range.

### putValue(stringValue, isConverted, setStyle) {#putvalue}

Puts a value into the range, if appropriate the value will be converted to other data type and cell's number format will be reset.

| Parameter | Type | Description |
| --- | --- | --- |
| stringValue | String | Input value |
| isConverted | boolean | True: converted to other data type if appropriate. |
| setStyle | boolean | True: set the number format to cell's style when converting to other data type |

### setName() {#setname}

Gets or sets the name of the range. Named range is supported. For example, range.Name = "Sheet1!MyRange";

### setOutlineBorders(borderStyles, borderColors) {#setoutlineborders}

Sets out line borders around a range of cells. Both the length of borderStyles and borderStyles must be 4. The order of borderStyles and borderStyles must be top,bottom,left,right

| Parameter | Type | Description |
| --- | --- | --- |
| borderStyles | Array of Number | Border styles. |
| borderColors | Array ofColor | Border colors. |

### setOutlineBorders(borderStyle, borderColor) {#setoutlineborders-1}

Sets the outline borders around a range of cells with same border style and color.

| Parameter | Type | Description |
| --- | --- | --- |
| borderStyle | Number | CellBorderType |
| borderColor | Color | Border color. |

### setStyle(style) {#setstyle}

Sets the style of the range.

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The Style object. |

### setValue() {#setvalue}

Gets and sets the values of the range.

### unMerge() {#unmerge}

Unmerges merged cells of this range.

### union(range) {#union}

Union another range.

| Parameter | Type | Description |
| --- | --- | --- |
| range | String | The range. |

**Returns:** UnionRange — `UnionRange`

### union(unionRange) {#union-1}

Union another range.

| Parameter | Type | Description |
| --- | --- | --- |
| unionRange | UnionRange | The range. |

**Returns:** UnionRange — `UnionRange`

### union(ranges) {#union-2}

Union the ranges.

| Parameter | Type | Description |
| --- | --- | --- |
| ranges | Array ofRange | The ranges. |

**Returns:** UnionRange — `UnionRange`
