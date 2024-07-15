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


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets a [Trendline](../trendline/) object by its index. |
| [add(TrendlineType)](#add-trendlinetype-)| Adds a [Trendline](../trendline/) object to this collection with specified type. |
| [add(TrendlineType, string)](#add-trendlinetype-string-)| Adds a [Trendline](../trendline/) object to this collection with specified type and name. |
| [getCount()](#getCount--)| Gets the number of elements contained in. |


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



