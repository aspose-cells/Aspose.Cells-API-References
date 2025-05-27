---
title: TextBox.GetEquationParagraph
second_title: Aspose.Cells for .NET API Reference
description: TextBox method. Get the specified math paragraph from the TextBody property of the TextBox object. Notice 1 Returns NULL when the index is out of bounds or not found. 2 Also returns NULL if the specified index position is not a math paragraph
type: docs
url: /net/aspose.cells.drawing/textbox/getequationparagraph/
---
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

---

## GetEquationParagraph() {#getequationparagraph}

Gets the first math paragraph from the TextBody property of the TextBox object.

```csharp
public EquationNode GetEquationParagraph()
```

### Return Value

If there has math paragraph, returns the first one, otherwise returns null.

### Examples

```csharp
// Called: EquationNode mathNode2 = textBoxRead.GetEquationParagraph().GetChild(0);
public void TextBox_Method_GetEquationParagraph()
{
    Workbook workbook = new Workbook();
    TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

    //test get mathnode
    EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
    Assert.AreNotEqual(null, mathNode);

    BarEquationNode node = (BarEquationNode)mathNode.AddChild(EquationNodeType.Bar);
    node.BarPosition = EquationCharacterPositionType.Top;

    EquationNode subBase = node.AddChild(EquationNodeType.Base);
    TextRunEquationNode TR = (TextRunEquationNode)(subBase.AddChild(EquationNodeType.Text));
    TR.Text = "x";

    string resultFile = Constants.destPath + "BarEquationTest.xlsx";
    workbook.Save(resultFile);
    Workbook workbook2 = new Workbook(resultFile);

    TextBox textBoxRead = (TextBox)workbook2.Worksheets[0].Shapes[0];
    EquationNode mathNode2 = textBoxRead.GetEquationParagraph().GetChild(0);
    Assert.AreNotEqual(null, mathNode2);

    BarEquationNode node2 = (BarEquationNode)mathNode2.GetChild(0);
    Assert.AreNotEqual(null, node2);
    Assert.AreEqual(EquationNodeType.Bar, node2.EquationType);
    Assert.AreEqual(EquationCharacterPositionType.Top, node2.BarPosition);

    EquationNode node3 = node2.GetChild(0);
    Assert.AreNotEqual(null, node3);
    Assert.AreEqual(EquationNodeType.Base, node3.EquationType);

    TR = (TextRunEquationNode)node3.GetChild(0);
    Assert.AreNotEqual(null, TR);
    Assert.AreEqual(EquationNodeType.Text, TR.EquationType);
    Assert.AreEqual("x", TR.Text);
}
```

### See Also

* class [EquationNode](../../../aspose.cells.drawing.equations/equationnode/)
* class [TextBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


