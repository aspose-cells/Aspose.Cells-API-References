---
title: "NameCollection Class"
linktitle: "NameCollection"
articleTitle: "NameCollection"
second_title: "Aspose.Cells for Python via Java"
description: "Represents a collection of all the Name objects in the spreadsheet."
type: docs
weight: 3850
url: /python-java/asposecells.api/namecollection/
---

## NameCollection class

Represents a collection of all the Name objects in the spreadsheet.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Count](#count) | int |  |
| [Item (int)](#itemint) | Name | Gets the Name element at the specified index. |
| [Item (java.lang.String)](#itemjavalangstring) | Name | Gets the Name element with the specified name. |

## Methods

| Name | Description |
| --- | --- |
| [add](#add) | Defines a new name.

Name cannot include spaces and cannot look like cell references. |
| [filter](#filter) | Gets all defined name by scope. |
| [remove](#remove) | Remove an array of name |
| [removeAt](#removeat) | Remove the name at the specific index.

Please make sure that the name is not referred by the other formulas before call |
| [clear](#clear) | Remove all defined names which are not referenced by the formulas and data source. If the defined name is referred, we o |
| [removeDuplicateNames](#removeduplicatenames) | Remove the duplicate defined names |
| [sort](#sort) | Sorts defined names.

If you create a large amount of named ranges in the Excel file, please call this method after all  |
| [iterator](#iterator) |  |
| [get](#get) | Reserved for internal use. |
| [contains](#contains) | Reserved for internal use. |
| [indexOf](#indexof) | Reserved for internal use. |

### NameCollection.Count property {#count}

**Type:** int

### NameCollection.Item (int) property {#itemint}

Gets the Name element at the specified index.

**Type:** Name

### NameCollection.Item (java.lang.String) property {#itemjavalangstring}

Gets the Name element with the specified name.

**Type:** Name

### add(text) (1 of 2) {#add}

Defines a new name.

Name cannot include spaces and cannot look like cell references.

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | The text to use as the name. |

**Returns:** Name object index.

---

### add(value) (2 of 2) {#add-1}

Reserved for internal use.

### filter(type, sheetIndex) {#filter}

Gets all defined name by scope.

| Parameter | Type | Description |
| --- | --- | --- |
| type | int | A NameScopeType value. The scope type. |
| sheetIndex | int | The sheet index. Only effects when scope type is NameScopeType.WORKSHEET |

### remove(names) (1 of 2) {#remove}

Remove an array of name

| Parameter | Type | Description |
| --- | --- | --- |
| names | String[] | The names' text. |

---

### remove(text) (2 of 2) {#remove-1}

Remove the name.

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | The name text. |

### removeAt(index) {#removeat}

Remove the name at the specific index.

Please make sure that the name is not referred by the other formulas before calling the method. And if the name is referred, setting Name.RefersTo as null is better.

| Parameter | Type | Description |
| --- | --- | --- |
| index | int | index of the Name to be removed. |

### clear() {#clear}

Remove all defined names which are not referenced by the formulas and data source. If the defined name is referred, we only set Name.ReferTo as null and hide them.

### removeDuplicateNames() {#removeduplicatenames}

Remove the duplicate defined names

### sort() {#sort}

Sorts defined names.

If you create a large amount of named ranges in the Excel file, please call this method after all named ranges are created and before saving

### iterator() {#iterator}

### get(index) {#get}

Reserved for internal use.

### contains(value) {#contains}

Reserved for internal use.

### indexOf(value) {#indexof}

Reserved for internal use.
