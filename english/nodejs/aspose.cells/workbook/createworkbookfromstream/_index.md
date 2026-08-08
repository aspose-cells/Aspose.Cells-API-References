---
title: "Workbook.createWorkbookFromStream"
linktitle: "createWorkbookFromStream"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Initializes a new instance of the Workbook class and open a stream."
type: docs
weight: 960
url: /nodejs/aspose.cells/workbook/createworkbookfromstream/
---

## createWorkbookFromStream(stream, callback) (static)

Initializes a new instance of the Workbook class and open a stream.

| Parameter | Type | Description |
| --- | --- | --- |
| stream | ReadableStream | The stream |
| callback | Callback | The callback function |

**Example:**

```js
var aspose = aspose || {};
aspose.cells = require("aspose.cells");
var fs = require("fs");
var readStream = fs.createReadStream("Book2.xlsx");
aspose.cells.Workbook.createWorkbookFromStream(readStream, function(workbook, err) {
if (err) {
console.log("open workbook error");
return;
}
workbook.save('result.xlsx');
console.log('saved to file');
});
```
