﻿---
title: UnionRange
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents union range.
type: docs
url: /nodejs-cpp/unionrange/
---

## UnionRange class

Represents union range.

```javascript
class UnionRange;
```


## Properties

| Property | Type | Description |
| --- | --- | --- |
| [firstRow](#firstRow--)| number | Readonly. Gets the index of the first row of the range. |
| [firstColumn](#firstColumn--)| number | Readonly. Gets the index of the first column of the range. |
| [rowCount](#rowCount--)| number | Readonly. Gets the count of rows in the range. |
| [columnCount](#columnCount--)| number | Readonly. Gets the count of rows in the range. |
| [value](#value--)| Object | Gets and sets the values of the range. |
| [name](#name--)| string | Gets or sets the name of the range. |
| [refersTo](#refersTo--)| string | Readonly. Gets the range's refers to. |
| [hasRange](#hasRange--)| boolean | Readonly. Indicates whether this has range. |
| [hyperlinks](#hyperlinks--)| Hyperlink[] | Readonly. Gets all hyperlink in the range. |
| [cellCount](#cellCount--)| number | Readonly. Gets all cell count in the range. |
| [rangeCount](#rangeCount--)| number | Readonly. Gets the count of the ranges. |
| [ranges](#ranges--)| Range[] | Readonly. Gets all union ranges. |

## Methods

| Method | Description |
| --- | --- |
| [getFirstRow()](#getFirstRow--)| <b>@deprecated.</b> Please use the 'firstRow' property instead. Gets the index of the first row of the range. |
| [getFirstColumn()](#getFirstColumn--)| <b>@deprecated.</b> Please use the 'firstColumn' property instead. Gets the index of the first column of the range. |
| [getRowCount()](#getRowCount--)| <b>@deprecated.</b> Please use the 'rowCount' property instead. Gets the count of rows in the range. |
| [getColumnCount()](#getColumnCount--)| <b>@deprecated.</b> Please use the 'columnCount' property instead. Gets the count of rows in the range. |
| [getValue()](#getValue--)| <b>@deprecated.</b> Please use the 'value' property instead. Gets and sets the values of the range. |
| [setValue(Object)](#setValue-object-)| <b>@deprecated.</b> Please use the 'value' property instead. Gets and sets the values of the range. |
| [getName()](#getName--)| <b>@deprecated.</b> Please use the 'name' property instead. Gets or sets the name of the range. |
| [setName(string)](#setName-string-)| <b>@deprecated.</b> Please use the 'name' property instead. Gets or sets the name of the range. |
| [getRefersTo()](#getRefersTo--)| <b>@deprecated.</b> Please use the 'refersTo' property instead. Gets the range's refers to. |
| [getHasRange()](#getHasRange--)| <b>@deprecated.</b> Please use the 'hasRange' property instead. Indicates whether this has range. |
| [getHyperlinks()](#getHyperlinks--)| <b>@deprecated.</b> Please use the 'hyperlinks' property instead. Gets all hyperlink in the range. |
| [getCellCount()](#getCellCount--)| <b>@deprecated.</b> Please use the 'cellCount' property instead. Gets all cell count in the range. |
| [getRangeCount()](#getRangeCount--)| <b>@deprecated.</b> Please use the 'rangeCount' property instead. Gets the count of the ranges. |
| [getRanges()](#getRanges--)| <b>@deprecated.</b> Please use the 'ranges' property instead. Gets all union ranges. |
| [merge()](#merge--)| Combines a range of cells into a single cell. |
| [unMerge()](#unMerge--)| Unmerges merged cells of this range. |
| [putValue(string, boolean, boolean)](#putValue-string-boolean-boolean-)| Puts a value into the range, if appropriate the value will be converted to other data type and cell's number format will be reset. |
| [setStyle(Style)](#setStyle-style-)| Sets the style of the range. |
| [applyStyle(Style, StyleFlag)](#applyStyle-style-styleflag-)| Applies formats for a whole range. |
| [copy(UnionRange, PasteOptions)](#copy-unionrange-pasteoptions-)| Copying the range with paste special options. |
| [getEnumerator()](#getEnumerator--)| Gets the enumerator for cells in this Range. |
| [setOutlineBorders(CellBorderType[], Color[])](#setOutlineBorders-cellbordertypearray-colorarray-)| Sets out line borders around a range of cells. |
| [setOutlineBorders(CellBorderType, Color)](#setOutlineBorders-cellbordertype-color-)| Sets the outline borders around a range of cells with same border style and color. |
| [intersect(string)](#intersect-string-)| Intersects another range. |
| [intersect(UnionRange)](#intersect-unionrange-)| Intersects another range. |
| [intersect(Range[])](#intersect-rangearray-)| Intersects another range. |
| [union(string)](#union-string-)| Union another range. |
| [union(UnionRange)](#union-unionrange-)| Union another range. |
| [union(Range[])](#union-rangearray-)| Union the ranges. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### firstRow {#firstRow--}

Readonly. Gets the index of the first row of the range.

```javascript
firstRow : number;
```


**Remarks**

Only effects when it only contains one range.

### firstColumn {#firstColumn--}

Readonly. Gets the index of the first column of the range.

```javascript
firstColumn : number;
```


**Remarks**

Only effects when it only contains one range.

### rowCount {#rowCount--}

Readonly. Gets the count of rows in the range.

```javascript
rowCount : number;
```


**Remarks**

Only effects when it only contains one range.

### columnCount {#columnCount--}

Readonly. Gets the count of rows in the range.

```javascript
columnCount : number;
```


**Remarks**

Only effects when it only contains one range.

### value {#value--}

Gets and sets the values of the range.

```javascript
value : Object;
```


### name {#name--}

Gets or sets the name of the range.

```javascript
name : string;
```


**Remarks**

Named range is supported. For example, <p>range.Name = "Sheet1!MyRange";

### refersTo {#refersTo--}

Readonly. Gets the range's refers to.

```javascript
refersTo : string;
```


### hasRange {#hasRange--}

Readonly. Indicates whether this has range.

```javascript
hasRange : boolean;
```


### hyperlinks {#hyperlinks--}

Readonly. Gets all hyperlink in the range.

```javascript
hyperlinks : Hyperlink[];
```


### cellCount {#cellCount--}

Readonly. Gets all cell count in the range.

```javascript
cellCount : number;
```


### rangeCount {#rangeCount--}

Readonly. Gets the count of the ranges.

```javascript
rangeCount : number;
```


### ranges {#ranges--}

Readonly. Gets all union ranges.

```javascript
ranges : Range[];
```


### getFirstRow() {#getFirstRow--}

<b>@deprecated.</b> Please use the 'firstRow' property instead. Gets the index of the first row of the range.

```javascript
getFirstRow() : number;
```


**Remarks**

Only effects when it only contains one range.

### getFirstColumn() {#getFirstColumn--}

<b>@deprecated.</b> Please use the 'firstColumn' property instead. Gets the index of the first column of the range.

```javascript
getFirstColumn() : number;
```


**Remarks**

Only effects when it only contains one range.

### getRowCount() {#getRowCount--}

<b>@deprecated.</b> Please use the 'rowCount' property instead. Gets the count of rows in the range.

```javascript
getRowCount() : number;
```


**Remarks**

Only effects when it only contains one range.

### getColumnCount() {#getColumnCount--}

<b>@deprecated.</b> Please use the 'columnCount' property instead. Gets the count of rows in the range.

```javascript
getColumnCount() : number;
```


**Remarks**

Only effects when it only contains one range.

### getValue() {#getValue--}

<b>@deprecated.</b> Please use the 'value' property instead. Gets and sets the values of the range.

```javascript
getValue() : Object;
```


### setValue(Object) {#setValue-object-}

<b>@deprecated.</b> Please use the 'value' property instead. Gets and sets the values of the range.

```javascript
setValue(value: Object) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Object | The value to set. |

### getName() {#getName--}

<b>@deprecated.</b> Please use the 'name' property instead. Gets or sets the name of the range.

```javascript
getName() : string;
```


**Remarks**

Named range is supported. For example, <p>range.Name = "Sheet1!MyRange";

### setName(string) {#setName-string-}

<b>@deprecated.</b> Please use the 'name' property instead. Gets or sets the name of the range.

```javascript
setName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

**Remarks**

Named range is supported. For example, <p>range.Name = "Sheet1!MyRange";

### getRefersTo() {#getRefersTo--}

<b>@deprecated.</b> Please use the 'refersTo' property instead. Gets the range's refers to.

```javascript
getRefersTo() : string;
```


### getHasRange() {#getHasRange--}

<b>@deprecated.</b> Please use the 'hasRange' property instead. Indicates whether this has range.

```javascript
getHasRange() : boolean;
```


### getHyperlinks() {#getHyperlinks--}

<b>@deprecated.</b> Please use the 'hyperlinks' property instead. Gets all hyperlink in the range.

```javascript
getHyperlinks() : Hyperlink[];
```


**Returns**

[Hyperlink](../hyperlink/)[]

### getCellCount() {#getCellCount--}

<b>@deprecated.</b> Please use the 'cellCount' property instead. Gets all cell count in the range.

```javascript
getCellCount() : number;
```


### getRangeCount() {#getRangeCount--}

<b>@deprecated.</b> Please use the 'rangeCount' property instead. Gets the count of the ranges.

```javascript
getRangeCount() : number;
```


### getRanges() {#getRanges--}

<b>@deprecated.</b> Please use the 'ranges' property instead. Gets all union ranges.

```javascript
getRanges() : Range[];
```


**Returns**

[Range](../range/)[]

### merge() {#merge--}

Combines a range of cells into a single cell.

```javascript
merge() : void;
```


**Remarks**

Reference the merged cell via the address of the upper-left cell in the range.

### unMerge() {#unMerge--}

Unmerges merged cells of this range.

```javascript
unMerge() : void;
```


### putValue(string, boolean, boolean) {#putValue-string-boolean-boolean-}

Puts a value into the range, if appropriate the value will be converted to other data type and cell's number format will be reset.

```javascript
putValue(stringValue: string, isConverted: boolean, setStyle: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stringValue | string | Input value |
| isConverted | boolean | True: converted to other data type if appropriate. |
| setStyle | boolean | True: set the number format to cell's style when converting to other data type |

### setStyle(Style) {#setStyle-style-}

Sets the style of the range.

```javascript
setStyle(style: Style) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [Style](../style/) | The Style object. |

### applyStyle(Style, StyleFlag) {#applyStyle-style-styleflag-}

Applies formats for a whole range.

```javascript
applyStyle(style: Style, flag: StyleFlag) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [Style](../style/) | The style object which will be applied. |
| flag | [StyleFlag](../styleflag/) | Flags which indicates applied formatting properties. |

**Remarks**

Each cell in this range will contains a [Style](../style/) object. So this is a memory-consuming method. Please use it carefully.

### copy(UnionRange, PasteOptions) {#copy-unionrange-pasteoptions-}

Copying the range with paste special options.

```javascript
copy(range: UnionRange, options: PasteOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| range | [UnionRange](../unionrange/) | The source range. |
| options | [PasteOptions](../pasteoptions/) | The paste special options. |

### getEnumerator() {#getEnumerator--}

Gets the enumerator for cells in this Range.

```javascript
getEnumerator() : CellEnumerator;
```


**Returns**

The cells enumerator

**Remarks**

When traversing elements by the returned Enumerator, the cells collection should not be modified(such as operations that will cause new Cell/Row be instantiated or existing Cell/Row be deleted). Otherwise the enumerator may not be able to traverse all cells correctly(some elements may be traversed repeatedly or skipped).

### setOutlineBorders(CellBorderType[], Color[]) {#setOutlineBorders-cellbordertypearray-colorarray-}

Sets out line borders around a range of cells.

```javascript
setOutlineBorders(borderStyles: CellBorderType[], borderColors: Color[]) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| borderStyles | [CellBorderType](../cellbordertype/)[] | Border styles. |
| borderColors | [Color](../color/)[] | Border colors. |

**Remarks**

Both the length of borderStyles and borderStyles must be 4. The order of borderStyles and borderStyles must be top,bottom,left,right

### setOutlineBorders(CellBorderType, Color) {#setOutlineBorders-cellbordertype-color-}

Sets the outline borders around a range of cells with same border style and color.

```javascript
setOutlineBorders(borderStyle: CellBorderType, borderColor: Color) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| borderStyle | [CellBorderType](../cellbordertype/) | Border style. |
| borderColor | [Color](../color/) | Border color. |

### intersect(string) {#intersect-string-}

Intersects another range.

```javascript
intersect(range: string) : UnionRange;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| range | string | The range. |

**Returns**

[UnionRange](../unionrange/)

**Remarks**

If the two union ranges are not intersected, returns null.

### intersect(UnionRange) {#intersect-unionrange-}

Intersects another range.

```javascript
intersect(unionRange: UnionRange) : UnionRange;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| unionRange | [UnionRange](../unionrange/) | The range. |

**Returns**

[UnionRange](../unionrange/)

**Remarks**

If the two union ranges are not intersected, returns null.

### intersect(Range[]) {#intersect-rangearray-}

Intersects another range.

```javascript
intersect(ranges: Range[]) : UnionRange;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| ranges | [Range](../range/)[] | The range. |

**Returns**

[UnionRange](../unionrange/)

**Remarks**

If the two union ranges are not intersected, returns null.

### union(string) {#union-string-}

Union another range.

```javascript
union(range: string) : UnionRange;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| range | string | The range. |

**Returns**

[UnionRange](../unionrange/)

### union(UnionRange) {#union-unionrange-}

Union another range.

```javascript
union(unionRange: UnionRange) : UnionRange;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| unionRange | [UnionRange](../unionrange/) | The range. |

**Returns**

[UnionRange](../unionrange/)

### union(Range[]) {#union-rangearray-}

Union the ranges.

```javascript
union(ranges: Range[]) : UnionRange;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| ranges | [Range](../range/)[] | The ranges. |

**Returns**

[UnionRange](../unionrange/)

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



