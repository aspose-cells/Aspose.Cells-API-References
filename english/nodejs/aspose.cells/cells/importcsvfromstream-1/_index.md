---
title: "Cells.importCSVFromStream"
linktitle: "importCSVFromStream"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Import a CSV file to the cells."
type: docs
weight: 1840
url: /nodejs/aspose.cells/cells/importcsvfromstream-1/
---

## importCSVFromStream(cells, stream, options, firstRow, firstColumn, callback) (static)

Import a CSV file to the cells.

| Parameter | Type | Description |
| --- | --- | --- |
| cells | Cells | The Cells object |
| stream | ReadableStream | The CSV file stream |
| options | TxtLoadOptions | The load options for reading text file |
| firstRow | Number | The row number of the first cell to import in |
| firstColumn | Number | The column number of the first cell to import in |
| callback | Callback | The callback function |

**Example:**

```js
var aspose = aspose || {};
aspose.cells = require("aspose.cells");
var fs = require("fs");
var workbook = new aspose.cells.Workbook();
var cells = workbook.getWorksheets().get(0).getCells();
var loadOptions = new aspose.cells.TxtLoadOptions();
var readStream = fs.createReadStream("EmployeeList.csv");
aspose.cells.Cells.importCSVFromStream(cells, readStream, loadOptions, 0, 1,
function(err) {
workbook.save('result.xlsx');
}
);
```
