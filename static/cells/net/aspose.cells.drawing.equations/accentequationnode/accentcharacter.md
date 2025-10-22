##AccentEquationNode.AccentCharacter
AccentEquationNode property. This attribute specifies the type of combining diacritical mark attached to the base of the accent function. The default accent character is U0302. It is strongly recommended to use attribute AccentType to set accent character. Use this property setting if you cannot find the character you need in a known type
## AccentEquationNode.AccentCharacter property
This attribute specifies the type of combining diacritical mark attached to the base of the accent function. The default accent character is U+0302. It is strongly recommended to use attribute AccentType to set accent character. Use this property setting if you cannot find the character you need in a known type.
```csharp
public string AccentCharacter { get; set; }
```
### Remarks
It should be noted that this property only accepts one character, and if multiple characters are passed in, only the first character is accepted.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;
namespace AsposeCellsExamples
{
public class AccentEquationNodePropertyAccentCharacterDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add an equation shape to the first worksheet
TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);
// Get the equation node and add an accent node
EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
AccentEquationNode accentNode = (AccentEquationNode)mathNode.AddChild(EquationNodeType.Accent);
// Set the accent character (circumflex in this case)
accentNode.AccentCharacter = "\u0302";
// Add base text for the accent
EquationNode baseNode = accentNode.AddChild(EquationNodeType.Base);
TextRunEquationNode textNode = (TextRunEquationNode)(baseNode.AddChild(EquationNodeType.Text));
textNode.Text = "x";
// Save the workbook
workbook.Save("AccentEquationDemo.xlsx");
// Verify the saved file by loading it back
Workbook loadedWorkbook = new Workbook("AccentEquationDemo.xlsx");
TextBox loadedTextBox = (TextBox)loadedWorkbook.Worksheets[0].Shapes[0];
AccentEquationNode loadedAccentNode = (AccentEquationNode)loadedTextBox.GetEquationParagraph().GetChild(0).GetChild(0);
// Output the accent character to demonstrate the property
Console.WriteLine("Accent Character: " + loadedAccentNode.AccentCharacter);
}
}
}
```
### See Also
* class [AccentEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
