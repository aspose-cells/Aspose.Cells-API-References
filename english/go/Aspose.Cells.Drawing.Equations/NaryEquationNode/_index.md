---
title: NaryEquationNode Class 
linktitle: NaryEquationNode
second_title: Aspose.Cells for Go API Reference
description: 'NaryEquationNode class. Encapsulates the object that represents naryequationnode in Go.'
type: docs
weight: 200
url: /go/aspose.cells.drawing.equations/naryequationnode/
---

## NaryEquationNode class

This class specifies an n-ary operator equation consisting of an n-ary operator, a base (or operand), and optional upper and lower bounds.

```go

type NaryEquationNode struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |
|[NewNaryEquationNode](./newnaryequationnode/) | Constructs from a parent object. | 

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[IsHideSubscript](./ishidesubscript/) | Whether to display the lower bound | 
|[SetIsHideSubscript](./setishidesubscript/) | Whether to display the lower bound | 
|[IsHideSuperscript](./ishidesuperscript/) | Whether to display the upper bound | 
|[SetIsHideSuperscript](./setishidesuperscript/) | Whether to display the upper bound | 
|[GetLimitLocation](./getlimitlocation/) | This attribute specifies the location of limits in n-ary operators. Limits can be either centered above and below the n-ary operator, or positioned just to the right of the operator. | 
|[SetLimitLocation](./setlimitlocation/) | This attribute specifies the location of limits in n-ary operators. Limits can be either centered above and below the n-ary operator, or positioned just to the right of the operator. | 
|[GetNaryOperator](./getnaryoperator/) | an n-ary operator.e.g "∑".It is strongly recommended to use attribute NaryOperatorType to set n-ary operator.Use this property setting if you cannot find the character you need in a known type. | 
|[SetNaryOperator](./setnaryoperator/) | an n-ary operator.e.g "∑".It is strongly recommended to use attribute NaryOperatorType to set n-ary operator.Use this property setting if you cannot find the character you need in a known type. | 
|[GetNaryOperatorType](./getnaryoperatortype/) | an n-ary operator.e.g "∑" | 
|[SetNaryOperatorType](./setnaryoperatortype/) | an n-ary operator.e.g "∑" | 
|[GetNaryGrow](./getnarygrow/) | This attribute specifies the growth property of n-ary operators at the document level. When off, n-ary operators such as integrals and summations do not grow to match the size of their operand height. When on, the n-ary operator grows vertically to match its operand height. | 
|[SetNaryGrow](./setnarygrow/) | This attribute specifies the growth property of n-ary operators at the document level. When off, n-ary operators such as integrals and summations do not grow to match the size of their operand height. When on, the n-ary operator grows vertically to match its operand height. | 
|[Equals](./equals/) | Determine whether the current equation node is equal to the specified node | 
|[GetParentNode](./getparentnode/) | Specifies the parent node of the current node | 
|[SetParentNode](./setparentnode/) | Specifies the parent node of the current node | 
|[ToLaTeX](./tolatex/) | Convert this equtation to LaTeX expression. | 
|[ToMathML](./tomathml/) | Convert this equtation to MathML expression. | 
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
