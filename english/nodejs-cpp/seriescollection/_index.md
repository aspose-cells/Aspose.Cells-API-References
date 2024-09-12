---
title: SeriesCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Encapsulates a collection of Series..series objects.
type: docs
url: /nodejs-cpp/seriescollection/
---

## SeriesCollection class

Encapsulates a collection of [Series](../series/) objects.

```javascript
class SeriesCollection;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the [Series](../series/) element at the specified index. |
| [getCategoryData()](#getCategoryData--)| Gets or sets the range of category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}"). |
| [setCategoryData(string)](#setCategoryData-string-)| Gets or sets the range of category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}"). |
| [getSecondCategoryData()](#getSecondCategoryData--)| Gets or sets the range of second category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}"). Only effects when some ASerieses plot on the second axis. |
| [setSecondCategoryData(string)](#setSecondCategoryData-string-)| Gets or sets the range of second category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}"). Only effects when some ASerieses plot on the second axis. |
| [isColorVaried()](#isColorVaried--)| Represents if the color of points is varied. |
| [setIsColorVaried(boolean)](#setIsColorVaried-boolean-)| Represents if the color of points is varied. |
| [getSeriesByOrder(number)](#getSeriesByOrder-number-)| Gets the [Series](../series/) element by order. |
| [removeAt(number)](#removeAt-number-)| Remove at a series at the specific index. |
| [changeSeriesOrder(number, number)](#changeSeriesOrder-number-number-)| Directly changes the orders of the two series. |
| [swapSeries(number, number)](#swapSeries-number-number-)| Directly changes the orders of the two series. |
| [setSeriesNames(number, string, boolean)](#setSeriesNames-number-string-boolean-)| Sets the name of all the serieses in the chart. |
| [addR1C1(string, boolean)](#addR1C1-string-boolean-)| Adds the [Series](../series/) collection to a chart. |
| [add(string, boolean)](#add-string-boolean-)| Adds the [Series](../series/) collection to a chart. |
| [add(string, boolean, boolean)](#add-string-boolean-boolean-)| Adds the [Series](../series/) collection to a chart. |
| [clear()](#clear--)| Clears the collection |
| [getCount()](#getCount--)| Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### get(number) {#get-number-}

Gets the [Series](../series/) element at the specified index.

```javascript
get(index: number) : Series;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The zero based index of the element. |

**Returns**

The element at the specified index.

### getCategoryData() {#getCategoryData--}

Gets or sets the range of category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}").

```javascript
getCategoryData() : string;
```


### setCategoryData(string) {#setCategoryData-string-}

Gets or sets the range of category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}").

```javascript
setCategoryData(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getSecondCategoryData() {#getSecondCategoryData--}

Gets or sets the range of second category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}"). Only effects when some ASerieses plot on the second axis.

```javascript
getSecondCategoryData() : string;
```


### setSecondCategoryData(string) {#setSecondCategoryData-string-}

Gets or sets the range of second category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}"). Only effects when some ASerieses plot on the second axis.

```javascript
setSecondCategoryData(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### isColorVaried() {#isColorVaried--}

Represents if the color of points is varied.

```javascript
isColorVaried() : boolean;
```


### setIsColorVaried(boolean) {#setIsColorVaried-boolean-}

Represents if the color of points is varied.

```javascript
setIsColorVaried(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getSeriesByOrder(number) {#getSeriesByOrder-number-}

Gets the [Series](../series/) element by order.

```javascript
getSeriesByOrder(order: number) : Series;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| order | number | The order of series |

**Returns**

The element series

### removeAt(number) {#removeAt-number-}

Remove at a series at the specific index.

```javascript
removeAt(index: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |

### changeSeriesOrder(number, number) {#changeSeriesOrder-number-number-}

Directly changes the orders of the two series.

```javascript
changeSeriesOrder(sourceIndex: number, destIndex: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceIndex | number | The current index |
| destIndex | number | The dest index |

**Remarks**

NOTE: This method is now obsolete. Instead, please use SeriesCollection.SwapSeries method. This method will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

### swapSeries(number, number) {#swapSeries-number-number-}

Directly changes the orders of the two series.

```javascript
swapSeries(sourceIndex: number, destIndex: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceIndex | number | The current index |
| destIndex | number | The dest index |

### setSeriesNames(number, string, boolean) {#setSeriesNames-number-string-boolean-}

Sets the name of all the serieses in the chart.

```javascript
setSeriesNames(startIndex: number, area: string, isVertical: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | number | The index of the first series which you want to set the name. |
| area | string | Specifies the area for the series name. |
| isVertical | boolean | >Specifies whether to plot the series from a range of cell values by row or by column. |

**Remarks**

<br>If the start index is larger than the count of the serieses, it will return and do nothing.</br> <br>If set data on contiguous cells, use colon to seperate them.For example, $C$2:$C$5.</br> <br>If set data on contiguous cells, use comma to seperate them.For example, ($C$2,$D$5).</br>

### addR1C1(string, boolean) {#addR1C1-string-boolean-}

Adds the [Series](../series/) collection to a chart.

```javascript
addR1C1(area: string, isVertical: boolean) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| area | string | Specifies values from which to plot the data series |
| isVertical | boolean | Specifies whether to plot the series from a range of cell values by row or by column. |

**Returns**

Return the first index of the added ASeries in the NSeries.

**Remarks**

<br>If set data on contiguous cells, use colon to seperate them.For example, R[1]C[1]:R[3]C[2].</br> <br>If set data on contiguous cells, use comma to seperate them.For example,(R[1]C[1],R[3]C[2]).</br>

### add(string, boolean) {#add-string-boolean-}

Adds the [Series](../series/) collection to a chart.

```javascript
add(area: string, isVertical: boolean) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| area | string | Specifies values from which to plot the data series |
| isVertical | boolean | Specifies whether to plot the series from a range of cell values by row or by column. |

**Returns**

Return the first index of the added ASeries in the NSeries.

**Remarks**

<br>If set data on contiguous cells, use colon to seperate them.For example, $C$2:$C$5.</br> <br>If set data on non contiguous cells, use comma to seperate them.For example: ($C$2,$D$5).</br>

### add(string, boolean, boolean) {#add-string-boolean-boolean-}

Adds the [Series](../series/) collection to a chart.

```javascript
add(area: string, isVertical: boolean, checkLabels: boolean) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| area | string | Specifies values from which to plot the data series |
| isVertical | boolean | Specifies whether to plot the series from a range of cell values by row or by column. |
| checkLabels | boolean | Indicates whether the range contains series's name |

**Returns**

Return the first index of the added ASeries in the NSeries.

**Remarks**

<br>If set data on contiguous cells, use colon to seperate them.For example, $C$2:$C$5.</br> <br>If set data on non contiguous cells, use comma to seperate them.For example, ($C$2,$D$5).</br>

### clear() {#clear--}

Clears the collection

```javascript
clear() : void;
```


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



