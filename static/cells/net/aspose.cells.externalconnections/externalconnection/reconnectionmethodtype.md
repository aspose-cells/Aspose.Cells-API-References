##ExternalConnection.ReconnectionMethodType
ExternalConnection property. Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodType.Required
## ExternalConnection.ReconnectionMethodType property
Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodType.Required.
```csharp
public ReConnectionMethodType ReconnectionMethodType { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using System;
public class ExternalConnectionPropertyReconnectionMethodTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
try
{
// Access the first external connection (assuming one exists)
ExternalConnection connection = workbook.DataConnections[0];
// Display the current ReconnectionMethodType value
Console.WriteLine("Initial ReconnectionMethodType: " + connection.ReconnectionMethodType);
// Demonstrate setting the property (since it's read-write)
connection.ReconnectionMethodType = ReConnectionMethodType.Always;
Console.WriteLine("Updated ReconnectionMethodType: " + connection.ReconnectionMethodType);
// Cycle through possible values to demonstrate setting capability
foreach (ReConnectionMethodType method in Enum.GetValues(typeof(ReConnectionMethodType)))
{
connection.ReconnectionMethodType = method;
Console.WriteLine($"ReconnectionMethodType set to: {method}");
}
// Save the workbook with the modified connection settings
workbook.Save("ReconnectionMethodTypeDemo.xlsx");
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
* enum [ReConnectionMethodType](../../reconnectionmethodtype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)
