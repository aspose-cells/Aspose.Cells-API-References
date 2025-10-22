##TextRunEquationNode.Text
TextRunEquationNode property. Set the content of the text nodeUsually a node object per character
## TextRunEquationNode.Text property
Set the content of the text node(Usually a node object per character).
```csharp
public string Text { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;
namespace AsposeCellsExamples
{
public class TextRunEquationNodePropertyTextDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add an equation shape to the first worksheet
TextBox textBox = (TextBox)workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);
// Get the root equation node
EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
// Create a fraction equation
FractionEquationNode fractionNode = (FractionEquationNode)mathNode.AddChild(EquationNodeType.Fraction);
fractionNode.FractionType = EquationFractionType.Skewed;
// Add numerator with text "X"
EquationComponentNode numerator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Numerator);
TextRunEquationNode numeratorText = (TextRunEquationNode)numerator.AddChild(EquationNodeType.Text);
numeratorText.Text = "X";
// Add denominator with text "Y"
EquationComponentNode denominator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Denominator);
TextRunEquationNode denominatorText = (TextRunEquationNode)denominator.AddChild(EquationNodeType.Text);
denominatorText.Text = "Y";
// Save the workbook
workbook.Save("TextRunEquationNodeDemo.xlsx");
// Verify the saved file by loading it back
Workbook loadedWorkbook = new Workbook("TextRunEquationNodeDemo.xlsx");
TextBox loadedTextBox = (TextBox)loadedWorkbook.Worksheets[0].Shapes[0];
// Access the text properties to demonstrate functionality
TextRunEquationNode loadedNumeratorText = (TextRunEquationNode)((FractionEquationNode)loadedTextBox
.GetEquationParagraph()
.GetChild(0)
.GetChild(0))
.GetChild(0)
.GetChild(0);
Console.WriteLine("Numerator text: " + loadedNumeratorText.Text);
}
}
}
```
### See Also
* class [TextRunEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
