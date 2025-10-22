##ArcShape.EndArrowheadStyle
ArcShape property. Gets and sets the end arrow head style of the line
## ArcShape.EndArrowheadStyle property
Gets and sets the end arrow head style of the line.
```csharp
[Obsolete("Use Shape.Line.EndArrowheadStyle property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MsoArrowheadStyle EndArrowheadStyle { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please use Shape.Line.EndArrowheadStyle property. This property will be removed 12 months later since August 2016. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ArcShapePropertyEndArrowheadStyleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add an Arc shape
ArcShape arc = worksheet.Shapes.AddArc(1, 0, 1, 0, 100, 100);
// Set line properties
arc.LineFormat.IsVisible = true;
arc.LineFormat.ForeColor = System.Drawing.Color.Blue;
arc.LineFormat.Weight = 2;
// Demonstrate EndArrowheadStyle property
arc.EndArrowheadStyle = MsoArrowheadStyle.ArrowOpen;
arc.EndArrowheadWidth = MsoArrowheadWidth.Medium;
arc.EndArrowheadLength = MsoArrowheadLength.Medium;
// Save the workbook
workbook.Save("ArcShapeEndArrowheadStyleDemo.xlsx");
// Display status
Console.WriteLine("Arc shape created with EndArrowheadStyle: " + arc.EndArrowheadStyle);
}
}
}
```
### See Also
* enum [MsoArrowheadStyle](../../msoarrowheadstyle/)
* class [ArcShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
