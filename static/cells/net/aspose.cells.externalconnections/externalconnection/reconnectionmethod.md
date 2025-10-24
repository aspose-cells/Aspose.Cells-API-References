##ExternalConnection.ReconnectionMethod
ExternalConnection property. Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodType.Required
## ExternalConnection.ReconnectionMethod property
Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodType.Required.
```csharp
[Obsolete("Use ExternalConnection.ReconnectionMethodType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ReConnectionMethodType ReconnectionMethod { get; set; }
```
### Remarks
NOTE: This property is now obsolete. Instead, please use ExternalConnection.ReconnectionMethodType property. This property will be removed 12 months later since October 2017. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using System;
public class ExternalConnectionPropertyReconnectionMethodDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
try
{
// Access the first external connection (assuming one exists)
ExternalConnection connection = workbook.DataConnections[0];
// Display the current ReconnectionMethod value (read operation)
Console.WriteLine("Initial ReconnectionMethod value: " + connection.ReconnectionMethod);
// Set new ReconnectionMethod values (since it's read-write)
connection.ReconnectionMethod = ReConnectionMethodType.Always;
Console.WriteLine("Updated ReconnectionMethod value: " + connection.ReconnectionMethod);
connection.ReconnectionMethod = ReConnectionMethodType.Never;
Console.WriteLine("Updated ReconnectionMethod value: " + connection.ReconnectionMethod);
// Reset to default value
connection.ReconnectionMethod = ReConnectionMethodType.Required;
Console.WriteLine("Reset ReconnectionMethod value: " + connection.ReconnectionMethod);
// Save the workbook with the modified connection settings
workbook.Save("ReconnectionMethodDemo.xlsx");
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
