##PowerQueryFormula.Name
PowerQueryFormula property. Gets and sets the name of the power query formula
## PowerQueryFormula.Name property
Gets and sets the name of the power query formula.
```csharp
public string Name { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;
namespace AsposeCellsExamples
{
public class PowerQueryFormulaPropertyNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Load an existing file with Power Query formulas
workbook = new Workbook("example.xlsx");
// Access existing Power Query formulas
if (workbook.DataMashup.PowerQueryFormulas.Count > 0)
{
PowerQueryFormula formula = workbook.DataMashup.PowerQueryFormulas[0];
// Demonstrate Name property usage
Console.WriteLine("Original Power Query Formula Name: " + formula.Name);
// Change the name
formula.Name = "UpdatedSalesFilter";
Console.WriteLine("Updated Power Query Formula Name: " + formula.Name);
// Save the workbook
workbook.Save("PowerQueryFormulaDemo.xlsx");
}
else
{
Console.WriteLine("No Power Query formulas found in the workbook.");
}
}
}
}
```
### See Also
* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)
