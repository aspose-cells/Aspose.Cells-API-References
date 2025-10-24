##Style.RotationAngle
Style property. Represents text rotation angle
## Style.RotationAngle property
Represents text rotation angle.
```csharp
public int RotationAngle { get; set; }
```
### Remarks
0: Not rotated.
255: Top to Bottom.
-90: Downward.
90: Upward.
You can set 255 or value ranged from -90 to 90.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StylePropertyRotationAngleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a style with different rotation angles
Style style1 = workbook.CreateStyle();
style1.RotationAngle = -90;
worksheet.Cells["B2"].PutValue("Text rotated -90°");
worksheet.Cells["B2"].SetStyle(style1);
Style style2 = workbook.CreateStyle();
style2.RotationAngle = 90;
worksheet.Cells["C3"].PutValue("Text rotated 90°");
worksheet.Cells["C3"].SetStyle(style2);
Style style3 = workbook.CreateStyle();
style3.RotationAngle = 255;
worksheet.Cells["D4"].PutValue("Text rotated 255°");
worksheet.Cells["D4"].SetStyle(style3);
// Save the workbook
workbook.Save("output_rotation_angles.xlsx");
}
}
}
```
### See Also
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
