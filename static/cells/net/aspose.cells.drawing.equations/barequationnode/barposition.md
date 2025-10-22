##BarEquationNode.BarPosition
BarEquationNode property. This attribute specifies the position of the bar in the bar object
## BarEquationNode.BarPosition property
This attribute specifies the position of the bar in the bar object
```csharp
public EquationCharacterPositionType BarPosition { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;
namespace AsposeCellsExamples
{
public class BarEquationNodePropertyBarPositionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add an equation shape to the first worksheet
TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);
// Get the equation node
EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
// Create a bar equation node
BarEquationNode barNode = (BarEquationNode)mathNode.AddChild(EquationNodeType.Bar);
// Set the bar position to Top
barNode.BarPosition = EquationCharacterPositionType.Top;
// Add base content for the bar
EquationNode baseNode = barNode.AddChild(EquationNodeType.Base);
TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
textNode.Text = "x";
// Save the workbook
workbook.Save("BarEquationDemo.xlsx");
// Verify the saved file
Workbook verifyWorkbook = new Workbook("BarEquationDemo.xlsx");
TextBox verifyTextBox = (TextBox)verifyWorkbook.Worksheets[0].Shapes[0];
BarEquationNode verifyBarNode = (BarEquationNode)verifyTextBox.GetEquationParagraph().GetChild(0).GetChild(0);
Console.WriteLine("Bar Position: " + verifyBarNode.BarPosition);
Console.WriteLine("Base Content: " + ((TextRunEquationNode)verifyBarNode.GetChild(0).GetChild(0)).Text);
}
}
}
```
### See Also
* enum [EquationCharacterPositionType](../../equationcharacterpositiontype/)
* class [BarEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
