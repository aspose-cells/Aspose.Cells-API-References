﻿---
title: SparklineGroupCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Encapsulates a collection of SparklineGroupnodejscppsparklinegroup objects.
type: docs
url: /nodejs-cpp/sparklinegroupcollection/
---

## SparklineGroupCollection class

Encapsulates a collection of [SparklineGroup](/nodejs-cpp/sparklinegroup/) objects.

```javascript
class SparklineGroupCollection;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the [SparklineGroup](/nodejs-cpp/sparklinegroup/) element at the specified index. |
| [add(SparklineType)](#add-sparklinetype-)| Adds an [SparklineGroup](/nodejs-cpp/sparklinegroup/) with a [SparklineGroup](/nodejs-cpp/sparklinegroup/) to the collection. |
| [add(SparklineType, string, boolean, CellArea)](#add-sparklinetype-string-boolean-cellarea-)| Adds an [SparklineGroup](/nodejs-cpp/sparklinegroup/) with [SparklineGroup](/nodejs-cpp/sparklinegroup/) to the collection. |
| [clearSparklines(CellArea)](#clearSparklines-cellarea-)| Clears the sparklines that is inside an area of cells. |
| [clearSparklineGroups(CellArea)](#clearSparklineGroups-cellarea-)| Clears the sparkline groups that overlaps an area of cells. |
| [getCount()](#getCount--)| Gets the number of elements contained in. |


### get(number) {#get-number-}

Gets the [SparklineGroup](/nodejs-cpp/sparklinegroup/) element at the specified index.

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

Adds an [SparklineGroup](/nodejs-cpp/sparklinegroup/) with a [SparklineGroup](/nodejs-cpp/sparklinegroup/) to the collection.

```javascript
add(type: SparklineType) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [SparklineType](/nodejs-cpp/sparklinetype/) | Specifies the type of the Sparkline group. |

**Returns**

[SparklineGroup](/nodejs-cpp/sparklinegroup/) object index.

### add(SparklineType, string, boolean, CellArea) {#add-sparklinetype-string-boolean-cellarea-}

Adds an [SparklineGroup](/nodejs-cpp/sparklinegroup/) with [SparklineGroup](/nodejs-cpp/sparklinegroup/) to the collection.

```javascript
add(type: SparklineType, dataRange: string, isVertical: boolean, locationRange: CellArea) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [SparklineType](/nodejs-cpp/sparklinetype/) | Specifies the type of the Sparkline group. |
| dataRange | string | Specifies the data range of the sparkline group. |
| isVertical | boolean | Specifies whether to plot the sparklines from the data range by row or by column. |
| locationRange | [CellArea](/nodejs-cpp/cellarea/) | Specifies where the sparklines to be placed. |

**Returns**

[SparklineGroup](/nodejs-cpp/sparklinegroup/) object index.

### clearSparklines(CellArea) {#clearSparklines-cellarea-}

Clears the sparklines that is inside an area of cells.

```javascript
clearSparklines(cellArea: CellArea) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | [CellArea](/nodejs-cpp/cellarea/) | Specifies the area of cells |

### clearSparklineGroups(CellArea) {#clearSparklineGroups-cellarea-}

Clears the sparkline groups that overlaps an area of cells.

```javascript
clearSparklineGroups(cellArea: CellArea) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | [CellArea](/nodejs-cpp/cellarea/) | Specifies the area of cells |

### getCount() {#getCount--}

Gets the number of elements contained in.

```javascript
getCount() : number;
```



