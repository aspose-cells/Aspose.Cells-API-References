##DelimiterEquationNode.EndChar
DelimiterEquationNode property. Delimiter ending character
## DelimiterEquationNode.EndChar property
Delimiter ending character.
```csharp
public string EndChar { get; set; }
```
### Remarks
It should be noted that this property only accepts one character, and if multiple characters are passed in, only the first character is accepted.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;
namespace AsposeCellsExamples
{
public class DelimiterEquationNodePropertyEndCharDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
var textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);
// Get the equation node
var mathNode = textBox.GetEquationParagraph().GetChild(0);
// Create a delimiter node with custom end character
var delimiterNode = (DelimiterEquationNode)mathNode.AddChild(EquationNodeType.Delimiter);
delimiterNode.BeginChar = "[";
delimiterNode.EndChar = "]"; // Demonstrating EndChar property
delimiterNode.DelimiterShape = EquationDelimiterShapeType.Match;
// Add content inside the delimiter
var baseNode = delimiterNode.AddChild(EquationNodeType.Base);
var textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
textNode.Text = "Content";
// Save and verify
string outputPath = "DelimiterEquationDemo.xlsx";
workbook.Save(outputPath);
// Verify the saved file
Workbook verifyWorkbook = new Workbook(outputPath);
var verifyTextBox = (TextBox)verifyWorkbook.Worksheets[0].Shapes[0];
var verifyNode = (DelimiterEquationNode)verifyTextBox.GetEquationParagraph().GetChild(0).GetChild(0);
Console.WriteLine("BeginChar: " + verifyNode.BeginChar);
Console.WriteLine("EndChar: " + verifyNode.EndChar); // Output the EndChar value
}
}
}
```
### See Also
* class [DelimiterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
