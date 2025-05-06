---
title: Class EquationNode
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.Equations.EquationNode class. Abstract class for deriving other equation nodes
type: docs
url: /net/aspose.cells.drawing.equations/equationnode/
---
## EquationNode class

Abstract class for deriving other equation nodes.

```csharp
public abstract class EquationNode : FontSetting
```

## Properties

| Name | Description |
| --- | --- |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | Get the equation type of the current node |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Returns the font of this object.(Inherited from [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Gets the length of the characters.(Inherited from [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [ParentNode](../../aspose.cells.drawing.equations/equationnode/parentnode/) { get; set; } | Specifies the parent node of the current node |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Gets the start index of the characters.(Inherited from [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Returns the text options.(Inherited from [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.equations/equationnode/type/) { get; } | Represents the type of the node. |

## Methods

| Name | Description |
| --- | --- |
| static [CreateNode](../../aspose.cells.drawing.equations/equationnode/createnode/)(EquationNodeType, Workbook, EquationNode) | Create a node of the specified type. |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/#addchild_1)(EquationNode) | Inserts the specified node at the end of the current node's list of child nodes. |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/#addchild)(EquationNodeType) | Insert a node of the specified type at the end of the child node list of the current node. |
| override [Equals](../../aspose.cells.drawing.equations/equationnode/equals/)(object) | Determine whether the current equation node is equal to the specified node |
| [GetChild](../../aspose.cells.drawing.equations/equationnode/getchild/)(int) | Returns the node at the specified index among the children of the current node. |
| [InsertAfter](../../aspose.cells.drawing.equations/equationnode/insertafter/)(EquationNodeType) | Inserts the specified node after the current node. |
| [InsertBefore](../../aspose.cells.drawing.equations/equationnode/insertbefore/)(EquationNodeType) | Inserts the specified node before the current node. |
| [InsertChild](../../aspose.cells.drawing.equations/equationnode/insertchild/)(int, EquationNodeType) | Inserts a node of the specified type at the specified index position in the current node's child node list. |
| [Remove](../../aspose.cells.drawing.equations/equationnode/remove/)() | Removes itself from the parent. |
| [RemoveAllChildren](../../aspose.cells.drawing.equations/equationnode/removeallchildren/)() | Removes all the child nodes of the current node. |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild/#removechild)(EquationNode) | Removes the specified node from the current node's children. |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild/#removechild_1)(int) | Removes the node at the specified index from the current node's children. |
| [SetWordArtStyle](../../aspose.cells/fontsetting/setwordartstyle/)(PresetWordArtStyle) | Sets the preset WordArt style.(Inherited from [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [ToLaTeX](../../aspose.cells.drawing.equations/equationnode/tolatex/)() | Convert this equtation to LaTeX expression. |
| [ToMathML](../../aspose.cells.drawing.equations/equationnode/tomathml/)() | Convert this equtation to MathML expression. |

### Examples

```csharp
// Called: EquationNode node = textBox.GetEquationParagraph();
[Test]
        public void Type_EquationNode()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet56177.xlsx&quot;);
            TextBox textBox = workbook.Worksheets[0].TextBoxes[0];
            EquationNode node = textBox.GetEquationParagraph();
            Assert.IsTrue(node!= null);
        }
```

### See Also

* class [FontSetting](../../aspose.cells/fontsetting/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


