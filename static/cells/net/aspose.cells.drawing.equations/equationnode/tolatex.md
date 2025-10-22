##EquationNode.ToLaTeX
EquationNode method. Convert this equtation to LaTeX expression
## EquationNode.ToLaTeX method
Convert this equtation to LaTeX expression.
```csharp
public string ToLaTeX()
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing.Equations;
using System;
public class EquationNodeMethodToLaTeXDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a shape to hold the equation
var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 0, 0);
// Get the equation node
var equationNode = shape.GetEquationParagraph();
// Create a simple fraction equation
var fractionNode = equationNode.AddChild(EquationNodeType.Fraction);
var numerator = fractionNode.AddChild(EquationNodeType.Numerator);
var numeratorText = numerator.AddChild(EquationNodeType.Text) as TextRunEquationNode;
numeratorText.Text = "1";
var denominator = fractionNode.AddChild(EquationNodeType.Denominator);
var denominatorText = denominator.AddChild(EquationNodeType.Text) as TextRunEquationNode;
denominatorText.Text = "2";
try
{
// Call the ToLaTeX method
string latexExpression = equationNode.ToLaTeX();
// Display the result
Console.WriteLine("LaTeX expression: " + latexExpression);
// Add the LaTeX output to a cell
worksheet.Cells["A1"].PutValue("LaTeX Output:");
worksheet.Cells["B1"].PutValue(latexExpression);
}
catch (Exception ex)
{
Console.WriteLine($"Error executing ToLaTeX method: {ex.Message}");
}
// Save the result
workbook.Save("EquationToLaTeXDemo.xlsx");
}
}
}
```
### See Also
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
