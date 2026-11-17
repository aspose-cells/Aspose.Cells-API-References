---
title: "Clase MatrixEquationNode"
linktitle: "MatrixEquationNode"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Clase MatrixEquationNode. Encapsula el objeto que representa matrixequationnode en Go."
type: docs
weight: 200
url: /es/go-cpp/matrixequationnode/
---

## MatrixEquationNode class

This class specifies the Matrix equation, consisting of one or more elements laid out in one or more rows and one or more columns.

```go

type MatrixEquationNode struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |
| [NewMatrixEquationNode](./newmatrixequationnode/) | Constructs from a parent object. |

## Methods

| Method | Description |
| --- | --- |
| [IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
| [GetBaseJc](./getbasejc/) | Este atributo especifica la justificación de la matriz. El texto fuera de la matriz puede alinearse con la parte inferior, superior o central de una función de matriz. Por defecto, la matriz asume justificación centrada. |
| [SetBaseJc](./setbasejc/) | Este atributo especifica la justificación de la matriz. El texto fuera de la matriz puede alinearse con la parte inferior, superior o central de una función de matriz. Por defecto, la matriz asume justificación centrada. |
| [IsHidePlaceholder](./ishideplaceholder/) | Este atributo especifica la propiedad Hide Placeholders en una matriz. Cuando esta propiedad está activada, los marcadores de posición no aparecen en la matriz. Por defecto, los marcadores de posición sí aparecen, de modo que las ubicaciones donde se puede insertar texto son visibles. |
| [SetIsHidePlaceholder](./setishideplaceholder/) | Este atributo especifica la propiedad Hide Placeholders en una matriz. Cuando esta propiedad está activada, los marcadores de posición no aparecen en la matriz. Por defecto, los marcadores de posición sí aparecen, de modo que las ubicaciones donde se puede insertar texto son visibles. |
| [Equals](./equals/) | Determine whether the current equation node is equal to the specified node |
| [GetStartIndex](./getstartindex/) | Gets the start index of the characters. |
| [GetLength](./getlength/) | Gets the length of the characters. |
| [GetFont](./getfont/) | Returns the font of this object. |
| [SetWordArtStyle](./setwordartstyle/) | Sets the preset WordArt style. |
| [GetTextOptions](./gettextoptions/) | Returns the text options. |
| [GetType](./gettype/) | Gets the type of text node. |
| [GetParentNode](./getparentnode/) | Specifies the parent node of the current node |
| [SetParentNode](./setparentnode/) | Specifies the parent node of the current node |
| [ToLaTeX](./tolatex/) | Convert this equtation to LaTeX expression. |
| [ToMathML](./tomathml/) | Convert this equtation to MathML expression. |
| [AddChild_EquationNodeType](./addchild_equationnodetype/) | Insert a node of the specified type at the end of the child node list of the current node. |
| [InsertChild](./insertchild/) | Inserts a node of the specified type at the specified index position in the current node's child node list. |
| [InsertAfter](./insertafter/) | Inserts the specified node after the current node. |
| [InsertBefore](./insertbefore/) | Inserts the specified node before the current node. |
| [GetChild](./getchild/) | Returns the node at the specified index among the children of the current node. |
| [Remove](./remove/) | Removes itself from the parent. |
| [RemoveChild_EquationNode](./removechild_equationnode/) | Removes the specified node from the current node's children. |
| [RemoveAllChildren](./removeallchildren/) | Removes all the child nodes of the current node. |
| [GetEquationType](./getequationtype/) | Get the equation type of the current node |
| [MatrixEquationNode_CreateNode](./matrixequationnode_createnode/) | Create a node of the specified type. |
