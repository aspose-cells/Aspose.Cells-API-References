---
title: "PictureCollection"
linktitle: "PictureCollection"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Encapsulates a collection of Picture objects."
type: docs
weight: 2640
url: /nodejs/aspose.cells/picturecollection/
---

## PictureCollection class

Encapsulates a collection of Picture objects.

## Methods

| Name | Description |
| --- | --- |
| [add(upperLeftRow, upperLeftColumn, lowerRightRow, lowerRightColumn, fileName)](#add) | Adds a picture to the collection. /// |
| [add(upperLeftRow, upperLeftColumn, fileName)](#add-1) | Adds a picture to the collection. |
| [add(upperLeftRow, upperLeftColumn, fileName, widthScale, heightScale)](#add-2) | Adds a picture to the collection. |
| [camera()](#camera) |  |
| [clear()](#clear) | Clear all pictures. |
| [contains()](#contains) | Reserved for internal use. |
| [get(index)](#get) | Gets the Picture element at the specified index. |
| [get()](#get-1) | Reserved for internal use. |
| [getCount()](#getcount) |  |
| [indexOf()](#indexof) | Reserved for internal use. |
| [iterator()](#iterator) |  |
| [removeAt()](#removeat) | Remove shapes at the specific index |
| [addPictureFromStream(pictures, upperLeftRow, upperLeftColumn, lowerRightRow, lowerRightColumn, stream, callback)](#addpicturefromstream) *(static)* | Adds a picture to the collection. |
| [addPictureFromStream(pictures, upperLeftRow, upperLeftColumn, stream, callback)](#addpicturefromstream-1) *(static)* | Adds a picture to the collection. |
| [addPictureFromStream(pictures, upperLeftRow, upperLeftColumn, stream, widthScale, heightScale, callback)](#addpicturefromstream-2) *(static)* | Adds a picture to the collection. |

### add(upperLeftRow, upperLeftColumn, lowerRightRow, lowerRightColumn, fileName) {#add}

Adds a picture to the collection. ///

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| upperLeftColumn |  | Upper left column index. |
| lowerRightRow |  | Lower right row index |
| lowerRightColumn |  | Lower right column index |
| fileName | String | Image filename. |

**Returns:** Number — `Number` Picture object index.

### add(upperLeftRow, upperLeftColumn, fileName) {#add-1}

Adds a picture to the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| upperLeftColumn |  | Upper left column index. |
| fileName | String | Image filename. |

**Returns:** Number — `Number` Picture object index.

### add(upperLeftRow, upperLeftColumn, fileName, widthScale, heightScale) {#add-2}

Adds a picture to the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| upperLeftColumn |  | Upper left column index. |
| fileName | String | Image filename. |
| widthScale | Number | Scale of image width, a percentage. |
| heightScale | Number | Scale of image height, a percentage. |

**Returns:** Number — `Number` Picture object index.

### camera() {#camera}

### clear() {#clear}

Clear all pictures.

### contains() {#contains}

Reserved for internal use.

### get(index) {#get}

Gets the Picture element at the specified index.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The zero based index of the element. |

**Returns:** Picture — `Picture` The element at the specified index.

### get() {#get-1}

Reserved for internal use.

### getCount() {#getcount}

### indexOf() {#indexof}

Reserved for internal use.

### iterator() {#iterator}

### removeAt() {#removeat}

Remove shapes at the specific index

### addPictureFromStream(pictures, upperLeftRow, upperLeftColumn, lowerRightRow, lowerRightColumn, stream, callback) (static) {#addpicturefromstream}

Adds a picture to the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| pictures | PictureCollection | The PictureCollection object |
| upperLeftRow | Number | Upper left row index |
| upperLeftColumn | Number | Upper left column index |
| lowerRightRow | Number | Lower right row index |
| lowerRightColumn | Number | Lower right column index |
| stream | ReadableStream | Stream object which contains the image data |
| callback | Callback | The callback function |

**Returns:** Picture — `Picture` Picture object index.

**Example:**

```js
var aspose = aspose || {};
aspose.cells = require("aspose.cells");
var fs = require("fs");
var workbook = new aspose.cells.Workbook();
var pictures = workbook.getWorksheets().add("picture").getPictures();
var pictureStream = fs.createReadStream("boxing.PNG");
aspose.cells.PictureCollection.addPictureFromStream(pictures, 0, 0, 10, 8, pictureStream,
function(index, err) {
if (err) {
console.log("addPictureFromStream error");
return;
}
console.log("picture add index: " + index);
workbook.save('result.xlsx');
console.log('saved to file');
}
);
```

### addPictureFromStream(pictures, upperLeftRow, upperLeftColumn, stream, callback) (static) {#addpicturefromstream-1}

Adds a picture to the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| pictures | PictureCollection | The PictureCollection object |
| upperLeftRow | Number | Upper left row index |
| upperLeftColumn | Number | Upper left column index |
| stream | ReadableStream | Stream object which contains the image data |
| callback | Callback | The callback function |

**Returns:** Picture — `Picture` Picture object index.

**Example:**

```js
var aspose = aspose || {};
aspose.cells = require("aspose.cells");
var fs = require("fs");
var workbook = new aspose.cells.Workbook();
var pictures = workbook.getWorksheets().add("picture").getPictures();
var pictureStream = fs.createReadStream("boxing.PNG");
aspose.cells.PictureCollection.addPictureFromStream(pictures, 0, 0, pictureStream,
function(index, err) {
if (err) {
console.log("addPictureFromStream error");
return;
}
console.log("picture add index: " + index);
workbook.save('result.xlsx');
console.log('saved to file');
}
);
```

### addPictureFromStream(pictures, upperLeftRow, upperLeftColumn, stream, widthScale, heightScale, callback) (static) {#addpicturefromstream-2}

Adds a picture to the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| pictures | PictureCollection | The PictureCollection object |
| upperLeftRow | Number | Upper left row index |
| upperLeftColumn | Number | Upper left column index |
| stream | ReadableStream | Stream object which contains the image data |
| widthScale | Number | Scale of image width, a percentage |
| heightScale | Number | Scale of image height, a percentage |
| callback | Callback | The callback function |

**Returns:** Picture — `Picture` Picture object index.

**Example:**

```js
var aspose = aspose || {};
aspose.cells = require("aspose.cells");
var fs = require("fs");
var workbook = new aspose.cells.Workbook();
var pictures = workbook.getWorksheets().add("picture").getPictures();
var pictureStream = fs.createReadStream("boxing.PNG");
aspose.cells.PictureCollection.addPictureFromStream(pictures, 0, 0, pictureStream, 80, 60,
function(index, err) {
if (err) {
console.log("addPictureFromStream error");
return;
}
console.log("picture add index: " + index);
workbook.save('result.xlsx');
console.log('saved to file');
}
);
```
