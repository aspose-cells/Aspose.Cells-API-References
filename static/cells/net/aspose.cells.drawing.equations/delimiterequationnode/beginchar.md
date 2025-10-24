##DelimiterEquationNode.BeginChar
DelimiterEquationNode property. Delimiter beginning character
## DelimiterEquationNode.BeginChar property
Delimiter beginning character.
```csharp
public string BeginChar { get; set; }
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
public class DelimiterEquationNodePropertyBeginCharDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add an equation to the first worksheet
var textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);
// Get the equation's root node
var mathNode = textBox.GetEquationParagraph().GetChild(0);
// Add a delimiter node with custom begin/end characters
var delimiterNode = mathNode.AddChild(EquationNodeType.Delimiter) as DelimiterEquationNode;
delimiterNode.BeginChar = "#";
delimiterNode.EndChar = "*";
delimiterNode.DelimiterShape = EquationDelimiterShapeType.Match;
// Add content inside the delimiter
var baseNode = delimiterNode.AddChild(EquationNodeType.Base);
var textNode = baseNode.AddChild(EquationNodeType.Text) as TextRunEquationNode;
textNode.Text = "Sample Content";
// Save the workbook
string outputPath = "DelimiterEquationDemo.xlsx";
workbook.Save(outputPath);
Console.WriteLine("Workbook saved with custom delimiter equation. BeginChar: " + delimiterNode.BeginChar);
}
}
}
```
### See Also
* class [DelimiterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
