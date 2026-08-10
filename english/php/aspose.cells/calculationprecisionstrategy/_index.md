---
title: "CalculationPrecisionStrategy Enum"
linktitle: "CalculationPrecisionStrategy"
articleTitle: "CalculationPrecisionStrategy"
second_title: "Aspose.Cells for PHP via Java"
description: "Utility class containing constants."
type: docs
weight: 510
url: /php/aspose.cells/calculationprecisionstrategy/
---

## CalculationPrecisionStrategy enumeration

Utility class containing constants. Enumerates strategies for handling calculation precision. Because of the precision issue of IEEE 754 Floating-Point Arithmetic, some "seemingly simple" formulas may not be calculated as the expected result. Such as formula "=-0.45+0.43+0.02", when calculating operands by '+' operator directly, the result is not zero. For such kind of precision issue, some special strategies may give the expected result.

## Values

| Name | Description |
| --- | --- |
| NONE | No strategy applied on calculation. When calculating just use the original double value as operand and return the result directly. Most efficient for performance and applicable for most cases. |
| ROUND | Rounds the calculation result according with significant digits. |
| DECIMAL | Uses decimal as operands when possible. Most inefficient for performance. |
