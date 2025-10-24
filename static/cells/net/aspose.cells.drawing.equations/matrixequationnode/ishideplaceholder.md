##MatrixEquationNode.IsHidePlaceholder
MatrixEquationNode property. This attribute specifies the Hide Placeholders property on a matrix. When this property is on placeholders do not appear in the matrix.Default placeholders do appear such that the locations where text can be inserted are made visible
## MatrixEquationNode.IsHidePlaceholder property
This attribute specifies the Hide Placeholders property on a matrix. When this property is on, placeholders do not appear in the matrix.Default, placeholders do appear such that the locations where text can be inserted are made visible.
```csharp
public bool IsHidePlaceholder { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;
namespace AsposeCellsExamples
{
public class MatrixEquationNodePropertyIsHidePlaceholderDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add equation shape
TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);
// Get math node and add matrix
EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
MatrixEquationNode matrixNode = (MatrixEquationNode)mathNode.AddChild(EquationNodeType.Matrix);
// Set matrix properties
matrixNode.BaseJc = EquationVerticalJustificationType.Bottom;
matrixNode.IsHidePlaceholder = true; // Demonstrate IsHidePlaceholder property
// Add 2x2 matrix with diagonal 1s
for (int row = 0; row < 2; row++)
{
EquationNode matrixRow = matrixNode.AddChild(EquationNodeType.MatrixRow);
for (int col = 0; col < 2; col++)
{
EquationNode baseNode = matrixRow.AddChild(EquationNodeType.Base);
TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
textNode.Text = (row == col) ? "1" : "0";
}
}
// Save and verify
string outputPath = "MatrixEquationWithHiddenPlaceholder.xlsx";
workbook.Save(outputPath);
Console.WriteLine("Matrix equation created with IsHidePlaceholder=true. File saved to: " + outputPath);
}
}
}
```
### See Also
* class [MatrixEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
