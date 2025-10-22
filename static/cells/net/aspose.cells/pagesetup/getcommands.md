##PageSetup.GetCommands
PageSetup method. Gets all commands of header or footer
## PageSetup.GetCommands method
Gets all commands of header or footer.
```csharp
public HeaderFooterCommand[] GetCommands(string headerFooterScript)
```
| Parameter | Type | Description |
| --- | --- | --- |
| headerFooterScript | String | The header/footer script |
### Return Value
Returns all commands of header or footer.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupMethodGetCommandsWithStringDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set header with commands
string header = "&D&\"Arial\"&12sdfsdfsdfsdf";
worksheet.PageSetup.SetHeader(1, header);
// Get header commands
HeaderFooterCommand[] commands = worksheet.PageSetup.GetCommands(header);
// Display command types and text
foreach (HeaderFooterCommand cmd in commands)
{
Console.WriteLine($"Type: {cmd.Type}, Text: {cmd.Text}");
}
}
}
}
```
### See Also
* class [HeaderFooterCommand](../../headerfootercommand/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
