---
title: BorderBoxEquationNode Class 
linktitle: BorderBoxEquationNode
second_title: Aspose.Cells for Go via C++ API Reference
description: 'BorderBoxEquationNode class. Encapsulates the object that represents borderboxequationnode in Go.'
type: docs
weight: 200
url: /go-cpp/borderboxequationnode/
---

## BorderBoxEquationNode class

This class specifies the Border Box function, consisting of a border drawn around an equation.

```go

type BorderBoxEquationNode struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |
|[NewBorderBoxEquationNode](./newborderboxequationnode/) | Constructs from a parent object. | 

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[Equals](./equals/) | Determine whether the current equation node is equal to the specified node | 
|[GetParentNode](./getparentnode/) | Specifies the parent node of the current node | 
|[SetParentNode](./setparentnode/) | Specifies the parent node of the current node | 
|[ToLaTeX](./tolatex/) | Convert this equtation to LaTeX expression. | 
|[ToMathML](./tomathml/) | Convert this equtation to MathML expression. | 
|[AddChild_EquationNodeType](./addchild_equationnodetype/) | Insert a node of the specified type at the end of the child node list of the current node. | 
|[AddChild_EquationNode](./addchild_equationnode/) | Inserts the specified node at the end of the current node's list of child nodes. | 
|[InsertChild](./insertchild/) | Inserts a node of the specified type at the specified index position in the current node's child node list. | 
|[InsertAfter](./insertafter/) | Inserts the specified node after the current node. | 
|[InsertBefore](./insertbefore/) | Inserts the specified node before the current node. | 
|[GetChild](./getchild/) | Returns the node at the specified index among the children of the current node. | 
|[Remove](./remove/) | Removes itself from the parent. | 
|[RemoveChild_EquationNode](./removechild_equationnode/) | Removes the specified node from the current node's children. | 
|[RemoveChild_Int](./removechild_int/) | Removes the node at the specified index from the current node's children. | 
|[RemoveAllChildren](./removeallchildren/) | Removes all the child nodes of the current node. | 
|[GetType](./gettype/) | Represents the type of the node. | 
|[GetEquationType](./getequationtype/) | Get the equation type of the current node | 
|[BorderBoxEquationNode_CreateNode](./borderboxequationnode_createnode/) | Create a node of the specified type. | 
