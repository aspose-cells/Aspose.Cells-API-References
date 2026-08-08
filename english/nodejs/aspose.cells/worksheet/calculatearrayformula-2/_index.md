---
title: "Worksheet.calculateArrayFormula"
linktitle: "calculateArrayFormula"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Calculates a formula as array formula."
type: docs
weight: 220
url: /nodejs/aspose.cells/worksheet/calculatearrayformula-2/
---

## calculateArrayFormula(formula, pOpts, cOpts, baseCellRow, baseCellColumn, maxRowCount, maxColumnCount, calculationData)

Calculates a formula as array formula. The formula will be taken as dynamic array formula to calculate the dimension and result. User specified maximum dimension is used for cases that the calculated result is large data set (for example, the calculated result may correspond to a whole row or column data) but user does not need so large an array according to business requirement or for performance consideration.

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | Formula to be calculated. |
| pOpts | FormulaParseOptions | Options for parsing formula |
| cOpts | CalculationOptions | Options for calculating formula |
| baseCellRow | Number | The row index of the base cell. |
| baseCellColumn | Number | The column index of the base cell. |
| maxRowCount | Number | The maximum row count of resultant data. If it is non-positive or greater than the actual row count, then actual row count will be used. |
| maxColumnCount | Number | The maximum column count of resultant data. If it is non-positive or greater than the actual row count, then actual column count will be used. |
| calculationData | CalculationData | The calculation data. It is used for the situation that user needs to calculate some static formulas when implementing custom calculation engine. For such kind of situation, user needs to specify it with the calculation data provided for |

**Returns:** Array of Array of Object — `Array of Array of Object` Calculated formula result.
