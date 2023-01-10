---
title: CalculationPrecisionStrategy enumeration
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 1820
url: /python-net/aspose.cells/calculationprecisionstrategy/
is_root: false
---

## CalculationPrecisionStrategy enumeration

Enumerates strategies for handling calculation precision.
Because of the precision issue of IEEE 754 Floating-Point Arithmetic, some "seemingly simple" formulas may not be calculated as the expected result.
Such as formula "=-0.45+0.43+0.02", when calculating operands by '+' operator directly, the result is not zero. For such kind of precision issue,
some special strategies may give the expected result.



The CalculationPrecisionStrategy type exposes the following members:

### Fields
| Field | Description |
| :- | :- |
| NONE | No strategy applied on calculation.<br/>When calculating just use the original double value as operand and return the result directly.<br/>Most efficient for performance and applicable for most cases. |
| ROUND | Rounds the calculation result according with significant digits. |
| DECIMAL | Uses decimal as operands when possible.<br/>Most inefficient for performance. |


### See Also

* module [aspose.cells](../)
