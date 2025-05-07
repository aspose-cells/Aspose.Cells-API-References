---
title: GroupCharacterEquationNode.ChrType
second_title: Aspose.Cells for .NET API Reference
description: GroupCharacterEquationNode property. Specify combining characters by type value
type: docs
url: /net/aspose.cells.drawing.equations/groupcharacterequationnode/chrtype/
---
## GroupCharacterEquationNode.ChrType property

Specify combining characters by type value.

```csharp
public EquationCombiningCharacterType ChrType { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(EquationCombiningCharacterType.RightwardsDoubleArrow, node2.ChrType);
[Test]
        public void Property_ChrType()
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
            TR.Text = "abc";

            string resultFile = Constants.destPath + "GroupCharacterEquationTest.xlsx";
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
            Assert.AreEqual("⇒", node2.GroupChr);

            EquationNode node3 = node2.GetChild(0);
            Assert.AreNotEqual(null, node3);
            Assert.AreEqual(EquationNodeType.Base, node3.EquationType);

            TR = (TextRunEquationNode)node3.GetChild(0);
            Assert.AreNotEqual(null, TR);
            Assert.AreEqual(EquationNodeType.Text, TR.EquationType);
            Assert.AreEqual("abc", TR.Text);
        }
```

### See Also

* enum [EquationCombiningCharacterType](../../equationcombiningcharactertype/)
* class [GroupCharacterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


