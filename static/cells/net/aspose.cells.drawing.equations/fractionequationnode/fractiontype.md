##FractionEquationNode.FractionType
FractionEquationNode property. This specifies the type of fraction  the default is Bar
## FractionEquationNode.FractionType property
This specifies the type of fraction ; the default is 'Bar'.
```csharp
public EquationFractionType FractionType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;
namespace AsposeCellsExamples
{
public class FractionEquationNodePropertyFractionTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add equation shape
TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);
// Get math node
EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
// Create fraction node
FractionEquationNode fractionNode = (FractionEquationNode)mathNode.AddChild(EquationNodeType.Fraction);
fractionNode.FractionType = EquationFractionType.Skewed;
// Add numerator
EquationComponentNode numerator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Numerator);
TextRunEquationNode numeratorText = (TextRunEquationNode)numerator.AddChild(EquationNodeType.Text);
numeratorText.Text = "A";
// Add denominator
EquationComponentNode denominator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Denominator);
TextRunEquationNode denominatorText = (TextRunEquationNode)denominator.AddChild(EquationNodeType.Text);
denominatorText.Text = "B";
// Save and verify
string outputPath = "FractionEquationDemo.xlsx";
workbook.Save(outputPath);
// Reload to verify
Workbook verifyWorkbook = new Workbook(outputPath);
TextBox verifyTextBox = (TextBox)verifyWorkbook.Worksheets[0].Shapes[0];
FractionEquationNode verifyFraction = (FractionEquationNode)verifyTextBox.GetEquationParagraph().GetChild(0).GetChild(0);
Console.WriteLine("Fraction Type: " + verifyFraction.FractionType);
Console.WriteLine("Numerator: " + ((TextRunEquationNode)verifyFraction.GetChild(0).GetChild(0)).Text);
Console.WriteLine("Denominator: " + ((TextRunEquationNode)verifyFraction.GetChild(1).GetChild(0)).Text);
}
}
}
```
### See Also
* enum [EquationFractionType](../../equationfractiontype/)
* class [FractionEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
