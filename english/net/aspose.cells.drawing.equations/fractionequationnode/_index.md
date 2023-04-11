---
title: FractionEquationNode
second_title: Aspose.Cells for .NET API Reference
description: This class specifies the fraction equation consisting of a numerator and denominator separated by a fraction bar. The fraction bar can be horizontal or diagonal depending on the fraction properties. The fraction equation is also used to represent the stack function which places one element above another with no fraction bar.
type: docs
url: /net/aspose.cells.drawing.equations/fractionequationnode/
---
## FractionEquationNode class

This class specifies the fraction equation, consisting of a numerator and denominator separated by a fraction bar. The fraction bar can be horizontal or diagonal, depending on the fraction properties. The fraction equation is also used to represent the stack function, which places one element above another, with no fraction bar.

```csharp
public class FractionEquationNode : EquationNode
```

## Properties

| Name | Description |
| --- | --- |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype) { get; } | Get the equation type of the current node(Inherited from [`EquationNode`](../equationnode).) |
| [Font](../../aspose.cells/fontsetting/font) { get; } | Returns the font of this object.(Inherited from [`FontSetting`](../../aspose.cells/fontsetting).) |
| [FractionType](../../aspose.cells.drawing.equations/fractionequationnode/fractiontype) { get; set; } | This specifies the type of fraction ; the default is 'Bar'. |
| [Length](../../aspose.cells/fontsetting/length) { get; } | Gets the length of the characters.(Inherited from [`FontSetting`](../../aspose.cells/fontsetting).) |
| [ParentNode](../../aspose.cells.drawing.equations/equationnode/parentnode) { get; set; } | Specifies the parent node of the current node(Inherited from [`EquationNode`](../equationnode).) |
| [StartIndex](../../aspose.cells/fontsetting/startindex) { get; } | Gets the start index of the characters.(Inherited from [`FontSetting`](../../aspose.cells/fontsetting).) |
| [TextOptions](../../aspose.cells/fontsetting/textoptions) { get; } | Returns the text options.(Inherited from [`FontSetting`](../../aspose.cells/fontsetting).) |
| override [Type](../../aspose.cells.drawing.equations/equationnode/type) { get; } | Represents the type of the node.(Inherited from [`EquationNode`](../equationnode).) |

## Methods

| Name | Description |
| --- | --- |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild)(EquationNode) | Inserts the specified node at the end of the current node's list of child nodes.(Inherited from [`EquationNode`](../equationnode).) |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild)(EquationNodeType) | Insert a node of the specified type at the end of the child node list of the current node.(Inherited from [`EquationNode`](../equationnode).) |
| override [Equals](../../aspose.cells.drawing.equations/fractionequationnode/equals)(object) | Determine whether the current equation node is equal to the specified node |
| [GetChild](../../aspose.cells.drawing.equations/equationnode/getchild)(int) | Returns the node at the specified index among the children of the current node.(Inherited from [`EquationNode`](../equationnode).) |
| [InsertAfter](../../aspose.cells.drawing.equations/equationnode/insertafter)(EquationNodeType) | Inserts the specified node after the current node.(Inherited from [`EquationNode`](../equationnode).) |
| [InsertBefore](../../aspose.cells.drawing.equations/equationnode/insertbefore)(EquationNodeType) | Inserts the specified node before the current node.(Inherited from [`EquationNode`](../equationnode).) |
| [InsertChild](../../aspose.cells.drawing.equations/equationnode/insertchild)(int, EquationNodeType) | Inserts a node of the specified type at the specified index position in the current node's child node list.(Inherited from [`EquationNode`](../equationnode).) |
| [Remove](../../aspose.cells.drawing.equations/equationnode/remove)() | Removes itself from the parent.(Inherited from [`EquationNode`](../equationnode).) |
| [RemoveAllChildren](../../aspose.cells.drawing.equations/equationnode/removeallchildren)() | Removes all the child nodes of the current node.(Inherited from [`EquationNode`](../equationnode).) |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild)(EquationNode) | Removes the specified node from the current node's children.(Inherited from [`EquationNode`](../equationnode).) |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild)(int) | Removes the node at the specified index from the current node's children.(Inherited from [`EquationNode`](../equationnode).) |
| [SetWordArtStyle](../../aspose.cells/fontsetting/setwordartstyle)(PresetWordArtStyle) | Sets the preset WordArt style.(Inherited from [`FontSetting`](../../aspose.cells/fontsetting).) |

### See Also

* class [EquationNode](../equationnode)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations)
* assembly [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
