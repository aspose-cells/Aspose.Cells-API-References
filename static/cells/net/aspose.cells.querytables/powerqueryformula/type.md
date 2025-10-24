##PowerQueryFormula.Type
PowerQueryFormula property. Gets the type of this power query formula
## PowerQueryFormula.Type property
Gets the type of this power query formula.
```csharp
public virtual PowerQueryFormulaType Type { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;
namespace AsposeCellsExamples
{
public class PowerQueryFormulaPropertyTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Get existing formulas (none in new workbook) to demonstrate Type property
var formulas = workbook.DataMashup.PowerQueryFormulas;
// In a real scenario with existing formulas, we would check their types
Console.WriteLine("Power Query Formula Types:");
// This demonstrates checking the Type property
foreach (PowerQueryFormula formula in formulas)
{
Console.WriteLine($"- {formula.Name}: {formula.Type}");
}
// For demonstration purposes, add output when no formulas exist
if (formulas.Count == 0)
{
Console.WriteLine("No power query formulas found in the workbook.");
Console.WriteLine("Example formula types would be:");
Console.WriteLine("- Function: " + PowerQueryFormulaType.Function);
Console.WriteLine("- Parameter: " + PowerQueryFormulaType.Parameter);
Console.WriteLine("- Formula: " + PowerQueryFormulaType.Formula);
}
// Save the workbook
workbook.Save("PowerQueryFormulaTypes.xlsx");
}
}
}
```
### See Also
* enum [PowerQueryFormulaType](../../powerqueryformulatype/)
* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)
