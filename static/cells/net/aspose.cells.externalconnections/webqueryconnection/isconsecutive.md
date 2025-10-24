##WebQueryConnection.IsConsecutive
WebQueryConnection property. Flag indicating whether consecutive delimiters should be treated as just one delimiter
## WebQueryConnection.IsConsecutive property
Flag indicating whether consecutive delimiters should be treated as just one delimiter.
```csharp
public bool IsConsecutive { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using System;
public class WebQueryConnectionPropertyIsConsecutiveDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Create a web query connection by accessing the first connection
// (assuming there's at least one connection available)
WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[0];
try
{
// Display initial IsConsecutive value (default)
Console.WriteLine("Initial IsConsecutive value: " + connection.IsConsecutive);
// Set IsConsecutive to true
connection.IsConsecutive = true;
Console.WriteLine("Updated IsConsecutive value: " + connection.IsConsecutive);
// Set IsConsecutive back to false
connection.IsConsecutive = false;
Console.WriteLine("Final IsConsecutive value: " + connection.IsConsecutive);
// Save the workbook with the web query connection
workbook.Save("WebQueryConnectionIsConsecutiveDemo.xlsx");
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
