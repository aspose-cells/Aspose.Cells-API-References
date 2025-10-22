##MatrixEquationNode.BaseJc
MatrixEquationNode property. This attribute specifies the justification of the matrix. Text outside of the matrix can be aligned with the bottom top or center of a matrix function. Default the matrix assumes center justification
## MatrixEquationNode.BaseJc property
This attribute specifies the justification of the matrix. Text outside of the matrix can be aligned with the bottom, top, or center of a matrix function. Default, the matrix assumes center justification.
```csharp
public EquationVerticalJustificationType BaseJc { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;
namespace AsposeCellsExamples
{
public class MatrixEquationNodePropertyBaseJcDemo
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
// Set matrix properties including BaseJc
matrixNode.BaseJc = EquationVerticalJustificationType.Bottom;
matrixNode.IsHidePlaceholder = true;
// Add 2x2 matrix content (identity matrix)
for (int row = 0; row < 2; row++)
{
EquationNode rowNode = matrixNode.AddChild(EquationNodeType.MatrixRow);
for (int col = 0; col < 2; col++)
{
EquationNode baseNode = rowNode.AddChild(EquationNodeType.Base);
TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
textNode.Text = (row == col) ? "1" : "0";
}
}
// Save the workbook
string outputPath = "MatrixEquationDemo.xlsx";
workbook.Save(outputPath);
Console.WriteLine("Matrix equation with BaseJc property demo completed.");
}
}
}
```
### See Also
* enum [EquationVerticalJustificationType](../../equationverticaljustificationtype/)
* class [MatrixEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
