##PowerQueryFormula.FormulaDefinition
PowerQueryFormula property. Gets the definition of the power query formula
## PowerQueryFormula.FormulaDefinition property
Gets the definition of the power query formula.
```csharp
public virtual string FormulaDefinition { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;
namespace AsposeCellsExamples
{
public class PowerQueryFormulaPropertyFormulaDefinitionDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample table that Power Query can reference
worksheet.Cells["A1"].PutValue("ID");
worksheet.Cells["B1"].PutValue("Name");
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["B2"].PutValue("Test");
// Get existing Power Query formulas (will be empty for new workbook)
PowerQueryFormulaCollection formulas = workbook.DataMashup.PowerQueryFormulas;
// Access first formula if exists (demonstrating FormulaDefinition usage)
if (formulas.Count > 0)
{
PowerQueryFormula formula = formulas[0];
Console.WriteLine("Formula Definition: " + formula.FormulaDefinition);
Console.WriteLine("Formula Name: " + formula.Name);
Console.WriteLine("Formula Description: " + formula.Description);
}
else
{
Console.WriteLine("No Power Query formulas found in the workbook.");
}
workbook.Save("PowerQueryFormulaDemo.xlsx");
}
}
}
```
### See Also
* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)
