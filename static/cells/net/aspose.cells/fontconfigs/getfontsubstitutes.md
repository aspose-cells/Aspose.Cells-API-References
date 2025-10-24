##FontConfigs.GetFontSubstitutes
FontConfigs method. Returns array containing font substitute names to be used if original font is not presented
## FontConfigs.GetFontSubstitutes method
Returns array containing font substitute names to be used if original font is not presented.
```csharp
public static string[] GetFontSubstitutes(string originalFontName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| originalFontName | String | originalFontName |
### Return Value
An array containing font substitute names to be used if original font is not presented.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class FontConfigsMethodGetFontSubstitutesWithStringDemo
{
public static void Run()
{
// Initialize FontConfigs
FontConfigs fontConfigs = new FontConfigs();
try
{
// Call GetFontSubstitutes with a font name
string originalFontName = "Arial";
string[] substitutes = FontConfigs.GetFontSubstitutes(originalFontName);
// Display the results
Console.WriteLine($"Substitute fonts for '{originalFontName}':");
if (substitutes != null && substitutes.Length > 0)
{
foreach (string substitute in substitutes)
{
Console.WriteLine(substitute);
}
}
else
{
Console.WriteLine("No substitutes found for the specified font.");
}
// Demonstrate setting substitutes and getting them
string[] newSubstitutes = new string[] { "Liberation Sans", "DejaVu Sans" };
FontConfigs.SetFontSubstitutes(originalFontName, newSubstitutes);
// Get the substitutes again to verify
substitutes = FontConfigs.GetFontSubstitutes(originalFontName);
Console.WriteLine("\nAfter setting substitutes:");
foreach (string substitute in substitutes)
{
Console.WriteLine(substitute);
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetFontSubstitutes method: {ex.Message}");
}
}
}
}
```
### See Also
* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
