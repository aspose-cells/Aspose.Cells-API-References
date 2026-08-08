---
title: "Cells.get"
linktitle: "get"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Gets the Cell element at the specified cell row index and column index."
type: docs
weight: 500
url: /nodejs/aspose.cells/cells/get/
---

## get(row, column)

Gets the Cell element at the specified cell row index and column index.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Row index. |
| column | Number | Column index. |

**Returns:** Cell — `Cell` The Cell object.

**Example:**

```js
var cells = excel.getWorksheets().get(0).getCells();
var cell = cells.get(0, 0);    //Gets the cell at "A1"
```
