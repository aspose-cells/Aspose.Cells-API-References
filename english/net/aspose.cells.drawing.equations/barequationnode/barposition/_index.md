---
title: BarEquationNode.BarPosition
second_title: Aspose.Cells for .NET API Reference
description: BarEquationNode property. This attribute specifies the position of the bar in the bar object
type: docs
url: /net/aspose.cells.drawing.equations/barequationnode/barposition/
---
## BarEquationNode.BarPosition property

This attribute specifies the position of the bar in the bar object

```csharp
public EquationCharacterPositionType BarPosition { get; set; }
```

### Examples

```csharp
// Called: node.BarPosition = EquationCharacterPositionType.Top;
[Test]
        public void Property_BarPosition()
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
            TR.Text = &quot;x&quot;;

            string resultFile = Constants.destPath + &quot;BarEquationTest.xlsx&quot;;
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
            Assert.AreEqual(&quot;x&quot;, TR.Text);
        }
```

### See Also

* enum [EquationCharacterPositionType](../../equationcharacterpositiontype/)
* class [BarEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


