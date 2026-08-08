---
title: "Workbook.refreshDynamicArrayFormulas"
linktitle: "refreshDynamicArrayFormulas"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data) For performance consideration, we do not refresh all dynam"
type: docs
weight: 680
url: /nodejs/aspose.cells/workbook/refreshdynamicarrayformulas-1/
---

## refreshDynamicArrayFormulas(calculate, copts)

Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data) For performance consideration, we do not refresh all dynamic array formulas automatically when the formula itself or the data it references to changed. So user need to call this method manually after those operations which may influence dynamic array formulas, such as importing/setting cell values, inserting/deleting rows/columns/ranges, ...etc. For most formulas with functions, calculating the spill range also needs to calculating the formula, so in general true value for "calculate" flag is preferred. If the formula is simple, such as a range reference or array(for example "=C1:E5", "={1,2;3,4}", ...), simple function on a range or array(for example "=ABS(C1:E5)", "=1+{1,2;3,4}", ...), and all formulas will be calculated later(such as by calculateFormula(com.aspose.cells.CalculationOptions)), then using false vlaue for "calculate" flag may avoid the duplicated calculation for the benefit of performance.

| Parameter | Type | Description |
| --- | --- | --- |
| calculate | boolean | Whether calculates and updates cell values for those dynamic array formulas |
| copts | CalculationOptions | The options for calculating formulas |
