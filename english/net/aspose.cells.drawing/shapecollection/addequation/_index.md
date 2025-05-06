---
title: ShapeCollection.AddEquation
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Add an equation object to the worksheet
type: docs
url: /net/aspose.cells.drawing/shapecollection/addequation/
---
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
// Called: TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook();
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            //test get mathnode
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            Assert.AreNotEqual(null, mathNode);

            GroupCharacterEquationNode node = (GroupCharacterEquationNode)mathNode.AddChild(EquationNodeType.GroupChr);
            node.Position = EquationCharacterPositionType.Top;
            node.ChrType = EquationCombiningCharacterType.RightwardsDoubleArrow;

            EquationNode subBase = node.AddChild(EquationNodeType.Base);
            TextRunEquationNode TR = (TextRunEquationNode)(subBase.AddChild(EquationNodeType.Text));
            TR.Text = &quot;abc&quot;;

            string resultFile = Constants.destPath + &quot;GroupCharacterEquationTest.xlsx&quot;;
            workbook.Save(resultFile);
            Workbook workbook2 = new Workbook(resultFile);
            TextBox textBoxRead = (TextBox)workbook2.Worksheets[0].Shapes[0];
            EquationNode mathNode2 = textBoxRead.GetEquationParagraph().GetChild(0);
            Assert.AreNotEqual(null, mathNode2);

            GroupCharacterEquationNode node2 = (GroupCharacterEquationNode)mathNode2.GetChild(0);
            Assert.AreNotEqual(null, node2);
            Assert.AreEqual(EquationNodeType.GroupChr, node2.EquationType);
            Assert.AreEqual(EquationCharacterPositionType.Top, node2.Position);
            Assert.AreEqual(EquationCombiningCharacterType.RightwardsDoubleArrow, node2.ChrType);
            Assert.AreEqual(&quot;⇒&quot;, node2.GroupChr);

            EquationNode node3 = node2.GetChild(0);
            Assert.AreNotEqual(null, node3);
            Assert.AreEqual(EquationNodeType.Base, node3.EquationType);

            TR = (TextRunEquationNode)node3.GetChild(0);
            Assert.AreNotEqual(null, TR);
            Assert.AreEqual(EquationNodeType.Text, TR.EquationType);
            Assert.AreEqual(&quot;abc&quot;, TR.Text);
        }
```

### See Also

* class [TextBox](../../textbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


