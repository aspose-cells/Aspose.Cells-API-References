##FillFormat.Type
FillFormat property. Gets and sets the fill type
## FillFormat.Type property
Gets and sets the fill type.
```csharp
[Obsolete("Use FillFormat.FillType  instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public FillType Type { get; set; }
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
public class FillFormatPropertyTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape
Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 200);
FillFormat fill = shape.Fill;
// Display current Type value
Console.WriteLine("Current Type value: " + fill.Type);
// Change Type to Gradient (obsolete property used for demonstration)
fill.Type = FillType.Gradient;
// Apply two-color gradient effect
fill.SetTwoColorGradient(Color.Blue, Color.Green, GradientStyleType.Horizontal, 1);
// Save the modified workbook
workbook.Save("FillFormatTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [FillType](../../filltype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
