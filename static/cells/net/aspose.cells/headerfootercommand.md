##Class HeaderFooterCommand
Aspose.Cells.HeaderFooterCommand class. Represents the command of header/footer
## HeaderFooterCommand class
Represents the command of header/footer
```csharp
public class HeaderFooterCommand
```
## Properties
| Name | Description |
| --- | --- |
| [Font](../../aspose.cells/headerfootercommand/font/) { get; } | Gets the font of the command's value. |
| [Text](../../aspose.cells/headerfootercommand/text/) { get; } | Gets the text of the command. |
| [Type](../../aspose.cells/headerfootercommand/type/) { get; } | Gets the header/footer' command type . |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsClassHeaderFooterCommandDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access PageSetup and set header with commands
PageSetup pageSetup = worksheet.PageSetup;
pageSetup.SetHeader(1, "&D&\"Arial\"sdfsdfsdfsdf");
// Get header commands
HeaderFooterCommand[] commands = pageSetup.GetCommands(pageSetup.GetHeader(1));
// Display command types and text
Console.WriteLine("Command 1 Type: " + commands[0].Type);
Console.WriteLine("Command 2 Type: " + commands[1].Type);
Console.WriteLine("Command 2 Text: " + commands[1].Text);
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
