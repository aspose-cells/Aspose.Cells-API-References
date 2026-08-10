---
title: "PictureCollection Class"
linktitle: "PictureCollection"
articleTitle: "PictureCollection"
second_title: "Aspose.Cells for Python via Java"
description: "Encapsulates a collection of Picture objects."
type: docs
weight: 4420
url: /python-java/asposecells.api/picturecollection/
---

## PictureCollection class

Encapsulates a collection of Picture objects.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Count](#count) | int |  |
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
| [addPictureFromBytes](#addpicturefrombytes) | Adds a picture to the collection. |

### PictureCollection.Count property {#count}

**Type:** int

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
| widthScale | int | Scale of image width, a percentage. |
| heightScale | int | Scale of image height, a percentage. |

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

### addPictureFromBytes(upperLeftRow, upperLeftColumn, byte_array, lowerRightRow, lowerRightColumn) (1 of 3) {#addpicturefrombytes}

Adds a picture to the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | int | Upper left row index |
| upperLeftColumn | int | Upper left column index |
| byte_array | bytes | The byte array |
| lowerRightRow | int | Lower right row index |
| lowerRightColumn | int | Lower right column index |

**Returns:** Picture object index.

**Example:**

```python
import jpype
import asposecells
jpype.startJVM()
from asposecells.api import *

wb = Workbook(FileFormatType.XLSX)
with open('cells.png', 'rb') as pic:
    pic_bytes = pic.read()
    wb.getWorksheets().get(0).getPictures().addPictureFromBytes(2, 7, byte_array=pic_bytes, lowerRightRow=10, lowerRightColumn=10)
wb.save("wb.xlsx")

jpype.shutdownJVM()
```

---

### addPictureFromBytes(upperLeftRow, upperLeftColumn, byte_array) (2 of 3) {#addpicturefrombytes-1}

Adds a picture to the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | int | Upper left row index |
| upperLeftColumn | int | Upper left column index |
| byte_array | bytes | The byte array |

**Returns:** Picture object index.

**Example:**

```python
import jpype
import asposecells
jpype.startJVM()
from asposecells.api import *

wb = Workbook(FileFormatType.XLSX)
with open('cells.png', 'rb') as pic:
    pic_bytes = pic.read()
    wb.getWorksheets().get(0).getPictures().addPictureFromBytes(2, 2, byte_array=pic_bytes)
wb.save("wb.xlsx")

jpype.shutdownJVM()
```

---

### addPictureFromBytes(upperLeftRow, upperLeftColumn, widthScale, heightScale, byte_array) (3 of 3) {#addpicturefrombytes-2}

Adds a picture to the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | int | Upper left row index |
| upperLeftColumn | int | Upper left column index |
| widthScale | int | Scale of image width, a percentage |
| heightScale | int | Scale of image height, a percentage |
| byte_array | bytes | The byte array |

**Returns:** Picture object index.

**Example:**

```python
import jpype
import asposecells
jpype.startJVM()
from asposecells.api import *

wb = Workbook(FileFormatType.XLSX)
with open('cells.png', 'rb') as pic:
    pic_bytes = pic.read()
    wb.getWorksheets().get(0).getPictures().addPictureFromBytes(0, 0, widthScale=200, heightScale=150, byte_array=pic_bytes)
wb.save("wb.xlsx")

jpype.shutdownJVM()
```
