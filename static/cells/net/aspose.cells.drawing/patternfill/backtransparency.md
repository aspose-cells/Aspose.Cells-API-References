##PatternFill.BackTransparency
PatternFill property. Gets or sets the transparency of background color
## PatternFill.BackTransparency property
Gets or sets the transparency of background color.
```csharp
public double BackTransparency { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
using System.Drawing;
public class PatternFillPropertyBackTransparencyDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape to the worksheet
Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 200, 200);
// Get the existing PatternFill instance from the shape and configure properties
shape.Fill.FillType = FillType.Pattern;
PatternFill patternFill = shape.Fill.PatternFill;
patternFill.Pattern = FillPattern.Solid;
patternFill.BackgroundColor = Color.Blue;
// Display initial BackTransparency value
Console.WriteLine("Current BackTransparency value: " + patternFill.BackTransparency);
// Set new BackTransparency value (50% transparency)
patternFill.BackTransparency = 0.5;
// Save the modified workbook
workbook.Save("PatternFillBackTransparencyDemo.xlsx");
}
}
}
```
### See Also
* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
