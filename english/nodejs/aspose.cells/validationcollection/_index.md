---
title: "ValidationCollection"
linktitle: "ValidationCollection"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents data validation collection."
type: docs
weight: 4450
url: /nodejs/aspose.cells/validationcollection/
---

## ValidationCollection class

Represents data validation collection.

## Methods

| Name | Description |
| --- | --- |
| [add()](#add) | Adds a data validation to the collection. NOTE: This member is now obsolete. Instead, please use ValidationCollection.Ad |
| [add(ca)](#add-1) | Adds a data validation to the collection. |
| [add()](#add-2) | Reserved for internal use. |
| [clear()](#clear) |  |
| [contains()](#contains) | Reserved for internal use. |
| [get(index)](#get) | Gets the Validation element at the specified index. |
| [get()](#get-1) | Reserved for internal use. |
| [getCount()](#getcount) |  |
| [getValidationInCell(row, column)](#getvalidationincell) | Gets the validation applied to given cell. |
| [indexOf()](#indexof) | Reserved for internal use. |
| [iterator()](#iterator) |  |
| [removeACell(row, column)](#removeacell) | Removes all validation setting on the cell. |
| [removeArea(ca)](#removearea) | Removes all validation setting on the range.. |
| [removeAt()](#removeat) |  |

### add() {#add}

Adds a data validation to the collection. NOTE: This member is now obsolete. Instead, please use ValidationCollection.Add(CellArea) method. This property will be removed 12 months later since JANUARY 2015. Aspose apologizes for any inconvenience you may have experienced.@return {Number} Validation object index.

### add(ca) {#add-1}

Adds a data validation to the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| ca | CellArea | The area contains this validation. |

**Returns:** Number — `Number` Validation object index.

### add() {#add-2}

Reserved for internal use.

### clear() {#clear}

### contains() {#contains}

Reserved for internal use.

### get(index) {#get}

Gets the Validation element at the specified index.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The zero based index of the element. |

**Returns:** Validation — `Validation` The element at the specified index.

### get() {#get-1}

Reserved for internal use.

### getCount() {#getcount}

### getValidationInCell(row, column) {#getvalidationincell}

Gets the validation applied to given cell.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | The row index. |
| column | Number | The column index. |

**Returns:** Validation — `Validation` Returns a Validation object or null if there is no validation for given cell

### indexOf() {#indexof}

Reserved for internal use.

### iterator() {#iterator}

### removeACell(row, column) {#removeacell}

Removes all validation setting on the cell.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | The row index of the cell. |
| column | Number | The column index of the cell. |

### removeArea(ca) {#removearea}

Removes all validation setting on the range..

| Parameter | Type | Description |
| --- | --- | --- |
| ca | CellArea | The range which contains the validations setting. |

### removeAt() {#removeat}
