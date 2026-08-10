---
title: "SeriesCollection"
linktitle: "SeriesCollection"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Encapsulates a collection of Series objects."
type: docs
weight: 3490
url: /nodejs/aspose.cells/seriescollection/
---

## SeriesCollection class

Encapsulates a collection of Series objects.

## Methods

| Name | Description |
| --- | --- |
| [add(area, isVertical)](#add) | Adds the Series collection to a chart. If set data on contiguous cells, use colon to seperate them.For example, $C$2:$C$ |
| [add(area, isVertical, checkLabels)](#add-1) | Adds the Series collection to a chart. If set data on contiguous cells, use colon to seperate them.For example, $C$2:$C$ |
| [add()](#add-2) | Reserved for internal use. |
| [addR1C1(area, isVertical)](#addr1c1) | Adds the Series collection to a chart. If set data on contiguous cells, use colon to seperate them.For example, R[1]C[1] |
| [changeColors()](#changecolors) |  |
| [changeSeriesOrder(sourceIndex, destIndex)](#changeseriesorder) | Directly changes the orders of the two series. |
| [clear()](#clear) | Clears the collection |
| [contains()](#contains) | Reserved for internal use. |
| [get(index)](#get) | Gets the Series element at the specified index. |
| [get()](#get-1) | Reserved for internal use. |
| [getCategoryData()](#getcategorydata) | Gets or sets the range of category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values  |
| [getCount()](#getcount) |  |
| [getSecondCategoryData()](#getsecondcategorydata) | Gets or sets the range of second category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of  |
| [getSeriesByOrder(order)](#getseriesbyorder) | Gets the Series element by order. |
| [indexOf()](#indexof) | Reserved for internal use. |
| [isColorVaried()](#iscolorvaried) | Represents if the color of points is varied. |
| [iterator()](#iterator) |  |
| [removeAt(index)](#removeat) | Remove at a series at the specific index. |
| [setCategoryData()](#setcategorydata) | Gets or sets the range of category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values  |
| [setColorVaried()](#setcolorvaried) | Represents if the color of points is varied. |
| [setSecondCategoryData()](#setsecondcategorydata) | Gets or sets the range of second category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of  |
| [setSeriesNames(startIndex, area, isVertical)](#setseriesnames) | Sets the name of all the serieses in the chart. If the start index is larger than the count of the serieses, it will ret |
| [swapSeries()](#swapseries) |  |

### add(area, isVertical) {#add}

Adds the Series collection to a chart. If set data on contiguous cells, use colon to seperate them.For example, $C$2:$C$5.If set data on non contiguous cells, use comma to seperate them.For example: ($C$2,$D$5).

| Parameter | Type | Description |
| --- | --- | --- |
| area |  | Specifies values from which to plot the data series |
| isVertical | boolean | Specifies whether to plot the series from a range of cell values by row or by column. |

**Returns:** Number — `Number` Return the first index of the added ASeries in the NSeries.

### add(area, isVertical, checkLabels) {#add-1}

Adds the Series collection to a chart. If set data on contiguous cells, use colon to seperate them.For example, $C$2:$C$5.If set data on non contiguous cells, use comma to seperate them.For example, ($C$2,$D$5).

| Parameter | Type | Description |
| --- | --- | --- |
| area | String | Specifies values from which to plot the data series |
| isVertical | boolean | Specifies whether to plot the series from a range of cell values by row or by column. |
| checkLabels | boolean | Indicates whether the range contains series's name |

**Returns:** Number — `Number` Return the first index of the added ASeries in the NSeries.

### add() {#add-2}

Reserved for internal use.

### addR1C1(area, isVertical) {#addr1c1}

Adds the Series collection to a chart. If set data on contiguous cells, use colon to seperate them.For example, R[1]C[1]:R[3]C[2].If set data on contiguous cells, use comma to seperate them.For example,(R[1]C[1],R[3]C[2]).

| Parameter | Type | Description |
| --- | --- | --- |
| area | String | Specifies values from which to plot the data series |
| isVertical | boolean | Specifies whether to plot the series from a range of cell values by row or by column. |

**Returns:** Number — `Number` Return the first index of the added ASeries in the NSeries.

### changeColors() {#changecolors}

### changeSeriesOrder(sourceIndex, destIndex) {#changeseriesorder}

Directly changes the orders of the two series.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceIndex | Number | The current index |
| destIndex | Number | The dest index |

### clear() {#clear}

Clears the collection

### contains() {#contains}

Reserved for internal use.

### get(index) {#get}

Gets the Series element at the specified index.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The zero based index of the element. |

**Returns:** Series — `Series` The element at the specified index.

### get() {#get-1}

Reserved for internal use.

### getCategoryData() {#getcategorydata}

Gets or sets the range of category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}").

### getCount() {#getcount}

### getSecondCategoryData() {#getsecondcategorydata}

Gets or sets the range of second category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}"). Only effects when some ASerieses plot on the second axis.

### getSeriesByOrder(order) {#getseriesbyorder}

Gets the Series element by order.

| Parameter | Type | Description |
| --- | --- | --- |
| order | Number | The order of series |

**Returns:** Series — `Series` The element series

### indexOf() {#indexof}

Reserved for internal use.

### isColorVaried() {#iscolorvaried}

Represents if the color of points is varied.

### iterator() {#iterator}

### removeAt(index) {#removeat}

Remove at a series at the specific index.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The index. |

### setCategoryData() {#setcategorydata}

Gets or sets the range of category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}").

### setColorVaried() {#setcolorvaried}

Represents if the color of points is varied.

### setSecondCategoryData() {#setsecondcategorydata}

Gets or sets the range of second category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}"). Only effects when some ASerieses plot on the second axis.

### setSeriesNames(startIndex, area, isVertical) {#setseriesnames}

Sets the name of all the serieses in the chart. If the start index is larger than the count of the serieses, it will return and do nothing.If set data on contiguous cells, use colon to seperate them.For example, $C$2:$C$5.If set data on contiguous cells, use comma to seperate them.For example, ($C$2,$D$5).

| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | Number | The index of the first series which you want to set the name. |
| area | String | Specifies the area for the series name. |
| isVertical | boolean | Specifies whether to plot the series from a range of cell values by row or by column. |

### swapSeries() {#swapseries}
