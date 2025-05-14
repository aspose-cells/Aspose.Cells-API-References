---
title: Class DelimiterEquationNode
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.Equations.DelimiterEquationNode class. This class specifies the delimiter equation consisting of opening and closing delimiters such as parentheses braces brackets and vertical bars and a component contained inside. The delimiter may have more than one component with a designated separator character between each component
type: docs
url: /net/aspose.cells.drawing.equations/delimiterequationnode/
---
## DelimiterEquationNode class

This class specifies the delimiter equation, consisting of opening and closing delimiters (such as parentheses, braces, brackets, and vertical bars), and a component contained inside. The delimiter may have more than one component, with a designated separator character between each component.

```csharp
public class DelimiterEquationNode : EquationNode
```

## Properties

| Name | Description |
| --- | --- |
| [BeginChar](../../aspose.cells.drawing.equations/delimiterequationnode/beginchar/) { get; set; } | Delimiter beginning character. |
| [DelimiterShape](../../aspose.cells.drawing.equations/delimiterequationnode/delimitershape/) { get; set; } | Specifies the shape of delimiters in the delimiter object. |
| [EndChar](../../aspose.cells.drawing.equations/delimiterequationnode/endchar/) { get; set; } | Delimiter ending character. |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | Get the equation type of the current node(Inherited from [`EquationNode`](../equationnode/).) |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Returns the font of this object.(Inherited from [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Gets the length of the characters.(Inherited from [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [NaryGrow](../../aspose.cells.drawing.equations/delimiterequationnode/narygrow/) { get; set; } |  |
| [ParentNode](../../aspose.cells.drawing.equations/equationnode/parentnode/) { get; set; } | Specifies the parent node of the current node(Inherited from [`EquationNode`](../equationnode/).) |
| [SeparatorChar](../../aspose.cells.drawing.equations/delimiterequationnode/separatorchar/) { get; set; } | Delimiter separator character. |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Gets the start index of the characters.(Inherited from [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Returns the text options.(Inherited from [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.equations/equationnode/type/) { get; } | Represents the type of the node.(Inherited from [`EquationNode`](../equationnode/).) |

## Methods

| Name | Description |
| --- | --- |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNode) | Inserts the specified node at the end of the current node's list of child nodes.(Inherited from [`EquationNode`](../equationnode/).) |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNodeType) | Insert a node of the specified type at the end of the child node list of the current node.(Inherited from [`EquationNode`](../equationnode/).) |
| override [Equals](../../aspose.cells.drawing.equations/delimiterequationnode/equals/)(object) | Determine whether the current equation node is equal to the specified node |
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
// Called: node2 = (DelimiterEquationNode)mathNode2.GetChild(1);
public void Equations_Type_DelimiterEquationNode()
{
    Workbook workbook = new Workbook();
    TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

    //test get mathnode
    EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
    Assert.AreNotEqual(null, mathNode);

    //add 1
    DelimiterEquationNode node = (DelimiterEquationNode)mathNode.AddChild(EquationNodeType.Delimiter);

    //add 2
    node = (DelimiterEquationNode)mathNode.AddChild(EquationNodeType.Delimiter);
    node.DelimiterShape = EquationDelimiterShapeType.Match;
    node.NaryGrow = false;
    node.SeparatorChar = "!";
    node.BeginChar = "#";
    node.EndChar = "*";

    EquationNode e = node.AddChild(EquationNodeType.Base);

    FractionEquationNode Fra = (FractionEquationNode)e.AddChild(EquationNodeType.Fraction);

    EquationComponentNode numerator = (EquationComponentNode)Fra.AddChild(EquationNodeType.Numerator);
    TextRunEquationNode TR = (TextRunEquationNode)(numerator.AddChild(EquationNodeType.Text));
    TR.Text = "A";

    EquationComponentNode denominator = (EquationComponentNode)Fra.AddChild(EquationNodeType.Denominator);
    TR = (TextRunEquationNode)(denominator.AddChild(EquationNodeType.Text));
    TR.Text = "B";

    EquationNode e2 = node.AddChild(EquationNodeType.Base);
    TextRunEquationNode tr2 = (TextRunEquationNode)e2.AddChild(EquationNodeType.Text);
    tr2.Text = "a";

    string resultFile = Constants.destPath + "BracketEquationTest.xlsx";
    workbook.Save(resultFile);
    Workbook workbook2 = new Workbook(resultFile);

    TextBox textBoxRead = (TextBox)workbook2.Worksheets[0].Shapes[0];
    EquationNode mathNode2 = textBoxRead.GetEquationParagraph().GetChild(0);
    Assert.AreNotEqual(null, mathNode2);

    //test 1
    DelimiterEquationNode node2 = (DelimiterEquationNode)mathNode2.GetChild(0);
    Assert.AreNotEqual(null, node2);
    Assert.AreEqual(EquationNodeType.Delimiter, node2.EquationType);

    Assert.AreEqual("(", node2.BeginChar);
    Assert.AreEqual(")", node2.EndChar);
    Assert.AreEqual(false, node2.NaryGrow);
    Assert.AreEqual("|", node2.SeparatorChar);
    Assert.AreEqual(EquationDelimiterShapeType.Centered, node2.DelimiterShape);

    //test 2
    node2 = (DelimiterEquationNode)mathNode2.GetChild(1);
    Assert.AreNotEqual(null, node2);
    Assert.AreEqual(EquationNodeType.Delimiter, node2.EquationType);

    Assert.AreEqual("#", node2.BeginChar);
    Assert.AreEqual("*", node2.EndChar);
    Assert.AreEqual(false, node2.NaryGrow);
    Assert.AreEqual("!", node2.SeparatorChar);
    Assert.AreEqual(EquationDelimiterShapeType.Match, node2.DelimiterShape);

}
```

### See Also

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


