##WebQueryConnection.IsXmlSourceData
WebQueryConnection property. Flag indicating that XML source data should be imported instead of the HTML table itself
## WebQueryConnection.IsXmlSourceData property
Flag indicating that XML source data should be imported instead of the HTML table itself.
```csharp
public bool IsXmlSourceData { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using System;
public class WebQueryConnectionPropertyIsXmlSourceDataDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
try
{
// Access an existing web query connection or create one through proper initialization
if (workbook.DataConnections.Count > 0 &&
workbook.DataConnections[0] is WebQueryConnection connection)
{
// Display initial IsXmlSourceData value
Console.WriteLine("Initial IsXmlSourceData value: " + connection.IsXmlSourceData);
// Set IsXmlSourceData to true
connection.IsXmlSourceData = true;
Console.WriteLine("Updated IsXmlSourceData value: " + connection.IsXmlSourceData);
// Set IsXmlSourceData back to false
connection.IsXmlSourceData = false;
Console.WriteLine("Final IsXmlSourceData value: " + connection.IsXmlSourceData);
// Save the workbook
workbook.Save("WebQueryConnectionIsXmlSourceDataDemo.xlsx");
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
