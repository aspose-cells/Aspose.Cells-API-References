##GroupCharacterEquationNode.GroupChr
GroupCharacterEquationNode property. Specifies a symboldefault U23DF. It is strongly recommended to use attribute ChrType to set accent character. Use this property setting if you cannot find the character you need in a known type
## GroupCharacterEquationNode.GroupChr property
Specifies a symbol(default U+23DF). It is strongly recommended to use attribute ChrType to set accent character. Use this property setting if you cannot find the character you need in a known type.
```csharp
public string GroupChr { get; set; }
```
### Remarks
It should be noted that this property only accepts one character, and if multiple characters are passed in, only the first character is accepted.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;
namespace AsposeCellsExamples
{
public class GroupCharacterEquationNodePropertyGroupChrDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add an equation to the first worksheet
TextBox textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);
// Get the equation's root node
EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
// Create a group character node with rightwards double arrow
GroupCharacterEquationNode groupNode =
(GroupCharacterEquationNode)mathNode.AddChild(EquationNodeType.GroupChr);
groupNode.Position = EquationCharacterPositionType.Top;
groupNode.ChrType = EquationCombiningCharacterType.RightwardsDoubleArrow;
// Add base text to the group character
EquationNode baseNode = groupNode.AddChild(EquationNodeType.Base);
TextRunEquationNode textNode =
(TextRunEquationNode)(baseNode.AddChild(EquationNodeType.Text));
textNode.Text = "abc";
// Demonstrate GroupChr property usage
Console.WriteLine("Group Character: " + groupNode.GroupChr); // Should output "⇒"
// Save the workbook
workbook.Save("GroupCharacterEquationDemo.xlsx");
}
}
}
```
### See Also
* class [GroupCharacterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
