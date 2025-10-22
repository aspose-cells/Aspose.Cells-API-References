##FontConfigs.DefaultFontName
FontConfigs property. Gets or sets the default font name
## FontConfigs.DefaultFontName property
Gets or sets the default font name.
```csharp
public static string DefaultFontName { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class FontConfigsPropertyDefaultFontNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Display the current default font name
Console.WriteLine("Current DefaultFontName value: " + FontConfigs.DefaultFontName);
// Set a new default font name
FontConfigs.DefaultFontName = "Arial";
// Create a style with no explicit font set to demonstrate default font usage
Style style = workbook.CreateStyle();
style.Font.Name = ""; // Empty to use default font
// Apply the style to a cell
Cell cell = worksheet.Cells["A1"];
cell.PutValue("This text should use the default font");
cell.SetStyle(style);
// Save the workbook to see the effect
workbook.Save("PropertyDefaultFontNameDemo.xlsx");
// Verify the font was applied correctly
Console.WriteLine("Cell font after setting DefaultFontName: " + cell.GetStyle().Font.Name);
}
}
}
```
### See Also
* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
