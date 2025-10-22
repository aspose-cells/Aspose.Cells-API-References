##CalculationPrecisionStrategy Enum
'CalculationPrecisionStrategy enum. Encapsulates the object that represents calculationprecisionstrategy in Go.'
## CalculationPrecisionStrategy Enum
Enumerates strategies for handling calculation precision.Because of the precision issue of IEEE 754 Floating-Point Arithmetic, some "seemingly simple" formulas may not be calculated as the expected result.Such as formula "=-0.45+0.43+0.02", when calculating operands by '+' operator directly, the result is not zero. For such kind of precision issue,some special strategies may give the expected result.
```go
type CalculationPrecisionStrategy int32
```
## Fields
| Field | Description |
| --- | --- |
|[None](./none/) | No strategy applied on calculation.When calculating just use the original double value as operand and return the result directly.Most efficient for performance and applicable for most cases. |
|[Round](./round/) | Rounds the calculation result according with significant digits. |
|[Decimal](./decimal/) | Uses decimal as operands when possible.Most inefficient for performance. |
