##TextBox.GetEquationParagraph
TextBox method. Get the specified math paragraph from the TextBody property of the TextBox object. Notice 1 Returns NULL when the index is out of bounds or not found. 2 Also returns NULL if the specified index position is not a math paragraph
## GetEquationParagraph(int) {#getequationparagraph_1}
Get the specified math paragraph from the TextBody property of the TextBox object. Notice: (1) Returns NULL when the index is out of bounds or not found. (2) Also returns NULL if the specified index position is not a math paragraph.
```csharp
public EquationNode GetEquationParagraph(int index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The position index of the math paragraph, starting from 0. |
### Return Value
Returns the math paragraph specified by index.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;
using System;
public class TextBoxMethodGetEquationParagraphWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a textbox to the worksheet
TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);
// Add some equation content to the textbox
textBox.Text = "\\sqrt{x^2 + y^2}";
try
{
// Call GetEquationParagraph with index parameter (Int32)
EquationNode equationNode = textBox.GetEquationParagraph(0);
if (equationNode != null)
{
Console.WriteLine("Equation paragraph retrieved successfully.");
Console.WriteLine($"Equation type: {equationNode.EquationType}");
Console.WriteLine($"LaTeX representation: {equationNode.ToLaTeX()}");
}
else
{
Console.WriteLine("No equation paragraph found at the specified index.");
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetEquationParagraph method: {ex.Message}");
}
// Save the workbook
workbook.Save("TextBoxMethodGetEquationParagraphWithInt32Demo.xlsx");
}
}
}
```
### See Also
* class [EquationNode](../../../aspose.cells.drawing.equations/equationnode/)
* class [TextBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
## GetEquationParagraph() {#getequationparagraph}
Gets the first math paragraph from the TextBody property of the TextBox object.
```csharp
public EquationNode GetEquationParagraph()
```
### Return Value
If there has math paragraph, returns the first one, otherwise returns null.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;
namespace AsposeCellsExamples
{
public class TextBoxMethodGetEquationParagraphDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
int textBoxIndex = worksheet.TextBoxes.Add(5, 5, 200, 200);
TextBox textBox = worksheet.TextBoxes[textBoxIndex];
textBox.Text = "$$\\sqrt{x^2+y^2}$$";
EquationNode equationNode = textBox.GetEquationParagraph();
if (equationNode != null)
{
Console.WriteLine("Equation LaTeX: " + equationNode.ToLaTeX());
Console.WriteLine("Equation MathML: " + equationNode.ToMathML());
}
else
{
Console.WriteLine("No equation paragraph found");
}
}
}
}
```
### See Also
* class [EquationNode](../../../aspose.cells.drawing.equations/equationnode/)
* class [TextBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
