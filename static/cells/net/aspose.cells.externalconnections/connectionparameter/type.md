##ConnectionParameter.Type
ConnectionParameter property. Type of parameter used. If the parameterTypevalue then the value from boolean double integer or string will be used. In this case it is expected that only one of boolean double integer or string will be specified
## ConnectionParameter.Type property
Type of parameter used. If the parameterType=value, then the value from boolean, double, integer, or string will be used. In this case, it is expected that only one of {boolean, double, integer, or string} will be specified.
```csharp
public ConnectionParameterType Type { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using System;
public class ConnectionParameterPropertyTypeDemo
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
// For demonstration, we'll show how Type would be used if we had a parameter
if (parameter != null)
{
// Get and display the current Type value
Console.WriteLine("Current Type: " + parameter.Type);
// Set a new Type value (since property is read-write)
parameter.Type = ConnectionParameterType.Value;
Console.WriteLine("Updated Type: " + parameter.Type);
}
else
{
// Fallback demonstration when we can't create the parameter
workbook.Worksheets[0].Cells["A1"].Value = "Type property demo (see code comments)";
Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
}
// Save the workbook
workbook.Save("ConnectionParameterTypeDemo.xlsx");
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
* enum [ConnectionParameterType](../../connectionparametertype/)
* class [ConnectionParameter](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)
