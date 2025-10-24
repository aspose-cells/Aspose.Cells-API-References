##DataMashup.PowerQueryFormulas
DataMashup property. Gets all power query formulas
## DataMashup.PowerQueryFormulas property
Gets all power query formulas.
```csharp
public PowerQueryFormulaCollection PowerQueryFormulas { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;
namespace AsposeCellsExamples
{
public class DataMashupPropertyPowerQueryFormulasDemo
{
public static void Run()
{
// Load workbook with Power Query formulas
Workbook workbook = new Workbook("source.xlsx");
// Get DataMashup object
DataMashup mashupData = workbook.DataMashup;
// Check if there are any Power Query formulas
if (mashupData != null && mashupData.PowerQueryFormulas != null)
{
Console.WriteLine("Power Query Formulas Found:");
// Iterate through each Power Query formula
foreach (PowerQueryFormula formula in mashupData.PowerQueryFormulas)
{
Console.WriteLine("Formula Definition:");
Console.WriteLine(formula.FormulaDefinition);
Console.WriteLine("----------------------");
}
}
else
{
Console.WriteLine("No Power Query formulas found in the workbook.");
}
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [PowerQueryFormulaCollection](../../powerqueryformulacollection/)
* class [DataMashup](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)
