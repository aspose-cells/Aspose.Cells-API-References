##Enum LightRigDirectionType
Aspose.Cells.Drawing.LightRigDirectionType enum. Represents the light rig direction type
## LightRigDirectionType enumeration
Represents the light rig direction type.
```csharp
public enum LightRigDirectionType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Bottom | `0` | Bottom |
| BottomLeft | `1` | Bottom left. |
| BottomRight | `2` | Bottom Right. |
| Left | `3` | Left. |
| Right | `4` | Right. |
| Top | `5` | Top. |
| TopLeft | `6` | Top left. |
| TopRight | `7` | Top Right. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class DrawingClassLightRigDirectionTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to demonstrate light rig direction
Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 10, 10, 200, 200, 0, 0);
// Set the light rig direction for the shape's 3D format
shape.ThreeDFormat.LightingDirection = LightRigDirectionType.TopRight;
// Demonstrate different light rig directions
Console.WriteLine("Current Light Rig Direction: " + shape.ThreeDFormat.LightingDirection);
// Change light rig direction
shape.ThreeDFormat.LightingDirection = LightRigDirectionType.BottomLeft;
Console.WriteLine("Changed Light Rig Direction: " + shape.ThreeDFormat.LightingDirection);
// Iterate through all possible light rig directions
Console.WriteLine("\nAll Light Rig Direction Types:");
foreach (LightRigDirectionType direction in Enum.GetValues(typeof(LightRigDirectionType)))
{
Console.WriteLine(direction.ToString());
}
// Save the workbook
workbook.Save("LightRigDirectionTypeDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
