##WebQueryConnection.EditPage
WebQueryConnection property. The URL of the userfacing web page showing the web query data. This URL is persisted in the case that sourceDatatrue and url has been redirected to reference an XML file. Then the userfacing page can be shown in the UI and the XML data can be retrieved behind the scenes
## WebQueryConnection.EditPage property
The URL of the user-facing web page showing the web query data. This URL is persisted in the case that sourceData="true" and url has been redirected to reference an XML file. Then the user-facing page can be shown in the UI, and the XML data can be retrieved behind the scenes.
```csharp
[Obsolete("Use WebQueryConnection.EditWebPage property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string EditPage { get; set; }
```
### Remarks
NOTE: This property is now obsolete. Instead, please use WebQueryConnection.EditWebPage property. This property will be removed 12 months later since October 2017. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using System;
public class WebQueryConnectionPropertyEditPageDemo
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
// Display initial EditPage value
Console.WriteLine("Initial EditPage value: " + connection.EditPage);
// Set EditPage to a new URL (since it's read-write)
connection.EditPage = "https://example.com/editpage";
Console.WriteLine("Updated EditPage value: " + connection.EditPage);
// Save the workbook
workbook.Save("WebQueryConnectionEditPageDemo.xlsx");
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
