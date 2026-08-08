---
title: "Cell.setDynamicArrayFormula"
linktitle: "setDynamicArrayFormula"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Sets dynamic array formula and make the formula spill into neighboring cells if possible."
type: docs
weight: 900
url: /nodejs/aspose.cells/cell/setdynamicarrayformula-1/
---

## setDynamicArrayFormula(arrayFormula, options, values, calculateRange, calculateValue)

Sets dynamic array formula and make the formula spill into neighboring cells if possible.

| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | String | the formula expression |
| options | FormulaParseOptions | options to parse formula. "Parse" option will be ignored and the formula will always be parsed immediately |
| values | Array of Array of Object | values(calculated results) for those cells with given dynamic array formula |
| calculateRange | boolean | Whether calculate the spilled range for this dynamic array formula. If the "values" parameter is not null and this flag is false, then the spilled range's height will be values.Length and width will be values[0].Length. |
| calculateValue | boolean | whether calculate this dynamic array formula for those cells in the spilled range when "values" is null or corresponding item in "values" for one cell is null. |

**Returns:** CellArea — `CellArea` the range that the formula should spill into.
