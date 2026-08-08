---
title: "Worksheet.calculateArrayFormula"
linktitle: "calculateArrayFormula"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Calculates a formula as array formula."
type: docs
weight: 210
url: /nodejs/aspose.cells/worksheet/calculatearrayformula-1/
---

## calculateArrayFormula(formula, opts, maxRowCount, maxColumnCount)

Calculates a formula as array formula. The formula will be taken as dynamic array formula to calculate the dimension and result. User specified maximum dimension is used for cases that the calculated result is large data set (for example, the calculated result may correspond to a whole row or column data) but user does not need so large an array according to business requirement or for performance consideration.

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | Formula to be calculated. |
| opts | CalculationOptions | Options for calculating formula |
| maxRowCount | Number | the maximum row count of resultant data. If it is non-positive or greater than the actual row count, then actual row count will be used. |
| maxColumnCount | Number | the maximum column count of resultant data. If it is non-positive or greater than the actual row count, then actual column count will be used. |

**Returns:** Array of Array of Object — `Array of Array of Object` Calculated formula result.
