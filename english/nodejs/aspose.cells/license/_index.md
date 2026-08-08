---
title: "License"
linktitle: "License"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Provides methods to license the component."
type: docs
weight: 2030
url: /nodejs/aspose.cells/license/
---

## License class

Provides methods to license the component.

```js
new License()
```

Initializes a new instance of this class.

## Methods

| Name | Description |
| --- | --- |
| [setLicense()](#setlicense) | Licenses the component. Tries to find the license in the following locations:1. Explicit path.2. The current working dir |
| [setLicenseFromStream(license, stream, callback)](#setlicensefromstream) *(static)* | Licenses the component. Use this method to load a license from a stream. |

### setLicense() {#setlicense}

Licenses the component. Tries to find the license in the following locations:1. Explicit path.2. The current working directory of the java application.3. The folder that contains the Aspose component JAR file.4. The folder that contains the client's calling JAR file.

### setLicenseFromStream(license, stream, callback) (static) {#setlicensefromstream}

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
