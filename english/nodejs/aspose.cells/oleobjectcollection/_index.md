---
title: "OleObjectCollection"
linktitle: "OleObjectCollection"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents embedded OLE objects."
type: docs
weight: 2450
url: /nodejs/aspose.cells/oleobjectcollection/
---

## OleObjectCollection class

Represents embedded OLE objects.

## Methods

| Name | Description |
| --- | --- |
| [add(upperLeftRow, upperLeftColumn, height, width, imageData)](#add) | Adds an OleObject to the collection. |
| [add(upperLeftRow, upperLeftColumn, height, width, imageData, linkedFile)](#add-1) | Adds a linked OleObject to the collection. |
| [add()](#add-2) | Reserved for internal use. |
| [clear()](#clear) | Remove all embedded OLE objects. |
| [contains()](#contains) | Reserved for internal use. |
| [get(index)](#get) | Gets the OleObject element at the specified index. |
| [get()](#get-1) | Reserved for internal use. |
| [getCount()](#getcount) |  |
| [indexOf()](#indexof) | Reserved for internal use. |
| [iterator()](#iterator) |  |
| [removeAt(index)](#removeat) | Removes the element at the specified index. |

### add(upperLeftRow, upperLeftColumn, height, width, imageData) {#add}

Adds an OleObject to the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| upperLeftColumn |  | Upper left column index. |
| height | Number | Height of oleObject, in unit of pixel. |
| width | Number | Width of oleObject, in unit of pixel. |
| imageData | Array of byte | Image of ole object as byte array. |

**Returns:** Number — `Number` OleObject object index.

### add(upperLeftRow, upperLeftColumn, height, width, imageData, linkedFile) {#add-1}

Adds a linked OleObject to the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| upperLeftColumn |  | Upper left column index. |
| height | Number | Height of oleObject, in unit of pixel. |
| width | Number | Width of oleObject, in unit of pixel. |
| imageData | Array of byte | Image of ole object as byte array. |
| linkedFile | String |  |

**Returns:** Number — `Number` OleObject object index.

### add() {#add-2}

Reserved for internal use.

### clear() {#clear}

Remove all embedded OLE objects.

### contains() {#contains}

Reserved for internal use.

### get(index) {#get}

Gets the OleObject element at the specified index.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The zero based index of the element. |

**Returns:** OleObject — `OleObject` The element at the specified index.

### get() {#get-1}

Reserved for internal use.

### getCount() {#getcount}

### indexOf() {#indexof}

Reserved for internal use.

### iterator() {#iterator}

### removeAt(index) {#removeat}

Removes the element at the specified index.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The specified index. |
