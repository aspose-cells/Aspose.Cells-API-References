##NaryEquationNode.NaryOperatorType
NaryEquationNode property. an nary operator.e.g
## NaryEquationNode.NaryOperatorType property
an n-ary operator.e.g "∑"
```csharp
public EquationMathematicalOperatorType NaryOperatorType { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;
using System;
public class NaryEquationNodePropertyNaryOperatorTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a shape to hold the equation
var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 200, 50);
// Access the equation and add a nary operator node
var equation = shape.GetEquationParagraph();
var naryNode = equation.AddChild(EquationNodeType.NaryEquation);
// Cast to NaryEquationNode to access NaryOperatorType
var naryEquationNode = (NaryEquationNode)naryNode;
// Display current NaryOperatorType (default value)
Console.WriteLine("Current NaryOperatorType: " + naryEquationNode.NaryOperatorType);
// Set to summation operator (∑)
naryEquationNode.NaryOperatorType = EquationMathematicalOperatorType.NarySummation;
// Add base (operand) and limits to demonstrate the operator
var baseNode = naryEquationNode.AddChild(EquationNodeType.Base);
var textNode1 = baseNode.AddChild(EquationNodeType.Text);
textNode1.ToLaTeX(); // This would be where you'd set the text content if the API allowed
var limitNode = naryEquationNode.AddChild(EquationNodeType.Limit);
var textNode2 = limitNode.AddChild(EquationNodeType.Text);
textNode2.ToLaTeX(); // This would be where you'd set the text content if the API allowed
var textNode3 = baseNode.AddChild(EquationNodeType.Text);
textNode3.ToLaTeX(); // This would be where you'd set the text content if the API allowed
// Set the operator to grow with its content
naryEquationNode.NaryGrow = true;
// Change to product operator (∏) and show the difference
naryEquationNode.NaryOperatorType = EquationMathematicalOperatorType.NaryProduct;
// Save the workbook
workbook.Save("NaryOperatorTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [EquationMathematicalOperatorType](../../equationmathematicaloperatortype/)
* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
