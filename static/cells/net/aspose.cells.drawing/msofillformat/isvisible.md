##MsoFillFormat.IsVisible
MsoFillFormat property. Indicates whether there is fill
## MsoFillFormat.IsVisible property
Indicates whether there is fill.
```csharp
public bool IsVisible { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class MsoFillFormatPropertyIsVisibleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a sample shape
Shape shape1 = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);
Shape shape2 = worksheet.Shapes.AddRectangle(2, 0, 2, 0, 100, 150);
// Set fill visibility for shape1 (visible)
shape1.FillFormat.IsVisible = true;
shape1.FillFormat.ForeColor = System.Drawing.Color.Red;
// Set fill visibility for shape2 (invisible)
shape2.FillFormat.IsVisible = false;
// Demonstrate IsVisible property usage
Console.WriteLine("Shape1 Fill Visible: " + shape1.FillFormat.IsVisible);
Console.WriteLine("Shape2 Fill Visible: " + shape2.FillFormat.IsVisible);
// Compare fill visibility between shapes
if (shape1.FillFormat.IsVisible && shape2.FillFormat.IsVisible)
{
Console.WriteLine("Both shapes have visible fills");
}
else
{
Console.WriteLine("At least one shape has invisible fill");
}
// Save the workbook
workbook.Save("MsoFillFormatIsVisibleDemo.xlsx");
}
}
}
```
### See Also
* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
