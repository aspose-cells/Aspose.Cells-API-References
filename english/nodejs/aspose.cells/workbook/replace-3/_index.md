---
title: "Workbook.replace"
linktitle: "replace"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Replaces a cell's value with a new string array."
type: docs
weight: 770
url: /nodejs/aspose.cells/workbook/replace-3/
---

## replace(placeHolder, newValues, isVertical)

Replaces a cell's value with a new string array.

| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | String | Cell placeholder |
| newValues | Array of String | String array to replace |
| isVertical | boolean | True - Vertical, False - Horizontal |

**Example:**

```js
var aspose = aspose || {};
aspose.cells = require("aspose.cells");
var java = require("java");
var workbook = new aspose.cells.Workbook();
var newValues = java.newArray("java.lang.String", ["Tom", "Alice", "Jerry"]);
workbook.replace("AnOldValue", newValues, true);
```
