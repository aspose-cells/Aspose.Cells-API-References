##IndividualFontConfigs.SetFontSubstitutes
IndividualFontConfigs method. Font substitute names for given original font name
## IndividualFontConfigs.SetFontSubstitutes method
Font substitute names for given original font name.
```csharp
public void SetFontSubstitutes(string originalFontName, string[] substituteFontNames)
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
public class IndividualFontConfigsMethodSetFontSubstitutesWithStringStringDemo
{
public static void Run()
{
// Create an instance of IndividualFontConfigs
IndividualFontConfigs fontConfigs = new IndividualFontConfigs();
// Original font name and its substitutes
string originalFont = "Arial";
string[] substitutes = new string[] { "Helvetica", "Verdana", "Times New Roman" };
try
{
// Call SetFontSubstitutes with the specified parameters
fontConfigs.SetFontSubstitutes(originalFont, substitutes);
Console.WriteLine($"Successfully set font substitutes for '{originalFont}'");
Console.WriteLine("Substitutes are:");
foreach (var sub in substitutes)
{
Console.WriteLine($"- {sub}");
}
// Create a workbook to demonstrate the effect
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set style with original font
Style style = workbook.CreateStyle();
style.Font.Name = originalFont;
style.Font.Size = 14;
worksheet.Cells["A1"].Value = "This text uses " + originalFont;
worksheet.Cells["A1"].SetStyle(style);
// Save the workbook
workbook.Save("FontSubstitutesDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error setting font substitutes: {ex.Message}");
}
}
}
}
```
### See Also
* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
