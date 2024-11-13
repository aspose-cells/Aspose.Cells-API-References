---
title: TrendlineCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a collection of all the Trendline..trendline objects for the specified data series.
type: docs
url: /nodejs-cpp/trendlinecollection/
---

## TrendlineCollection class

Represents a collection of all the [Trendline](../trendline/) objects for the specified data series.

```javascript
class TrendlineCollection;
```


### Example
```javascript
const { Workbook, ChartType, TrendlineType, Color } = require("aspose.cells.node");

var excel = new Workbook();
var chartIndex = excel.getWorksheets().get(0).getCharts().add(ChartType.Column, 3, 3, 15, 10);
var chart = excel.getWorksheets().get(0).getCharts().get(chartIndex);
chart.getNSeries().add("A1:a3", true);
chart.getNSeries().get(0).getTrendLines().add(TrendlineType.Linear, "MyTrendLine");
var line = chart.getNSeries().get(0).getTrendLines().get(0);
line.setDisplayEquation(true);
line.setDisplayRSquared(true);
line.setColor(Color.Red);
```
## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets a [Trendline](../trendline/) object by its index. |
| [add(TrendlineType)](#add-trendlinetype-)| Adds a [Trendline](../trendline/) object to this collection with specified type. |
| [add(TrendlineType, string)](#add-trendlinetype-string-)| Adds a [Trendline](../trendline/) object to this collection with specified type and name. |
| [getCount()](#getCount--)| Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### get(number) {#get-number-}

Gets a [Trendline](../trendline/) object by its index.

```javascript
get(index: number) : Trendline;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number |  |

**Returns**

[Trendline](../trendline/)

### add(TrendlineType) {#add-trendlinetype-}

Adds a [Trendline](../trendline/) object to this collection with specified type.

```javascript
add(type: TrendlineType) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [TrendlineType](../trendlinetype/) | Trendline type. |

**Returns**

[Trendline](../trendline/) object index.

### add(TrendlineType, string) {#add-trendlinetype-string-}

Adds a [Trendline](../trendline/) object to this collection with specified type and name.

```javascript
add(type: TrendlineType, name: string) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [TrendlineType](../trendlinetype/) | Trendline type. |
| name | string | Trendline name. |

**Returns**

[Trendline](../trendline/) object index.

### getCount() {#getCount--}

Gets the number of elements contained in.

```javascript
getCount() : number;
```


### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



