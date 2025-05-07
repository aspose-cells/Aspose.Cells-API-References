---
title: AccentEquationNode.AccentCharacter
second_title: Aspose.Cells for .NET API Reference
description: AccentEquationNode property. This attribute specifies the type of combining diacritical mark attached to the base of the accent function. The default accent character is U0302. It is strongly recommended to use attribute AccentType to set accent character. Use this property setting if you cannot find the character you need in a known type
type: docs
url: /net/aspose.cells.drawing.equations/accentequationnode/accentcharacter/
---
## AccentEquationNode.AccentCharacter property

This attribute specifies the type of combining diacritical mark attached to the base of the accent function. The default accent character is U+0302. It is strongly recommended to use attribute AccentType to set accent character. Use this property setting if you cannot find the character you need in a known type.

```csharp
public string AccentCharacter { get; set; }
```

### Remarks

It should be noted that this property only accepts one character, and if multiple characters are passed in, only the first character is accepted.

### Examples

```csharp
// Called: Assert.AreEqual("\u0302", node2.AccentCharacter);
[Test]
        public void Property_AccentCharacter()
        {
            Workbook workbook = new Workbook();
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            //test get mathnode
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            Assert.AreNotEqual(null, mathNode);

            AccentEquationNode node = (AccentEquationNode)mathNode.AddChild(EquationNodeType.Accent);
            node.AccentCharacter = "\u0302";

            EquationNode subBase = node.AddChild(EquationNodeType.Base);
            TextRunEquationNode TR = (TextRunEquationNode)(subBase.AddChild(EquationNodeType.Text));
            TR.Text = "x";

            string resultFile = Constants.destPath + "AccentEquationTest.xlsx";
            workbook.Save(resultFile);
            Workbook workbook2 = new Workbook(resultFile);

            TextBox textBoxRead = (TextBox)workbook2.Worksheets[0].Shapes[0];
            EquationNode mathNode2 = textBoxRead.GetEquationParagraph().GetChild(0);
            Assert.AreNotEqual(null, mathNode2);

            AccentEquationNode node2 = (AccentEquationNode)mathNode2.GetChild(0);
            Assert.AreNotEqual(null, node2);
            Assert.AreEqual(EquationNodeType.Accent, node2.EquationType);
            Assert.AreEqual("\u0302", node2.AccentCharacter);

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

* class [AccentEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


