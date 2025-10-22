##WebQueryConnection.EditWebPage
WebQueryConnection property. The URL of the userfacing web page showing the web query data. This URL is persisted in the case that sourceDatatrue and url has been redirected to reference an XML file. Then the userfacing page can be shown in the UI and the XML data can be retrieved behind the scenes
## WebQueryConnection.EditWebPage property
The URL of the user-facing web page showing the web query data. This URL is persisted in the case that sourceData="true" and url has been redirected to reference an XML file. Then the user-facing page can be shown in the UI, and the XML data can be retrieved behind the scenes.
```csharp
public string EditWebPage { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using System;
public class WebQueryConnectionPropertyEditWebPageDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
try
{
// Access the first existing web query connection (if any)
if (workbook.DataConnections.Count > 0 &&
workbook.DataConnections[0] is WebQueryConnection connection)
{
// Set initial EditWebPage value
connection.EditWebPage = "https://example.com/user-facing-page.html";
Console.WriteLine("Initial EditWebPage value: " + connection.EditWebPage);
// Update EditWebPage value
connection.EditWebPage = "https://example.com/updated-user-page.html";
Console.WriteLine("Updated EditWebPage value: " + connection.EditWebPage);
// Save the workbook with the web query connection
workbook.Save("WebQueryConnectionEditWebPageDemo.xlsx");
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
