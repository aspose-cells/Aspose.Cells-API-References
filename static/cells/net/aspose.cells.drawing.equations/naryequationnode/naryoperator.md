##NaryEquationNode.NaryOperator
NaryEquationNode property. an nary operator.e.g . It is strongly recommended to use attribute NaryOperatorType to set nary operator. Use this property setting if you cannot find the character you need in a known type
## NaryEquationNode.NaryOperator property
an n-ary operator.e.g "∑". It is strongly recommended to use attribute NaryOperatorType to set n-ary operator. Use this property setting if you cannot find the character you need in a known type.
```csharp
public string NaryOperator { get; set; }
```
### Remarks
It should be noted that this property only accepts one character, and if multiple characters are passed in, only the first character is accepted.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
using Aspose.Cells.Drawing.Equations;
namespace AsposeCellsExamples
{
public class NaryEquationNodePropertyNaryOperatorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add an equation shape
TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);
// Get the equation node
EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
// Create a nary operator node
NaryEquationNode naryNode = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);
// Set nary operator properties
naryNode.NaryOperator = "\u2211"; // Summation symbol
naryNode.NaryGrow = true;
// Add subscript (optional)
EquationNode subscript = naryNode.AddChild(EquationNodeType.Subscript);
TextRunEquationNode subscriptText = (TextRunEquationNode)subscript.AddChild(EquationNodeType.Text);
subscriptText.Text = "i=1";
// Add superscript (optional)
EquationNode superscript = naryNode.AddChild(EquationNodeType.Superscript);
TextRunEquationNode superscriptText = (TextRunEquationNode)superscript.AddChild(EquationNodeType.Text);
superscriptText.Text = "n";
// Add base expression
EquationNode baseNode = naryNode.AddChild(EquationNodeType.Base);
TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
baseText.Text = "x_i";
// Save the workbook
workbook.Save("NaryOperatorDemo.xlsx");
Console.WriteLine("Nary operator equation created successfully.");
}
}
}
```
### See Also
* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
