##EquationNodeParagraph.Justification
EquationNodeParagraph property. This specifies justification of the math paragraph a series of adjacent equations within the same paragraph. A math paragraph can be Left Justified Right Justified Centered or Centered as Group. By default the math paragraph is Centered as Group. This means that the equations can be aligned with respect to each other but the entire group of equations is centered as a whole
## EquationNodeParagraph.Justification property
This specifies justification of the math paragraph (a series of adjacent equations within the same paragraph). A math paragraph can be Left Justified, Right Justified, Centered, or Centered as Group. By default, the math paragraph is Centered as Group. This means that the equations can be aligned with respect to each other, but the entire group of equations is centered as a whole.
```csharp
public EquationHorizontalJustificationType Justification { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;
using System;
public class EquationNodeParagraphPropertyJustificationDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a shape to hold the equation
var shape = worksheet.Shapes.AddTextBox(0, 0, 200, 50, 200, 50);
// Get the equation paragraph
var equationParagraph = shape.GetEquationParagraph() as EquationNodeParagraph;
// Display current justification value
Console.WriteLine("Current Justification value: " + equationParagraph.Justification);
// Set different justification values and observe effects
equationParagraph.Justification = EquationHorizontalJustificationType.Left;
Console.WriteLine("Set to Left justification");
equationParagraph.Justification = EquationHorizontalJustificationType.Center;
Console.WriteLine("Set to Center justification");
equationParagraph.Justification = EquationHorizontalJustificationType.CenterGroup;
Console.WriteLine("Set to CenterGroup justification");
equationParagraph.Justification = EquationHorizontalJustificationType.Right;
Console.WriteLine("Set to Right justification");
// Save the workbook
workbook.Save("EquationJustificationDemo.xlsx");
}
}
}
```
### See Also
* enum [EquationHorizontalJustificationType](../../equationhorizontaljustificationtype/)
* class [EquationNodeParagraph](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
