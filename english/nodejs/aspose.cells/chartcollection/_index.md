---
title: "ChartCollection"
linktitle: "ChartCollection"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Encapsulates a collection of Chart objects."
type: docs
weight: 510
url: /nodejs/aspose.cells/chartcollection/
---

## ChartCollection class

Encapsulates a collection of Chart objects.

## Methods

| Name | Description |
| --- | --- |
| [add(type, upperLeftRow, upperLeftColumn, lowerRightRow, lowerRightColumn)](#add) | Adds a chart to the collection. |
| [add(type, dataRange, topRow, leftColumn, rightRow, bottomColumn)](#add-1) | Adds a chart to the collection. NOTE: This member is now obsolete. Instead, please use add(int, java.lang.String, boolea |
| [add(data, dataRange, isVertical, topRow, leftColumn, rightRow, bottomColumn)](#add-2) | Adds a chart with preset template. |
| [add(type, dataRange, isVertical, topRow, leftColumn, rightRow, bottomColumn)](#add-3) | Adds a chart to the collection. |
| [add()](#add-4) | Reserved for internal use. |
| [addFloatingChart(type, left, top, width, height)](#addfloatingchart) | Adds a chart to the collection. |
| [clear()](#clear) | Clear all charts. |
| [contains()](#contains) | Reserved for internal use. |
| [get(index)](#get) | Gets the Chart element at the specified index. |
| [get(name)](#get-1) | Gets the chart by the name. The default chart name is null. So you have to explicitly set the name of the chart. |
| [get()](#get-2) | Reserved for internal use. |
| [getCount()](#getcount) |  |
| [indexOf()](#indexof) | Reserved for internal use. |
| [iterator()](#iterator) |  |
| [remove(chart)](#remove) | Remove the specific chart. |
| [removeAt(index)](#removeat) | Remove a chart at the specific index. |

### add(type, upperLeftRow, upperLeftColumn, lowerRightRow, lowerRightColumn) {#add}

Adds a chart to the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | ChartType |
| upperLeftRow |  | Upper left row index. |
| upperLeftColumn |  | Upper left column index. |
| lowerRightRow |  | Lower right row index |
| lowerRightColumn |  | Lower right column index |

**Returns:** Number — `Number` Chart object index.

### add(type, dataRange, topRow, leftColumn, rightRow, bottomColumn) {#add-1}

Adds a chart to the collection. NOTE: This member is now obsolete. Instead, please use add(int, java.lang.String, boolean, int, int, int, int) property. This property will be removed 12 months later since May 2022. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | ChartType |
| dataRange | String | Specifies the data range of the chart |
| topRow | Number | Upper left row index. |
| leftColumn | Number | Upper left column index. |
| rightRow | Number | Lower right row index |
| bottomColumn | Number | Lower right column index |

**Returns:** Number — `Number` Chart object index.

### add(data, dataRange, isVertical, topRow, leftColumn, rightRow, bottomColumn) {#add-2}

Adds a chart with preset template.

| Parameter | Type | Description |
| --- | --- | --- |
| data | Array of byte | The data of chart template file(.crtx). |
| dataRange | String | Specifies the data range of the chart |
| isVertical | boolean | Specifies whether to plot the series from a range of cell values by row or by column. |
| topRow | Number | Upper left row index. |
| leftColumn | Number | Upper left column index. |
| rightRow | Number | Lower right row index |
| bottomColumn | Number | Lower right column index |

**Returns:** Number — `Number` Chart object index.

### add(type, dataRange, isVertical, topRow, leftColumn, rightRow, bottomColumn) {#add-3}

Adds a chart to the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | ChartType |
| dataRange | String | Specifies the data range of the chart |
| isVertical | boolean | Specifies whether to plot the series from a range of cell values by row or by column. |
| topRow | Number | Upper left row index. |
| leftColumn | Number | Upper left column index. |
| rightRow | Number | Lower right row index |
| bottomColumn | Number | Lower right column index |

**Returns:** Number — `Number` Chart object index.

### add() {#add-4}

Reserved for internal use.

### addFloatingChart(type, left, top, width, height) {#addfloatingchart}

Adds a chart to the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | ChartType |
| left | Number | The x offset to corner |
| top | Number | The y offset to corner |
| width | Number | The chart width |
| height | Number | The chart height |

**Returns:** Number — `Number` Chart object index.

### clear() {#clear}

Clear all charts.

### contains() {#contains}

Reserved for internal use.

### get(index) {#get}

Gets the Chart element at the specified index.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The zero based index of the element. |

**Returns:** Chart — `Chart` The element at the specified index.

### get(name) {#get-1}

Gets the chart by the name. The default chart name is null. So you have to explicitly set the name of the chart.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The chart name. |

**Returns:** Chart — `Chart` The chart.

### get() {#get-2}

Reserved for internal use.

### getCount() {#getcount}

### indexOf() {#indexof}

Reserved for internal use.

### iterator() {#iterator}

### remove(chart) {#remove}

Remove the specific chart.

| Parameter | Type | Description |
| --- | --- | --- |
| chart | Chart |  |

### removeAt(index) {#removeat}

Remove a chart at the specific index.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The chart index. |
