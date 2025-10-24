##EquationNode.GetChild
EquationNode method. Returns the node at the specified index among the children of the current node
## EquationNode.GetChild method
Returns the node at the specified index among the children of the current node.
```csharp
public EquationNode GetChild(int index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | Index of the node |
### Return Value
Returns the corresponding node if the specified node exists, otherwise returns null.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;
namespace AsposeCellsExamples
{
public class EquationNodeMethodGetChildWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add an equation shape to the first worksheet
TextBox textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);
// Get the equation paragraph and its first child node
EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
// Add a delimiter node as child
DelimiterEquationNode delimiterNode = (DelimiterEquationNode)mathNode.AddChild(EquationNodeType.Delimiter);
delimiterNode.BeginChar = "[";
delimiterNode.EndChar = "]";
// Add a fraction node inside the delimiter
EquationNode baseNode = delimiterNode.AddChild(EquationNodeType.Base);
FractionEquationNode fractionNode = (FractionEquationNode)baseNode.AddChild(EquationNodeType.Fraction);
// Add numerator and denominator
EquationComponentNode numerator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Numerator);
TextRunEquationNode textNode = (TextRunEquationNode)numerator.AddChild(EquationNodeType.Text);
textNode.Text = "X";
EquationComponentNode denominator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Denominator);
textNode = (TextRunEquationNode)denominator.AddChild(EquationNodeType.Text);
textNode.Text = "Y";
// Save the workbook
workbook.Save("EquationNodeGetChildDemo.xlsx");
// Load the saved file to verify
Workbook loadedWorkbook = new Workbook("EquationNodeGetChildDemo.xlsx");
TextBox loadedTextBox = (TextBox)loadedWorkbook.Worksheets[0].Shapes[0];
// Demonstrate GetChild method
EquationNode loadedMathNode = loadedTextBox.GetEquationParagraph().GetChild(0);
DelimiterEquationNode loadedDelimiter = (DelimiterEquationNode)loadedMathNode.GetChild(0);
Console.WriteLine("Delimiter BeginChar: " + loadedDelimiter.BeginChar);
Console.WriteLine("Delimiter EndChar: " + loadedDelimiter.EndChar);
EquationNode loadedBaseNode = loadedDelimiter.GetChild(0);
FractionEquationNode loadedFraction = (FractionEquationNode)loadedBaseNode.GetChild(0);
Console.WriteLine("Fraction node type: " + loadedFraction.EquationType);
}
}
}
```
### See Also
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
