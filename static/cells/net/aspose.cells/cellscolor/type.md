##CellsColor.Type
CellsColor property. The color type
## CellsColor.Type property
The color type.
```csharp
public ColorType Type { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class CellsColorPropertyTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a shape to demonstrate CellsColor
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
CellsColor cellsColor = shape.Fill.SolidFill.CellsColor;
// Display initial color type
Console.WriteLine("Initial Color Type: " + cellsColor.Type);
// Set RGB color and show type change
cellsColor.Color = System.Drawing.Color.Red;
Console.WriteLine("After setting RGB Color - Type: " + cellsColor.Type);
// Set indexed color and show type change
cellsColor.ColorIndex = 5; // Standard Excel color index
Console.WriteLine("After setting ColorIndex - Type: " + cellsColor.Type);
// Set theme color and show type change
cellsColor.ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.0); // Added tint parameter
Console.WriteLine("After setting ThemeColor - Type: " + cellsColor.Type);
// Demonstrate different color types in cells
Cell cell1 = worksheet.Cells["A1"];
cell1.PutValue("RGB Color");
Style style1 = cell1.GetStyle(); // Use GetStyle() instead of Style property
style1.ForegroundColor = System.Drawing.Color.Blue;
style1.Pattern = BackgroundType.Solid;
cell1.SetStyle(style1);
Cell cell2 = worksheet.Cells["A2"];
cell2.PutValue("Indexed Color");
Style style2 = cell2.GetStyle(); // Use GetStyle() instead of Style property
style2.ForegroundColor = System.Drawing.Color.FromArgb(5); // Using color index
style2.Pattern = BackgroundType.Solid;
cell2.SetStyle(style2);
// Save the result
workbook.Save("CellsColorTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [ColorType](../../colortype/)
* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
