##RadicalEquationNode.IsDegHide
RadicalEquationNode property. Whether to hide the degree of radicals
## RadicalEquationNode.IsDegHide property
Whether to hide the degree of radicals.
```csharp
public bool IsDegHide { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;
namespace AsposeCellsExamples
{
public class RadicalEquationNodePropertyIsDegHideDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
TextBox textBox = worksheet.Shapes.AddEquation(0, 0, 0, 0, 200, 100);
EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
RadicalEquationNode radicalNode = (RadicalEquationNode)mathNode.AddChild(EquationNodeType.Radical);
radicalNode.IsDegHide = true;
EquationNode degNode = radicalNode.AddChild(EquationNodeType.Degree);
TextRunEquationNode degText = (TextRunEquationNode)degNode.AddChild(EquationNodeType.Text);
degText.Text = "3";
EquationNode baseNode = radicalNode.AddChild(EquationNodeType.Base);
TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
baseText.Text = "x";
workbook.Save("RadicalEquationNodePropertyIsDegHideDemo_Out.xlsx");
Workbook reloadedWorkbook = new Workbook("RadicalEquationNodePropertyIsDegHideDemo_Out.xlsx");
TextBox reloadedTextBox = (TextBox)reloadedWorkbook.Worksheets[0].Shapes[0];
RadicalEquationNode reloadedRadical = (RadicalEquationNode)reloadedTextBox.GetEquationParagraph()
.GetChild(0).GetChild(0);
Console.WriteLine("Reloaded IsDegHide: " + reloadedRadical.IsDegHide);
// Fixed: Use GetChild(0) and null check instead of ChildCount property
EquationNode degreeNode = reloadedRadical.GetChild(0);
EquationNode firstChildOfDegree = degreeNode.GetChild(0);
Console.WriteLine("Degree node has child: " + (firstChildOfDegree != null));
}
}
}
```
### See Also
* class [RadicalEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
