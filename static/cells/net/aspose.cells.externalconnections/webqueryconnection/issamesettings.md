##WebQueryConnection.IsSameSettings
WebQueryConnection property. Flag indicating whether to parse all tables inside a PRE block with the same width settings as the first row
## WebQueryConnection.IsSameSettings property
Flag indicating whether to parse all tables inside a PRE block with the same width settings as the first row.
```csharp
public bool IsSameSettings { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using System;
public class WebQueryConnectionPropertyIsSameSettingsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
try
{
// Access the first existing web query connection if available
if (workbook.DataConnections.Count > 0 &&
workbook.DataConnections[0] is WebQueryConnection connection)
{
// Display initial IsSameSettings value
Console.WriteLine("Initial IsSameSettings value: " + connection.IsSameSettings);
// Set IsSameSettings to true (since it's read-write)
connection.IsSameSettings = true;
Console.WriteLine("Updated IsSameSettings value: " + connection.IsSameSettings);
// Set IsSameSettings back to false
connection.IsSameSettings = false;
Console.WriteLine("Final IsSameSettings value: " + connection.IsSameSettings);
// Save the workbook
workbook.Save("WebQueryConnectionIsSameSettingsDemo.xlsx");
}
else
{
Console.WriteLine("No web query connection found in the workbook.");
}
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
* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)
