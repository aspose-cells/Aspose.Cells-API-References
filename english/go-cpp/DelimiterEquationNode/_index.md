---
title: DelimiterEquationNode Class 
linktitle: DelimiterEquationNode
second_title: Aspose.Cells for Go via C++ API Reference
description: 'DelimiterEquationNode class. Encapsulates the object that represents delimiterequationnode in Go.'
type: docs
weight: 200
url: /go-cpp/delimiterequationnode/
---

## DelimiterEquationNode class

This class specifies the delimiter equation, consisting of opening and closing delimiters (such as parentheses, braces, brackets, and vertical bars), and a component contained inside.The delimiter may have more than one component, with a designated separator character between each component.

```go

type DelimiterEquationNode struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |
|[NewDelimiterEquationNode](./newdelimiterequationnode/) | Constructs from a parent object. | 

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[GetBeginChar](./getbeginchar/) | Delimiter beginning character. | 
|[SetBeginChar](./setbeginchar/) | Delimiter beginning character. | 
|[GetEndChar](./getendchar/) | Delimiter ending character. | 
|[SetEndChar](./setendchar/) | Delimiter ending character. | 
|[GetNaryGrow](./getnarygrow/) | Specifies whether the delimiter should automatically expand and contract with the height of the formula. | 
|[SetNaryGrow](./setnarygrow/) | Specifies whether the delimiter should automatically expand and contract with the height of the formula. | 
|[GetSeparatorChar](./getseparatorchar/) | Delimiter separator character. | 
|[SetSeparatorChar](./setseparatorchar/) | Delimiter separator character. | 
|[GetDelimiterShape](./getdelimitershape/) | Specifies the shape of delimiters in the delimiter object. | 
|[SetDelimiterShape](./setdelimitershape/) | Specifies the shape of delimiters in the delimiter object. | 
|[Equals](./equals/) | Determine whether the current equation node is equal to the specified node | 
|[GetStartIndex](./getstartindex/) | Gets the start index of the characters. | 
|[GetLength](./getlength/) | Gets the length of the characters. | 
|[GetFont](./getfont/) | Returns the font of this object. | 
|[SetWordArtStyle](./setwordartstyle/) | Sets the preset WordArt style. | 
|[GetTextOptions](./gettextoptions/) | Returns the text options. | 
|[GetType](./gettype/) | Gets the type of text node. | 
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
|[GetEquationType](./getequationtype/) | Get the equation type of the current node | 
|[DelimiterEquationNode_CreateNode](./delimiterequationnode_createnode/) | Create a node of the specified type. | 
