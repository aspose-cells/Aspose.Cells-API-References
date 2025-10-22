##EquationComponentNode.Equals
EquationComponentNode method. Determine whether the current equation node is equal to the specified node
## EquationComponentNode.Equals method
Determine whether the current equation node is equal to the specified node
```csharp
public override bool Equals(object obj)
```
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | The specified node |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;
using System;
public class EquationComponentNodeMethodEqualsWithObjectDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);
//test get mathnode
EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
//test insert Fraction
FractionEquationNode node = (FractionEquationNode)mathNode.AddChild(EquationNodeType.Fraction);
node.FractionType = EquationFractionType.Skewed;
string str1 = "A";
EquationComponentNode numerator = (EquationComponentNode)node.AddChild(EquationNodeType.Numerator);
TextRunEquationNode TR = (TextRunEquationNode)(numerator.AddChild(EquationNodeType.Text));
TR.Text = str1;
string str2 = "B";
EquationComponentNode denominator = (EquationComponentNode)node.AddChild(EquationNodeType.Denominator);
TR = (TextRunEquationNode)(denominator.AddChild(EquationNodeType.Text));
TR.Text = str2;
// Compare the nodes using Equals method
bool areEqual = numerator?.Equals((object)denominator) ?? false;
// Display the comparison result
Console.WriteLine($"Nodes are equal: {areEqual}");
workbook.Save("EquationComponentNodeMethodEqualsWithObjectDemo.xlsx");
}
}
}
```
### See Also
* class [EquationComponentNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
