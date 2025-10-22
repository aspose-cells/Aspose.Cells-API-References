##Aspose::Cells::FormulaParseOptions class
'Aspose::Cells::FormulaParseOptions class. Represents options when parsing formula in C++.'
## FormulaParseOptions class
Represents options when parsing formula.
```cpp
class FormulaParseOptions
```
## Methods
| Method | Description |
| --- | --- |
| [FormulaParseOptions()](./formulaparseoptions/) | Default constructor. |
| [FormulaParseOptions(FormulaParseOptions_Impl* impl)](./formulaparseoptions/) | Constructs from an implementation object. |
| [FormulaParseOptions(const FormulaParseOptions\& src)](./formulaparseoptions/) | Copy constructor. |
| [GetCheckAddIn()](./getcheckaddin/) | Whether check addins in existing external links of current workbook for user defined function without external link. Default is true(if user defined function matches one addin in existing external links, then take it as the addin). |
| [GetCustomFunctionDefinition()](./getcustomfunctiondefinition/) | Definition for parsing custom functions. |
| [GetLocaleDependent()](./getlocaledependent/) | Whether the formula is locale formatted. Default is false. |
| [GetParse()](./getparse/) | Whether parse given formula. Default is true. If it is false, then given formula string will be kept as it is for the cell until user call other methods to parse them or parsed formula data is required by other operations such as calculating formulas. |
| [GetR1C1Style()](./getr1c1style/) | Whether the formula is R1C1 reference style. Default is false. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const FormulaParseOptions\& src)](./operator_asm/) | operator= |
| [SetCheckAddIn(bool value)](./setcheckaddin/) | Whether check addins in existing external links of current workbook for user defined function without external link. Default is true(if user defined function matches one addin in existing external links, then take it as the addin). |
| [SetCustomFunctionDefinition(CustomFunctionDefinition* value)](./setcustomfunctiondefinition/) | Definition for parsing custom functions. |
| [SetLocaleDependent(bool value)](./setlocaledependent/) | Whether the formula is locale formatted. Default is false. |
| [SetParse(bool value)](./setparse/) | Whether parse given formula. Default is true. If it is false, then given formula string will be kept as it is for the cell until user call other methods to parse them or parsed formula data is required by other operations such as calculating formulas. |
| [SetR1C1Style(bool value)](./setr1c1style/) | Whether the formula is R1C1 reference style. Default is false. |
| [~FormulaParseOptions()](./~formulaparseoptions/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
