---
title: "VerticalPageBreakCollection Class"
linktitle: "VerticalPageBreakCollection"
articleTitle: "VerticalPageBreakCollection"
second_title: "Aspose.Cells for PHP via Java"
description: "Encapsulates a collection of VerticalPageBreak objects."
type: docs
weight: 7350
url: /php/aspose.cells/verticalpagebreakcollection/
---

## VerticalPageBreakCollection class

Encapsulates a collection of VerticalPageBreak objects.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Count](#count) | Number |  |
| [Item (int)](#itemint) | VerticalPageBreak | Gets the VerticalPageBreak element at the specified index. |
| [Item (java.lang.String)](#itemjavalangstring) | VerticalPageBreak | Gets the VerticalPageBreak element with the specified cell name. |

## Methods

| Name | Description |
| --- | --- |
| [add](#add) | Adds a vertical page break to the collection.

This method is used to add a vertical pagebreak within a print area. |
| [removeAt](#removeat) | Removes the VPageBreak element at a specified name. |
| [clear](#clear) |  |
| [iterator](#iterator) |  |
| [get](#get) | Reserved for internal use. |
| [contains](#contains) | Reserved for internal use. |
| [indexOf](#indexof) | Reserved for internal use. |

### VerticalPageBreakCollection.Count property {#count}

**Type:** Number

### VerticalPageBreakCollection.Item (int) property {#itemint}

Gets the VerticalPageBreak element at the specified index.

**Type:** VerticalPageBreak

### VerticalPageBreakCollection.Item (java.lang.String) property {#itemjavalangstring}

Gets the VerticalPageBreak element with the specified cell name.

**Type:** VerticalPageBreak

### add(startRow, endRow, column) (1 of 5) {#add}

Adds a vertical page break to the collection.

This method is used to add a vertical pagebreak within a print area.

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Number | Start row index, zero based. |
| endRow | Number | End row index, zero based. |
| column | Number | Column index, zero based. |

**Returns:** VerticalPageBreak object index.

---

### add(column) (2 of 5) {#add-1}

Adds a vertical page break to the collection.

Page break is added in the top left of the cell. Please set a horizontal page break and a vertical page break concurrently.

| Parameter | Type | Description |
| --- | --- | --- |
| column | Number | Cell column index, zero based. |

**Returns:** VerticalPageBreak object index.

---

### add(row, column) (3 of 5) {#add-2}

Adds a vertical page break to the collection.

Page break is added in the top left of the cell. Please set a horizontal page break and a vertical page break concurrently.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Cell row index, zero based. |
| column | Number | Cell column index, zero based. |

**Returns:** VerticalPageBreak object index.

---

### add(cellName) (4 of 5) {#add-3}

Adds a vertical page break to the collection.

Page break is added in the top left of the cell. Please set a horizontal page break and a vertical page break concurrently.

| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | Cell name. |

**Returns:** VerticalPageBreak object index.

---

### add(value) (5 of 5) {#add-4}

Reserved for internal use.

### removeAt(index) {#removeat}

Removes the VPageBreak element at a specified name.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | Element index, zero based. |

### clear() {#clear}

### iterator() {#iterator}

### get(index) {#get}

Reserved for internal use.

### contains(value) {#contains}

Reserved for internal use.

### indexOf(value) {#indexof}

Reserved for internal use.
