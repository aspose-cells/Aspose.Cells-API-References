---
title: Class NaryEquationNode
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.Equations.NaryEquationNode class. This class specifies an nary operator equation consisting of an nary operator a base or operand and optional upper and lower bounds
type: docs
url: /net/aspose.cells.drawing.equations/naryequationnode/
---
## NaryEquationNode class

This class specifies an n-ary operator equation consisting of an n-ary operator, a base (or operand), and optional upper and lower bounds.

```csharp
public class NaryEquationNode : EquationNode
```

## Properties

| Name | Description |
| --- | --- |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | Get the equation type of the current node(Inherited from [`EquationNode`](../equationnode/).) |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Returns the font of this object.(Inherited from [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [IsHideSubscript](../../aspose.cells.drawing.equations/naryequationnode/ishidesubscript/) { get; set; } | Whether to display the lower bound |
| [IsHideSuperscript](../../aspose.cells.drawing.equations/naryequationnode/ishidesuperscript/) { get; set; } | Whether to display the upper bound |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Gets the length of the characters.(Inherited from [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [LimitLocation](../../aspose.cells.drawing.equations/naryequationnode/limitlocation/) { get; set; } | This attribute specifies the location of limits in n-ary operators. Limits can be either centered above and below the n-ary operator, or positioned just to the right of the operator. |
| [NaryGrow](../../aspose.cells.drawing.equations/naryequationnode/narygrow/) { get; set; } | This attribute specifies the growth property of n-ary operators at the document level. When off, n-ary operators such as integrals and summations do not grow to match the size of their operand height. When on, the n-ary operator grows vertically to match its operand height. |
| [NaryOperator](../../aspose.cells.drawing.equations/naryequationnode/naryoperator/) { get; set; } | an n-ary operator.e.g "∑". It is strongly recommended to use attribute NaryOperatorType to set n-ary operator. Use this property setting if you cannot find the character you need in a known type. |
| [NaryOperatorType](../../aspose.cells.drawing.equations/naryequationnode/naryoperatortype/) { get; set; } | an n-ary operator.e.g "∑" |
| [ParentNode](../../aspose.cells.drawing.equations/equationnode/parentnode/) { get; set; } | Specifies the parent node of the current node(Inherited from [`EquationNode`](../equationnode/).) |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Gets the start index of the characters.(Inherited from [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Returns the text options.(Inherited from [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.equations/equationnode/type/) { get; } | Represents the type of the node.(Inherited from [`EquationNode`](../equationnode/).) |

## Methods

| Name | Description |
| --- | --- |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNode) | Inserts the specified node at the end of the current node's list of child nodes.(Inherited from [`EquationNode`](../equationnode/).) |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNodeType) | Insert a node of the specified type at the end of the child node list of the current node.(Inherited from [`EquationNode`](../equationnode/).) |
| override [Equals](../../aspose.cells.drawing.equations/naryequationnode/equals/)(object) | Determine whether the current equation node is equal to the specified node |
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
// Called: NaryEquationNode node2 = (NaryEquationNode)mathNode2.GetChild(i);
[Test]
        public void Type_NaryEquationNode()
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

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


