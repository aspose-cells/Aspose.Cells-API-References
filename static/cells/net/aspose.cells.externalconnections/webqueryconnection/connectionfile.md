##WebQueryConnection.ConnectionFile
WebQueryConnection property. Gets the connection file
## WebQueryConnection.ConnectionFile property
Gets the connection file.
```csharp
public override string ConnectionFile { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using System;
public class WebQueryConnectionPropertyConnectionFileDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
try
{
// Create a sample worksheet with web query data
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].Value = "Sample Web Query Data";
// Get the first existing web query connection (if any)
if (workbook.DataConnections.Count > 0 &&
workbook.DataConnections[0] is WebQueryConnection connection)
{
// Display the ConnectionFile value (read-only property)
Console.WriteLine("ConnectionFile value: " + connection.ConnectionFile);
// Save the workbook
workbook.Save("WebQueryConnectionFileDemo.xlsx");
}
else
{
Console.WriteLine("No web query connections found in the workbook.");
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
