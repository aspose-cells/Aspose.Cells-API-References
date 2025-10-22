##EquationNode.ToMathML
EquationNode method. Convert this equtation to MathML expression
## EquationNode.ToMathML method
Convert this equtation to MathML expression.
```csharp
public string ToMathML()
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing.Equations;
using System;
public class EquationNodeMethodToMathMLDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create an equation shape - added width parameter (300) and height parameter (100)
var shape = worksheet.Shapes.AddEquation(0, 0, 300, 100, 300, 100);
var equation = shape.GetEquationParagraph();
// Build a simple equation: (a+b)^2 = a^2 + 2ab + b^2
var equationNode = equation.AddChild(EquationNodeType.Text);
var textNode = equationNode as TextRunEquationNode;
textNode.Text = "(";
var variableA = equation.AddChild(EquationNodeType.Text) as TextRunEquationNode;
variableA.Text = "a";
var plus = equation.AddChild(EquationNodeType.Text) as TextRunEquationNode;
plus.Text = "+";
var variableB = equation.AddChild(EquationNodeType.Text) as TextRunEquationNode;
variableB.Text = "b";
var closeParen = equation.AddChild(EquationNodeType.Text) as TextRunEquationNode;
closeParen.Text = ")";
var superscript = equation.AddChild(EquationNodeType.Superscript);
var baseNode = superscript.AddChild(EquationNodeType.Base);
var baseText = baseNode.AddChild(EquationNodeType.Text) as TextRunEquationNode;
baseText.Text = "2";
try
{
// Convert the equation to MathML
string mathML = equation.ToMathML();
// Output the MathML to console
Console.WriteLine("MathML Output:");
Console.WriteLine(mathML);
// Write the MathML to a cell
worksheet.Cells["A1"].PutValue("MathML Representation:");
worksheet.Cells["A2"].PutValue(mathML);
// Changed from worksheet.Cells.AutoFitColumns() to:
worksheet.AutoFitColumns();
}
catch (Exception ex)
{
Console.WriteLine($"Error converting to MathML: {ex.Message}");
}
// Save the workbook
workbook.Save("EquationToMathMLDemo.xlsx");
}
}
}
```
### See Also
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
