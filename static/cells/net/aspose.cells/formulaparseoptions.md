##Class FormulaParseOptions
Aspose.Cells.FormulaParseOptions class. Represents options when parsing formula
## FormulaParseOptions class
Represents options when parsing formula.
```csharp
public class FormulaParseOptions
```
## Constructors
| Name | Description |
| --- | --- |
| [FormulaParseOptions](formulaparseoptions/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [CheckAddIn](../../aspose.cells/formulaparseoptions/checkaddin/) { get; set; } | Whether check addins in existing external links of current workbook for user defined function without external link. Default is true(if user defined function matches one addin in existing external links, then take it as the addin). |
| [CustomFunctionDefinition](../../aspose.cells/formulaparseoptions/customfunctiondefinition/) { get; set; } | Definition for parsing custom functions. |
| [LocaleDependent](../../aspose.cells/formulaparseoptions/localedependent/) { get; set; } | Whether the formula is locale formatted. Default is false. |
| [Parse](../../aspose.cells/formulaparseoptions/parse/) { get; set; } | Whether parse given formula. Default is true. If it is false, then given formula string will be kept as it is for the cell until user call other methods to parse them or parsed formula data is required by other operations such as calculating formulas. |
| [R1C1Style](../../aspose.cells/formulaparseoptions/r1c1style/) { get; set; } | Whether the formula is R1C1 reference style. Default is false. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class FormulaParseOptionsDemo
{
public static void FormulaParseOptionsExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create an instance of FormulaParseOptions
FormulaParseOptions options = new FormulaParseOptions
{
LocaleDependent = true,
R1C1Style = false,
CheckAddIn = true,
Parse = true,
CustomFunctionDefinition = null // Assuming no custom function definition for this example
};
// Add a formula to a cell using the options
Cell cell = worksheet.Cells["A1"];
cell.SetFormula("=SUM(B1:B10)", options);
// Save the workbook
workbook.Save("FormulaParseOptionsExample.xlsx");
workbook.Save("FormulaParseOptionsExample.pdf");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
