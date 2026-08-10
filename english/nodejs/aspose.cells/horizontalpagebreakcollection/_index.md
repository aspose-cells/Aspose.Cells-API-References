---
title: "HorizontalPageBreakCollection"
linktitle: "HorizontalPageBreakCollection"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Encapsulates a collection of HorizontalPageBreak objects."
type: docs
weight: 1790
url: /nodejs/aspose.cells/horizontalpagebreakcollection/
---

## HorizontalPageBreakCollection class

Encapsulates a collection of HorizontalPageBreak objects.

## Methods

| Name | Description |
| --- | --- |
| [add(row, startColumn, endColumn)](#add) | Adds a horizontal page break to the collection. This method is used to add a horizontal pagebreak within a print area. |
| [add(row)](#add-1) | Adds a horizontal page break to the collection. Page break is added in the top left of the cell. Please set a horizontal |
| [add(row, column)](#add-2) | Adds a horizontal page break to the collection. Page break is added in the top left of the cell. Please set a horizontal |
| [add(cellName)](#add-3) | Adds a horizontal page break to the collection. Page break is added in the top left of the cell. Please set a horizontal |
| [add()](#add-4) | Reserved for internal use. |
| [clear()](#clear) |  |
| [contains()](#contains) | Reserved for internal use. |
| [get(index)](#get) | Gets the HorizontalPageBreak element at the specified index. |
| [get(cellName)](#get-1) | Gets the HorizontalPageBreak element with the specified cell name. |
| [get()](#get-2) | Reserved for internal use. |
| [getCount()](#getcount) |  |
| [indexOf()](#indexof) | Reserved for internal use. |
| [iterator()](#iterator) |  |
| [removeAt(index)](#removeat) | Removes the HPageBreak element at a specified name. |

### add(row, startColumn, endColumn) {#add}

Adds a horizontal page break to the collection. This method is used to add a horizontal pagebreak within a print area.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Row index, zero based. |
| startColumn | Number | Start column index, zero based. |
| endColumn | Number | End column index, zero based. |

**Returns:** Number — `Number` HorizontalPageBreak object index.

### add(row) {#add-1}

Adds a horizontal page break to the collection. Page break is added in the top left of the cell. Please set a horizontal page break and a vertical page break concurrently.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Cell row index, zero based. |

**Returns:** Number — `Number` HorizontalPageBreak object index.

### add(row, column) {#add-2}

Adds a horizontal page break to the collection. Page break is added in the top left of the cell. Please set a horizontal page break and a vertical page break concurrently.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Cell row index, zero based. |
| column | Number | Cell column index, zero based. |

**Returns:** Number — `Number` HorizontalPageBreak object index.

### add(cellName) {#add-3}

Adds a horizontal page break to the collection. Page break is added in the top left of the cell. Please set a horizontal page break and a vertical page break concurrently.

| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | Cell name. |

**Returns:** Number — `Number` HorizontalPageBreak object index.

### add() {#add-4}

Reserved for internal use.

### clear() {#clear}

### contains() {#contains}

Reserved for internal use.

### get(index) {#get}

Gets the HorizontalPageBreak element at the specified index.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The zero based index of the element. |

**Returns:** HorizontalPageBreak — `HorizontalPageBreak` The element at the specified index.

### get(cellName) {#get-1}

Gets the HorizontalPageBreak element with the specified cell name.

| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | Cell name. |

**Returns:** HorizontalPageBreak — `HorizontalPageBreak` The element with the specified cell name.

### get() {#get-2}

Reserved for internal use.

### getCount() {#getcount}

### indexOf() {#indexof}

Reserved for internal use.

### iterator() {#iterator}

### removeAt(index) {#removeat}

Removes the HPageBreak element at a specified name.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | Element index, zero based. |
