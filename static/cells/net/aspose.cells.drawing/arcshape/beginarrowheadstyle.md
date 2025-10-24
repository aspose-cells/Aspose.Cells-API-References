##ArcShape.BeginArrowheadStyle
ArcShape property. Gets and sets the begin arrow head style of the line
## ArcShape.BeginArrowheadStyle property
Gets and sets the begin arrow head style of the line.
```csharp
[Obsolete("Use Shape.Line.BeginArrowheadStyle property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MsoArrowheadStyle BeginArrowheadStyle { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please use Shape.Line.BeginArrowheadStyle property. This property will be removed 12 months later since August 2016. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ArcShapePropertyBeginArrowheadStyleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create two arc shapes with different arrowhead styles
ArcShape arc1 = worksheet.Shapes.AddArc(1, 0, 1, 0, 100, 100);
ArcShape arc2 = worksheet.Shapes.AddArc(2, 0, 2, 0, 100, 100);
// Set different arrowhead styles for demonstration
arc1.BeginArrowheadStyle = MsoArrowheadStyle.ArrowOpen;
arc1.BeginArrowheadLength = MsoArrowheadLength.Medium;
arc1.BeginArrowheadWidth = MsoArrowheadWidth.Medium;
arc2.BeginArrowheadStyle = MsoArrowheadStyle.ArrowStealth;
arc2.BeginArrowheadLength = MsoArrowheadLength.Long;
arc2.BeginArrowheadWidth = MsoArrowheadWidth.Wide;
// Display the arrowhead style information
Console.WriteLine("Arc1 Begin Arrowhead Style: " + arc1.BeginArrowheadStyle);
Console.WriteLine("Arc2 Begin Arrowhead Style: " + arc2.BeginArrowheadStyle);
// Save the workbook
workbook.Save("ArcShapeArrowheadDemo.xlsx");
}
}
}
```
### See Also
* enum [MsoArrowheadStyle](../../msoarrowheadstyle/)
* class [ArcShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
