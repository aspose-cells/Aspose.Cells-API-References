---
title: "ShapeCollection.addPictureFromStream"
linktitle: "addPictureFromStream"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Adds a picture to the collection."
type: docs
weight: 570
url: /nodejs/aspose.cells/shapecollection/addpicturefromstream/
---

## addPictureFromStream(pictures, upperLeftRow, upperLeftColumn, lowerRightRow, lowerRightColumn, stream, callback) (static)

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

**Returns:** object — `object` Returns a Picture objct

**Example:**

```js
var aspose = aspose || {};
aspose.cells = require("aspose.cells");
var fs = require("fs");
var workbook = new aspose.cells.Workbook();
var shapes = workbook.getWorksheets().get(0).getShapes();
var shapeStream = fs.createReadStream("boxing.PNG");
aspose.cells.ShapeCollection.addPictureFromStream(shapes, 1, 1, 10, 5, shapeStream,
function(picture, err) {
if (!err) {
console.log("addPictureFromStream done");
}
workbook.save('result.xlsx');
}
);
```
