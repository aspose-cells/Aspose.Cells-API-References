##Class ShadowEffect
Aspose.Cells.Drawing.ShadowEffect class. This class specifies the shadow effect of the chart element or shape
## ShadowEffect class
This class specifies the shadow effect of the chart element or shape.
```csharp
public class ShadowEffect
```
## Properties
| Name | Description |
| --- | --- |
| [Angle](../../aspose.cells.drawing/shadoweffect/angle/) { get; set; } | Gets and sets the lighting angle. Range from 0 to 359.9 degrees. |
| [Blur](../../aspose.cells.drawing/shadoweffect/blur/) { get; set; } | Gets and sets the blur of the shadow. Range from 0 to 100 points. |
| [Color](../../aspose.cells.drawing/shadoweffect/color/) { get; set; } | Gets and sets the color of the shadow. |
| [Distance](../../aspose.cells.drawing/shadoweffect/distance/) { get; set; } | Gets and sets the distance of the shadow. Range from 0 to 200 points. |
| [PresetType](../../aspose.cells.drawing/shadoweffect/presettype/) { get; set; } | Gets and sets the preset shadow type of the shadow. |
| [Size](../../aspose.cells.drawing/shadoweffect/size/) { get; set; } | Gets and sets the size of the shadow. Range from 0 to 2.0. Meaningless in inner shadow. |
| [Transparency](../../aspose.cells.drawing/shadoweffect/transparency/) { get; set; } | Gets and sets the degree of transparency of the shadow. Range from 0.0 (opaque) to 1.0 (clear). |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class DrawingClassShadowEffectDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a sample shape with all required parameters
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 100);
// Get the shadow effect of the shape
ShadowEffect shadow = shape.ShadowEffect;
// Set shadow properties
shadow.Angle = 150;
shadow.Blur = 30;
shadow.Size = 1.3;
shadow.Transparency = 0.4;
shadow.Distance = 80;
// Save the workbook
workbook.Save("output.xlsx");
Console.WriteLine("Shadow effect demo completed successfully.");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
