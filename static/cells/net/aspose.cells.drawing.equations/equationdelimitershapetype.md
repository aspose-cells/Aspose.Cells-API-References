##Enum EquationDelimiterShapeType
Aspose.Cells.Drawing.Equations.EquationDelimiterShapeType enum. This specifies the shape of delimiters in the delimiter object
## EquationDelimiterShapeType enumeration
This specifies the shape of delimiters in the delimiter object.
```csharp
public enum EquationDelimiterShapeType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Centered | `0` | The divider is centered around the entire height of its content. |
| Match | `1` | The divider is altered to exactly match their contents' height. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;
namespace AsposeCellsExamples
{
public class EquationsClassEquationDelimiterShapeTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add equation shape
TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);
// Get equation node
EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
// Create delimiter node with Match shape type
DelimiterEquationNode delimiterNode = (DelimiterEquationNode)mathNode.AddChild(EquationNodeType.Delimiter);
delimiterNode.DelimiterShape = EquationDelimiterShapeType.Match;
delimiterNode.BeginChar = "{";
delimiterNode.EndChar = "}";
// Add content inside the delimiter
EquationNode baseNode = delimiterNode.AddChild(EquationNodeType.Base);
TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
textNode.Text = "Content";
// Save the workbook
workbook.Save("EquationDelimiterShapeTypeDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)
