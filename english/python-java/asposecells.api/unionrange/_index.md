---
title: "UnionRange Class"
linktitle: "UnionRange"
articleTitle: "UnionRange"
second_title: "Aspose.Cells for Python via Java"
description: "Represents union range."
type: docs
weight: 7190
url: /python-java/asposecells.api/unionrange/
---

## UnionRange class

Represents union range.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [FirstRow](#firstrow) | int | Gets the index of the first row of the range. Only effects when it only contains one range. |
| [FirstColumn](#firstcolumn) | int | Gets the index of the first column of the range. Only effects when it only contains one range. |
| [RowCount](#rowcount) | int | Gets the count of rows in the range. Only effects when it only contains one range. |
| [ColumnCount](#columncount) | int | Gets the count of rows in the range. Only effects when it only contains one range. |
| [Value](#value) | Object | Gets and sets the values of the range. |
| [Name](#name) | String | Gets or sets the name of the range. Named range is supported. For example, range.Name = "Sheet1!MyRange"; |
| [RefersTo](#refersto) | String | Gets the range's refers to. |
| [HasRange](#hasrange) | boolean | Indicates whether this has range. |
| [Hyperlinks](#hyperlinks) | Hyperlink[] | Gets all hyperlink in the range. |
| [CellCount](#cellcount) | int | Gets all cell count in the range. |
| [RangeCount](#rangecount) | int | Gets the count of the ranges. |
| [Ranges](#ranges) | Range[] | Gets all union ranges. |

## Methods

| Name | Description |
| --- | --- |
| [merge](#merge) | Combines a range of cells into a single cell.

Reference the merged cell via the address of the upper-left cell in the r |
| [unMerge](#unmerge) | Unmerges merged cells of this range. |
| [putValue](#putvalue) | Puts a value into the range, if appropriate the value will be converted to other data type and cell's number format will |
| [setStyle](#setstyle) | Sets the style of the range. |
| [applyStyle](#applystyle) | Applies formats for a whole range.

Each cell in this range will contains a Style object. So this is a memory-consuming  |
| [copy](#copy) | Copying the range with paste special options. |
| [iterator](#iterator) | Gets the enumerator for cells in this Range.

When traversing elements by the returned Enumerator, the cells collection  |
| [setOutlineBorders](#setoutlineborders) | Sets out line borders around a range of cells.

Both the length of borderStyles and borderStyles must be 4. The order of |
| [intersect](#intersect) | Intersects another range.

If the two union ranges are not intersected, returns null. |
| [union](#union) | Union another range. |

### UnionRange.FirstRow property {#firstrow}

Gets the index of the first row of the range. Only effects when it only contains one range.

**Type:** int

### UnionRange.FirstColumn property {#firstcolumn}

Gets the index of the first column of the range. Only effects when it only contains one range.

**Type:** int

### UnionRange.RowCount property {#rowcount}

Gets the count of rows in the range. Only effects when it only contains one range.

**Type:** int

### UnionRange.ColumnCount property {#columncount}

Gets the count of rows in the range. Only effects when it only contains one range.

**Type:** int

### UnionRange.Value property {#value}

Gets and sets the values of the range.

**Type:** Object

### UnionRange.Name property {#name}

Gets or sets the name of the range. Named range is supported. For example, range.Name = "Sheet1!MyRange";

**Type:** String

### UnionRange.RefersTo property {#refersto}

Gets the range's refers to.

**Type:** String

### UnionRange.HasRange property {#hasrange}

Indicates whether this has range.

**Type:** boolean

### UnionRange.Hyperlinks property {#hyperlinks}

Gets all hyperlink in the range.

**Type:** Hyperlink[]

### UnionRange.CellCount property {#cellcount}

Gets all cell count in the range.

**Type:** int

### UnionRange.RangeCount property {#rangecount}

Gets the count of the ranges.

**Type:** int

### UnionRange.Ranges property {#ranges}

Gets all union ranges.

**Type:** Range[]

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

### setStyle(style) {#setstyle}

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

### copy(range, options) {#copy}

Copying the range with paste special options.

| Parameter | Type | Description |
| --- | --- | --- |
| range | UnionRange | The source range. |
| options | PasteOptions | The paste special options. |

### iterator() {#iterator}

Gets the enumerator for cells in this Range.

When traversing elements by the returned Enumerator, the cells collection should not be modified(such as operations that will cause new Cell/Row be instantiated or existing Cell/Row be deleted). Otherwise the enumerator may not be able to traverse all cells correctly(some elements may be traversed repeatedly or skipped).

**Returns:** The cells enumerator

### setOutlineBorders(borderStyles, borderColors) (1 of 2) {#setoutlineborders}

Sets out line borders around a range of cells.

Both the length of borderStyles and borderStyles must be 4. The order of borderStyles and borderStyles must be top,bottom,left,right

| Parameter | Type | Description |
| --- | --- | --- |
| borderStyles | Number Array | Border styles. |
| borderColors | Color[] | Border colors. |

---

### setOutlineBorders(borderStyle, borderColor) (2 of 2) {#setoutlineborders-1}

Sets the outline borders around a range of cells with same border style and color.

| Parameter | Type | Description |
| --- | --- | --- |
| borderStyle | int | A CellBorderType value. Border style. |
| borderColor | Color | Border color. |

### intersect(range) (1 of 3) {#intersect}

Intersects another range.

If the two union ranges are not intersected, returns null.

| Parameter | Type | Description |
| --- | --- | --- |
| range | String | The range. |

---

### intersect(unionRange) (2 of 3) {#intersect-1}

Intersects another range.

If the two union ranges are not intersected, returns null.

| Parameter | Type | Description |
| --- | --- | --- |
| unionRange | UnionRange | The range. |

---

### intersect(ranges) (3 of 3) {#intersect-2}

Intersects another range.

If the two union ranges are not intersected, returns null.

| Parameter | Type | Description |
| --- | --- | --- |
| ranges | Range[] | The range. |

### union(range) (1 of 3) {#union}

Union another range.

| Parameter | Type | Description |
| --- | --- | --- |
| range | String | The range. |

---

### union(unionRange) (2 of 3) {#union-1}

Union another range.

| Parameter | Type | Description |
| --- | --- | --- |
| unionRange | UnionRange | The range. |

---

### union(ranges) (3 of 3) {#union-2}

Union the ranges.

| Parameter | Type | Description |
| --- | --- | --- |
| ranges | Range[] | The ranges. |
