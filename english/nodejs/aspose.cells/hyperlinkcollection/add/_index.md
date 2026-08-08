---
title: "HyperlinkCollection.add"
linktitle: "add"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Adds a hyperlink to a specified cell or a range of cells."
type: docs
weight: 10
url: /nodejs/aspose.cells/hyperlinkcollection/add/
---

## add(firstRow, firstColumn, totalRows, totalColumns, address)

Adds a hyperlink to a specified cell or a range of cells.

| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Number | First row of the hyperlink range. |
| firstColumn | Number | First column of the hyperlink range. |
| totalRows | Number | Number of rows in this hyperlink range. |
| totalColumns | Number | Number of columns of this hyperlink range. |
| address | String | Address of the hyperlink. |

**Returns:** Number — `Number` Hyperlink object index.

**Example:**

```js
var excel = new aspose.cells.Workbook();
var worksheet = excel.getWorksheets().get(0);
worksheet.getHyperlinks().add("A4", 1, 1, "http://www.aspose.com");
worksheet.getHyperlinks().add("A5", 1, 1, "c:\\book1.xls");
```
