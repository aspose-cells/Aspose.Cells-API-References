##ExternalConnection.RefreshOnLoad
ExternalConnection property. True if this connection should be refreshed when opening the file otherwise false
## ExternalConnection.RefreshOnLoad property
True if this connection should be refreshed when opening the file; otherwise, false.
```csharp
public bool RefreshOnLoad { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using System;
public class ExternalConnectionPropertyRefreshOnLoadDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
try
{
// Access the first external connection (workbook comes with default connections)
ExternalConnection connection = workbook.DataConnections[0];
// Display initial RefreshOnLoad value
Console.WriteLine("Initial RefreshOnLoad value: " + connection.RefreshOnLoad);
// Demonstrate setting the property (since it's read-write)
connection.RefreshOnLoad = !connection.RefreshOnLoad;
Console.WriteLine("Updated RefreshOnLoad value: " + connection.RefreshOnLoad);
// Save the workbook with the modified connection settings
workbook.Save("RefreshOnLoadDemo.xlsx");
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
