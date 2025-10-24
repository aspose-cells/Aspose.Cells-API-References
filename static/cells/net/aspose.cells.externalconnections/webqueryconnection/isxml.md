##WebQueryConnection.IsXml
WebQueryConnection property. true if the web query source is XML versus HTML otherwise false
## WebQueryConnection.IsXml property
true if the web query source is XML (versus HTML), otherwise false.
```csharp
public bool IsXml { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using System;
public class WebQueryConnectionPropertyIsXmlDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
try
{
// Access the first data connection (assuming it's a WebQueryConnection)
if (workbook.DataConnections.Count > 0 &&
workbook.DataConnections[0] is WebQueryConnection connection)
{
// Display initial IsXml value
Console.WriteLine("Initial IsXml value: " + connection.IsXml);
// Set IsXml to true (since it's read-write)
connection.IsXml = true;
Console.WriteLine("Updated IsXml value: " + connection.IsXml);
// Set IsXml back to false
connection.IsXml = false;
Console.WriteLine("Final IsXml value: " + connection.IsXml);
// Save the workbook
workbook.Save("WebQueryConnectionIsXmlDemo.xlsx");
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
