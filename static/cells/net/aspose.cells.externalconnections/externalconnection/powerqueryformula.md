##ExternalConnection.PowerQueryFormula
ExternalConnection property. Gets the definition of power query formula
## ExternalConnection.PowerQueryFormula property
Gets the definition of power query formula.
```csharp
public virtual PowerQueryFormula PowerQueryFormula { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using Aspose.Cells.QueryTables;
namespace AsposeCellsExamples
{
public class ExternalConnectionPropertyPowerQueryFormulaDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Load an existing workbook with data connections to demonstrate PowerQueryFormula
workbook = new Workbook("example.xlsx");
// Access an existing connection (assuming the workbook has at least one connection)
if (workbook.DataConnections.Count > 0)
{
var connection = workbook.DataConnections[0];
Console.WriteLine("Power Query Formula Demo:");
Console.WriteLine($"Connection Name: {connection.Name}");
// Access the PowerQueryFormula property
PowerQueryFormula powerQuery = connection.PowerQueryFormula;
if (powerQuery != null)
{
Console.WriteLine($"Formula Name: {powerQuery.Name}");
Console.WriteLine($"Formula Definition: {powerQuery.FormulaDefinition}");
}
else
{
Console.WriteLine("No Power Query Formula found for this connection");
}
}
else
{
Console.WriteLine("No data connections found in the workbook");
}
// Save the workbook
workbook.Save("PowerQueryFormulaDemo.xlsx");
}
}
}
```
### See Also
* class [PowerQueryFormula](../../../aspose.cells.querytables/powerqueryformula/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)
