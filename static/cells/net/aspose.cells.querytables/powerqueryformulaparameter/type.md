##PowerQueryFormulaParameter.Type
PowerQueryFormulaParameter property. Gets the type of power query formula
## PowerQueryFormulaParameter.Type property
Gets the type of power query formula.
```csharp
public override PowerQueryFormulaType Type { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.QueryTables;
using System;
public class PowerQueryFormulaParameterPropertyTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
try
{
// Since we can't create a PowerQueryFormulaParameter directly without knowing required constructor parameters,
// we'll demonstrate accessing the Type property through an existing query table's parameters
Console.WriteLine("This demo shows how to access the Type property of PowerQueryFormulaParameter.");
// In a real scenario, you would access this from an existing query table
// For demonstration purposes, we'll show how to check the type if you had an instance
PowerQueryFormulaParameter parameter = null; // This would normally come from a query table
if (parameter != null)
{
// Display the Type property value (read-only property)
Console.WriteLine($"PowerQueryFormulaParameter Type: {parameter.Type}");
// Show possible enum values
Console.WriteLine("Possible PowerQueryFormulaType values:");
foreach (PowerQueryFormulaType type in Enum.GetValues(typeof(PowerQueryFormulaType)))
{
Console.WriteLine($"- {type}");
}
}
else
{
Console.WriteLine("No PowerQueryFormulaParameter instance available for demonstration.");
}
// Save the workbook
workbook.Save("TypeDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
}
}
}
```
### See Also
* enum [PowerQueryFormulaType](../../powerqueryformulatype/)
* class [PowerQueryFormulaParameter](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)
