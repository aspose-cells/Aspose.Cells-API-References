##HeaderFooterCommand.Font
HeaderFooterCommand property. Gets the font of the commands value
## HeaderFooterCommand.Font property
Gets the font of the command's value.
```csharp
public Font Font { get; }
```
### Remarks
Useless for HeaderFooterCommandType.Picture.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class HeaderFooterCommandPropertyFontDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access page setup for header/footer
PageSetup pageSetup = worksheet.PageSetup;
// Set a header with text that will have a HeaderFooterCommand
pageSetup.SetHeader(0, "&\"Arial\"&12&BThis is a header");
// Get header script
string headerScript = pageSetup.GetHeader(0);
// Get header commands
HeaderFooterCommand[] commands = pageSetup.GetCommands(headerScript);
// Find the text command (assuming it's the first one)
if (commands.Length > 0 && commands[0].Type == HeaderFooterCommandType.Text)
{
HeaderFooterCommand textCommand = commands[0];
// Access the Font property (read-only)
Font font = textCommand.Font;
// Display current font properties
Console.WriteLine("Current Font:");
Console.WriteLine($"Name: {font.Name}");
Console.WriteLine($"Size: {font.Size}");
Console.WriteLine($"Bold: {font.IsBold}");
Console.WriteLine($"Color: {font.Color}");
// Since Font is read-only, we can't assign a new Font object,
// but we can modify the existing font's properties
font.Name = "Times New Roman";
font.Size = 14;
font.IsBold = false;
font.Color = System.Drawing.Color.Blue;
// Save the workbook to see the changes
workbook.Save("HeaderFooterFontDemo.xlsx");
Console.WriteLine("\nModified Font:");
Console.WriteLine($"Name: {font.Name}");
Console.WriteLine($"Size: {font.Size}");
Console.WriteLine($"Bold: {font.IsBold}");
Console.WriteLine($"Color: {font.Color}");
}
}
}
}
```
### See Also
* class [Font](../../font/)
* class [HeaderFooterCommand](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
