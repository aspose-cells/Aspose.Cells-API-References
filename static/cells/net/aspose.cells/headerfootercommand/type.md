##HeaderFooterCommand.Type
HeaderFooterCommand property. Gets the header/footer command type
## HeaderFooterCommand.Type property
Gets the header/footer' command type .
```csharp
public HeaderFooterCommandType Type { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HeaderFooterCommandPropertyTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set header with different command types
PageSetup pageSetup = worksheet.PageSetup;
pageSetup.SetHeader(0, "&D&\"Arial\"&12sdfsdfsdfsdf");
// Get header commands
HeaderFooterCommand[] commands = pageSetup.GetCommands(pageSetup.GetHeader(0));
// Demonstrate Type property usage
Console.WriteLine("Command 0 Type: " + commands[0].Type); // CurrentDate
Console.WriteLine("Command 1 Type: " + commands[1].Type); // Text
Console.WriteLine("Command 1 Text: " + commands[1].Text); // sdfsdfsdfsdf
}
}
}
```
### See Also
* enum [HeaderFooterCommandType](../../headerfootercommandtype/)
* class [HeaderFooterCommand](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
