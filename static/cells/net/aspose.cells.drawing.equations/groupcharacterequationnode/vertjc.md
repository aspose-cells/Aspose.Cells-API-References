##GroupCharacterEquationNode.VertJc
GroupCharacterEquationNode property. This attribute combined with pos of groupChrPr specifies the vertical layout of the groupChr object. Where pos specifies the position of the grouping character vertJc specifies the alignment of the object with respect to the baseline
## GroupCharacterEquationNode.VertJc property
This attribute, combined with pos of groupChrPr, specifies the vertical layout of the groupChr object. Where pos specifies the position of the grouping character, vertJc specifies the alignment of the object with respect to the baseline.
```csharp
public EquationCharacterPositionType VertJc { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing.Equations;
using System;
public class GroupCharacterEquationNodePropertyVertJcDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a text box shape to contain the equation
var shape = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 100, 100);
// Create a GroupCharacterEquationNode instance
var equationNode = (GroupCharacterEquationNode)shape.GetEquationParagraph().AddChild(EquationNodeType.GroupChr);
try
{
// Set initial properties for the equation node
equationNode.GroupChr = "⏟";
equationNode.ChrType = EquationCombiningCharacterType.BottomCurlyBracket;
equationNode.Position = EquationCharacterPositionType.Bottom;
// Demonstrate VertJc property (read and write)
Console.WriteLine("Initial VertJc value: " + equationNode.VertJc);
// Change the VertJc value
equationNode.VertJc = EquationCharacterPositionType.Top;
Console.WriteLine("Modified VertJc value: " + equationNode.VertJc);
// Save the workbook
workbook.Save("VertJcDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
}
}
}
```
### See Also
* enum [EquationCharacterPositionType](../../equationcharacterpositiontype/)
* class [GroupCharacterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
