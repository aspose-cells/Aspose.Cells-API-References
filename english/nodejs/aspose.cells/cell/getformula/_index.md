---
title: "Cell.getFormula"
linktitle: "getFormula"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Gets or sets a formula of the Cell."
type: docs
weight: 250
url: /nodejs/aspose.cells/cell/getformula/
---

## getFormula()

Gets or sets a formula of the Cell. A formula string always begins with an equal sign (=). And please always use comma(,) as parameters delimiter, such as "=SUM(A1, E1, H2)".

**Example:**

```js
var excel = new aspose.cells.Workbook();
var cells = excel.getWorksheets().get(0).getCells();
cells.get("B6").setFormula("=SUM(B2:B5, E1) + sheet2!A1");
```
