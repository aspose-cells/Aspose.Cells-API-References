---
title: "CellWatchCollection Class"
linktitle: "CellWatchCollection"
articleTitle: "CellWatchCollection"
second_title: "Aspose.Cells for PHP via Java"
description: "Represents the collection of cells on this worksheet being watched in the 'watch window'."
type: docs
weight: 610
url: /php/aspose.cells/cellwatchcollection/
---

## CellWatchCollection class

Represents the collection of cells on this worksheet being watched in the 'watch window'.

## Constructors

| Name | Description |
| --- | --- |
| [CellWatchCollection](#constructor) |  |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Count](#count) | Number |  |
| [Item (int)](#itemint) | CellWatch | Gets and sets CellWatch by index. |
| [Item (java.lang.String)](#itemjavalangstring) | CellWatch | Gets and sets CellWatch by the name of the cell. |

## Methods

| Name | Description |
| --- | --- |
| [add](#add) | Adds CellWatch with row and column. |
| [clear](#clear) |  |
| [removeAt](#removeat) |  |
| [iterator](#iterator) |  |
| [get](#get) | Reserved for internal use. |
| [contains](#contains) | Reserved for internal use. |
| [indexOf](#indexof) | Reserved for internal use. |

### CellWatchCollection() {#constructor}

### CellWatchCollection.Count property {#count}

**Type:** Number

### CellWatchCollection.Item (int) property {#itemint}

Gets and sets CellWatch by index.

**Type:** CellWatch

### CellWatchCollection.Item (java.lang.String) property {#itemjavalangstring}

Gets and sets CellWatch by the name of the cell.

**Type:** CellWatch

### add(row, column) (1 of 3) {#add}

Adds CellWatch with row and column.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | The row index. |
| column | Number | The column index. |

**Returns:** Returns the position of this item in the collection.

---

### add(cellName) (2 of 3) {#add-1}

Adds CellWatch with the name the of cell.

| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | The name of the cell. |

---

### add(value) (3 of 3) {#add-2}

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
