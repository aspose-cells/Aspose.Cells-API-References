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
[Test]
        public void Method_GetEquationParagraph()
        {
            Workbook workbook = new Workbook();
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            //test get mathnode
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            Assert.AreNotEqual(null, mathNode);

            BoxEquationNode node = (BoxEquationNode)mathNode.AddChild(EquationNodeType.Box);
            //node.BarPosition = BarPositionType.Top;

            EquationNode subBase = node.AddChild(EquationNodeType.Base);
            TextRunEquationNode TR = (TextRunEquationNode)(subBase.AddChild(EquationNodeType.Text));
            TR.Text = &quot;==&quot;;

            string resultFile = Constants.destPath + &quot;BoxEquationTest.xlsx&quot;;
            workbook.Save(resultFile);
            Workbook workbook2 = new Workbook(resultFile);

            TextBox textBoxRead = (TextBox)workbook2.Worksheets[0].Shapes[0];
            EquationNode mathNode2 = textBoxRead.GetEquationParagraph().GetChild(0);
            Assert.AreNotEqual(null, mathNode2);

            BoxEquationNode node2 = (BoxEquationNode)mathNode2.GetChild(0);
            Assert.AreNotEqual(null, node2);
            Assert.AreEqual(EquationNodeType.Box, node2.EquationType);

            EquationNode node3 = node2.GetChild(0);
            Assert.AreNotEqual(null, node3);
            Assert.AreEqual(EquationNodeType.Base, node3.EquationType);

            TR = (TextRunEquationNode)node3.GetChild(0);
            Assert.AreNotEqual(null, TR);
            Assert.AreEqual(EquationNodeType.Text, TR.EquationType);
            Assert.AreEqual(&quot;==&quot;, TR.Text);

        }
```

### See Also

* class [EquationNode](../../../aspose.cells.drawing.equations/equationnode/)
* class [TextBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


