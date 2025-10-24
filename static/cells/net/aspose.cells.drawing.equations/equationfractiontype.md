##Enum EquationFractionType
Aspose.Cells.Drawing.Equations.EquationFractionType enum. This specifies the display style of the fraction bar
## EquationFractionType enumeration
This specifies the display style of the fraction bar.
```csharp
public enum EquationFractionType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Bar | `0` | This specifies that the numerator is above and the denominator below is separated by a bar in the middle. |
| NoBar | `1` | This specifies that the numerator is above and the denominator below is not separated by a bar in the middle. |
| Linear | `2` | This specifies that the numerator is on the left and the denominator is on the right, separated by a '/' in between. |
| Skewed | `3` | This specifies that the numerator is on the upper left and the denominator is on the lower right, separated by a "/". |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;
namespace AsposeCellsExamples
{
public class EquationsClassEquationFractionTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add equation shape
TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);
// Get math node and add fraction
EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
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
workbook.Save("EquationFractionTypeDemo.xlsx");
Console.WriteLine("Equation with skewed fraction created successfully.");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)
