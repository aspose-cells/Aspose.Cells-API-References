---
title: "Chart.toImage"
linktitle: "toImage"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Creates the chart image and saves it to a file."
type: docs
weight: 970
url: /nodejs/aspose.cells/chart/toimage-4/
---

## toImage(imageFile, options)

Creates the chart image and saves it to a file. The extension of the file name determines the format of the image. The format of the image is specified by using the extension of the file name. For example, if you specify "myfile.png", then the image will be saved in the PNG format. The following file extensions are recognized: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf. If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing. Please refer to Supported Charts List for more details.

| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | String | The image file name with full path. |
| options | ImageOrPrintOptions | Additional image creation options |

**Example:**

```js
var options = new aspose.cells.ImageOrPrintOptions();
options.setHorizontalResolution(300);
options.setVerticalResolution(300);
var book = new aspose.cells.Workbook("Book1.xls");
book.getWorksheets().get(0).getCharts().get(0).toImage("chart.png", options);
```
