---
title: "TextBoxCollection Class"
linktitle: "TextBoxCollection"
articleTitle: "TextBoxCollection"
second_title: "Aspose.Cells for Python via Java"
description: "Encapsulates a collection of TextBox objects."
type: docs
weight: 6640
url: /python-java/asposecells.api/textboxcollection/
---

## TextBoxCollection class

Encapsulates a collection of TextBox objects.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Count](#count) | int |  |
| [Item (int)](#itemint) | TextBox | Gets the TextBox element at the specified index. |
| [Item (java.lang.String)](#itemjavalangstring) | TextBox | Gets the TextBox element by the name. |

## Methods

| Name | Description |
| --- | --- |
| [add](#add) | Adds a textbox to the collection. |
| [removeAt](#removeat) | Remove a text box from the file. |
| [clear](#clear) | Clear all text boxes. |
| [iterator](#iterator) |  |
| [get](#get) | Reserved for internal use. |
| [contains](#contains) | Reserved for internal use. |
| [indexOf](#indexof) | Reserved for internal use. |

### TextBoxCollection.Count property {#count}

**Type:** int

### TextBoxCollection.Item (int) property {#itemint}

Gets the TextBox element at the specified index.

**Type:** TextBox

### TextBoxCollection.Item (java.lang.String) property {#itemjavalangstring}

Gets the TextBox element by the name.

**Type:** TextBox

### add(topRow, leftColumn, height, width) (1 of 2) {#add}

Adds a textbox to the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| upperLeftColumn |  | Upper left column index. |
| height | int | Height of textbox, in unit of pixel. |
| width | int | Width of textbox, in unit of pixel. |

**Returns:** TextBox object index.

---

### add(value) (2 of 2) {#add-1}

Reserved for internal use.

### removeAt(index) {#removeat}

Remove a text box from the file.

| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The text box index. |

### clear() {#clear}

Clear all text boxes.

### iterator() {#iterator}

### get(index) {#get}

Reserved for internal use.

### contains(value) {#contains}

Reserved for internal use.

### indexOf(value) {#indexof}

Reserved for internal use.
