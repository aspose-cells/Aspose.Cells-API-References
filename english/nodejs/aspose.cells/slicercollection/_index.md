---
title: "SlicerCollection"
linktitle: "SlicerCollection"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Specifies the collection of all the Slicer objects on the specified worksheet."
type: docs
weight: 3750
url: /nodejs/aspose.cells/slicercollection/
---

## SlicerCollection class

Specifies the collection of all the Slicer objects on the specified worksheet.

## Methods

| Name | Description |
| --- | --- |
| [add(pivot, destCellName, baseFieldName)](#add) | Add a new Slicer using PivotTable as data source |
| [add(pivot, row, column, baseFieldName)](#add-1) | Add a new Slicer using PivotTable as data source |
| [add(pivot, row, column, baseFieldIndex)](#add-2) | Add a new Slicer using PivotTable as data source |
| [add(pivot, destCellName, baseFieldIndex)](#add-3) | Add a new Slicer using PivotTable as data source |
| [add(pivot, row, column, baseField)](#add-4) | Add a new Slicer using PivotTable as data source |
| [add(pivot, destCellName, baseField)](#add-5) | Add a new Slicer using PivotTable as data source |
| [add(table, index, destCellName)](#add-6) | Add a new Slicer using ListObjet as data source |
| [add(table, listColumn, destCellName)](#add-7) | Add a new Slicer using ListObjet as data source |
| [add(table, listColumn, row, column)](#add-8) | Add a new Slicer using ListObjet as data source |
| [add()](#add-9) | Reserved for internal use. |
| [clear()](#clear) |  |
| [contains()](#contains) | Reserved for internal use. |
| [get()](#get) | Gets the Slicer by index. |
| [get()](#get-1) | Gets the Slicer by slicer's name. |
| [get()](#get-2) | Reserved for internal use. |
| [getCount()](#getcount) |  |
| [indexOf()](#indexof) | Reserved for internal use. |
| [iterator()](#iterator) |  |
| [remove(slicer)](#remove) | Remove the specified Slicer |
| [removeAt(index)](#removeat) | Deletes the Slicer at the specified index |

### add(pivot, destCellName, baseFieldName) {#add}

Add a new Slicer using PivotTable as data source

| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| destCellName | String | The cell in the upper-left corner of the Slicer range. |
| baseFieldName | String | The name of PivotField in PivotTable.BaseFields |

**Returns:** Number — `Number` The new add Slicer index

### add(pivot, row, column, baseFieldName) {#add-1}

Add a new Slicer using PivotTable as data source

| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| row | Number | Row index of the cell in the upper-left corner of the Slicer range. |
| column | Number | Column index of the cell in the upper-left corner of the Slicer range. |
| baseFieldName | String | The name of PivotField in PivotTable.BaseFields |

**Returns:** Number — `Number` The new add Slicer index

### add(pivot, row, column, baseFieldIndex) {#add-2}

Add a new Slicer using PivotTable as data source

| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| row | Number | Row index of the cell in the upper-left corner of the Slicer range. |
| column | Number | Column index of the cell in the upper-left corner of the Slicer range. |
| baseFieldIndex | Number | The index of PivotField in PivotTable.BaseFields |

**Returns:** Number — `Number` The new add Slicer index

### add(pivot, destCellName, baseFieldIndex) {#add-3}

Add a new Slicer using PivotTable as data source

| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| destCellName | String | The cell in the upper-left corner of the Slicer range. |
| baseFieldIndex | Number | The index of PivotField in PivotTable.BaseFields |

**Returns:** Number — `Number` The new add Slicer index

### add(pivot, row, column, baseField) {#add-4}

Add a new Slicer using PivotTable as data source

| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| row | Number | Row index of the cell in the upper-left corner of the Slicer range. |
| column | Number | Column index of the cell in the upper-left corner of the Slicer range. |
| baseField | PivotField | The PivotField in PivotTable.BaseFields |

**Returns:** Number — `Number` The new add Slicer index

### add(pivot, destCellName, baseField) {#add-5}

Add a new Slicer using PivotTable as data source

| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| destCellName | String | The cell in the upper-left corner of the Slicer range. |
| baseField | PivotField | The PivotField in PivotTable.BaseFields |

**Returns:** Number — `Number` The new add Slicer index

### add(table, index, destCellName) {#add-6}

Add a new Slicer using ListObjet as data source

| Parameter | Type | Description |
| --- | --- | --- |
| table | ListObject | ListObject object |
| index | Number | The index of ListColumn in ListObject.ListColumns |
| destCellName | String | The cell in the upper-left corner of the Slicer range. |

**Returns:** Number — `Number` The new add Slicer index

### add(table, listColumn, destCellName) {#add-7}

Add a new Slicer using ListObjet as data source

| Parameter | Type | Description |
| --- | --- | --- |
| table | ListObject | ListObject object |
| listColumn | ListColumn | The ListColumn in ListObject.ListColumns |
| destCellName | String | The cell in the upper-left corner of the Slicer range. |

**Returns:** Number — `Number` The new add Slicer index

### add(table, listColumn, row, column) {#add-8}

Add a new Slicer using ListObjet as data source

| Parameter | Type | Description |
| --- | --- | --- |
| table | ListObject | ListObject object |
| listColumn | ListColumn | The ListColumn in ListObject.ListColumns |
| row | Number | Row index of the cell in the upper-left corner of the Slicer range. |
| column | Number | Column index of the cell in the upper-left corner of the Slicer range. |

**Returns:** Number — `Number` The new add Slicer index

### add() {#add-9}

Reserved for internal use.

### clear() {#clear}

### contains() {#contains}

Reserved for internal use.

### get() {#get}

Gets the Slicer by index.

### get() {#get-1}

Gets the Slicer by slicer's name.

### get() {#get-2}

Reserved for internal use.

### getCount() {#getcount}

### indexOf() {#indexof}

Reserved for internal use.

### iterator() {#iterator}

### remove(slicer) {#remove}

Remove the specified Slicer

| Parameter | Type | Description |
| --- | --- | --- |
| slicer | Slicer | The Slicer object |

### removeAt(index) {#removeat}

Deletes the Slicer at the specified index

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The position index in Slicer collection |
