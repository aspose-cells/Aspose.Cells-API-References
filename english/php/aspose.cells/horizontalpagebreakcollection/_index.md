---
title: "HorizontalPageBreakCollection Class"
linktitle: "HorizontalPageBreakCollection"
articleTitle: "HorizontalPageBreakCollection"
second_title: "Aspose.Cells for PHP via Java"
description: "Encapsulates a collection of HorizontalPageBreak objects."
type: docs
weight: 2840
url: /php/aspose.cells/horizontalpagebreakcollection/
---

## HorizontalPageBreakCollection class

Encapsulates a collection of HorizontalPageBreak objects.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Count](#count) | Number |  |
| [Item (int)](#itemint) | HorizontalPageBreak | Gets the HorizontalPageBreak element at the specified index. |
| [Item (java.lang.String)](#itemjavalangstring) | HorizontalPageBreak | Gets the HorizontalPageBreak element with the specified cell name. |

## Methods

| Name | Description |
| --- | --- |
| [add](#add) | Adds a horizontal page break to the collection.

This method is used to add a horizontal pagebreak within a print area. |
| [removeAt](#removeat) | Removes the HPageBreak element at a specified name. |
| [clear](#clear) |  |
| [iterator](#iterator) |  |
| [get](#get) | Reserved for internal use. |
| [contains](#contains) | Reserved for internal use. |
| [indexOf](#indexof) | Reserved for internal use. |

### HorizontalPageBreakCollection.Count property {#count}

**Type:** Number

### HorizontalPageBreakCollection.Item (int) property {#itemint}

Gets the HorizontalPageBreak element at the specified index.

**Type:** HorizontalPageBreak

### HorizontalPageBreakCollection.Item (java.lang.String) property {#itemjavalangstring}

Gets the HorizontalPageBreak element with the specified cell name.

**Type:** HorizontalPageBreak

### add(row, startColumn, endColumn) (1 of 5) {#add}

Adds a horizontal page break to the collection.

This method is used to add a horizontal pagebreak within a print area.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Row index, zero based. |
| startColumn | Number | Start column index, zero based. |
| endColumn | Number | End column index, zero based. |

**Returns:** HorizontalPageBreak object index.

---

### add(row) (2 of 5) {#add-1}

Adds a horizontal page break to the collection.

Page break is added in the top left of the cell. Please set a horizontal page break and a vertical page break concurrently.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Cell row index, zero based. |

**Returns:** HorizontalPageBreak object index.

---

### add(row, column) (3 of 5) {#add-2}

Adds a horizontal page break to the collection.

Page break is added in the top left of the cell. Please set a horizontal page break and a vertical page break concurrently.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Cell row index, zero based. |
| column | Number | Cell column index, zero based. |

**Returns:** HorizontalPageBreak object index.

---

### add(cellName) (4 of 5) {#add-3}

Adds a horizontal page break to the collection.

Page break is added in the top left of the cell. Please set a horizontal page break and a vertical page break concurrently.

| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | Cell name. |

**Returns:** HorizontalPageBreak object index.

---

### add(value) (5 of 5) {#add-4}

Reserved for internal use.

### removeAt(index) {#removeat}

Removes the HPageBreak element at a specified name.

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
