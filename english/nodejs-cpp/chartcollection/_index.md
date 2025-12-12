---
title: ChartCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Encapsulates a collection of Chart..chart objects.
type: docs
url: /nodejs-cpp/chartcollection/
---

## ChartCollection class

Encapsulates a collection of [Chart](../chart/) objects.

```javascript
class ChartCollection;
```


### Example
```javascript
const { Workbook } = require("aspose.cells.node");

var workbook = new Workbook();
var charts = workbook.worksheets.get(0).charts;
```
## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the [Chart](../chart/) element at the specified index. |
| [get(string)](#get-string-)| Gets the chart by the name. |
| [addFloatingChart(ChartType, number, number, number, number)](#addFloatingChart-charttype-number-number-number-number-)| Adds a chart to the collection. |
| [add(ChartType, number, number, number, number)](#add-charttype-number-number-number-number-)| Adds a chart to the collection. |
| [add(Uint8Array, string, boolean, number, number, number, number)](#add-uint8array-string-boolean-number-number-number-number-)| Adds a chart with preset template. |
| [add(ChartType, string, boolean, number, number, number, number)](#add-charttype-string-boolean-number-number-number-number-)| Adds a chart to the collection. |
| [removeAt(number)](#removeAt-number-)| Remove a chart at the specific index. |
| [clear()](#clear--)| Clear all charts. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### get(number) {#get-number-}

Gets the [Chart](../chart/) element at the specified index.

```javascript
get(index: number) : Chart;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The zero based index of the element. |

**Returns**

The element at the specified index.

### get(string) {#get-string-}

Gets the chart by the name.

```javascript
get(name: string) : Chart;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The chart name. |

**Returns**

The chart.

**Remarks**

The default chart name is null. So you have to explicitly set the name of the chart.

### addFloatingChart(ChartType, number, number, number, number) {#addFloatingChart-charttype-number-number-number-number-}

Adds a chart to the collection.

```javascript
addFloatingChart(type: ChartType, left: number, top: number, width: number, height: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [ChartType](../charttype/) | Chart type |
| left | number | The x offset to corner |
| top | number | The y offset to corner |
| width | number | The chart width |
| height | number | The chart height |

**Returns**

[Chart](../chart/) object index.

### add(ChartType, number, number, number, number) {#add-charttype-number-number-number-number-}

Adds a chart to the collection.

```javascript
add(type: ChartType, topRow: number, leftColumn: number, bottomRow: number, rightColumn: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [ChartType](../charttype/) | Chart type |
| topRow | number | Upper left row index. |
| leftColumn | number | Upper left column index. |
| bottomRow | number | Lower right row index |
| rightColumn | number | Lower right column index |

**Returns**

[Chart](../chart/) object index.

### add(Uint8Array, string, boolean, number, number, number, number) {#add-uint8array-string-boolean-number-number-number-number-}

Adds a chart with preset template.

```javascript
add(data: Uint8Array, dataRange: string, isVertical: boolean, topRow: number, leftColumn: number, rightRow: number, bottomColumn: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| data | number[] | The data of chart template file(.crtx). |
| dataRange | string | Specifies the data range of the chart |
| isVertical | boolean | Specifies whether to plot the series from a range of cell values by row or by column. |
| topRow | number | Upper left row index. |
| leftColumn | number | Upper left column index. |
| rightRow | number | Lower right row index |
| bottomColumn | number | Lower right column index |

**Returns**

[Chart](../chart/) object index.

### add(ChartType, string, boolean, number, number, number, number) {#add-charttype-string-boolean-number-number-number-number-}

Adds a chart to the collection.

```javascript
add(type: ChartType, dataRange: string, isVertical: boolean, topRow: number, leftColumn: number, rightRow: number, bottomColumn: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [ChartType](../charttype/) | Chart type |
| dataRange | string | Specifies the data range of the chart |
| isVertical | boolean | Specifies whether to plot the series from a range of cell values by row or by column. |
| topRow | number | Upper left row index. |
| leftColumn | number | Upper left column index. |
| rightRow | number | Lower right row index |
| bottomColumn | number | Lower right column index |

**Returns**

[Chart](../chart/) object index.

### removeAt(number) {#removeAt-number-}

Remove a chart at the specific index.

```javascript
removeAt(index: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The chart index. |

### clear() {#clear--}

Clear all charts.

```javascript
clear() : void;
```


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



