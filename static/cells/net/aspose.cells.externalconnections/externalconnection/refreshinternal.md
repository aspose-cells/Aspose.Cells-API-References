##ExternalConnection.RefreshInternal
ExternalConnection property. Specifies the number of minutes between automatic refreshes of the connection
## ExternalConnection.RefreshInternal property
Specifies the number of minutes between automatic refreshes of the connection.
```csharp
public int RefreshInternal { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using System;
public class ExternalConnectionPropertyRefreshInternalDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to make the example meaningful
worksheet.Cells["A1"].Value = "Connection Demo";
try
{
// Create a data connection (using the base ExternalConnection class)
ExternalConnection connection = workbook.DataConnections[0];
// Set and display the RefreshInternal property
connection.RefreshInternal = 30; // Refresh every 30 minutes
Console.WriteLine("RefreshInternal value: " + connection.RefreshInternal);
// Modify the refresh interval
connection.RefreshInternal = 60;
Console.WriteLine("Updated RefreshInternal value: " + connection.RefreshInternal);
// Save the workbook with the connection settings
workbook.Save("RefreshInternalDemo.xlsx");
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
