---
title: "PictureCollection.addPictureFromStream"
linktitle: "addPictureFromStream"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Adds a picture to the collection."
type: docs
weight: 140
url: /nodejs/aspose.cells/picturecollection/addpicturefromstream-1/
---

## addPictureFromStream(pictures, upperLeftRow, upperLeftColumn, stream, callback) (static)

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
