##Class PowerQueryFormulaParameter
Aspose.Cells.QueryTables.PowerQueryFormulaParameter class. Represents the parameter of power query formula
## PowerQueryFormulaParameter class
Represents the parameter of power query formula.
```csharp
public class PowerQueryFormulaParameter : PowerQueryFormula
```
## Properties
| Name | Description |
| --- | --- |
| [Description](../../aspose.cells.querytables/powerqueryformula/description/) { get; set; } | Gets and sets the description of the power query formula.(Inherited from [`PowerQueryFormula`](../powerqueryformula/).) |
| override [FormulaDefinition](../../aspose.cells.querytables/powerqueryformulaparameter/formuladefinition/) { get; } | Gets the definition of the parameter. |
| [GroupName](../../aspose.cells.querytables/powerqueryformula/groupname/) { get; } | Gets the name of group which contains this power query formula.(Inherited from [`PowerQueryFormula`](../powerqueryformula/).) |
| [Name](../../aspose.cells.querytables/powerqueryformula/name/) { get; set; } | Gets and sets the name of the power query formula.(Inherited from [`PowerQueryFormula`](../powerqueryformula/).) |
| [ParameterDefinition](../../aspose.cells.querytables/powerqueryformulaparameter/parameterdefinition/) { get; } | (**Obsolete.**) Gets the definition of the parameter. |
| [PowerQueryFormulaItems](../../aspose.cells.querytables/powerqueryformula/powerqueryformulaitems/) { get; } | Gets all items of power query formula.(Inherited from [`PowerQueryFormula`](../powerqueryformula/).) |
| override [Type](../../aspose.cells.querytables/powerqueryformulaparameter/type/) { get; } | Gets the type of power query formula. |
| [Value](../../aspose.cells.querytables/powerqueryformulaparameter/value/) { get; set; } | Gets the value of parameter. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.QueryTables;
using System;
public class PowerQueryFormulaParameterDemo
{
public static void PowerQueryFormulaParameterExample()
{
// Create a new workbook
Workbook workbook = new Workbook("PowerQueryFormulaDemo_original.xlsx");
// Access the DataMashup property of the workbook
DataMashup dataMashup = workbook.DataMashup;
if (dataMashup != null)
{
// Access the PowerQueryFormulas property
PowerQueryFormulaCollection powerQueryFormulas = dataMashup.PowerQueryFormulas;
// Access the PowerQueryFormulaParameters property
PowerQueryFormulaParameterCollection powerQueryFormulaParameters = dataMashup.PowerQueryFormulaParameters;
// Example usage: Iterate through PowerQueryFormulas
foreach (PowerQueryFormula formula in powerQueryFormulas)
{
Console.WriteLine(formula.Name);
}
// Example usage: Iterate through PowerQueryFormulaParameters
foreach (PowerQueryFormulaParameter para in powerQueryFormulaParameters)
{
// Display the parameter details
Console.WriteLine("Parameter Name: " + para.Name);
Console.WriteLine("Parameter Value: " + para.Value);
Console.WriteLine("Parameter Definition: " + para.ParameterDefinition);
}
}
// Save the workbook
workbook.Save("PowerQueryFormulaParameterExample.xlsx");
return;
}
}
}
```
### See Also
* class [PowerQueryFormula](../powerqueryformula/)
* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)
