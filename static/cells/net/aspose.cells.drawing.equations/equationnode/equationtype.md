##EquationNode.EquationType
EquationNode property. Get the equation type of the current node
## EquationNode.EquationType property
Get the equation type of the current node
```csharp
public EquationNodeType EquationType { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class EquationNodePropertyEquationTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Aspose.Cells.Drawing.TextBox textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);
// Create equation structure
Aspose.Cells.Drawing.Equations.EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
// Create subscript node
Aspose.Cells.Drawing.Equations.EquationNode subNode = mathNode.AddChild(Aspose.Cells.Drawing.Equations.EquationNodeType.Sub);
// Add base and subscript components
Aspose.Cells.Drawing.Equations.EquationNode baseNode = subNode.AddChild(Aspose.Cells.Drawing.Equations.EquationNodeType.Base);
Aspose.Cells.Drawing.Equations.TextRunEquationNode baseText = (Aspose.Cells.Drawing.Equations.TextRunEquationNode)(baseNode.AddChild(Aspose.Cells.Drawing.Equations.EquationNodeType.Text));
baseText.Text = "Base";
Aspose.Cells.Drawing.Equations.EquationNode subscriptNode = subNode.AddChild(Aspose.Cells.Drawing.Equations.EquationNodeType.Subscript);
Aspose.Cells.Drawing.Equations.TextRunEquationNode subText = (Aspose.Cells.Drawing.Equations.TextRunEquationNode)(subscriptNode.AddChild(Aspose.Cells.Drawing.Equations.EquationNodeType.Text));
subText.Text = "Sub";
// Verify EquationType property
Console.WriteLine("Main node type: " + mathNode.EquationType);
Console.WriteLine("Subscript node type: " + subNode.EquationType);
Console.WriteLine("Base component type: " + baseNode.EquationType);
Console.WriteLine("Subscript component type: " + subscriptNode.EquationType);
// Save and reload to verify persistence
workbook.Save("EquationTypeDemo.xlsx");
workbook = new Workbook("EquationTypeDemo.xlsx");
// Verify loaded equation types
Aspose.Cells.Drawing.TextBox loadedTextBox = (Aspose.Cells.Drawing.TextBox)workbook.Worksheets[0].Shapes[0];
Aspose.Cells.Drawing.Equations.EquationNode loadedMathNode = loadedTextBox.GetEquationParagraph().GetChild(0);
Aspose.Cells.Drawing.Equations.SubSupEquationNode loadedSubNode = (Aspose.Cells.Drawing.Equations.SubSupEquationNode)loadedMathNode.GetChild(0);
Console.WriteLine("\nAfter loading:");
Console.WriteLine("Subscript node type: " + loadedSubNode.EquationType);
Console.WriteLine("Base component type: " + loadedSubNode.GetChild(0).EquationType);
Console.WriteLine("Subscript component type: " + loadedSubNode.GetChild(1).EquationType);
}
}
}
```
### See Also
* enum [EquationNodeType](../../equationnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
