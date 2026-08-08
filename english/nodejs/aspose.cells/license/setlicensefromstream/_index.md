---
title: "License.setLicenseFromStream"
linktitle: "setLicenseFromStream"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Licenses the component."
type: docs
weight: 30
url: /nodejs/aspose.cells/license/setlicensefromstream/
---

## setLicenseFromStream(license, stream, callback) (static)

Licenses the component. Use this method to load a license from a stream.

| Parameter | Type | Description |
| --- | --- | --- |
| license | License | The license object |
| stream | ReadableStream | The stream |
| callback | Callback | The callback function |

**Example:**

```js
var aspose = aspose || {};
aspose.cells = require("aspose.cells");
var fs = require("fs");
var licenseStream = fs.createReadStream("Aspose.Cells.lic");
var license = new aspose.cells.License();
aspose.cells.License.setLicenseFromStream(license, licenseStream,
function(err) {
if (err) {
console.log("license error");
return;
}
var workbook = new aspose.cells.Workbook("Book2.xlsx");
var writeStream = fs.createWriteStream("result-stream.xlsx");
aspose.cells.Workbook.saveToStream(workbook, writeStream, aspose.cells.SaveFormat.XLSX);
});
```
