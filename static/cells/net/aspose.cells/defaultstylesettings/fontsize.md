##DefaultStyleSettings.FontSize
DefaultStyleSettings property. Gets/Sets the default standard font size for the workbook
## DefaultStyleSettings.FontSize property
Gets/Sets the default standard font size for the workbook.
```csharp
public double FontSize { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DefaultStyleSettingsPropertyFontSizeDemo
{
public static void Run()
{
HtmlLoadOptions htmlLoadOptions = new HtmlLoadOptions();
// Set default font name and size
htmlLoadOptions.DefaultStyleSettings.FontName = "Calibri";
htmlLoadOptions.DefaultStyleSettings.FontSize = 11.0;
// Load HTML file with these settings
Workbook workbook = new Workbook("example.html", htmlLoadOptions);
// Access a cell and display its font size
Cell cell = workbook.Worksheets[0].Cells["A1"];
Console.WriteLine("Cell A1 Font Size: " + cell.GetStyle().Font.Size);
}
}
}
```
### See Also
* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
