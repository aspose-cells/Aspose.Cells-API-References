---
title: "Worksheet.calculateFormula"
linktitle: "calculateFormula"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Calculates a formula expression directly."
type: docs
weight: 250
url: /nodejs/aspose.cells/worksheet/calculateformula-2/
---

## calculateFormula(formula, pOpts, cOpts, baseCellRow, baseCellColumn, calculationData)

Calculates a formula expression directly. The formula will be calculated just like it has been set to the specified base cell. And the formula will be taken as normal formula. If you need the formula be calculated as an array formula and to get an array for the calculated result, please use calculateArrayFormula(java.lang.String, com.aspose.cells.FormulaParseOptions, com.aspose.cells.CalculationOptions, int, int, int, int, com.aspose.cells.CalculationData) instead.

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | Formula to be calculated. |
| pOpts | FormulaParseOptions | Options for parsing formula. |
| cOpts | CalculationOptions | Options for calculating formula. |
| baseCellRow | Number | The row index of the base cell. |
| baseCellColumn | Number | The column index of the base cell. |
| calculationData | CalculationData | The calculation data. It is used for the situation that user needs to calculate some static formulas when implementing custom calculation engine. For such kind of situation, user needs to specify it with the calculation data provided for |

**Returns:** Object — `Object` Calculated result of given formula. The returned object may be of possible types of Cell.Value, or ReferredArea.
