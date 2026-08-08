---
title: "FileFormatUtil.detectFileFormatFromStream"
linktitle: "detectFileFormatFromStream"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Detects and returns the information about a format of an excel stored in a stream."
type: docs
weight: 50
url: /nodejs/aspose.cells/fileformatutil/detectfileformatfromstream/
---

## detectFileFormatFromStream(stream, callback) (static)

Detects and returns the information about a format of an excel stored in a stream.

| Parameter | Type | Description |
| --- | --- | --- |
| stream | ReadableStream | The stream |
| callback | Callback | The callback function |

**Returns:** FileFormatInfo — `FileFormatInfo` A FileFormatInfo object that contains the detected information.

**Example:**

```js
var aspose = aspose || {};
aspose.cells = require("aspose.cells");
var fs = require("fs");
var readStream = fs.createReadStream("Book2.xlsx");
aspose.cells.FileFormatUtil.detectFileFormatFromStream(readStream, function(result, err) {
if (!err) {
console.log("detect result: " + result.getFileFormatType());
}
});
```
