##GroupCharacterEquationNode.ChrType
GroupCharacterEquationNode property. Specify combining characters by type value
## GroupCharacterEquationNode.ChrType property
Specify combining characters by type value.
```csharp
public EquationCombiningCharacterType ChrType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;
namespace AsposeCellsExamples
{
public class GroupCharacterEquationNodePropertyChrTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add an equation to the first worksheet
TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);
// Get the equation's root node
EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
// Add a group character node
GroupCharacterEquationNode groupNode = (GroupCharacterEquationNode)mathNode.AddChild(EquationNodeType.GroupChr);
// Set group character properties
groupNode.Position = EquationCharacterPositionType.Top;
groupNode.ChrType = EquationCombiningCharacterType.RightwardsDoubleArrow;
// Add base text
EquationNode baseNode = groupNode.AddChild(EquationNodeType.Base);
TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
textNode.Text = "test";
// Save the workbook
workbook.Save("GroupCharacterEquationDemo.xlsx");
// Verify the saved file
Workbook verifyWorkbook = new Workbook("GroupCharacterEquationDemo.xlsx");
TextBox verifyTextBox = (TextBox)verifyWorkbook.Worksheets[0].Shapes[0];
GroupCharacterEquationNode verifyNode = (GroupCharacterEquationNode)verifyTextBox.GetEquationParagraph()
.GetChild(0).GetChild(0);
Console.WriteLine("Group Character Type: " + verifyNode.ChrType);
Console.WriteLine("Group Character: " + verifyNode.GroupChr);
Console.WriteLine("Base Text: " + ((TextRunEquationNode)verifyNode.GetChild(0).GetChild(0)).Text);
}
}
}
```
### See Also
* enum [EquationCombiningCharacterType](../../equationcombiningcharactertype/)
* class [GroupCharacterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
