##FontConfigs.PreferSystemFontSubstitutes
FontConfigs property. Indicate whether to use system font substitutes first or not when a font is not presented and the substitute of this font is not set. e.g. On Ubuntu Arial font is generally substituted by Liberation Sans. Default value is false
## FontConfigs.PreferSystemFontSubstitutes property
Indicate whether to use system font substitutes first or not when a font is not presented and the substitute of this font is not set. e.g. On Ubuntu, "Arial" font is generally substituted by "Liberation Sans". Default value is false.
```csharp
public static bool PreferSystemFontSubstitutes { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class FontConfigsPropertyPreferSystemFontSubstitutesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Display current PreferSystemFontSubstitutes value
Console.WriteLine("Current PreferSystemFontSubstitutes value: " + FontConfigs.PreferSystemFontSubstitutes);
// Set PreferSystemFontSubstitutes to true
FontConfigs.PreferSystemFontSubstitutes = true;
Console.WriteLine("PreferSystemFontSubstitutes set to: " + FontConfigs.PreferSystemFontSubstitutes);
// Create a cell with a font that might need substitution
Cell cell = worksheet.Cells["A1"];
cell.PutValue("Text with Arial font");
Style style = cell.GetStyle();
style.Font.Name = "Arial";
cell.SetStyle(style);
// Save the workbook to see font substitution effects
workbook.Save("FontSubstitutionDemo.xlsx");
// Reset to default value
FontConfigs.PreferSystemFontSubstitutes = false;
Console.WriteLine("PreferSystemFontSubstitutes reset to: " + FontConfigs.PreferSystemFontSubstitutes);
}
}
}
```
### See Also
* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
