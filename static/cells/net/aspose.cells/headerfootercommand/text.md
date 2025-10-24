##HeaderFooterCommand.Text
HeaderFooterCommand property. Gets the text of the command
## HeaderFooterCommand.Text property
Gets the text of the command.
```csharp
public string Text { get; }
```
### Remarks
Only valid for HeaderFooterCommandType.Text.
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class HeaderFooterCommandPropertyTextDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set header with text command
worksheet.PageSetup.SetHeader(1, "&\"Arial\"&12&KFF0000Sample Text Header");
// Get header commands
HeaderFooterCommand[] commands = worksheet.PageSetup.GetCommands(worksheet.PageSetup.GetHeader(1));
// Display information about text command
foreach (HeaderFooterCommand cmd in commands)
{
if (cmd.Type == HeaderFooterCommandType.Text)
{
Console.WriteLine("Text command found:");
Console.WriteLine("Text: " + cmd.Text);
Console.WriteLine("Font: " + cmd.Font);
Console.WriteLine("Color: " + ColorTranslator.ToHtml(cmd.Font.Color));
}
}
// Save the workbook
workbook.Save("HeaderFooterTextDemo.xlsx");
}
}
}
```
### See Also
* class [HeaderFooterCommand](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
