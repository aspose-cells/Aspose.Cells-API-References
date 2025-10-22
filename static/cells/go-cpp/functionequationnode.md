##FunctionEquationNode Class
'FunctionEquationNode class. Encapsulates the object that represents functionequationnode in Go.'
## FunctionEquationNode class
This class specifies the Function-Apply equation, which consists of a function name and an argument acted upon.The types of the name and argument components are 'EquationNodeType.FunctionName' and 'EquationNodeType.Base' respectively.
```go
type FunctionEquationNode struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewFunctionEquationNode](./newfunctionequationnode/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
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
|[FunctionEquationNode_CreateNode](./functionequationnode_createnode/) | Create a node of the specified type. |
