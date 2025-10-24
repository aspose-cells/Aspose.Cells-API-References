##FormulaParseOptions Class
'FormulaParseOptions class. Encapsulates the object that represents formulaparseoptions in Go.'
## FormulaParseOptions class
Represents options when parsing formula.
```go
type FormulaParseOptions struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewFormulaParseOptions](./newformulaparseoptions/) | Default constructor. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetLocaleDependent](./getlocaledependent/) | Whether the formula is locale formatted. Default is false. |
|[SetLocaleDependent](./setlocaledependent/) | Whether the formula is locale formatted. Default is false. |
|[GetR1C1Style](./getr1c1style/) | Whether the formula is R1C1 reference style. Default is false. |
|[SetR1C1Style](./setr1c1style/) | Whether the formula is R1C1 reference style. Default is false. |
|[GetCheckAddIn](./getcheckaddin/) | Whether check addins in existing external links of current workbook for user defined function without external link.Default is true(if user defined function matches one addin in existing external links, then take it as the addin). |
|[SetCheckAddIn](./setcheckaddin/) | Whether check addins in existing external links of current workbook for user defined function without external link.Default is true(if user defined function matches one addin in existing external links, then take it as the addin). |
|[GetParse](./getparse/) | Whether parse given formula. Default is true.If it is false, then given formula string will be kept as it is for the cell until user call other methods to parse themor parsed formula data is required by other operations such as calculating formulas. |
|[SetParse](./setparse/) | Whether parse given formula. Default is true.If it is false, then given formula string will be kept as it is for the cell until user call other methods to parse themor parsed formula data is required by other operations such as calculating formulas. |
|[GetCustomFunctionDefinition](./getcustomfunctiondefinition/) | Definition for parsing custom functions. |
|[SetCustomFunctionDefinition](./setcustomfunctiondefinition/) | Definition for parsing custom functions. |
