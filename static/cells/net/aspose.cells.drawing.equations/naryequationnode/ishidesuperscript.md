##NaryEquationNode.IsHideSuperscript
NaryEquationNode property. Whether to display the upper bound
## NaryEquationNode.IsHideSuperscript property
Whether to display the upper bound
```csharp
public bool IsHideSuperscript { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;
namespace AsposeCellsExamples
{
public class NaryEquationNodePropertyIsHideSuperscriptDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);
EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
// Create a nary equation node with hidden superscript
NaryEquationNode node = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);
node.NaryOperator = "∫";
node.IsHideSuperscript = true; // Demonstrating the IsHideSuperscript property
// Add base component
EquationNode baseNode = node.AddChild(EquationNodeType.Base);
TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
baseText.Text = "x";
// Add superscript (will be hidden due to IsHideSuperscript = true)
EquationNode supNode = node.AddChild(EquationNodeType.Superscript);
TextRunEquationNode supText = (TextRunEquationNode)supNode.AddChild(EquationNodeType.Text);
supText.Text = "2";
// Save and reload to verify the superscript is hidden
workbook.Save("NaryEquationDemo.xlsx");
workbook = new Workbook("NaryEquationDemo.xlsx");
// Verify the saved equation
TextBox savedTextBox = (TextBox)workbook.Worksheets[0].Shapes[0];
EquationNode savedMathNode = savedTextBox.GetEquationParagraph().GetChild(0);
NaryEquationNode savedNode = (NaryEquationNode)savedMathNode.GetChild(0);
Console.WriteLine("Nary Operator: " + savedNode.NaryOperator);
Console.WriteLine("IsHideSuperscript: " + savedNode.IsHideSuperscript);
Console.WriteLine("Superscript exists: " + (savedNode.GetChild(1).GetChild(0) != null));
}
}
}
```
### See Also
* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
