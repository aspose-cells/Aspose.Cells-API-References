##Enum EquationCharacterPositionType
Aspose.Cells.Drawing.Equations.EquationCharacterPositionType enum. Specifies the position of a particular subobject within its parent
## EquationCharacterPositionType enumeration
Specifies the position of a particular subobject within its parent
```csharp
public enum EquationCharacterPositionType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Top | `0` | At the top of the parent object |
| Bottom | `1` | At the bottom of the parent object |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;
namespace AsposeCellsExamples
{
public class EquationsClassEquationCharacterPositionTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add equation shape
TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);
// Get equation node and add bar with top position
EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
BarEquationNode barNode = (BarEquationNode)mathNode.AddChild(EquationNodeType.Bar);
barNode.BarPosition = EquationCharacterPositionType.Top;
// Add base text
EquationNode baseNode = barNode.AddChild(EquationNodeType.Base);
TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
textNode.Text = "x";
// Save and verify
string outputFile = "EquationCharacterPositionTypeDemo.xlsx";
workbook.Save(outputFile);
// Reload and verify
Workbook loadedWorkbook = new Workbook(outputFile);
TextBox loadedTextBox = (TextBox)loadedWorkbook.Worksheets[0].Shapes[0];
BarEquationNode loadedBarNode = (BarEquationNode)loadedTextBox.GetEquationParagraph().GetChild(0).GetChild(0);
Console.WriteLine("Bar Position: " + loadedBarNode.BarPosition);
Console.WriteLine("Text Content: " + ((TextRunEquationNode)loadedBarNode.GetChild(0).GetChild(0)).Text);
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)
