---
title: Class SubSupEquationNode
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.Equations.SubSupEquationNode class. This class specifies an equation that can optionally be superscript or subscript. There are four main forms of this equation superscriptsubscriptsuperscript and subscript placed to the left of the base superscript and subscript placed to the right of the base
type: docs
url: /net/aspose.cells.drawing.equations/subsupequationnode/
---
## SubSupEquationNode class

This class specifies an equation that can optionally be superscript or subscript. There are four main forms of this equation, superscript，subscript，superscript and subscript placed to the left of the base, superscript and subscript placed to the right of the base.

```csharp
public class SubSupEquationNode : EquationNode
```

## Properties

| Name | Description |
| --- | --- |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | Get the equation type of the current node(Inherited from [`EquationNode`](../equationnode/).) |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Returns the font of this object.(Inherited from [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Gets the length of the characters.(Inherited from [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [ParentNode](../../aspose.cells.drawing.equations/equationnode/parentnode/) { get; set; } | Specifies the parent node of the current node(Inherited from [`EquationNode`](../equationnode/).) |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Gets the start index of the characters.(Inherited from [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Returns the text options.(Inherited from [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.equations/equationnode/type/) { get; } | Represents the type of the node.(Inherited from [`EquationNode`](../equationnode/).) |

## Methods

| Name | Description |
| --- | --- |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNode) | Inserts the specified node at the end of the current node's list of child nodes.(Inherited from [`EquationNode`](../equationnode/).) |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNodeType) | Insert a node of the specified type at the end of the child node list of the current node.(Inherited from [`EquationNode`](../equationnode/).) |
| override [Equals](../../aspose.cells.drawing.equations/subsupequationnode/equals/)(object) | Determine whether the current equation node is equal to the specified node |
| [GetChild](../../aspose.cells.drawing.equations/equationnode/getchild/)(int) | Returns the node at the specified index among the children of the current node.(Inherited from [`EquationNode`](../equationnode/).) |
| [InsertAfter](../../aspose.cells.drawing.equations/equationnode/insertafter/)(EquationNodeType) | Inserts the specified node after the current node.(Inherited from [`EquationNode`](../equationnode/).) |
| [InsertBefore](../../aspose.cells.drawing.equations/equationnode/insertbefore/)(EquationNodeType) | Inserts the specified node before the current node.(Inherited from [`EquationNode`](../equationnode/).) |
| [InsertChild](../../aspose.cells.drawing.equations/equationnode/insertchild/)(int, EquationNodeType) | Inserts a node of the specified type at the specified index position in the current node's child node list.(Inherited from [`EquationNode`](../equationnode/).) |
| [Remove](../../aspose.cells.drawing.equations/equationnode/remove/)() | Removes itself from the parent.(Inherited from [`EquationNode`](../equationnode/).) |
| [RemoveAllChildren](../../aspose.cells.drawing.equations/equationnode/removeallchildren/)() | Removes all the child nodes of the current node.(Inherited from [`EquationNode`](../equationnode/).) |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild/)(EquationNode) | Removes the specified node from the current node's children.(Inherited from [`EquationNode`](../equationnode/).) |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild/)(int) | Removes the node at the specified index from the current node's children.(Inherited from [`EquationNode`](../equationnode/).) |
| [SetWordArtStyle](../../aspose.cells/fontsetting/setwordartstyle/)(PresetWordArtStyle) | Sets the preset WordArt style.(Inherited from [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [ToLaTeX](../../aspose.cells.drawing.equations/equationnode/tolatex/)() | Convert this equtation to LaTeX expression.(Inherited from [`EquationNode`](../equationnode/).) |
| [ToMathML](../../aspose.cells.drawing.equations/equationnode/tomathml/)() | Convert this equtation to MathML expression.(Inherited from [`EquationNode`](../equationnode/).) |

### Examples

```csharp
// Called: SubSupEquationNode node2 = (SubSupEquationNode)mathNode2.GetChild(i);
[Test]
        public void Type_SubSupEquationNode()
        {
            Workbook workbook = new Workbook();
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            //test get mathnode
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            Assert.AreNotEqual(null, mathNode);

            string[] vals = new string[] { &quot;A&quot;, &quot;B&quot;, &quot;C&quot; };
            int[] vs = null;
            EquationNode node = null;
            for (int i = 0; i &lt; 4; i++)
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

            workbook.Save(Constants.destPath + &quot;SubSupEquationTest.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;SubSupEquationTest.xlsx&quot;);

            TextBox textBoxRead = (TextBox)workbook.Worksheets[0].Shapes[0];
            EquationNode mathNode2 = textBoxRead.GetEquationParagraph().GetChild(0);
            Assert.AreNotEqual(null, mathNode2);

            for (int i = 0; i &lt; 4; i++)
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

                for (int j = 0; j &lt; vs.Length; j++)
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

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


