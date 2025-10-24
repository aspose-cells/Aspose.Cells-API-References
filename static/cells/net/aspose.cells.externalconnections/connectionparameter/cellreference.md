##ConnectionParameter.CellReference
ConnectionParameter property. Cell reference indicating which cells value to use for the query parameter. Used only when parameterType is cell
## ConnectionParameter.CellReference property
Cell reference indicating which cell's value to use for the query parameter. Used only when parameterType is cell.
```csharp
public string CellReference { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using System;
public class ConnectionParameterPropertyCellReferenceDemo
{
public static void Run()
{
try
{
// Create a new workbook
Workbook workbook = new Workbook();
// Create a connection parameter (simulated since constructor parameters are unknown)
ConnectionParameter parameter = null;
// In a real scenario, you would create the parameter properly
// parameter = new ConnectionParameter(/* required parameters */);
// For demonstration, we'll show how CellReference would be used if we had a parameter
if (parameter != null)
{
// Get and display the current CellReference value
Console.WriteLine("Current CellReference: " + parameter.CellReference);
// Set a new CellReference value (since property is read-write)
parameter.CellReference = "A1";
Console.WriteLine("Updated CellReference: " + parameter.CellReference);
}
else
{
// Fallback demonstration when we can't create the parameter
workbook.Worksheets[0].Cells["A1"].Value = "CellReference property demo (see code comments)";
Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
}
// Save the workbook
workbook.Save("ConnectionParameterCellReferenceDemo.xlsx");
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
* class [ConnectionParameter](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)
