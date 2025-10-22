##FontConfigs.SetFontSubstitutes
FontConfigs method. Font substitute names for given original font name
## FontConfigs.SetFontSubstitutes method
Font substitute names for given original font name.
```csharp
public static void SetFontSubstitutes(string originalFontName, string[] substituteFontNames)
```
| Parameter | Type | Description |
| --- | --- | --- |
| originalFontName | String | Original font name. |
| substituteFontNames | String[] | List of font substitute names to be used if original font is not presented. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class FontConfigsMethodSetFontSubstitutesWithStringStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Original font name that might not be available
string originalFontName = "Arial";
// Substitute font names to use when original is not available
string[] substituteFontNames = new string[] { "Liberation Sans", "Helvetica", "Verdana" };
try
{
// Call SetFontSubstitutes method to configure font substitutions
FontConfigs.SetFontSubstitutes(originalFontName, substituteFontNames);
Console.WriteLine($"Font substitutes set successfully for '{originalFontName}'");
// Verify the substitutes by retrieving them
string[] retrievedSubstitutes = FontConfigs.GetFontSubstitutes(originalFontName);
Console.WriteLine("Current substitutes for '{0}':", originalFontName);
foreach (string font in retrievedSubstitutes)
{
Console.WriteLine("- " + font);
}
// Apply the font to a cell to demonstrate substitution
worksheet.Cells["A1"].PutValue("Text with potential font substitution");
Style style = worksheet.Cells["A1"].GetStyle();
style.Font.Name = originalFontName;
worksheet.Cells["A1"].SetStyle(style);
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetFontSubstitutes method: {ex.Message}");
}
// Save the workbook
workbook.Save("FontSubstitutionDemo.xlsx");
}
}
}
```
### See Also
* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
