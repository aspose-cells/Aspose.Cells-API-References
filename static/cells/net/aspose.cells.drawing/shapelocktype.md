##Enum ShapeLockType
Aspose.Cells.Drawing.ShapeLockType enum. Represents type of the property to be locked
## ShapeLockType enumeration
Represents type of the property to be locked.
```csharp
public enum ShapeLockType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Group | `0` | Group |
| AdjustHandles | `1` | AdjustHandles |
| Text | `2` | Text |
| Points | `3` | Points |
| Crop | `4` | Crop |
| Selection | `5` | Selection |
| Move | `6` | Move |
| AspectRatio | `7` | AspectRatio |
| Rotation | `8` | Rotation |
| Ungroup | `9` | Ungroup |
| Resize | `10` | Resize |
| ShapeType | `11` | ShapeType |
| Arrowhead | `12` | Arrowhead |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class DrawingClassShapeLockTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a picture to the worksheet
int index = worksheet.Pictures.Add(0, 0, "example.jpg");
Aspose.Cells.Drawing.Picture picture = worksheet.Pictures[index];
// Demonstrate ShapeLockType functionality
picture.SetLockedProperty(Aspose.Cells.Drawing.ShapeLockType.AspectRatio, false);
bool isAspectRatioLocked = picture.GetLockedProperty(Aspose.Cells.Drawing.ShapeLockType.AspectRatio);
Console.WriteLine("Aspect Ratio locked: " + isAspectRatioLocked);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
