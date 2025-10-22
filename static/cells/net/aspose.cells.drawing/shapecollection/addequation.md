##ShapeCollection.AddEquation
ShapeCollection method. Add an equation object to the worksheet
## ShapeCollection.AddEquation method
Add an equation object to the worksheet.
```csharp
public TextBox AddEquation(int topRow, int top, int leftColumn, int left, int height, int width)
```
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | Int32 | The top row index. |
| top | Int32 | The vertical offset its top row, in unit of pixel. |
| leftColumn | Int32 | The left column index. |
| left | Int32 | The horizontal offset from its left column, in unit of pixel. |
| height | Int32 | The height of equation, in unit of pixel. |
| width | Int32 | The width of equation, in unit of pixel. |
### Examples
```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;
namespace AsposeCellsExamples
{
public class ShapeCollectionMethodAddEquationWithInt32Int32Int32Int32Int32Int32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);
EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
FractionEquationNode fraction = (FractionEquationNode)mathNode.AddChild(EquationNodeType.Fraction);
fraction.FractionType = EquationFractionType.Skewed;
EquationComponentNode numerator = (EquationComponentNode)fraction.AddChild(EquationNodeType.Numerator);
TextRunEquationNode numText = (TextRunEquationNode)numerator.AddChild(EquationNodeType.Text);
numText.Text = "A";
EquationComponentNode denominator = (EquationComponentNode)fraction.AddChild(EquationNodeType.Denominator);
TextRunEquationNode denText = (TextRunEquationNode)denominator.AddChild(EquationNodeType.Text);
denText.Text = "B";
workbook.Save("ShapeEquationDemo.xlsx");
}
}
}
```
### See Also
* class [TextBox](../../textbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
