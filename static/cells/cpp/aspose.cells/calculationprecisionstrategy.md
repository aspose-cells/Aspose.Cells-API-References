##Aspose::Cells::CalculationPrecisionStrategy enum
'Aspose::Cells::CalculationPrecisionStrategy enum. Enumerates strategies for handling calculation precision. Because of the precision issue of IEEE 754 Floating-Point Arithmetic, some "seemingly simple" formulas may not be calculated as the expected result. Such as formula "=-0.45+0.43+0.02", when calculating operands by ''+'' operator directly, the result is not zero. For such kind of precision issue, some special strategies may give the expected result in C++.'
## CalculationPrecisionStrategy enum
Enumerates strategies for handling calculation precision. Because of the precision issue of IEEE 754 Floating-Point Arithmetic, some "seemingly simple" formulas may not be calculated as the expected result. Such as formula "=-0.45+0.43+0.02", when calculating operands by '+' operator directly, the result is not zero. For such kind of precision issue, some special strategies may give the expected result.
```cpp
enum class CalculationPrecisionStrategy
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| None | 0 | <br>No strategy applied on calculation. When calculating just use the original double value as operand and return the result directly. Most efficient for performance and applicable for most cases. |
| Round | 1 | <br>Rounds the calculation result according with significant digits. |
| Decimal | 2 | <br>Uses decimal as operands when possible. Most inefficient for performance. |
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
