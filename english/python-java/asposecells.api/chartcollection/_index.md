---
title: "ChartCollection Class"
linktitle: "ChartCollection"
articleTitle: "ChartCollection"
second_title: "Aspose.Cells for Python via Java"
description: "Encapsulates a collection of Chart objects."
type: docs
weight: 740
url: /python-java/asposecells.api/chartcollection/
---

## ChartCollection class

Encapsulates a collection of Chart objects.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Count](#count) | int |  |
| [Item (int)](#itemint) | Chart | Gets the Chart element at the specified index. |
| [Item (java.lang.String)](#itemjavalangstring) | Chart | Gets the chart by the name. The default chart name is null. So you have to explicitly set the name of the chart. |

## Methods

| Name | Description |
| --- | --- |
| [addFloatingChart](#addfloatingchart) | Adds a chart to the collection. |
| [add](#add) | Adds a chart to the collection. |
| [remove](#remove) | Remove the specific chart. |
| [removeAt](#removeat) | Remove a chart at the specific index. |
| [clear](#clear) | Clear all charts. |
| [iterator](#iterator) |  |
| [get](#get) | Reserved for internal use. |
| [contains](#contains) | Reserved for internal use. |
| [indexOf](#indexof) | Reserved for internal use. |

### ChartCollection.Count property {#count}

**Type:** int

### ChartCollection.Item (int) property {#itemint}

Gets the Chart element at the specified index.

**Type:** Chart

### ChartCollection.Item (java.lang.String) property {#itemjavalangstring}

Gets the chart by the name. The default chart name is null. So you have to explicitly set the name of the chart.

**Type:** Chart

### addFloatingChart(type, left, top, width, height) {#addfloatingchart}

Adds a chart to the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| type | int | A ChartType value. Chart type |
| left | int | The x offset to corner |
| top | int | The y offset to corner |
| width | int | The chart width |
| height | int | The chart height |

**Returns:** Chart object index.

### add(type, topRow, leftColumn, bottomRow, rightColumn) (1 of 5) {#add}

Adds a chart to the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| type | int | A ChartType value. Chart type |
| upperLeftRow |  | Upper left row index. |
| upperLeftColumn |  | Upper left column index. |
| lowerRightRow |  | Lower right row index |
| lowerRightColumn |  | Lower right column index |

**Returns:** Chart object index.

---

### add(type, dataRange, topRow, leftColumn, rightRow, bottomColumn) (2 of 5) {#add-1}

Adds a chart to the collection.

NOTE: This member is now obsolete. Instead, please use add(int, java.lang.String, boolean, int, int, int, int) property. This property will be removed 12 months later since May 2022. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| type | int | A ChartType value. Chart type |
| dataRange | String | Specifies the data range of the chart |
| topRow | int | Upper left row index. |
| leftColumn | int | Upper left column index. |
| rightRow | int | Lower right row index |
| bottomColumn | int | Lower right column index |

**Returns:** Chart object index.

---

### add(data, dataRange, isVertical, topRow, leftColumn, rightRow, bottomColumn) (3 of 5) {#add-2}

Adds a chart with preset template.

| Parameter | Type | Description |
| --- | --- | --- |
| data | byte[] | The data of chart template file(.crtx). |
| dataRange | String | Specifies the data range of the chart |
| isVertical | boolean | Specifies whether to plot the series from a range of cell values by row or by column. |
| topRow | int | Upper left row index. |
| leftColumn | int | Upper left column index. |
| rightRow | int | Lower right row index |
| bottomColumn | int | Lower right column index |

**Returns:** Chart object index.

---

### add(type, dataRange, isVertical, topRow, leftColumn, rightRow, bottomColumn) (4 of 5) {#add-3}

Adds a chart to the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| type | int | A ChartType value. Chart type |
| dataRange | String | Specifies the data range of the chart |
| isVertical | boolean | Specifies whether to plot the series from a range of cell values by row or by column. |
| topRow | int | Upper left row index. |
| leftColumn | int | Upper left column index. |
| rightRow | int | Lower right row index |
| bottomColumn | int | Lower right column index |

**Returns:** Chart object index.

---

### add(value) (5 of 5) {#add-4}

Reserved for internal use.

### remove(chart) {#remove}

Remove the specific chart.

| Parameter | Type | Description |
| --- | --- | --- |
| chart | Chart |  |

### removeAt(index) {#removeat}

Remove a chart at the specific index.

| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The chart index. |

### clear() {#clear}

Clear all charts.

### iterator() {#iterator}

### get(index) {#get}

Reserved for internal use.

### contains(value) {#contains}

Reserved for internal use.

### indexOf(value) {#indexof}

Reserved for internal use.
