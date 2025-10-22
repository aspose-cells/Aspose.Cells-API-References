##EquationNode.Type
EquationNode property. Represents the type of the node
## EquationNode.Type property
Represents the type of the node.
```csharp
public override TextNodeType Type { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;
using Aspose.Cells.Drawing.Texts;
using System;
public class EquationNodePropertyTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create an equation shape
var shape = worksheet.Shapes.AddEquation(0, 0, 300, 100, 0, 0);
var equationRoot = shape.GetEquationParagraph();
// Create different types of equation nodes
var fractionNode = equationRoot.AddChild(EquationNodeType.Fraction);
var textNode = equationRoot.AddChild(EquationNodeType.Text) as TextRunEquationNode;
textNode.Text = "Sample Text";
// Display the Type property for different nodes
Console.WriteLine($"Root equation node type: {equationRoot.Type}");
Console.WriteLine($"Fraction node type: {fractionNode.Type}");
Console.WriteLine($"Text node type: {textNode.Type}");
// Create a complex equation structure
var numerator = fractionNode.AddChild(EquationNodeType.Numerator);
var numeratorText = numerator.AddChild(EquationNodeType.Text) as TextRunEquationNode;
numeratorText.Text = "Numerator";
var denominator = fractionNode.AddChild(EquationNodeType.Denominator);
var denominatorText = denominator.AddChild(EquationNodeType.Text) as TextRunEquationNode;
denominatorText.Text = "Denominator";
// Check types of child nodes
Console.WriteLine($"Numerator node type: {numerator.Type}");
Console.WriteLine($"Numerator text node type: {numeratorText.Type}");
Console.WriteLine($"Denominator node type: {denominator.Type}");
// Demonstrate how Type affects node behavior
if (textNode.Type == TextNodeType.TextRun)
{
Console.WriteLine("Text node is a TextRun type - can contain text content");
}
if (fractionNode.Type == TextNodeType.Equation)
{
Console.WriteLine("Fraction node is an Equation type - can contain child nodes");
}
// Save the result
workbook.Save("EquationNodePropertyTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [TextNodeType](../../../aspose.cells.drawing.texts/textnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
