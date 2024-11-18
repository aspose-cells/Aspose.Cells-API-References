---
title: FractionEquationNode Class 
linktitle: FractionEquationNode
second_title: Aspose.Cells for Go API Reference
description: 'FractionEquationNode class. Encapsulates the object that represents fractionequationnode in Go.'
type: docs
weight: 200
url: /go/aspose.cells.drawing.equations/fractionequationnode/
---

## FractionEquationNode class

This class  specifies the fraction equation, consisting of a numerator and denominator separated by a fraction bar. The fraction bar can be horizontal or diagonal, depending on the fraction properties. The fraction equation is also used to represent the stack function, which places one element above another, with no fraction bar.

```go

type FractionEquationNode struct 

fractionequationnode, _ := asposecells.NewFractionEquationNode()

```

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[GetFractionType](./getfractiontype/) | This specifies the type of fraction ; the default is 'Bar'. | 
|[SetFractionType](./setfractiontype/) | This specifies the type of fraction ; the default is 'Bar'. | 
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
