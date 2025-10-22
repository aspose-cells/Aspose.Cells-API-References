##NaryEquationNode.NaryGrow
NaryEquationNode property. This attribute specifies the growth property of nary operators at the document level. When off nary operators such as integrals and summations do not grow to match the size of their operand height. When on the nary operator grows vertically to match its operand height
## NaryEquationNode.NaryGrow property
This attribute specifies the growth property of n-ary operators at the document level. When off, n-ary operators such as integrals and summations do not grow to match the size of their operand height. When on, the n-ary operator grows vertically to match its operand height.
```csharp
public bool NaryGrow { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;
namespace AsposeCellsExamples
{
public class NaryEquationNodePropertyNaryGrowDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add equation shape
TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);
// Get the equation node
EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
// Create a nary operator node with NaryGrow property set to true
NaryEquationNode naryNode = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);
naryNode.NaryOperator = "∑";
naryNode.NaryGrow = true; // This is the key property we're demonstrating
// Add subscript (optional)
EquationNode sub = naryNode.AddChild(EquationNodeType.Subscript);
TextRunEquationNode subText = (TextRunEquationNode)sub.AddChild(EquationNodeType.Text);
subText.Text = "i=1";
// Add superscript (optional)
EquationNode sup = naryNode.AddChild(EquationNodeType.Superscript);
TextRunEquationNode supText = (TextRunEquationNode)sup.AddChild(EquationNodeType.Text);
supText.Text = "n";
// Add base (required)
EquationNode baseNode = naryNode.AddChild(EquationNodeType.Base);
TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
baseText.Text = "x_i";
// Save the workbook
workbook.Save("NaryGrowDemo.xlsx");
Console.WriteLine("Equation with NaryGrow property created successfully.");
}
}
}
```
### See Also
* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
