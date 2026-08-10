---
title: "OleObjectCollection Class"
linktitle: "OleObjectCollection"
articleTitle: "OleObjectCollection"
second_title: "Aspose.Cells for Python via Java"
description: "Represents embedded OLE objects."
type: docs
weight: 4060
url: /python-java/asposecells.api/oleobjectcollection/
---

## OleObjectCollection class

Represents embedded OLE objects.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Count](#count) | int |  |
| [Item (int)](#itemint) | OleObject | Gets the OleObject element at the specified index. |

## Methods

| Name | Description |
| --- | --- |
| [add](#add) | Adds an OleObject to the collection. |
| [clear](#clear) | Remove all embedded OLE objects. |
| [removeAt](#removeat) | Removes the element at the specified index. |
| [iterator](#iterator) |  |
| [get](#get) | Reserved for internal use. |
| [contains](#contains) | Reserved for internal use. |
| [indexOf](#indexof) | Reserved for internal use. |

### OleObjectCollection.Count property {#count}

**Type:** int

### OleObjectCollection.Item (int) property {#itemint}

Gets the OleObject element at the specified index.

**Type:** OleObject

### add(topRow, leftColumn, height, width, imageData) (1 of 3) {#add}

Adds an OleObject to the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| upperLeftColumn |  | Upper left column index. |
| height | int | Height of oleObject, in unit of pixel. |
| width | int | Width of oleObject, in unit of pixel. |
| imageData | byte[] | Image of ole object as byte array. |

**Returns:** OleObject object index.

---

### add(topRow, leftColumn, height, width, imageData, linkedFile) (2 of 3) {#add-1}

Adds a linked OleObject to the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| upperLeftColumn |  | Upper left column index. |
| height | int | Height of oleObject, in unit of pixel. |
| width | int | Width of oleObject, in unit of pixel. |
| imageData | byte[] | Image of ole object as byte array. |
| linkedFile | String |  |

**Returns:** OleObject object index.

---

### add(value) (3 of 3) {#add-2}

Reserved for internal use.

### clear() {#clear}

Remove all embedded OLE objects.

### removeAt(index) {#removeat}

Removes the element at the specified index.

| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The specified index. |

### iterator() {#iterator}

### get(index) {#get}

Reserved for internal use.

### contains(value) {#contains}

Reserved for internal use.

### indexOf(value) {#indexof}

Reserved for internal use.
