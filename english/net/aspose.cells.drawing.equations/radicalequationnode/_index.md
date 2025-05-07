---
title: Class RadicalEquationNode
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.Equations.RadicalEquationNode class. This class specifies the radical equation consisting of an optional degree degEquationNodeType.Degree and a base
type: docs
url: /net/aspose.cells.drawing.equations/radicalequationnode/
---
## RadicalEquationNode class

This class specifies the radical equation, consisting of an optional degree deg(EquationNodeType.Degree) and a base.

```csharp
public class RadicalEquationNode : EquationNode
```

## Properties

| Name | Description |
| --- | --- |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | Get the equation type of the current node(Inherited from [`EquationNode`](../equationnode/).) |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Returns the font of this object.(Inherited from [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [IsDegHide](../../aspose.cells.drawing.equations/radicalequationnode/isdeghide/) { get; set; } | Whether to hide the degree of radicals. |
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
| override [Equals](../../aspose.cells.drawing.equations/radicalequationnode/equals/)(object) | Determine whether the current equation node is equal to the specified node |
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
// Called: RadicalEquationNode node2 = (RadicalEquationNode)mathNode2.GetChild(0);
[Test]
        public void Type_RadicalEquationNode()
        {
            Workbook workbook = new Workbook();
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            //test get mathnode
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            Assert.AreNotEqual(null, mathNode);

            RadicalEquationNode node = (RadicalEquationNode)mathNode.AddChild(EquationNodeType.Radical);
            node.IsDegHide = true;
            //IsDegHide = true,deg invalid,do not write to file
            EquationNode deg = node.AddChild(EquationNodeType.Degree);
            TextRunEquationNode tr = (TextRunEquationNode)deg.AddChild(EquationNodeType.Text);
            tr.Text = "5";

            EquationNode e = node.AddChild(EquationNodeType.Base);
            TextRunEquationNode tr2 = (TextRunEquationNode)e.AddChild(EquationNodeType.Text);
            tr2.Text = "a";

            workbook.Save(Constants.destPath + "RadicalEquationTest.xlsx");
            workbook = new Workbook(Constants.destPath + "RadicalEquationTest.xlsx");

            TextBox textBoxRead = (TextBox)workbook.Worksheets[0].Shapes[0];
            EquationNode mathNode2 = textBoxRead.GetEquationParagraph().GetChild(0);
            Assert.AreNotEqual(null, mathNode2);

            RadicalEquationNode node2 = (RadicalEquationNode)mathNode2.GetChild(0);
            Assert.AreNotEqual(null, node2);
            Assert.AreEqual(true, node2.IsDegHide);

            EquationComponentNode deg2 = (EquationComponentNode)node2.GetChild(0);
            Assert.AreNotEqual(null, deg2);
            Assert.AreEqual(EquationNodeType.Degree, deg2.EquationType);

            EquationComponentNode e2 = (EquationComponentNode)node2.GetChild(1);
            Assert.AreNotEqual(null, e2);
            Assert.AreEqual(EquationNodeType.Base, e2.EquationType);

            TextRunEquationNode TR1 = (TextRunEquationNode)deg2.GetChild(0);
            Assert.AreEqual(null, TR1);

            TextRunEquationNode TR2 = (TextRunEquationNode)e2.GetChild(0);
            Assert.AreNotEqual(null, TR2);
            Assert.AreEqual("a", TR2.Text);
        }
```

### See Also

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


