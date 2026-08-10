---
title: "HtmlTableLoadOptionCollection Class"
linktitle: "HtmlTableLoadOptionCollection"
articleTitle: "HtmlTableLoadOptionCollection"
second_title: "Aspose.Cells for PHP via Java"
description: "Represents the table options when importing html."
type: docs
weight: 2990
url: /php/aspose.cells/htmltableloadoptioncollection/
---

## HtmlTableLoadOptionCollection class

Represents the table options when importing html.

## Constructors

| Name | Description |
| --- | --- |
| [HtmlTableLoadOptionCollection](#constructor) |  |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [TableToListObject](#tabletolistobject) | boolean | Indicates whether generate list objects from imported tables. The default value is false. |
| [Count](#count) | Number |  |
| [Item (int)](#itemint) | HtmlTableLoadOption | Gets the HtmlTableLoadOption element at the specified index. |

## Methods

| Name | Description |
| --- | --- |
| [add](#add) | Adds one HtmlTableLoadOption into this collection. |
| [addTableLoadOption](#addtableloadoption) |  |
| [clear](#clear) |  |
| [removeAt](#removeat) |  |
| [iterator](#iterator) |  |
| [get](#get) | Reserved for internal use. |
| [contains](#contains) | Reserved for internal use. |
| [indexOf](#indexof) | Reserved for internal use. |

### HtmlTableLoadOptionCollection() {#constructor}

### HtmlTableLoadOptionCollection.TableToListObject property {#tabletolistobject}

Indicates whether generate list objects from imported tables. The default value is false.

**Type:** boolean

### HtmlTableLoadOptionCollection.Count property {#count}

**Type:** Number

### HtmlTableLoadOptionCollection.Item (int) property {#itemint}

Gets the HtmlTableLoadOption element at the specified index.

**Type:** HtmlTableLoadOption

### add(item) (1 of 7) {#add}

Adds one HtmlTableLoadOption into this collection.

| Parameter | Type | Description |
| --- | --- | --- |
| item | HtmlTableLoadOption | one HtmlTableLoadOption |

**Returns:** the index of the added item

---

### add(tableIndex) (2 of 7) {#add-1}

Add a HtmlTableLoadOption to the list.

| Parameter | Type | Description |
| --- | --- | --- |
| tableIndex | Number | Table index |

---

### add(tableId) (3 of 7) {#add-2}

Add a HtmlTableLoadOption to the list.

| Parameter | Type | Description |
| --- | --- | --- |
| tableId | String | Table ID |

---

### add(tableIndex, targetSheetIndex) (4 of 7) {#add-3}

Add a HtmlTableLoadOption to the list.

| Parameter | Type | Description |
| --- | --- | --- |
| tableIndex | Number | Table index |
| targetSheetIndex | Number | The target index of worksheet in Excel |

---

### add(tableId, targetSheetIndex) (5 of 7) {#add-4}

Add a HtmlTableLoadOption to the list.

| Parameter | Type | Description |
| --- | --- | --- |
| tableId | String | Table ID |
| targetSheetIndex | Number | The target index of worksheet in Excel |

---

### add(tableIndex, targetSheetIndex, originalSheetIndex) (6 of 7) {#add-5}

Add a HtmlTableLoadOption to the list.

| Parameter | Type | Description |
| --- | --- | --- |
| tableIndex | Number | Table index |
| targetSheetIndex | Number | The target index of worksheet in Excel |
| originalSheetIndex | Number | The original index of worksheet in the html |

---

### add(tableId, targetSheetIndex, originalSheetIndex) (7 of 7) {#add-6}

Add a HtmlTableLoadOption to the list.

| Parameter | Type | Description |
| --- | --- | --- |
| tableId | String | Table ID |
| targetSheetIndex | Number | The target index of worksheet in Excel |
| originalSheetIndex | Number | The original index of worksheet in the html |

### addTableLoadOption(item) {#addtableloadoption}

### clear() {#clear}

### removeAt(index) {#removeat}

### iterator() {#iterator}

### get(index) {#get}

Reserved for internal use.

### contains(value) {#contains}

Reserved for internal use.

### indexOf(value) {#indexof}

Reserved for internal use.
