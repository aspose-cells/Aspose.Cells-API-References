##AccentEquationNode.AccentCharacterType
AccentEquationNode property. Specify combining characters by type value
## AccentEquationNode.AccentCharacterType property
Specify combining characters by type value.
```csharp
public EquationCombiningCharacterType AccentCharacterType { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;
using System;
public class AccentEquationNodePropertyAccentCharacterTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);
//test get mathnode
EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
AccentEquationNode node = (AccentEquationNode)mathNode.AddChild(EquationNodeType.Accent);
node.AccentCharacter = "\u0302";
node.AccentCharacterType = EquationCombiningCharacterType.GraveAccent;
EquationNode subBase = node.AddChild(EquationNodeType.Base);
TextRunEquationNode TR = (TextRunEquationNode)(subBase.AddChild(EquationNodeType.Text));
TR.Text = "x";
Console.WriteLine(node.AccentCharacterType == EquationCombiningCharacterType.GraveAccent);
workbook.Save("AccentEquationNodePropertyAccentCharacterType.xlsx");
}
}
}
```
### See Also
* enum [EquationCombiningCharacterType](../../equationcombiningcharactertype/)
* class [AccentEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
