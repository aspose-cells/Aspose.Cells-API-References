##Border.Color
Border property. Gets or sets the Color of the border
## Border.Color property
Gets or sets the Color of the border.
```csharp
public Color Color { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class BorderPropertyColorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access cell A1
Cell cell = worksheet.Cells["A1"];
// Set the cell value
cell.PutValue("Border Color Demo");
// Get the cell's style
Style style = cell.GetStyle();
// Set border colors and styles
style.Borders[BorderType.TopBorder].Color = Color.Red;
style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
style.Borders[BorderType.BottomBorder].Color = Color.Blue;
style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dotted;
style.Borders[BorderType.LeftBorder].Color = Color.Green;
style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dashed;
style.Borders[BorderType.RightBorder].Color = Color.FromArgb(255, 128, 0); // Orange
style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
// Apply the style to the cell
cell.SetStyle(style);
// Save the workbook
workbook.Save("BorderColorDemo.xlsx");
Console.WriteLine("Border color demo created successfully.");
}
}
}
```
### See Also
* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
