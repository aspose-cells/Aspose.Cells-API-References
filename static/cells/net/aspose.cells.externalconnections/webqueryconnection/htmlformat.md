##WebQueryConnection.HtmlFormat
WebQueryConnection property. How to handle formatting from the HTML source when bringing web query data into the worksheet. Relevant when sourceData is True
## WebQueryConnection.HtmlFormat property
How to handle formatting from the HTML source when bringing web query data into the worksheet. Relevant when sourceData is True.
```csharp
public HtmlFormatHandlingType HtmlFormat { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using System;
public class WebQueryConnectionPropertyHtmlFormatDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first existing web query connection (if any)
// Or create a new one by loading a file with web connections
if (workbook.DataConnections.Count > 0)
{
try
{
WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[0];
// Display initial HtmlFormat value
Console.WriteLine("Initial HtmlFormat value: " + connection.HtmlFormat);
// Set HtmlFormat to Rtf (demonstrating write operation)
connection.HtmlFormat = HtmlFormatHandlingType.Rtf;
Console.WriteLine("Updated HtmlFormat value: " + connection.HtmlFormat);
// Set HtmlFormat to None
connection.HtmlFormat = HtmlFormatHandlingType.None;
Console.WriteLine("Final HtmlFormat value: " + connection.HtmlFormat);
// Save the workbook with the web query connection
workbook.Save("WebQueryConnectionHtmlFormatDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
}
else
{
Console.WriteLine("No web query connections found in the workbook.");
}
}
}
}
```
### See Also
* enum [HtmlFormatHandlingType](../../htmlformathandlingtype/)
* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)
