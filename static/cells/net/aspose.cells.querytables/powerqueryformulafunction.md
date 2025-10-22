##Class PowerQueryFormulaFunction
Aspose.Cells.QueryTables.PowerQueryFormulaFunction class. Represents the function of power query
## PowerQueryFormulaFunction class
Represents the function of power query.
```csharp
public class PowerQueryFormulaFunction : PowerQueryFormula
```
## Properties
| Name | Description |
| --- | --- |
| [Description](../../aspose.cells.querytables/powerqueryformula/description/) { get; set; } | Gets and sets the description of the power query formula.(Inherited from [`PowerQueryFormula`](../powerqueryformula/).) |
| [F](../../aspose.cells.querytables/powerqueryformulafunction/f/) { get; set; } | Gets and sets the definition of function. |
| virtual [FormulaDefinition](../../aspose.cells.querytables/powerqueryformula/formuladefinition/) { get; } | Gets the definition of the power query formula.(Inherited from [`PowerQueryFormula`](../powerqueryformula/).) |
| [GroupName](../../aspose.cells.querytables/powerqueryformula/groupname/) { get; } | Gets the name of group which contains this power query formula.(Inherited from [`PowerQueryFormula`](../powerqueryformula/).) |
| [Name](../../aspose.cells.querytables/powerqueryformula/name/) { get; set; } | Gets and sets the name of the power query formula.(Inherited from [`PowerQueryFormula`](../powerqueryformula/).) |
| [PowerQueryFormulaItems](../../aspose.cells.querytables/powerqueryformula/powerqueryformulaitems/) { get; } | Gets all items of power query formula.(Inherited from [`PowerQueryFormula`](../powerqueryformula/).) |
| override [Type](../../aspose.cells.querytables/powerqueryformulafunction/type/) { get; } | Gets the type of power query formula. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;
namespace AsposeCellsExamples
{
public class QueryTablesClassPowerQueryFormulaFunctionDemo
{
public static void Run()
{
Workbook workbook = new Workbook("source.xlsx");
PowerQueryFormula formula = workbook.DataMashup.PowerQueryFormulas["from_timestamp"];
Console.WriteLine($"Name: {formula.Name}");
Console.WriteLine($"Type: {formula.Type}");
PowerQueryFormulaFunction function = (PowerQueryFormulaFunction)formula;
Console.WriteLine($"Signature: {function.F}");
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [PowerQueryFormula](../powerqueryformula/)
* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)
