##CalculationPrecisionStrategy enumeration
## CalculationPrecisionStrategy enumeration
Enumerates strategies for handling calculation precision.
Because of the precision issue of IEEE 754 Floating-Point Arithmetic, some "seemingly simple" formulas may not be calculated as the expected result.
Such as formula "=-0.45+0.43+0.02", when calculating operands by '+' operator directly, the result is not zero. For such kind of precision issue,
some special strategies may give the expected result.
The CalculationPrecisionStrategy type exposes the following members:
### Fields
| Field | Description |
| :- | :- |
| NONE | No strategy applied on calculation.
| ROUND | Rounds the calculation result according with significant digits. |
| DECIMAL | Uses decimal as operands when possible.
### See Also
* module [`aspose.cells`](..)
