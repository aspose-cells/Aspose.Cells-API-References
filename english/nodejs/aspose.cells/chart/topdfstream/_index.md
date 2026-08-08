---
title: "Chart.toPdfStream"
linktitle: "toPdfStream"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Creates the chart pdf and saves it to a stream."
type: docs
weight: 1010
url: /nodejs/aspose.cells/chart/topdfstream/
---

## toPdfStream(chart, stream) (static)

Creates the chart pdf and saves it to a stream.

| Parameter | Type | Description |
| --- | --- | --- |
| chart | Chart | The Chart object |
| stream | WritableStream | The output stream |

**Example:**

```js
var aspose = aspose || {};
aspose.cells = require("aspose.cells");
var fs = require("fs");
var workbook = new aspose.cells.Workbook("Book2.xlsx");
var chart = workbook.getWorksheets().get("Chart").getCharts().get(0);
var imgWriteStream = fs.createWriteStream("chart.pdf");
aspose.cells.Chart.toPdfStream(chart, imgWriteStream);
```
