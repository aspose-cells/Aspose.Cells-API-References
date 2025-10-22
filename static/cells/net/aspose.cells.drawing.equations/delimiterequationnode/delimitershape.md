##DelimiterEquationNode.DelimiterShape
DelimiterEquationNode property. Specifies the shape of delimiters in the delimiter object
## DelimiterEquationNode.DelimiterShape property
Specifies the shape of delimiters in the delimiter object.
```csharp
public EquationDelimiterShapeType DelimiterShape { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;
namespace AsposeCellsExamples
{
public class DelimiterEquationNodePropertyDelimiterShapeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
var textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);
// Get the equation node
var mathNode = textBox.GetEquationParagraph().GetChild(0);
// Create delimiter node with custom shape
var delimiterNode = mathNode.AddChild(EquationNodeType.Delimiter) as DelimiterEquationNode;
delimiterNode.DelimiterShape = EquationDelimiterShapeType.Match;
delimiterNode.BeginChar = "[";
delimiterNode.EndChar = "]";
// Add content inside the delimiter
var baseNode = delimiterNode.AddChild(EquationNodeType.Base);
var textNode = baseNode.AddChild(EquationNodeType.Text) as TextRunEquationNode;
textNode.Text = "Content";
// Save the workbook
workbook.Save("DelimiterShapeDemo.xlsx");
Console.WriteLine("Workbook saved with delimiter equation demonstrating DelimiterShape property.");
}
}
}
```
### See Also
* enum [EquationDelimiterShapeType](../../equationdelimitershapetype/)
* class [DelimiterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
