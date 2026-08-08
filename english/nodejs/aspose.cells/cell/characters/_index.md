---
title: "Cell.characters"
linktitle: "characters"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Returns a Characters object that represents a range of characters within the cell text."
type: docs
weight: 20
url: /nodejs/aspose.cells/cell/characters/
---

## characters(startIndex, length)

Returns a Characters object that represents a range of characters within the cell text. This method only works on cell with string value.

| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | Number | The index of the start of the character. |
| length | Number | The number of characters. |

**Returns:** FontSetting — `FontSetting` Characters object.

**Example:**

```js
excel.getWorksheets().get(0).getCells().get("A1").putValue("Helloworld");
excel.getWorksheets().get(0).getCells().get("A1").characters(5, 5).getFont().setBold(true);
excel.getWorksheets().get(0).getCells().get("A1").characters(5, 5).getFont().setColor(aspose.cells.Color.getBlue());
```
