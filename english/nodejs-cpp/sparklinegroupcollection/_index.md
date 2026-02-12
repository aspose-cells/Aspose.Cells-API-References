---
title: SparklineGroupCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Encapsulates a collection of SparklineGroup..sparklinegroup objects.
type: docs
url: /nodejs-cpp/sparklinegroupcollection/
---

## SparklineGroupCollection class

Encapsulates a collection of [SparklineGroup](../sparklinegroup/) objects.

```javascript
class SparklineGroupCollection;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the [SparklineGroup](../sparklinegroup/) element at the specified index. |
| [add(SparklineType)](#add-sparklinetype-)| Adds an [SparklineGroup](../sparklinegroup/) with a [Sparkline](../sparkline/) to the collection. |
| [add(SparklineType, string, boolean, CellArea)](#add-sparklinetype-string-boolean-cellarea-)| Adds an [SparklineGroup](../sparklinegroup/) with some [Sparkline](../sparkline/) to the collection. |
| [clearSparklines(CellArea)](#clearSparklines-cellarea-)| Clears the sparklines that is inside an area of cells. |
| [clearSparklineGroups(CellArea)](#clearSparklineGroups-cellarea-)| Clears the sparkline groups that overlaps an area of cells. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### get(number) {#get-number-}

Gets the [SparklineGroup](../sparklinegroup/) element at the specified index.

```javascript
get(index: number) : SparklineGroup;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The zero based index of the element. |

**Returns**

The element at the specified index.

### add(SparklineType) {#add-sparklinetype-}

Adds an [SparklineGroup](../sparklinegroup/) with a [Sparkline](../sparkline/) to the collection.

```javascript
add(type: SparklineType) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [SparklineType](../sparklinetype/) | Specifies the type of the Sparkline group. |

**Returns**

[SparklineGroup](../sparklinegroup/) object index.

### add(SparklineType, string, boolean, CellArea) {#add-sparklinetype-string-boolean-cellarea-}

Adds an [SparklineGroup](../sparklinegroup/) with some [Sparkline](../sparkline/) to the collection.

```javascript
add(type: SparklineType, dataRange: string, isVertical: boolean, locationRange: CellArea) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [SparklineType](../sparklinetype/) | Specifies the type of the Sparkline group. |
| dataRange | string | Specifies the data range of the sparkline group. |
| isVertical | boolean | Specifies whether to plot the sparklines from the data range by row or by column. |
| locationRange | [CellArea](../cellarea/) | Specifies where the sparklines to be placed. |

**Returns**

[SparklineGroup](../sparklinegroup/) object index.

**Remarks**

This method will create sparklines too. If <paramref name="isVertical"/> is true, the number of rows in dataRange and locationRange must be same. If <paramref name="isVertical"/> is false, the number of columns in dataRange and locationRange must be same.

### clearSparklines(CellArea) {#clearSparklines-cellarea-}

Clears the sparklines that is inside an area of cells.

```javascript
clearSparklines(cellArea: CellArea) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | [CellArea](../cellarea/) | Specifies the area of cells |

**Remarks**

[SparklineGroup](../sparklinegroup/) will be removed too if it does not contains any [Sparkline](../sparkline/).

### clearSparklineGroups(CellArea) {#clearSparklineGroups-cellarea-}

Clears the sparkline groups that overlaps an area of cells.

```javascript
clearSparklineGroups(cellArea: CellArea) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | [CellArea](../cellarea/) | Specifies the area of cells |

### getCount() {#getCount--}

<b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in.

```javascript
getCount() : number;
```


### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



