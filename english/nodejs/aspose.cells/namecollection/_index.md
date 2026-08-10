---
title: "NameCollection"
linktitle: "NameCollection"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents a collection of all the Name objects in the spreadsheet."
type: docs
weight: 2320
url: /nodejs/aspose.cells/namecollection/
---

## NameCollection class

Represents a collection of all the Name objects in the spreadsheet.

## Methods

| Name | Description |
| --- | --- |
| [add(text)](#add) | Defines a new name. Name cannot include spaces and cannot look like cell references. |
| [add()](#add-1) | Reserved for internal use. |
| [clear()](#clear) | Remove all defined names which are not referenced by the formulas and data source. If the defined name is referred, we o |
| [contains()](#contains) | Reserved for internal use. |
| [filter(type, sheetIndex)](#filter) | Gets all defined name by scope. |
| [get(index)](#get) | Gets the Name element at the specified index. |
| [get(text)](#get-1) | Gets the Name element with the specified name. |
| [get()](#get-2) | Reserved for internal use. |
| [getCount()](#getcount) |  |
| [indexOf()](#indexof) | Reserved for internal use. |
| [iterator()](#iterator) |  |
| [remove(names)](#remove) | Remove an array of name |
| [remove(text)](#remove-1) | Remove the name. |
| [removeAt(index)](#removeat) | Remove the name at the specific index. Please make sure that the name is not referred by the other formulas before calli |
| [removeDuplicateNames()](#removeduplicatenames) | Remove the duplicate defined names |
| [sort()](#sort) | Sorts defined names. If you create a large amount of named ranges in the Excel file, please call this method after all n |

### add(text) {#add}

Defines a new name. Name cannot include spaces and cannot look like cell references.

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | The text to use as the name. |

**Returns:** Number — `Number` Name object index.

### add() {#add-1}

Reserved for internal use.

### clear() {#clear}

Remove all defined names which are not referenced by the formulas and data source. If the defined name is referred, we only set Name.ReferTo as null and hide them.

### contains() {#contains}

Reserved for internal use.

### filter(type, sheetIndex) {#filter}

Gets all defined name by scope.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | NameScopeType |
| sheetIndex | Number | The sheet index. Only effects when scope type is |

**Returns:** Array ofName — `Array ofName`

### get(index) {#get}

Gets the Name element at the specified index.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The zero based index of the element. |

**Returns:** Name — `Name` The element at the specified index.

### get(text) {#get-1}

Gets the Name element with the specified name.

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | Name text. |

**Returns:** Name — `Name` The element with the specified name.

### get() {#get-2}

Reserved for internal use.

### getCount() {#getcount}

### indexOf() {#indexof}

Reserved for internal use.

### iterator() {#iterator}

### remove(names) {#remove}

Remove an array of name

| Parameter | Type | Description |
| --- | --- | --- |
| names | Array of String | The names' text. |

### remove(text) {#remove-1}

Remove the name.

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | The name text. |

### removeAt(index) {#removeat}

Remove the name at the specific index. Please make sure that the name is not referred by the other formulas before calling the method. And if the name is referred, setting Name.RefersTo as null is better.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | index of the Name to be removed. |

### removeDuplicateNames() {#removeduplicatenames}

Remove the duplicate defined names

### sort() {#sort}

Sorts defined names. If you create a large amount of named ranges in the Excel file, please call this method after all named ranges are created and before saving
