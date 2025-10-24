##Enum ReflectionEffectType
Aspose.Cells.Drawing.ReflectionEffectType enum. Represents the effect type of reflection
## ReflectionEffectType enumeration
Represents the effect type of reflection.
```csharp
public enum ReflectionEffectType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| None | `0` | No reflection effect. |
| Custom | `1` | Custom reflection effect. |
| TightReflectionTouching | `2` | Tight reflection, touching. |
| HalfReflectionTouching | `3` | Half reflection, touching. |
| FullReflectionTouching | `4` | Full reflection, touching. |
| TightReflection4PtOffset | `5` | Tight reflection, 4 pt offset. |
| HalfReflection4PtOffset | `6` | Half reflection, 4 pt offset. |
| FullReflection4PtOffset | `7` | Full reflection, 4 pt offset. |
| TightReflection8PtOffset | `8` | Tight reflection, 8 pt offset. |
| HalfReflection8PtOffset | `9` | Half reflection, 8 pt offset. |
| FullReflection8PtOffset | `10` | Full reflection, 8 pt offset. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class DrawingClassReflectionEffectTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape
Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
// Get the reflection effect
ReflectionEffect reflection = rectangle.Reflection;
// Set reflection properties
reflection.Type = ReflectionEffectType.HalfReflectionTouching;
reflection.Transparency = 0.5;
reflection.Size = 55;
reflection.Blur = 0.5;
reflection.Distance = 0;
// Save the workbook
workbook.Save("DrawingClassReflectionEffectTypeDemo.xlsx");
Console.WriteLine("Reflection effect demo completed successfully.");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
