---
title: "RowCollection Class"
linktitle: "RowCollection"
articleTitle: "RowCollection"
second_title: "Aspose.Cells for PHP via Java"
description: "Collects the Row objects that represent the individual rows in a worksheet."
type: docs
weight: 5620
url: /php/aspose.cells/rowcollection/
---

## RowCollection class

Collects the Row objects that represent the individual rows in a worksheet.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Count](#count) | Number | Gets the number of rows in this collection. |
| [Item (int)](#itemint) | Row | Gets a Row object by given row index. The Row object of given row index will be instantiated if it does not exist before |

## Methods

| Name | Description |
| --- | --- |
| [iterator](#iterator) | Gets an enumerator that iterates rows through this collection |
| [getRowByIndex](#getrowbyindex) | Gets the row object by the position in the list. |
| [clear](#clear) | Clear all rows and cells. |
| [removeAt](#removeat) | Remove the row item at the specified index(position) in this collection. |

### RowCollection.Count property {#count}

Gets the number of rows in this collection.

**Type:** Number

### RowCollection.Item (int) property {#itemint}

Gets a Row object by given row index. The Row object of given row index will be instantiated if it does not exist before.

**Type:** Row

### iterator() {#iterator}

Gets an enumerator that iterates rows through this collection

**Returns:** enumerator

### getRowByIndex(index) {#getrowbyindex}

Gets the row object by the position in the list.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The position. |

**Returns:** The Row object at given position.

### clear() {#clear}

Clear all rows and cells.

### removeAt(index) {#removeat}

Remove the row item at the specified index(position) in this collection.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | zero-based index(position, not Row.Index ) of the existing row item in this collection. |
