---
title: "TimelineCollection Class"
linktitle: "TimelineCollection"
articleTitle: "TimelineCollection"
second_title: "Aspose.Cells for PHP via Java"
description: "Specifies the collection of all the Timeline objects on the specified worksheet."
type: docs
weight: 7030
url: /php/aspose.cells/timelinecollection/
---

## TimelineCollection class

Specifies the collection of all the Timeline objects on the specified worksheet. Due to MS Excel, Excel 2003 does not support Timeline.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Count](#count) | Number |  |
| [Item (int)](#itemint) | Timeline | Gets the Timeline by index. |
| [Item (java.lang.String)](#itemjavalangstring) | Timeline | Gets the Timeline by Timeline's name. |

## Methods

| Name | Description |
| --- | --- |
| [add](#add) | Add a new Timeline using PivotTable as data source |
| [clear](#clear) |  |
| [removeAt](#removeat) |  |
| [iterator](#iterator) |  |
| [get](#get) | Reserved for internal use. |
| [contains](#contains) | Reserved for internal use. |
| [indexOf](#indexof) | Reserved for internal use. |

### TimelineCollection.Count property {#count}

**Type:** Number

### TimelineCollection.Item (int) property {#itemint}

Gets the Timeline by index.

**Type:** Timeline

### TimelineCollection.Item (java.lang.String) property {#itemjavalangstring}

Gets the Timeline by Timeline's name.

**Type:** Timeline

### add(pivot, row, column, baseFieldName) (1 of 7) {#add}

Add a new Timeline using PivotTable as data source

| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| row | Number | Row index of the cell in the upper-left corner of the Timeline range. |
| column | Number | Column index of the cell in the upper-left corner of the Timeline range. |
| baseFieldName | String | The name of PivotField in PivotTable.BaseFields |

**Returns:** The new add Timeline index

---

### add(pivot, destCellName, baseFieldName) (2 of 7) {#add-1}

Add a new Timeline using PivotTable as data source

| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| destCellName | String | The cell name in the upper-left corner of the Timeline range. |
| baseFieldName | String | The name of PivotField in PivotTable.BaseFields |

**Returns:** The new add Timeline index

---

### add(pivot, row, column, baseFieldIndex) (3 of 7) {#add-2}

Add a new Timeline using PivotTable as data source

| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| row | Number | Row index of the cell in the upper-left corner of the Timeline range. |
| column | Number | Column index of the cell in the upper-left corner of the Timeline range. |
| baseFieldIndex | Number | The index of PivotField in PivotTable.BaseFields |

**Returns:** The new add Timeline index

---

### add(pivot, destCellName, baseFieldIndex) (4 of 7) {#add-3}

Add a new Timeline using PivotTable as data source

| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| destCellName | String | The cell name in the upper-left corner of the Timeline range. |
| baseFieldIndex | Number | The index of PivotField in PivotTable.BaseFields |

**Returns:** The new add Timeline index

---

### add(pivot, row, column, baseField) (5 of 7) {#add-4}

Add a new Timeline using PivotTable as data source

| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| row | Number | Row index of the cell in the upper-left corner of the Timeline range. |
| column | Number | Column index of the cell in the upper-left corner of the Timeline range. |
| baseField | PivotField | The PivotField in PivotTable.BaseFields |

**Returns:** The new add Timeline index

---

### add(pivot, destCellName, baseField) (6 of 7) {#add-5}

Add a new Timeline using PivotTable as data source

| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| destCellName | String | The cell name in the upper-left corner of the Timeline range. |
| baseField | PivotField | The PivotField in PivotTable.BaseFields |

**Returns:** The new add Timeline index

---

### add(value) (7 of 7) {#add-6}

Reserved for internal use.

### clear() {#clear}

### removeAt(index) {#removeat}

### iterator() {#iterator}

### get(index) {#get}

Reserved for internal use.

### contains(value) {#contains}

Reserved for internal use.

### indexOf(value) {#indexof}

Reserved for internal use.
