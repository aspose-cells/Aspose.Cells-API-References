---
title: "Workbook.createWorkbookFromStream"
linktitle: "createWorkbookFromStream"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Initializes a new instance of the Workbook class and open a stream."
type: docs
weight: 970
url: /nodejs/aspose.cells/workbook/createworkbookfromstream-1/
---

## createWorkbookFromStream(stream, loadOptions, callback) (static)

Initializes a new instance of the Workbook class and open a stream.

| Parameter | Type | Description |
| --- | --- | --- |
| stream | ReadableStream | The stream |
| loadOptions | LoadOptions | The load options |
| callback | Callback | The callback function |

**Example:**

```js
var aspose = aspose || {};
aspose.cells = require("aspose.cells");
var fs = require("fs");
var readStream = fs.createReadStream("Book2.xlsx");
var loadOptions = new aspose.cells.LoadOptions();
aspose.cells.Workbook.createWorkbookFromStream(readStream, loadOptions, function(workbook, err) {
if (err) {
console.log("open workbook error");
return;
}
workbook.save('result.xlsx');
console.log('saved to file');
});
```
