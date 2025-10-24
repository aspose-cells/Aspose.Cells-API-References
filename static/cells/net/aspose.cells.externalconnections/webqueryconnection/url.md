##WebQueryConnection.Url
WebQueryConnection property. URL to use to refresh external data
## WebQueryConnection.Url property
URL to use to refresh external data.
```csharp
public string Url { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using System;
public class WebQueryConnectionPropertyUrlDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a web query connection by adding it to the collection
// The collection will likely create and return the connection object
WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[workbook.DataConnections.Count];
// Set initial URL for the web query
connection.Url = "https://example.com/data.html";
Console.WriteLine("Initial URL: " + connection.Url);
// Change the URL to a different source
connection.Url = "https://example.com/updated-data.xml";
Console.WriteLine("Updated URL: " + connection.Url);
// Configure the connection to parse XML data
connection.IsXml = true;
// Refresh the data connection (would normally retrieve data from the URL)
// Note: Actual web access would require network connectivity
// workbook.RefreshAllConnections();
// Save the workbook with the web query connection
workbook.Save("WebQueryConnectionUrlDemo.xlsx");
}
}
}
```
### See Also
* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)
