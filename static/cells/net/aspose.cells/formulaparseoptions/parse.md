##FormulaParseOptions.Parse
FormulaParseOptions property. Whether parse given formula. Default is true. If it is false then given formula string will be kept as it is for the cell until user call other methods to parse them or parsed formula data is required by other operations such as calculating formulas
## FormulaParseOptions.Parse property
Whether parse given formula. Default is true. If it is false, then given formula string will be kept as it is for the cell until user call other methods to parse them or parsed formula data is required by other operations such as calculating formulas.
```csharp
public bool Parse { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FormulaParseOptionsPropertyParseDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
Cells cells = sheet.Cells;
// Set formulas with Parse=false (formulas won't be parsed immediately)
cells["A1"].PutValue(10);
cells["A2"].PutValue(20);
cells["B1"].SetFormula("=A1+A2", new FormulaParseOptions() { Parse = false });
cells["B2"].SetFormula("=SUM(A1:A2)", new FormulaParseOptions() { Parse = false });
// Calculate formulas (parsing will occur now)
wb.CalculateFormula();
Console.WriteLine("B1 value: " + cells["B1"].Value);
Console.WriteLine("B2 value: " + cells["B2"].Value);
}
}
}
```
### See Also
* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
