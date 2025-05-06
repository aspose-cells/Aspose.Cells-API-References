---
title: NaryEquationNode.NaryGrow
second_title: Aspose.Cells for .NET API Reference
description: NaryEquationNode property. This attribute specifies the growth property of nary operators at the document level. When off nary operators such as integrals and summations do not grow to match the size of their operand height. When on the nary operator grows vertically to match its operand height
type: docs
url: /net/aspose.cells.drawing.equations/naryequationnode/narygrow/
---
## NaryEquationNode.NaryGrow property

This attribute specifies the growth property of n-ary operators at the document level. When off, n-ary operators such as integrals and summations do not grow to match the size of their operand height. When on, the n-ary operator grows vertically to match its operand height.

```csharp
public bool NaryGrow { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(true, node2.NaryGrow);
[Test]
        public void Property_NaryGrow()
        {
            Workbook workbook = new Workbook();
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            //test get mathnode
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            Assert.AreNotEqual(null, mathNode);

            //meaning of content:sub, sup, e
            string[] vals = new string[] { &quot;1&quot;, &quot;5&quot;, &quot;C&quot; };
            bool[] vs = null;//Whether to insert related objects
            int eqCount = 3;
            NaryEquationNode node = null;
            for (int i = 0; i &lt; eqCount; i++)
            {
                node = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);
                switch (i)
                {
                    case 0:
                        node.IsHideSubscript = true;//&quot;Sub&quot;objects are not written to the file
                        node.IsHideSuperscript = true;//&quot;Sup&quot;objects are not written to the file
                        vs = new bool[3] { false, false, true };
                        break;
                    case 1:
                        node.NaryOperator = &quot;\u222d&quot;;//&quot;∭&quot;
                        node.IsHideSubscript = true;
                        node.IsHideSuperscript = true;
                        vs = new bool[3] { true, true, true };
                        break;
                    case 2:
                        node.NaryOperator = &quot;∑&quot;;
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

            workbook.Save(Constants.destPath + &quot;NaryEquationTest.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;NaryEquationTest.xlsx&quot;);

            TextBox textBoxRead = (TextBox)workbook.Worksheets[0].Shapes[0];
            EquationNode mathNode2 = textBoxRead.GetEquationParagraph().GetChild(0);
            Assert.AreNotEqual(null, mathNode2);

            for (int i = 0; i &lt; eqCount; i++)
            {
                NaryEquationNode node2 = (NaryEquationNode)mathNode2.GetChild(i);
                Assert.AreNotEqual(null, node2);
                Assert.AreEqual(EquationNodeType.Nary, node2.EquationType);

                switch (i)
                {
                    case 0:
                        Assert.AreEqual(&quot;∫&quot;, node2.NaryOperator);
                        Assert.AreEqual(true, node2.IsHideSubscript);
                        Assert.AreEqual(true, node2.IsHideSuperscript);
                        break;
                    case 1:
                        Assert.AreEqual(&quot;∭&quot;, node2.NaryOperator);
                        Assert.AreEqual(true, node2.IsHideSubscript);
                        Assert.AreEqual(true, node2.IsHideSuperscript);
                        break;
                    case 2:
                        Assert.AreEqual(&quot;\u2211&quot;, node2.NaryOperator);
                        Assert.AreEqual(true, node2.NaryGrow);
                        Assert.AreEqual(false, node2.IsHideSubscript);
                        Assert.AreEqual(false, node2.IsHideSuperscript);
                        break;
                }

                for (int j = 0; j &lt; 3; j++)
                {
                    EquationComponentNode node3 = (EquationComponentNode)node2.GetChild(j);
                    Assert.AreNotEqual(null, node3);

                    TextRunEquationNode TR = (TextRunEquationNode)node3.GetChild(0);
                    if (j &gt; 1)
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

* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


