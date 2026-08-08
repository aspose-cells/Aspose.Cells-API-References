---
title: "Cells.get"
linktitle: "get"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Gets the Cell element at the specified cell name."
type: docs
weight: 510
url: /nodejs/aspose.cells/cells/get-1/
---

## get(cellName)

Gets the Cell element at the specified cell name.

| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | Cell name,including its column letter and row number, for example A5. |

**Returns:** Cell — `Cell` A Cell object

**Example:**

```js
var cells = excel.getWorksheets().get(0).getCells();
var cell = cells.get("A1");    //Gets the cell at "A1"
```
