---
title: ChartPointCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a collection that contains all the points in one series.
type: docs
url: /nodejs-cpp/chartpointcollection/
---

## ChartPointCollection class

Represents a collection that contains all the points in one series.

```javascript
class ChartPointCollection;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the [ChartPoint](/nodejs-cpp/chartpoint/) element at the specified index in the series. |
| [getCount()](#getCount--)| Gets the count of the chart point. |
| [getEnumerator()](#getEnumerator--)| Returns an enumerator for the entire [ChartPointCollection](/nodejs-cpp/chartpointcollection/). |
| [clear()](#clear--)| Remove all setting of the chart points. |
| [removeAt(number)](#removeAt-number-)| Removes point at the index of the series.. |


### get(number) {#get-number-}

Gets the [ChartPoint](/nodejs-cpp/chartpoint/) element at the specified index in the series.

```javascript
get(index: number) : ChartPoint;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index of chart point in the series. |

**Returns**

The ChartPoint object.

### getCount() {#getCount--}

Gets the count of the chart point.

```javascript
getCount() : number;
```


### getEnumerator() {#getEnumerator--}

Returns an enumerator for the entire [ChartPointCollection](/nodejs-cpp/chartpointcollection/).

```javascript
getEnumerator() : ChartPointEnumerator;
```


**Returns**

[ChartPointEnumerator](/nodejs-cpp/chartpointenumerator/)

### clear() {#clear--}

Remove all setting of the chart points.

```javascript
clear() : void;
```


### removeAt(number) {#removeAt-number-}

Removes point at the index of the series..

```javascript
removeAt(index: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index of the point. |


