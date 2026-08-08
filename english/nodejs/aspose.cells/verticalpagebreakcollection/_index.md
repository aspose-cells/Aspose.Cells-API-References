---
title: "VerticalPageBreakCollection"
linktitle: "VerticalPageBreakCollection"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Encapsulates a collection of VerticalPageBreak objects."
type: docs
weight: 4520
url: /nodejs/aspose.cells/verticalpagebreakcollection/
---

## VerticalPageBreakCollection class

Encapsulates a collection of VerticalPageBreak objects.

## Methods

| Name | Description |
| --- | --- |
| [add(startRow, endRow, column)](#add) | Adds a vertical page break to the collection. This method is used to add a vertical pagebreak within a print area. |
| [add(column)](#add-1) | Adds a vertical page break to the collection. Page break is added in the top left of the cell. Please set a horizontal p |
| [add(row, column)](#add-2) | Adds a vertical page break to the collection. Page break is added in the top left of the cell. Please set a horizontal p |
| [add(cellName)](#add-3) | Adds a vertical page break to the collection. Page break is added in the top left of the cell. Please set a horizontal p |
| [add()](#add-4) | Reserved for internal use. |
| [clear()](#clear) |  |
| [contains()](#contains) | Reserved for internal use. |
| [get(index)](#get) | Gets the VerticalPageBreak element at the specified index. |
| [get(cellName)](#get-1) | Gets the VerticalPageBreak element with the specified cell name. |
| [get()](#get-2) | Reserved for internal use. |
| [getCount()](#getcount) |  |
| [indexOf()](#indexof) | Reserved for internal use. |
| [iterator()](#iterator) |  |
| [removeAt(index)](#removeat) | Removes the VPageBreak element at a specified name. |

### add(startRow, endRow, column) {#add}

Adds a vertical page break to the collection. This method is used to add a vertical pagebreak within a print area.

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Number | Start row index, zero based. |
| endRow | Number | End row index, zero based. |
| column | Number | Column index, zero based. |

**Returns:** Number — `Number` VerticalPageBreak object index.

### add(column) {#add-1}

Adds a vertical page break to the collection. Page break is added in the top left of the cell. Please set a horizontal page break and a vertical page break concurrently.

| Parameter | Type | Description |
| --- | --- | --- |
| column | Number | Cell column index, zero based. |

**Returns:** Number — `Number` VerticalPageBreak object index.

### add(row, column) {#add-2}

Adds a vertical page break to the collection. Page break is added in the top left of the cell. Please set a horizontal page break and a vertical page break concurrently.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Cell row index, zero based. |
| column | Number | Cell column index, zero based. |

**Returns:** Number — `Number` VerticalPageBreak object index.

### add(cellName) {#add-3}

Adds a vertical page break to the collection. Page break is added in the top left of the cell. Please set a horizontal page break and a vertical page break concurrently.

| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | Cell name. |

**Returns:** Number — `Number` VerticalPageBreak object index.

### add() {#add-4}

Reserved for internal use.

### clear() {#clear}

### contains() {#contains}

Reserved for internal use.

### get(index) {#get}

Gets the VerticalPageBreak element at the specified index.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The zero based index of the element. |

**Returns:** VerticalPageBreak — `VerticalPageBreak` The element at the specified index.

### get(cellName) {#get-1}

Gets the VerticalPageBreak element with the specified cell name.

| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | Cell name. |

**Returns:** VerticalPageBreak — `VerticalPageBreak` The element with the specified cell name.

### get() {#get-2}

Reserved for internal use.

### getCount() {#getcount}

### indexOf() {#indexof}

Reserved for internal use.

### iterator() {#iterator}

### removeAt(index) {#removeat}

Removes the VPageBreak element at a specified name.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | Element index, zero based. |
