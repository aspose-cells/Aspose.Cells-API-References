---
title: "Worksheet.calculateFormula"
linktitle: "calculateFormula"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Calculates a formula expression directly."
type: docs
weight: 240
url: /nodejs/aspose.cells/worksheet/calculateformula-1/
---

## calculateFormula(formula, opts)

Calculates a formula expression directly. The formula will be calculated just like it has been set to cell A1. And the formula will be taken as normal formula. If you need the formula be calculated as an array formula and to get an array for the calculated result, please use calculateArrayFormula(java.lang.String, com.aspose.cells.CalculationOptions) instead.

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | Formula to be calculated. |
| opts | CalculationOptions | Options for calculating formula |

**Returns:** Object — `Object` Calculated result of given formula. The returned object may be of possible types of Cell.Value, or ReferredArea.
