---
title: "ColumnCollection"
linktitle: "ColumnCollection"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Collection of the Column objects that represent the individual column(setting)s in a worksheet."
type: docs
weight: 690
url: /nodejs/aspose.cells/columncollection/
---

## ColumnCollection class

Collection of the Column objects that represent the individual column(setting)s in a worksheet. The Column object only represents the settings such as column width, styles, .etc. for the whole column, has nothing to do with the fact that there are non-empty cells(data) or not in corresponding column. And the "Count" of this collection only represents the count Column objects that have been instantiated in this collection, has nothing to do with the fact that there are non-empty cells(data) or not in the worksheet.

## Methods

| Name | Description |
| --- | --- |
| [add()](#add) | Reserved for internal use. |
| [clear()](#clear) |  |
| [contains()](#contains) | Reserved for internal use. |
| [get()](#get) | Gets a Column object by column index. The Column object of given column index will be instantiated if it does not exist  |
| [get()](#get-1) | Reserved for internal use. |
| [getByIndex(index)](#getbyindex) | Gets the column object by the index. NOTE: This member is now obsolete. Instead, please use Columns.GetColumnByIndex() m |
| [getColumnByIndex(index)](#getcolumnbyindex) | Gets the Column object by the position in the list. |
| [getCount()](#getcount) |  |
| [indexOf()](#indexof) | Reserved for internal use. |
| [iterator()](#iterator) |  |
| [removeAt()](#removeat) |  |

### add() {#add}

Reserved for internal use.

### clear() {#clear}

### contains() {#contains}

Reserved for internal use.

### get() {#get}

Gets a Column object by column index. The Column object of given column index will be instantiated if it does not exist before.

### get() {#get-1}

Reserved for internal use.

### getByIndex(index) {#getbyindex}

Gets the column object by the index. NOTE: This member is now obsolete. Instead, please use Columns.GetColumnByIndex() method. This property will be removed 12 months later since June 2010. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number |  |

**Returns:** Column — `Column` Returns the column object.

### getColumnByIndex(index) {#getcolumnbyindex}

Gets the Column object by the position in the list.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The position in the list. |

**Returns:** Column — `Column` Returns the column object.

### getCount() {#getcount}

### indexOf() {#indexof}

Reserved for internal use.

### iterator() {#iterator}

### removeAt() {#removeat}
