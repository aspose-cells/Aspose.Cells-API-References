---
title: TextRunEquationNode.Text
second_title: Aspose.Cells for .NET API Reference
description: TextRunEquationNode property. Set the content of the text nodeUsually a node object per character
type: docs
url: /net/aspose.cells.drawing.equations/textrunequationnode/text/
---
## TextRunEquationNode.Text property

Set the content of the text node(Usually a node object per character).

```csharp
public string Text { get; set; }
```

### Examples

```csharp
// Called: TR.Text = vals[0];
public void TextRunEquationNode_Property_Text()
{
    Workbook workbook = new Workbook();
    TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

    //test get mathnode
    EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
    Assert.AreNotEqual(null, mathNode);

    //meaning of content:sub, sup, e
    string[] vals = new string[] { "1", "5", "C" };
    bool[] vs = null;//Whether to insert related objects
    int eqCount = 3;
    NaryEquationNode node = null;
    for (int i = 0; i < eqCount; i++)
    {
        node = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);
        switch (i)
        {
            case 0:
                node.IsHideSubscript = true;//"Sub"objects are not written to the file
                node.IsHideSuperscript = true;//"Sup"objects are not written to the file
                vs = new bool[3] { false, false, true };
                break;
            case 1:
                node.NaryOperator = "\u222d";//"∭"
                node.IsHideSubscript = true;
                node.IsHideSuperscript = true;
                vs = new bool[3] { true, true, true };
                break;
            case 2:
                node.NaryOperator = "∑";
                node.NaryGrow = true;
                vs = new bool[3] { false, false, true };
                break;
        }

        TextRunEquationNode TR = null;
        EquationNode sub = node.AddChild(EquationNodeType.Subscript);
        if (vs[0])
        {
            TR = (TextRunEquationNode)(sub.AddChild(EquationNodeType.Text));
            TR.Text = vals[0];
        }

        EquationNode sup = node.AddChild(EquationNodeType.Superscript);
        if (vs[1])
        {
            TR = (TextRunEquationNode)(sup.AddChild(EquationNodeType.Text));
            TR.Text = vals[1];
        }

        EquationNode e = node.AddChild(EquationNodeType.Base);
        if (vs[2])
        {
            TR = (TextRunEquationNode)(e.AddChild(EquationNodeType.Text));
            TR.Text = vals[2];
        }
    }

    workbook.Save(Constants.destPath + "NaryEquationTest.xlsx");
    workbook = new Workbook(Constants.destPath + "NaryEquationTest.xlsx");

    TextBox textBoxRead = (TextBox)workbook.Worksheets[0].Shapes[0];
    EquationNode mathNode2 = textBoxRead.GetEquationParagraph().GetChild(0);
    Assert.AreNotEqual(null, mathNode2);

    for (int i = 0; i < eqCount; i++)
    {
        NaryEquationNode node2 = (NaryEquationNode)mathNode2.GetChild(i);
        Assert.AreNotEqual(null, node2);
        Assert.AreEqual(EquationNodeType.Nary, node2.EquationType);

        switch (i)
        {
            case 0:
                Assert.AreEqual("∫", node2.NaryOperator);
                Assert.AreEqual(true, node2.IsHideSubscript);
                Assert.AreEqual(true, node2.IsHideSuperscript);
                break;
            case 1:
                Assert.AreEqual("∭", node2.NaryOperator);
                Assert.AreEqual(true, node2.IsHideSubscript);
                Assert.AreEqual(true, node2.IsHideSuperscript);
                break;
            case 2:
                Assert.AreEqual("\u2211", node2.NaryOperator);
                Assert.AreEqual(true, node2.NaryGrow);
                Assert.AreEqual(false, node2.IsHideSubscript);
                Assert.AreEqual(false, node2.IsHideSuperscript);
                break;
        }

        for (int j = 0; j < 3; j++)
        {
            EquationComponentNode node3 = (EquationComponentNode)node2.GetChild(j);
            Assert.AreNotEqual(null, node3);

            TextRunEquationNode TR = (TextRunEquationNode)node3.GetChild(0);
            if (j > 1)
            {
                Assert.AreNotEqual(null, TR);
                Assert.AreEqual(vals[j], TR.Text);
            }
            else
            {
                Assert.AreEqual(null, TR);
            }
        }


    }
}
```

### See Also

* class [TextRunEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


