---
title: "ListObjectCollection Class"
linktitle: "ListObjectCollection"
articleTitle: "ListObjectCollection"
second_title: "Aspose.Cells for PHP via Java"
description: "Represents a collection of ListObject objects in the worksheet."
type: docs
weight: 3450
url: /php/aspose.cells/listobjectcollection/
---

## ListObjectCollection class

Represents a collection of ListObject objects in the worksheet.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Count](#count) | Number |  |
| [Item (int)](#itemint) | ListObject | Gets the ListObject by index. |
| [Item (java.lang.String)](#itemjavalangstring) | ListObject | Gets the ListObject by specified name. |

## Methods

| Name | Description |
| --- | --- |
| [add](#add) | Adds a ListObject to the worksheet. |
| [removeAt](#removeat) |  |
| [updateColumnName](#updatecolumnname) | Update all column name of the tables. |
| [clear](#clear) |  |
| [iterator](#iterator) |  |
| [get](#get) | Reserved for internal use. |
| [contains](#contains) | Reserved for internal use. |
| [indexOf](#indexof) | Reserved for internal use. |

### ListObjectCollection.Count property {#count}

**Type:** Number

### ListObjectCollection.Item (int) property {#itemint}

Gets the ListObject by index.

**Type:** ListObject

### ListObjectCollection.Item (java.lang.String) property {#itemjavalangstring}

Gets the ListObject by specified name.

**Type:** ListObject

### add(startRow, startColumn, endRow, endColumn, hasHeaders) (1 of 3) {#add}

Adds a ListObject to the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Number | The start row of the list range. |
| startColumn | Number | The start row of the list range. |
| endRow | Number | The start row of the list range. |
| endColumn | Number | The start row of the list range. |
| hasHeaders | boolean | Whether the range has headers. |

**Returns:** The index of the new ListObject

---

### add(startCell, endCell, hasHeaders) (2 of 3) {#add-1}

Adds a ListObject to the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| startCell | String | The start cell of the list range. |
| endCell | String | The end cell of the list range. |
| hasHeaders | boolean | Whether the range has headers. |

**Returns:** The index of the new ListObject

---

### add(value) (3 of 3) {#add-2}

Reserved for internal use.

### removeAt(index) {#removeat}

### updateColumnName() {#updatecolumnname}

Update all column name of the tables.

### clear() {#clear}

### iterator() {#iterator}

### get(index) {#get}

Reserved for internal use.

### contains(value) {#contains}

Reserved for internal use.

### indexOf(value) {#indexof}

Reserved for internal use.
