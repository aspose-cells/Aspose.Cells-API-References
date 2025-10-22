##GroupCharacterEquationNode.Position
GroupCharacterEquationNode property. This attribute specifies the position of the character in the object
## GroupCharacterEquationNode.Position property
This attribute specifies the position of the character in the object
```csharp
public EquationCharacterPositionType Position { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;
namespace AsposeCellsExamples
{
public class GroupCharacterEquationNodePropertyPositionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add an equation shape to the first worksheet
TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);
// Get the equation paragraph and add a group character node
EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
GroupCharacterEquationNode groupNode = (GroupCharacterEquationNode)mathNode.AddChild(EquationNodeType.GroupChr);
// Set the position property (core demonstration)
groupNode.Position = EquationCharacterPositionType.Top;
groupNode.ChrType = EquationCombiningCharacterType.RightwardsDoubleArrow;
// Add base text
EquationNode baseNode = groupNode.AddChild(EquationNodeType.Base);
TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
textNode.Text = "abc";
// Save the workbook
string outputPath = "GroupCharacterEquationDemo.xlsx";
workbook.Save(outputPath);
Console.WriteLine("Equation with group character position set to Top has been created successfully.");
}
}
}
```
### See Also
* enum [EquationCharacterPositionType](../../equationcharacterpositiontype/)
* class [GroupCharacterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
