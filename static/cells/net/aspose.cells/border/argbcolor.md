##Border.ArgbColor
Border property. Gets and sets the color with a 32bit ARGB value
## Border.ArgbColor property
Gets and sets the color with a 32-bit ARGB value.
```csharp
public int ArgbColor { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class BorderPropertyArgbColorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access cell B2 and set a value
Cell cell = worksheet.Cells["B2"];
cell.PutValue("Border ARGB Color Demo");
// Get the style and borders
Style style = cell.GetStyle();
Border border = style.Borders[BorderType.TopBorder];
// Set border properties including ARGB color
border.LineStyle = CellBorderType.Thick;
unchecked
{
border.ArgbColor = (int)0xFFFF0000; // Red color in ARGB format with unchecked cast
}
// Apply the modified style to the cell
cell.SetStyle(style);
// Save the workbook
workbook.Save("BorderArgbColorDemo.xlsx");
// Verify the ARGB color was set correctly
Border savedBorder = workbook.Worksheets[0].Cells["B2"].GetStyle().Borders[BorderType.TopBorder];
Console.WriteLine("ARGB Color of top border: " + savedBorder.ArgbColor.ToString("X8"));
}
}
}
```
### See Also
* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
