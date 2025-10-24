##ExternalConnection.OnlyUseConnectionFile
ExternalConnection property. Indicates whether the spreadsheet application should always and only use the connection information in the external connection file indicated by the odcFile attribute when the connection is refreshed. If false then the spreadsheet application should follow the procedure indicated by the reconnectionMethod attribute
## ExternalConnection.OnlyUseConnectionFile property
Indicates whether the spreadsheet application should always and only use the connection information in the external connection file indicated by the odcFile attribute when the connection is refreshed. If false, then the spreadsheet application should follow the procedure indicated by the reconnectionMethod attribute
```csharp
public bool OnlyUseConnectionFile { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using System;
public class ExternalConnectionPropertyOnlyUseConnectionFileDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
try
{
// Access the first external connection (assuming one exists)
ExternalConnection connection = workbook.DataConnections[0];
// Display the current OnlyUseConnectionFile value
Console.WriteLine("Initial OnlyUseConnectionFile value: " + connection.OnlyUseConnectionFile);
// Set a new OnlyUseConnectionFile value (since it's read-write)
connection.OnlyUseConnectionFile = true;
Console.WriteLine("Updated OnlyUseConnectionFile value: " + connection.OnlyUseConnectionFile);
// Toggle the value to demonstrate setting capability
connection.OnlyUseConnectionFile = !connection.OnlyUseConnectionFile;
Console.WriteLine("Toggled OnlyUseConnectionFile value: " + connection.OnlyUseConnectionFile);
// Save the workbook with the modified connection settings
workbook.Save("OnlyUseConnectionFileDemo.xlsx");
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
