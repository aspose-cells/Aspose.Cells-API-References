---
title: "SlicerCollection Class"
linktitle: "SlicerCollection"
articleTitle: "SlicerCollection"
second_title: "Aspose.Cells for Python via Java"
description: "Specifies the collection of all the Slicer objects on the specified worksheet."
type: docs
weight: 6120
url: /python-java/asposecells.api/slicercollection/
---

## SlicerCollection class

Specifies the collection of all the Slicer objects on the specified worksheet.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Count](#count) | int |  |
| [Item (int)](#itemint) | Slicer | Gets the Slicer by index. |
| [Item (java.lang.String)](#itemjavalangstring) | Slicer | Gets the Slicer by slicer's name. |

## Methods

| Name | Description |
| --- | --- |
| [remove](#remove) | Remove the specified Slicer |
| [removeAt](#removeat) | Deletes the Slicer at the specified index |
| [clear](#clear) |  |
| [add](#add) | Add a new Slicer using PivotTable as data source |
| [iterator](#iterator) |  |
| [get](#get) | Reserved for internal use. |
| [contains](#contains) | Reserved for internal use. |
| [indexOf](#indexof) | Reserved for internal use. |

### SlicerCollection.Count property {#count}

**Type:** int

### SlicerCollection.Item (int) property {#itemint}

Gets the Slicer by index.

**Type:** Slicer

### SlicerCollection.Item (java.lang.String) property {#itemjavalangstring}

Gets the Slicer by slicer's name.

**Type:** Slicer

### remove(slicer) {#remove}

Remove the specified Slicer

| Parameter | Type | Description |
| --- | --- | --- |
| slicer | Slicer | The Slicer object |

### removeAt(index) {#removeat}

Deletes the Slicer at the specified index

| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The position index in Slicer collection |

### clear() {#clear}

### add(pivot, destCellName, baseFieldName) (1 of 10) {#add}

Add a new Slicer using PivotTable as data source

| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| destCellName | String | The cell in the upper-left corner of the Slicer range. |
| baseFieldName | String | The name of PivotField in PivotTable.BaseFields |

**Returns:** The new add Slicer index

---

### add(pivot, row, column, baseFieldName) (2 of 10) {#add-1}

Add a new Slicer using PivotTable as data source

| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| row | int | Row index of the cell in the upper-left corner of the Slicer range. |
| column | int | Column index of the cell in the upper-left corner of the Slicer range. |
| baseFieldName | String | The name of PivotField in PivotTable.BaseFields |

**Returns:** The new add Slicer index

---

### add(pivot, row, column, baseFieldIndex) (3 of 10) {#add-2}

Add a new Slicer using PivotTable as data source

| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| row | int | Row index of the cell in the upper-left corner of the Slicer range. |
| column | int | Column index of the cell in the upper-left corner of the Slicer range. |
| baseFieldIndex | int | The index of PivotField in PivotTable.BaseFields |

**Returns:** The new add Slicer index

---

### add(pivot, destCellName, baseFieldIndex) (4 of 10) {#add-3}

Add a new Slicer using PivotTable as data source

| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| destCellName | String | The cell in the upper-left corner of the Slicer range. |
| baseFieldIndex | int | The index of PivotField in PivotTable.BaseFields |

**Returns:** The new add Slicer index

---

### add(pivot, row, column, baseField) (5 of 10) {#add-4}

Add a new Slicer using PivotTable as data source

| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| row | int | Row index of the cell in the upper-left corner of the Slicer range. |
| column | int | Column index of the cell in the upper-left corner of the Slicer range. |
| baseField | PivotField | The PivotField in PivotTable.BaseFields |

**Returns:** The new add Slicer index

---

### add(pivot, destCellName, baseField) (6 of 10) {#add-5}

Add a new Slicer using PivotTable as data source

| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| destCellName | String | The cell in the upper-left corner of the Slicer range. |
| baseField | PivotField | The PivotField in PivotTable.BaseFields |

**Returns:** The new add Slicer index

---

### add(table, index, destCellName) (7 of 10) {#add-6}

Add a new Slicer using ListObjet as data source

| Parameter | Type | Description |
| --- | --- | --- |
| table | ListObject | ListObject object |
| index | int | The index of ListColumn in ListObject.ListColumns |
| destCellName | String | The cell in the upper-left corner of the Slicer range. |

**Returns:** The new add Slicer index

---

### add(table, listColumn, destCellName) (8 of 10) {#add-7}

Add a new Slicer using ListObjet as data source

| Parameter | Type | Description |
| --- | --- | --- |
| table | ListObject | ListObject object |
| listColumn | ListColumn | The ListColumn in ListObject.ListColumns |
| destCellName | String | The cell in the upper-left corner of the Slicer range. |

**Returns:** The new add Slicer index

---

### add(table, listColumn, row, column) (9 of 10) {#add-8}

Add a new Slicer using ListObjet as data source

| Parameter | Type | Description |
| --- | --- | --- |
| table | ListObject | ListObject object |
| listColumn | ListColumn | The ListColumn in ListObject.ListColumns |
| row | int | Row index of the cell in the upper-left corner of the Slicer range. |
| column | int | Column index of the cell in the upper-left corner of the Slicer range. |

**Returns:** The new add Slicer index

---

### add(value) (10 of 10) {#add-9}

Reserved for internal use.

### iterator() {#iterator}

### get(index) {#get}

Reserved for internal use.

### contains(value) {#contains}

Reserved for internal use.

### indexOf(value) {#indexof}

Reserved for internal use.
