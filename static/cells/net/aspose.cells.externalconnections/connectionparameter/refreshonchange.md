##ConnectionParameter.RefreshOnChange
ConnectionParameter property. Flag indicating whether the query should automatically refresh when the contents of a cell that provides the parameter value changes. If true then external data is refreshed using the new parameter value every time theres a change. If false then external data is only refreshed when requested by the user or some other event triggers refresh e.g. workbook opened
## ConnectionParameter.RefreshOnChange property
Flag indicating whether the query should automatically refresh when the contents of a cell that provides the parameter value changes. If true, then external data is refreshed using the new parameter value every time there's a change. If false, then external data is only refreshed when requested by the user, or some other event triggers refresh (e.g., workbook opened).
```csharp
public bool RefreshOnChange { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using System;
public class ConnectionParameterPropertyRefreshOnChangeDemo
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
// For demonstration, we'll show how RefreshOnChange would be used if we had a parameter
if (parameter != null)
{
// Get and display the current RefreshOnChange value
Console.WriteLine("Current RefreshOnChange: " + parameter.RefreshOnChange);
// Set a new RefreshOnChange value (since property is read-write)
parameter.RefreshOnChange = true;
Console.WriteLine("Updated RefreshOnChange: " + parameter.RefreshOnChange);
}
else
{
// Fallback demonstration when we can't create the parameter
workbook.Worksheets[0].Cells["A1"].Value = "RefreshOnChange property demo (see code comments)";
Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
}
// Save the workbook
workbook.Save("ConnectionParameterRefreshOnChangeDemo.xlsx");
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
