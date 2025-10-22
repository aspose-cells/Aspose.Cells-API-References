##GradientStopCollection.Add
GradientStopCollection method. Add a gradient stop
## Add(double, CellsColor, int) {#add}
Add a gradient stop.
```csharp
public void Add(double position, CellsColor color, int alpha)
```
| Parameter | Type | Description |
| --- | --- | --- |
| position | Double | The position of the stop,in unit of percentage. |
| color | CellsColor | The color of the stop. |
| alpha | Int32 | The alpha of the color. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
using System.Drawing;
public class GradientStopCollectionMethodAddWithDoubleCellsColorInt32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
var shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 2, 0, 2, 0, 300, 100);
shape.Fill.FillType = FillType.Gradient;
GradientStopCollection gradientStops = shape.Fill.GradientFill.GradientStops;
gradientStops.Clear();
try
{
// Create CellsColor using factory method
CellsColor gradientColor = workbook.CreateCellsColor();
gradientColor.Color = Color.DarkOrange;
gradientStops.Add(0.3, gradientColor, 192);
Console.WriteLine("Gradient stop added successfully");
workbook.Save("GradientStopAddDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error adding gradient stop: {ex.Message}");
}
}
}
}
```
### See Also
* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [GradientStopCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
## Add(double, Color, int) {#add_1}
Add a gradient stop.
```csharp
public void Add(double position, Color color, int alpha)
```
| Parameter | Type | Description |
| --- | --- | --- |
| position | Double | The position of the stop,in unit of percentage. |
| color | Color | The color of the stop. |
| alpha | Int32 | The alpha of the color. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
using System.Drawing;
public class GradientStopCollectionMethodAddWithDoubleColorInt32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a rectangle shape with gradient fill
var shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 2, 0, 2, 0, 300, 100);
shape.Fill.FillType = FillType.Gradient;
shape.Fill.GradientFill.GradientStops.Clear();
GradientStopCollection gradientStops = shape.Fill.GradientFill.GradientStops;
try
{
// Add gradient stops using (Double, Color, Int32) parameters
gradientStops.Add(0.0, Color.Red, 255);    // Opaque red at start position
gradientStops.Add(1.0, Color.Blue, 128);    // Semi-transparent blue at end position
Console.WriteLine("Added gradient stops with positions: 0.0 (Red) and 1.0 (Blue)");
}
catch (Exception ex)
{
Console.WriteLine($"Error adding gradient stops: {ex.Message}");
}
workbook.Save("GradientStopCollectionAddDemo.xlsx");
}
}
}
```
### See Also
* class [GradientStopCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
