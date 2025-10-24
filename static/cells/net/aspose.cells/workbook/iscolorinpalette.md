##Workbook.IsColorInPalette
Workbook method. Checks if a color is in the palette for the spreadsheet
## Workbook.IsColorInPalette method
Checks if a color is in the palette for the spreadsheet.
```csharp
public bool IsColorInPalette(Color color)
```
| Parameter | Type | Description |
| --- | --- | --- |
| color | Color | Color structure. |
### Return Value
Returns true if this color is in the palette. Otherwise, returns false
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodIsColorInPaletteWithColorDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
// Check if standard color exists in palette
bool isRedInPalette = workbook.IsColorInPalette(Color.Red);
Console.WriteLine("Is Red in palette: " + isRedInPalette);
// Check if custom color exists in palette
Color customColor = Color.FromArgb(255, 123, 123, 123);
bool isCustomInPalette = workbook.IsColorInPalette(customColor);
Console.WriteLine("Is custom color in palette: " + isCustomInPalette);
// Get matching color from palette
Color matchedColor = workbook.GetMatchingColor(customColor);
Console.WriteLine("Matched color R value: " + matchedColor.R);
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
