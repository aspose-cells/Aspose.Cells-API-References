---
title: EquationNode.GetChild
second_title: Aspose.Cells for .NET API Reference
description: EquationNode method. Returns the node at the specified index among the children of the current node
type: docs
url: /net/aspose.cells.drawing.equations/equationnode/getchild/
---
## EquationNode.GetChild method

Returns the node at the specified index among the children of the current node.

```csharp
public EquationNode GetChild(int index)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | Index of the node |

### Return Value

Returns the corresponding node if the specified node exists, otherwise returns null.

### Examples

```csharp
// Called: TextRunEquationNode TR = (TextRunEquationNode)node3.GetChild(0);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook();
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            //test get mathnode
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            Assert.AreNotEqual(null, mathNode);

            string[] vals = new string[] { "A", "B", "C" };
            int[] vs = null;
            EquationNode node = null;
            for (int i = 0; i < 4; i++)
            {
                switch (i)
                {
                    case 0:
                        node = mathNode.AddChild(EquationNodeType.Sub);
                        vs = new int[2] { 0, 1 };
                        break;
                    case 1:
                        node = mathNode.AddChild(EquationNodeType.Sup);
                        vs = new int[2] { 0, 2 };
                        break;
                    case 2:
                        node = mathNode.AddChild(EquationNodeType.SubSup);
                        vs = new int[3] { 0, 1, 2 };
                        break;
                    case 3:
                        node = mathNode.AddChild(EquationNodeType.PreSubSup);
                        vs = new int[3] { 1, 2, 0 };
                        break;
                }

                foreach (var v in vs)
                {
                    switch (v)
                    {
                        case 0:
                            EquationNode e = node.AddChild(EquationNodeType.Base);
                            TextRunEquationNode TR = (TextRunEquationNode)(e.AddChild(EquationNodeType.Text));
                            TR.Text = vals[v];
                            break;
                        case 1:
                            EquationNode sub = node.AddChild(EquationNodeType.Subscript);
                            TR = (TextRunEquationNode)(sub.AddChild(EquationNodeType.Text));
                            TR.Text = vals[v];
                            break;
                        case 2:
                            EquationNode sup = node.AddChild(EquationNodeType.Superscript);
                            TR = (TextRunEquationNode)(sup.AddChild(EquationNodeType.Text));
                            TR.Text = vals[v];
                            break;
                    }
                }
            }

            workbook.Save(Constants.destPath + "SubSupEquationTest.xlsx");
            workbook = new Workbook(Constants.destPath + "SubSupEquationTest.xlsx");

            TextBox textBoxRead = (TextBox)workbook.Worksheets[0].Shapes[0];
            EquationNode mathNode2 = textBoxRead.GetEquationParagraph().GetChild(0);
            Assert.AreNotEqual(null, mathNode2);

            for (int i = 0; i < 4; i++)
            {
                SubSupEquationNode node2 = (SubSupEquationNode)mathNode2.GetChild(i);
                Assert.AreNotEqual(null, node2);
                switch (i)
                {
                    case 0:
                        Assert.AreEqual(EquationNodeType.Sub, node2.EquationType);
                        vs = new int[2] { 0, 1 };
                        break;
                    case 1:
                        Assert.AreEqual(EquationNodeType.Sup, node2.EquationType);
                        vs = new int[2] { 0, 2 };
                        break;
                    case 2:
                        Assert.AreEqual(EquationNodeType.SubSup, node2.EquationType);
                        vs = new int[3] { 0, 1, 2 };
                        break;
                    case 3:
                        Assert.AreEqual(EquationNodeType.PreSubSup, node2.EquationType);
                        vs = new int[3] { 1, 2, 0 };
                        break;
                }

                for (int j = 0; j < vs.Length; j++)
                {
                    EquationComponentNode node3 = (EquationComponentNode)node2.GetChild(j);
                    Assert.AreNotEqual(null, node3);
                    int index = vs[j];
                    switch (index)
                    {
                        case 0:
                            Assert.AreEqual(EquationNodeType.Base, node3.EquationType);
                            break;
                        case 1:
                            Assert.AreEqual(EquationNodeType.Subscript, node3.EquationType);
                            break;
                        case 2:
                            Assert.AreEqual(EquationNodeType.Superscript, node3.EquationType);
                            break;
                    }
                    TextRunEquationNode TR = (TextRunEquationNode)node3.GetChild(0);
                    Assert.AreNotEqual(null, TR);
                    Assert.AreEqual(vals[index], TR.Text);
                }
            }
        }
```

### See Also

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


