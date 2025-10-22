##WebQueryConnection.IsParsePre
WebQueryConnection property. Flag indicating whether data contained within HTML PRE tags in the web page is parsed into columns when you import the page into a query table
## WebQueryConnection.IsParsePre property
Flag indicating whether data contained within HTML PRE tags in the web page is parsed into columns when you import the page into a query table.
```csharp
public bool IsParsePre { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using System;
public class WebQueryConnectionPropertyIsParsePreDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
try
{
// Create a new web query connection using the existing connection from workbook
WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[0];
// Display initial IsParsePre value (default)
Console.WriteLine("Initial IsParsePre value: " + connection.IsParsePre);
// Set IsParsePre to true
connection.IsParsePre = true;
Console.WriteLine("Updated IsParsePre value: " + connection.IsParsePre);
// Set IsParsePre back to false
connection.IsParsePre = false;
Console.WriteLine("Final IsParsePre value: " + connection.IsParsePre);
// Save the workbook
workbook.Save("WebQueryConnectionIsParsePreDemo.xlsx");
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
