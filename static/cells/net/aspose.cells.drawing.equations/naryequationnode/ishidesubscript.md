##NaryEquationNode.IsHideSubscript
NaryEquationNode property. Whether to display the lower bound
## NaryEquationNode.IsHideSubscript property
Whether to display the lower bound
```csharp
public bool IsHideSubscript { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;
namespace AsposeCellsExamples
{
public class NaryEquationNodePropertyIsHideSubscriptDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
TextBox textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);
EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
// Create a Nary equation node with hidden subscript
NaryEquationNode node = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);
node.NaryOperator = "∫";
node.IsHideSubscript = true; // Hide subscript
node.IsHideSuperscript = false; // Show superscript
// Add subscript (will be hidden)
EquationNode sub = node.AddChild(EquationNodeType.Subscript);
TextRunEquationNode subText = (TextRunEquationNode)(sub.AddChild(EquationNodeType.Text));
subText.Text = "1";
// Add superscript (will be visible)
EquationNode sup = node.AddChild(EquationNodeType.Superscript);
TextRunEquationNode supText = (TextRunEquationNode)(sup.AddChild(EquationNodeType.Text));
supText.Text = "5";
// Add base
EquationNode e = node.AddChild(EquationNodeType.Base);
TextRunEquationNode baseText = (TextRunEquationNode)(e.AddChild(EquationNodeType.Text));
baseText.Text = "C";
// Save and verify
workbook.Save("NaryEquationDemo.xlsx");
// Reload to verify properties
Workbook loadedWorkbook = new Workbook("NaryEquationDemo.xlsx");
TextBox loadedTextBox = (TextBox)loadedWorkbook.Worksheets[0].Shapes[0];
EquationNode loadedMathNode = loadedTextBox.GetEquationParagraph().GetChild(0);
NaryEquationNode loadedNode = (NaryEquationNode)loadedMathNode.GetChild(0);
Console.WriteLine("Nary Operator: " + loadedNode.NaryOperator);
Console.WriteLine("IsHideSubscript: " + loadedNode.IsHideSubscript);
Console.WriteLine("IsHideSuperscript: " + loadedNode.IsHideSuperscript);
}
}
}
```
### See Also
* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
