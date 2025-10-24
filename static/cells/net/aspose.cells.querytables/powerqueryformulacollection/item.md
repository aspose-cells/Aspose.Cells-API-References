##PowerQueryFormulaCollection.Item
PowerQueryFormulaCollection property. Gets PowerQueryFormula by the index in the list
## PowerQueryFormulaCollection indexer (1 of 2)
Gets [`PowerQueryFormula`](../../powerqueryformula/) by the index in the list.
```csharp
public PowerQueryFormula this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The index. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PowerQueryFormulaCollectionPropertyItemDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Get Power Query formulas
var dataMashup = workbook.DataMashup;
var formulas = dataMashup.PowerQueryFormulas;
// Create and add a new formula (if needed)
// Note: Actual implementation may require different approach to add formulas
// For demo purposes, we'll work with existing formulas if any
if (formulas.Count == 0)
{
// This is just for demonstration - actual API might require different approach
// to create new formulas
return;
}
// Access first formula using Item property
var formula = formulas[0];
// Get formula items
var formulaItems = formula.PowerQueryFormulaItems;
if (formulaItems.Count == 0)
{
// This is just for demonstration - actual API might require different approach
// to create new formula items
return;
}
// Access first item using Item property
var formulaItem = formulaItems[0];
// Set and get value using Item property
string formulaText = "Sql.Database(\"SERVER\", \"DB\", [Query=\"SELECT * FROM TABLE\"])";
formulaItem.Value = formulaText;
// Demonstrate Item property usage
string retrievedValue = formulaItems[0].Value;
Console.WriteLine("Power Query Formula Item Value: " + retrievedValue);
// Save the workbook
workbook.Save("PowerQueryDemo.xlsx");
}
}
}
```
### See Also
* class [PowerQueryFormula](../../powerqueryformula/)
* class [PowerQueryFormulaCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)
## PowerQueryFormulaCollection indexer (2 of 2)
Gets [`PowerQueryFormula`](../../powerqueryformula/) by the name of the power query formula.
```csharp
public PowerQueryFormula this[string name] { get; }
```
| Parameter | Description |
| --- | --- |
| name | The name of the item. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;
namespace AsposeCellsExamples
{
public class PowerQueryFormulaCollectionPropertyItemDemo1
{
public static void Run()
{
// Create a workbook by loading an existing file that contains Power Query formulas
Workbook workbook = new Workbook("example.xlsx");
// Get Power Query formulas collection
PowerQueryFormulaCollection formulas = workbook.DataMashup.PowerQueryFormulas;
// Demonstrate Item property usage
try
{
// Try to access an existing formula (if any)
if (formulas.Count > 0)
{
PowerQueryFormula formula = formulas[formulas[0].Name];
Console.WriteLine("First formula found: " + formula.Name);
Console.WriteLine("Formula definition: " + formula.FormulaDefinition);
Console.WriteLine("Formula type: " + formula.Type);
}
// This will throw an exception for non-existent formula
PowerQueryFormula nonExistent = formulas["NonExistentFormula"];
}
catch (Exception ex)
{
Console.WriteLine("Expected error accessing non-existent formula: " + ex.Message);
}
}
}
}
```
### See Also
* class [PowerQueryFormula](../../powerqueryformula/)
* class [PowerQueryFormulaCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)
