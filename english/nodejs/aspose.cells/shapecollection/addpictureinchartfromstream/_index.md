---
title: "ShapeCollection.addPictureInChartFromStream"
linktitle: "addPictureInChartFromStream"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Adds a picture to the chart."
type: docs
weight: 590
url: /nodejs/aspose.cells/shapecollection/addpictureinchartfromstream/
---

## addPictureInChartFromStream(pictures, top, left, stream, widthScale, heightScale, callback) (static)

Adds a picture to the chart.

| Parameter | Type | Description |
| --- | --- | --- |
| pictures | PictureCollection | The PictureCollection object |
| top | Number | Represents the vertical offset of shape from the upper left corner in units of 1/4000 of the chart area |
| left | Number | Represents the horizontal offset of shape from the upper left corner in units of 1/4000 of the chart area |
| stream | ReadableStream | Stream object which contains the image data |
| widthScale | Number | Scale of image width, a percentage |
| heightScale | Number | Scale of image height, a percentage |
| callback | Callback | The callback function |

**Returns:** object — `object` Returns a Picture objct

**Example:**

```js
var aspose = aspose || {};
aspose.cells = require("aspose.cells");
var fs = require("fs");
var workbook = new aspose.cells.Workbook("Book2.xlsx");
var shapes = workbook.getWorksheets().get("Chart").getCharts().get(0).getShapes();
var shapeStream = fs.createReadStream("boxing.PNG");
aspose.cells.ShapeCollection.addPictureInChartFromStream(shapes, 1, 1, shapeStream, 10, 5,
function(picture, err) {
if (!err) {
console.log("addPictureInChartFromStream done");
}
workbook.save('result.xlsx');
}
);
```
