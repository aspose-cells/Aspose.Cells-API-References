---
title: "SeriesCollection Class"
linktitle: "SeriesCollection"
articleTitle: "SeriesCollection"
second_title: "Aspose.Cells for Python via Java"
description: "Encapsulates a collection of Series objects."
type: docs
weight: 5740
url: /python-java/asposecells.api/seriescollection/
---

## SeriesCollection class

Encapsulates a collection of Series objects.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [CategoryData](#categorydata) | String | Gets or sets the range of category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values  |
| [SecondCategoryData](#secondcategorydata) | String | Gets or sets the range of second category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of  |
| [IsColorVaried](#iscolorvaried) | boolean | Represents if the color of points is varied. |
| [Count](#count) | int |  |
| [Item (int)](#itemint) | Series | Gets the Series element at the specified index. |

## Methods

| Name | Description |
| --- | --- |
| [getSeriesByOrder](#getseriesbyorder) | Gets the Series element by order. |
| [removeAt](#removeat) | Remove at a series at the specific index. |
| [changeSeriesOrder](#changeseriesorder) | Directly changes the orders of the two series.

NOTE: This method is now obsolete. Instead, please use SeriesCollection. |
| [swapSeries](#swapseries) | Directly changes the orders of the two series. |
| [setSeriesNames](#setseriesnames) | Sets the name of all the serieses in the chart.

If the start index is larger than the count of the serieses, it will re |
| [addR1C1](#addr1c1) | Adds the Series collection to a chart.

If set data on contiguous cells, use colon to seperate them.For example, R[1]C[1 |
| [add](#add) | Adds the Series collection to a chart.

If set data on contiguous cells, use colon to seperate them.For example, $C$2:$C |
| [clear](#clear) | Clears the collection |
| [changeColors](#changecolors) |  |
| [iterator](#iterator) |  |
| [get](#get) | Reserved for internal use. |
| [contains](#contains) | Reserved for internal use. |
| [indexOf](#indexof) | Reserved for internal use. |

### SeriesCollection.CategoryData property {#categorydata}

Gets or sets the range of category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}").

**Type:** String

### SeriesCollection.SecondCategoryData property {#secondcategorydata}

Gets or sets the range of second category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}"). Only effects when some ASerieses plot on the second axis.

**Type:** String

### SeriesCollection.IsColorVaried property {#iscolorvaried}

Represents if the color of points is varied.

**Type:** boolean

### SeriesCollection.Count property {#count}

**Type:** int

### SeriesCollection.Item (int) property {#itemint}

Gets the Series element at the specified index.

**Type:** Series

### getSeriesByOrder(order) {#getseriesbyorder}

Gets the Series element by order.

| Parameter | Type | Description |
| --- | --- | --- |
| order | int | The order of series |

**Returns:** The element series

### removeAt(index) {#removeat}

Remove at a series at the specific index.

| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The index. |

### changeSeriesOrder(sourceIndex, destIndex) {#changeseriesorder}

Directly changes the orders of the two series.

NOTE: This method is now obsolete. Instead, please use SeriesCollection.SwapSeries method. This method will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceIndex | int | The current index |
| destIndex | int | The dest index |

### swapSeries(sourceIndex, destIndex) {#swapseries}

Directly changes the orders of the two series.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceIndex | int | The current index |
| destIndex | int | The dest index |

### setSeriesNames(startIndex, area, isVertical) {#setseriesnames}

Sets the name of all the serieses in the chart.

If the start index is larger than the count of the serieses, it will return and do nothing. If set data on contiguous cells, use colon to seperate them.For example, $C$2:$C$5. If set data on contiguous cells, use comma to seperate them.For example, ($C$2,$D$5).

| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | int | The index of the first series which you want to set the name. |
| area | String | Specifies the area for the series name. |
| isVertical | boolean | >Specifies whether to plot the series from a range of cell values by row or by column. |

### addR1C1(area, isVertical) {#addr1c1}

Adds the Series collection to a chart.

If set data on contiguous cells, use colon to seperate them.For example, R[1]C[1]:R[3]C[2]. If set data on contiguous cells, use comma to seperate them.For example,(R[1]C[1],R[3]C[2]).

| Parameter | Type | Description |
| --- | --- | --- |
| area | String | Specifies values from which to plot the data series |
| isVertical | boolean | Specifies whether to plot the series from a range of cell values by row or by column. |

**Returns:** Return the first index of the added ASeries in the NSeries.

### add(dataArea, isVertical) (1 of 3) {#add}

Adds the Series collection to a chart.

If set data on contiguous cells, use colon to seperate them.For example, $C$2:$C$5. If set data on non contiguous cells, use comma to seperate them.For example: ($C$2,$D$5).

| Parameter | Type | Description |
| --- | --- | --- |
| area |  | Specifies values from which to plot the data series |
| isVertical | boolean | Specifies whether to plot the series from a range of cell values by row or by column. |

**Returns:** Return the first index of the added ASeries in the NSeries.

---

### add(area, isVertical, checkLabels) (2 of 3) {#add-1}

Adds the Series collection to a chart.

If set data on contiguous cells, use colon to seperate them.For example, $C$2:$C$5. If set data on non contiguous cells, use comma to seperate them.For example, ($C$2,$D$5).

| Parameter | Type | Description |
| --- | --- | --- |
| area | String | Specifies values from which to plot the data series |
| isVertical | boolean | Specifies whether to plot the series from a range of cell values by row or by column. |
| checkLabels | boolean | Indicates whether the range contains series's name |

**Returns:** Return the first index of the added ASeries in the NSeries.

---

### add(value) (3 of 3) {#add-2}

Reserved for internal use.

### clear() {#clear}

Clears the collection

### changeColors(type) {#changecolors}

### iterator() {#iterator}

### get(index) {#get}

Reserved for internal use.

### contains(value) {#contains}

Reserved for internal use.

### indexOf(value) {#indexof}

Reserved for internal use.
