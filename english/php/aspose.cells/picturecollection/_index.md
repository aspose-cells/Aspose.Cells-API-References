---
title: "PictureCollection Class"
linktitle: "PictureCollection"
articleTitle: "PictureCollection"
second_title: "Aspose.Cells for PHP via Java"
description: "Encapsulates a collection of Picture objects."
type: docs
weight: 4420
url: /php/aspose.cells/picturecollection/
---

## PictureCollection class

Encapsulates a collection of Picture objects.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Count](#count) | Number |  |
| [Item (int)](#itemint) | Picture | Gets the Picture element at the specified index. |

## Methods

| Name | Description |
| --- | --- |
| [camera](#camera) |  |
| [add](#add) | Adds a picture to the collection. |
| [clear](#clear) | Clear all pictures. |
| [removeAt](#removeat) | Remove shapes at the specific index |
| [iterator](#iterator) |  |
| [get](#get) | Reserved for internal use. |
| [contains](#contains) | Reserved for internal use. |
| [indexOf](#indexof) | Reserved for internal use. |

### PictureCollection.Count property {#count}

**Type:** Number

### PictureCollection.Item (int) property {#itemint}

Gets the Picture element at the specified index.

**Type:** Picture

### camera(row, column, range) {#camera}

### add(topRow, leftColumn, bottomRow, rightColumn, fileName) (1 of 3) {#add}

Adds a picture to the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| upperLeftColumn |  | Upper left column index. |
| lowerRightRow |  | Lower right row index |
| lowerRightColumn |  | Lower right column index |
| fileName | String | Image filename. |

**Returns:** Picture object index.

---

### add(topRow, leftColumn, fileName) (2 of 3) {#add-1}

Adds a picture to the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| upperLeftColumn |  | Upper left column index. |
| fileName | String | Image filename. |

**Returns:** Picture object index.

---

### add(topRow, leftColumn, fileName, widthScale, heightScale) (3 of 3) {#add-2}

Adds a picture to the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| upperLeftColumn |  | Upper left column index. |
| fileName | String | Image filename. |
| widthScale | Number | Scale of image width, a percentage. |
| heightScale | Number | Scale of image height, a percentage. |

**Returns:** Picture object index.

### clear() {#clear}

Clear all pictures.

### removeAt(index) {#removeat}

Remove shapes at the specific index

### iterator() {#iterator}

### get(index) {#get}

Reserved for internal use.

### contains(value) {#contains}

Reserved for internal use.

### indexOf(value) {#indexof}

Reserved for internal use.
