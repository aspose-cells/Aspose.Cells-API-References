##ExternalConnection.KeepAlive
ExternalConnection property. True when the spreadsheet application should make efforts to keep the connection open. When false the application should close the connection after retrieving the information
## ExternalConnection.KeepAlive property
True when the spreadsheet application should make efforts to keep the connection open. When false, the application should close the connection after retrieving the information.
```csharp
public bool KeepAlive { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using System;
public class ExternalConnectionPropertyKeepAliveDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
try
{
// Access the first external connection (assuming one exists)
ExternalConnection connection = workbook.DataConnections[0];
// Display the current KeepAlive value
Console.WriteLine("Initial KeepAlive value: " + connection.KeepAlive);
// Toggle the KeepAlive value since it's read-write
connection.KeepAlive = !connection.KeepAlive;
Console.WriteLine("Updated KeepAlive value: " + connection.KeepAlive);
// Save the workbook with the modified connection settings
workbook.Save("KeepAliveDemo.xlsx");
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
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)
