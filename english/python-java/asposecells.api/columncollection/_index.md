---
title: "ColumnCollection Class"
linktitle: "ColumnCollection"
articleTitle: "ColumnCollection"
second_title: "Aspose.Cells for Python via Java"
description: "Collection of the Column objects that represent the individual column(setting)s in a worksheet."
type: docs
weight: 1010
url: /python-java/asposecells.api/columncollection/
---

## ColumnCollection class

Collection of the Column objects that represent the individual column(setting)s in a worksheet. The Column object only represents the settings such as column width, styles, .etc. for the whole column, has nothing to do with the fact that there are non-empty cells(data) or not in corresponding column. And the "Count" of this collection only represents the count Column objects that have been instantiated in this collection, has nothing to do with the fact that there are non-empty cells(data) or not in the worksheet.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Count](#count) | int |  |
| [Item (int)](#itemint) | Column | Gets a Column object by column index. The Column object of given column index will be instantiated if it does not exist  |

## Methods

| Name | Description |
| --- | --- |
| [getByIndex](#getbyindex) | Gets the column object by the index.

NOTE: This member is now obsolete. Instead, please use Columns.GetColumnByIndex()  |
| [getColumnByIndex](#getcolumnbyindex) | Gets the Column object by the position in the list. |
| [clear](#clear) |  |
| [removeAt](#removeat) |  |
| [iterator](#iterator) |  |
| [get](#get) | Reserved for internal use. |
| [contains](#contains) | Reserved for internal use. |
| [add](#add) | Reserved for internal use. |
| [indexOf](#indexof) | Reserved for internal use. |

### ColumnCollection.Count property {#count}

**Type:** int

### ColumnCollection.Item (int) property {#itemint}

Gets a Column object by column index. The Column object of given column index will be instantiated if it does not exist before.

**Type:** Column

### getByIndex(index) {#getbyindex}

Gets the column object by the index.

NOTE: This member is now obsolete. Instead, please use Columns.GetColumnByIndex() method. This property will be removed 12 months later since June 2010. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| index | int |  |

**Returns:** Returns the column object.

### getColumnByIndex(index) {#getcolumnbyindex}

Gets the Column object by the position in the list.

| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The position in the list. |

**Returns:** Returns the column object.

### clear() {#clear}

### removeAt(index) {#removeat}

### iterator() {#iterator}

### get(index) {#get}

Reserved for internal use.

### contains(value) {#contains}

Reserved for internal use.

### add(value) {#add}

Reserved for internal use.

### indexOf(value) {#indexof}

Reserved for internal use.
