##ExternalConnection.BackgroundRefresh
ExternalConnection property. Indicates whether the connection can be refreshed in the background asynchronously. true if preferred usage of the connection is to refresh asynchronously in the background false if preferred usage of the connection is to refresh synchronously in the foreground
## ExternalConnection.BackgroundRefresh property
Indicates whether the connection can be refreshed in the background (asynchronously). true if preferred usage of the connection is to refresh asynchronously in the background; false if preferred usage of the connection is to refresh synchronously in the foreground.
```csharp
public bool BackgroundRefresh { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using System;
public class ExternalConnectionPropertyBackgroundRefreshDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
try
{
// Access the first external connection (assuming one exists)
ExternalConnection connection = workbook.DataConnections[0];
// Display the current BackgroundRefresh value
Console.WriteLine("Initial BackgroundRefresh value: " + connection.BackgroundRefresh);
// Toggle the BackgroundRefresh value
connection.BackgroundRefresh = !connection.BackgroundRefresh;
Console.WriteLine("Updated BackgroundRefresh value: " + connection.BackgroundRefresh);
// Save the workbook with the modified connection settings
workbook.Save("BackgroundRefreshDemo.xlsx");
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
