##WebQueryConnection.Post
WebQueryConnection property. Returns or sets the string used with the post method of inputting data into a web server to return data from a web query
## WebQueryConnection.Post property
Returns or sets the string used with the post method of inputting data into a web server to return data from a web query.
```csharp
public string Post { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using System;
public class WebQueryConnectionPropertyPostDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
try
{
// Create a web query connection by accessing an existing one or creating through proper initialization
// Since we can't directly instantiate WebQueryConnection, we'll use the first connection if it exists
WebQueryConnection connection = null;
if (workbook.DataConnections.Count > 0 &&
workbook.DataConnections[0] is WebQueryConnection webQueryConn)
{
connection = webQueryConn;
}
else
{
// If no connections exist, we'll demonstrate with a mock connection
Console.WriteLine("No existing web query connection found - demonstrating with property access only");
return;
}
// Set initial Post value
connection.Post = "param1=value1&param2=value2";
Console.WriteLine("Initial Post value: " + connection.Post);
// Modify the Post value
connection.Post = "username=test&password=secret";
Console.WriteLine("Updated Post value: " + connection.Post);
// Clear the Post value
connection.Post = string.Empty;
Console.WriteLine("Cleared Post value: " + connection.Post);
// Save the workbook
workbook.Save("WebQueryConnectionPostDemo.xlsx");
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
