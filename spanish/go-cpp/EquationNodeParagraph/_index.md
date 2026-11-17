---
title: "EquationNodeParagraph Clase"
linktitle: "EquationNodeParagraph"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Clase EquationNodeParagraph. Encapsula el objeto que representa equationnodeparagraph en Go."
type: docs
weight: 200
url: /es/go-cpp/equationnodeparagraph/
---

## EquationNodeParagraph class

This class specifies a mathematical paragraph containing one or more MathEquationNode(OMath) elements.

```go

type EquationNodeParagraph struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |
| [NewEquationNodeParagraph](./newequationnodeparagraph/) | Constructs from a parent object. |

## Methods

| Method | Description |
| --- | --- |
| [IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
| [GetJustification](./getjustification/) | Esto especifica la justificación del párrafo matemático (una serie de ecuaciones adyacentes dentro del mismo párrafo). Un párrafo matemático puede estar Alineado a la Izquierda, Alineado a la Derecha, Centrado, o Centrado como Grupo. Por defecto, el párrafo matemático está Centrado como Grupo. Esto significa que las ecuaciones pueden alinearse entre sí, pero todo el grupo de ecuaciones se centra como un todo. |
| [SetJustification](./setjustification/) | Esto especifica la justificación del párrafo matemático (una serie de ecuaciones adyacentes dentro del mismo párrafo). Un párrafo matemático puede estar Alineado a la Izquierda, Alineado a la Derecha, Centrado, o Centrado como Grupo. Por defecto, el párrafo matemático está Centrado como Grupo. Esto significa que las ecuaciones pueden alinearse entre sí, pero todo el grupo de ecuaciones se centra como un todo. |
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
| [EquationNodeParagraph_CreateNode](./equationnodeparagraph_createnode/) | Create a node of the specified type. |
