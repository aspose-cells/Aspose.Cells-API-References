##FillFormat.SetType
FillFormat property. Gets the fill format set type
## FillFormat.SetType property
Gets the fill format set type.
```csharp
[Obsolete("Use FillFormat.FillType instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public FormatSetType SetType { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please use FillFormat.FillType property instead. This property will be removed 12 months later since July 2016. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
using System.Drawing;
public class FillFormatPropertySetTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Shape shape = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 200, 200);
FillFormat fillFormat = shape.Fill;
Console.WriteLine("Current SetType value: " + fillFormat.SetType);
fillFormat.SetType = FormatSetType.IsGradientSet;
fillFormat.SetTwoColorGradient(Color.LightBlue, Color.DarkBlue, GradientStyleType.Horizontal, 1);
Console.WriteLine("New SetType value: " + fillFormat.SetType);
workbook.Save("FillFormatSetTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [FormatSetType](../../formatsettype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
