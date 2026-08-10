---
title: "ValidationCollection Class"
linktitle: "ValidationCollection"
articleTitle: "ValidationCollection"
second_title: "Aspose.Cells for Python via Java"
description: "Represents data validation collection."
type: docs
weight: 7250
url: /python-java/asposecells.api/validationcollection/
---

## ValidationCollection class

Represents data validation collection.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Count](#count) | int |  |
| [Item (int)](#itemint) | Validation | Gets the Validation element at the specified index. |

## Methods

| Name | Description |
| --- | --- |
| [add](#add) | Adds a data validation to the collection.

NOTE: This member is now obsolete. Instead, please use ValidationCollection.A |
| [removeACell](#removeacell) | Removes all validation setting on the cell. |
| [removeArea](#removearea) | Removes all validation setting on the range.. |
| [getValidationInCell](#getvalidationincell) | Gets the validation applied to given cell. |
| [clear](#clear) |  |
| [removeAt](#removeat) |  |
| [iterator](#iterator) |  |
| [get](#get) | Reserved for internal use. |
| [contains](#contains) | Reserved for internal use. |
| [indexOf](#indexof) | Reserved for internal use. |

### ValidationCollection.Count property {#count}

**Type:** int

### ValidationCollection.Item (int) property {#itemint}

Gets the Validation element at the specified index.

**Type:** Validation

### add() (1 of 3) {#add}

Adds a data validation to the collection.

NOTE: This member is now obsolete. Instead, please use ValidationCollection.Add(CellArea) method. This property will be removed 12 months later since JANUARY 2015. Aspose apologizes for any inconvenience you may have experienced.

**Returns:** Validation object index.

---

### add(ca) (2 of 3) {#add-1}

Adds a data validation to the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| ca | CellArea | The area contains this validation. |

**Returns:** Validation object index.

---

### add(value) (3 of 3) {#add-2}

Reserved for internal use.

### removeACell(row, column) {#removeacell}

Removes all validation setting on the cell.

| Parameter | Type | Description |
| --- | --- | --- |
| row | int | The row index of the cell. |
| column | int | The column index of the cell. |

### removeArea(ca) {#removearea}

Removes all validation setting on the range..

| Parameter | Type | Description |
| --- | --- | --- |
| ca | CellArea | The range which contains the validations setting. |

### getValidationInCell(row, column) {#getvalidationincell}

Gets the validation applied to given cell.

| Parameter | Type | Description |
| --- | --- | --- |
| row | int | The row index. |
| column | int | The column index. |

**Returns:** Returns a Validation object or null if there is no validation for given cell

### clear() {#clear}

### removeAt(index) {#removeat}

### iterator() {#iterator}

### get(index) {#get}

Reserved for internal use.

### contains(value) {#contains}

Reserved for internal use.

### indexOf(value) {#indexof}

Reserved for internal use.
