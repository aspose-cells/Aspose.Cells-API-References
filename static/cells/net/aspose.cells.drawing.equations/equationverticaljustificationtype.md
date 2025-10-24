##Enum EquationVerticalJustificationType
Aspose.Cells.Drawing.Equations.EquationVerticalJustificationType enum. This specifies the default vertical justification of equations in the document
## EquationVerticalJustificationType enumeration
This specifies the default vertical justification of equations in the document.
```csharp
public enum EquationVerticalJustificationType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Top | `0` | top |
| Center | `1` | center |
| Bottom | `2` | bottom |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;
namespace AsposeCellsExamples
{
public class EquationsClassEquationVerticalJustificationTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add an equation shape to the first worksheet
TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);
// Get the equation paragraph and add a matrix node
EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
MatrixEquationNode matrixNode = (MatrixEquationNode)mathNode.AddChild(EquationNodeType.Matrix);
// Set matrix properties
matrixNode.BaseJc = EquationVerticalJustificationType.Bottom;
matrixNode.IsHidePlaceholder = true;
// Add matrix rows and columns
for (int i = 0; i < 2; i++)
{
EquationNode rowNode = matrixNode.AddChild(EquationNodeType.MatrixRow);
for (int j = 0; j < 2; j++)
{
EquationNode baseNode = rowNode.AddChild(EquationNodeType.Base);
TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
textNode.Text = (i == j) ? "1" : "0";
}
}
// Save the workbook
string outputPath = "EquationVerticalJustificationDemo.xlsx";
workbook.Save(outputPath);
Console.WriteLine("File saved with vertical justification demo: " + outputPath);
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)
