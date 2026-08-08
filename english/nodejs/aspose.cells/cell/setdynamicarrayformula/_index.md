---
title: "Cell.setDynamicArrayFormula"
linktitle: "setDynamicArrayFormula"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Sets dynamic array formula and make the formula spill into neighboring cells if possible."
type: docs
weight: 890
url: /nodejs/aspose.cells/cell/setdynamicarrayformula/
---

## setDynamicArrayFormula(arrayFormula, options, calculateValue)

Sets dynamic array formula and make the formula spill into neighboring cells if possible.

| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | String | the formula expression |
| options | FormulaParseOptions | options to parse formula. "Parse" option will be ignored and the formula will always be parsed immediately |
| calculateValue | boolean | whether calculate this dynamic array formula for those cells in the spilled range. |

**Returns:** CellArea — `CellArea` the range that the formula should spill into.
