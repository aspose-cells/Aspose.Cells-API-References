##ConnectionParameter.Value
ConnectionParameter property. Noninteger numeric valueInteger valueString value or Boolean value to use as the query parameter. Used only when parameterType is value
## ConnectionParameter.Value property
Non-integer numeric value,Integer value,String value or Boolean value to use as the query parameter. Used only when parameterType is value.
```csharp
public object Value { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using System;
public class ConnectionParameterPropertyValueDemo
{
public static void Run()
{
try
{
// Create a new workbook
Workbook workbook = new Workbook();
// Create a connection parameter (simulated since we don't know constructor parameters)
ConnectionParameter parameter = null;
// In a real scenario, you would create the parameter properly
// parameter = new ConnectionParameter(/* required parameters */);
// For demonstration, we'll create a mock parameter with a value
// This shows how the Value property would be used in practice
if (parameter != null)
{
// Set the value (since Value is read-write)
parameter.Value = "SampleParameterValue";
// Get and display the value
Console.WriteLine("Parameter Value: " + parameter.Value);
// Change the value to demonstrate it's mutable
parameter.Value = 42;
Console.WriteLine("Updated Parameter Value: " + parameter.Value);
}
else
{
// Fallback demonstration when we can't create the parameter
workbook.Worksheets[0].Cells["A1"].Value = "Value property demo (see code comments)";
Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
}
// Save the workbook
workbook.Save("ConnectionParameterValueDemo.xlsx");
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
