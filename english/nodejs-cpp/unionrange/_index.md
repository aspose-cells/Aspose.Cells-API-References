---
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


## Methods

| Method | Description |
| --- | --- |
| [getFirstRow()](#getFirstRow--)| Gets the index of the first row of the range. |
| [getFirstColumn()](#getFirstColumn--)| Gets the index of the first column of the range. |
| [getRowCount()](#getRowCount--)| Gets the count of rows in the range. |
| [getColumnCount()](#getColumnCount--)| Gets the count of rows in the range. |
| [getValue()](#getValue--)| Gets and sets the values of the range. |
| [setValue(Object)](#setValue-object-)| Gets and sets the values of the range. |
| [getName()](#getName--)| Gets or sets the name of the range. |
| [setName(string)](#setName-string-)| Gets or sets the name of the range. |
| [getRefersTo()](#getRefersTo--)| Gets the range's refers to. |
| [getHasRange()](#getHasRange--)| Indicates whether this has range. |
| [getHyperlinks()](#getHyperlinks--)| Gets all hyperlink in the range. |
| [getCellCount()](#getCellCount--)| Gets all cell count in the range. |
| [getRangeCount()](#getRangeCount--)| Gets the count of the ranges. |
| [getRanges()](#getRanges--)| Gets all union ranges. |
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


### getFirstRow() {#getFirstRow--}

Gets the index of the first row of the range.

```javascript
getFirstRow() : number;
```


**Remarks**

Only effects when it only contains one range.

### getFirstColumn() {#getFirstColumn--}

Gets the index of the first column of the range.

```javascript
getFirstColumn() : number;
```


**Remarks**

Only effects when it only contains one range.

### getRowCount() {#getRowCount--}

Gets the count of rows in the range.

```javascript
getRowCount() : number;
```


**Remarks**

Only effects when it only contains one range.

### getColumnCount() {#getColumnCount--}

Gets the count of rows in the range.

```javascript
getColumnCount() : number;
```


**Remarks**

Only effects when it only contains one range.

### getValue() {#getValue--}

Gets and sets the values of the range.

```javascript
getValue() : Object;
```


### setValue(Object) {#setValue-object-}

Gets and sets the values of the range.

```javascript
setValue(value: Object) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Object | The value to set. |

### getName() {#getName--}

Gets or sets the name of the range.

```javascript
getName() : string;
```


**Remarks**

Named range is supported. For example, <p>range.Name = "Sheet1!MyRange";

### setName(string) {#setName-string-}

Gets or sets the name of the range.

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

Gets the range's refers to.

```javascript
getRefersTo() : string;
```


### getHasRange() {#getHasRange--}

Indicates whether this has range.

```javascript
getHasRange() : boolean;
```


### getHyperlinks() {#getHyperlinks--}

Gets all hyperlink in the range.

```javascript
getHyperlinks() : Hyperlink[];
```


**Returns**

[Hyperlink](../hyperlink/)[]

### getCellCount() {#getCellCount--}

Gets all cell count in the range.

```javascript
getCellCount() : number;
```


### getRangeCount() {#getRangeCount--}

Gets the count of the ranges.

```javascript
getRangeCount() : number;
```


### getRanges() {#getRanges--}

Gets all union ranges.

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



