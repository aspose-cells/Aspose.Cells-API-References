##EquationNode.RemoveAllChildren
EquationNode method. Removes all the child nodes of the current node
## EquationNode.RemoveAllChildren method
Removes all the child nodes of the current node.
```csharp
public void RemoveAllChildren()
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;
using System;
public class EquationNodeMethodRemoveAllChildrenDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a shape to hold the equation
var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 0, 0);
// Get the equation node
var equationNode = ((TextBox)shape).GetEquationParagraph();
// Add some child nodes to the equation
var fractionNode = equationNode.AddChild(EquationNodeType.Fraction);
var numerator = fractionNode.AddChild(EquationNodeType.Numerator);
numerator.AddChild(EquationNodeType.Text).ToLaTeX(); // Access text content through ToLaTeX or ToMathML
var denominator = fractionNode.AddChild(EquationNodeType.Denominator);
denominator.AddChild(EquationNodeType.Text).ToLaTeX(); // Access text content through ToLaTeX or ToMathML
Console.WriteLine($"Equation before RemoveAllChildren: {equationNode.ToMathML()}");
try
{
// Call the RemoveAllChildren method
equationNode.RemoveAllChildren();
Console.WriteLine("Method executed successfully");
Console.WriteLine($"Equation after RemoveAllChildren: {equationNode.ToMathML()}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing RemoveAllChildren method: {ex.Message}");
}
// Save the result
workbook.Save("EquationNodeMethodRemoveAllChildrenDemo.xlsx");
}
}
}
```
### See Also
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
