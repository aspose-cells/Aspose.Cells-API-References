---
title: "SparklineGroupCollection Class"
linktitle: "SparklineGroupCollection"
articleTitle: "SparklineGroupCollection"
second_title: "Aspose.Cells for PHP via Java"
description: "Encapsulates a collection of SparklineGroup objects."
type: docs
weight: 6310
url: /php/aspose.cells/sparklinegroupcollection/
---

## SparklineGroupCollection class

Encapsulates a collection of SparklineGroup objects.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Count](#count) | Number |  |
| [Item (int)](#itemint) | SparklineGroup | Gets the SparklineGroup element at the specified index. |

## Methods

| Name | Description |
| --- | --- |
| [add](#add) | Adds an SparklineGroup with a Sparkline to the collection. |
| [clearSparklines](#clearsparklines) | Clears the sparklines that is inside an area of cells. |
| [clearSparklineGroups](#clearsparklinegroups) | Clears the sparkline groups that overlaps an area of cells. |
| [clear](#clear) |  |
| [removeAt](#removeat) |  |
| [iterator](#iterator) |  |
| [get](#get) | Reserved for internal use. |
| [contains](#contains) | Reserved for internal use. |
| [indexOf](#indexof) | Reserved for internal use. |

### SparklineGroupCollection.Count property {#count}

**Type:** Number

### SparklineGroupCollection.Item (int) property {#itemint}

Gets the SparklineGroup element at the specified index.

**Type:** SparklineGroup

### add(type) (1 of 3) {#add}

Adds an SparklineGroup with a Sparkline to the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | A SparklineType value. Specifies the type of the Sparkline group. |

**Returns:** SparklineGroup object index.

---

### add(type, dataRange, isVertical, locationRange) (2 of 3) {#add-1}

Adds an SparklineGroup with Sparkline to the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | A SparklineType value. Specifies the type of the Sparkline group. |
| dataRange | String | Specifies the data range of the sparkline group. |
| isVertical | boolean | Specifies whether to plot the sparklines from the data range by row or by column. |
| locationRange | CellArea | Specifies where the sparklines to be placed. |

**Returns:** SparklineGroup object index.

---

### add(value) (3 of 3) {#add-2}

Reserved for internal use.

### clearSparklines(cellArea) {#clearsparklines}

Clears the sparklines that is inside an area of cells.

| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | CellArea | Specifies the area of cells |

### clearSparklineGroups(cellArea) {#clearsparklinegroups}

Clears the sparkline groups that overlaps an area of cells.

| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | CellArea | Specifies the area of cells |

### clear() {#clear}

### removeAt(index) {#removeat}

### iterator() {#iterator}

### get(index) {#get}

Reserved for internal use.

### contains(value) {#contains}

Reserved for internal use.

### indexOf(value) {#indexof}

Reserved for internal use.
