---
title: TextRunEquationNode Class 
linktitle: TextRunEquationNode
second_title: Aspose.Cells for Go API Reference
description: 'TextRunEquationNode class. Encapsulates the object that represents textrunequationnode in Go.'
type: docs
weight: 200
url: /go/aspose.cells.drawing.equations/textrunequationnode/
---

## TextRunEquationNode class

This class in the equation node is used to store the actual content(a sequence of mathematical text) of the equation.Usually a node object per character.

```go

type TextRunEquationNode struct 

textrunequationnode, _ := asposecells.NewTextRunEquationNode()

```

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[GetText](./gettext/) | Set the content of the text node(Usually a node object per character). | 
|[SetText](./settext/) | Set the content of the text node(Usually a node object per character). | 
|[GetParentNode](./getparentnode/) | Specifies the parent node of the current node | 
|[SetParentNode](./setparentnode/) | Specifies the parent node of the current node | 
|[ToLaTeX](./tolatex/) | Conver this equtation to LaTeX expression. | 
|[ToMathML](./tomathml/) | Conver this equtation to MathML expression. | 
|[AddChild](./addchild/) | Insert a node of the specified type at the end of the child node list of the current node. | 
|[AddChild](./addchild/) | Inserts the specified node at the end of the current node's list of child nodes. | 
|[InsertChild](./insertchild/) | Inserts a node of the specified type at the specified index position in the current node's child node list. | 
|[InsertAfter](./insertafter/) | Inserts the specified node after the current node. | 
|[InsertBefore](./insertbefore/) | Inserts the specified node before the current node. | 
|[GetChild](./getchild/) | Returns the node at the specified index among the children of the current node. | 
|[Remove](./remove/) | Removes itself from the parent. | 
|[RemoveChild](./removechild/) | Removes the specified node from the current node's children. | 
|[RemoveChild](./removechild/) | Removes the node at the specified index from the current node's children. | 
|[RemoveAllChildren](./removeallchildren/) | Removes all the child nodes of the current node. | 
|[GetType](./gettype/) | Represents the type of the node. | 
|[GetEquationType](./getequationtype/) | Get the equation type of the current node | 
|[CreateNode](./createnode/) | Create a node of the specified type. | 
