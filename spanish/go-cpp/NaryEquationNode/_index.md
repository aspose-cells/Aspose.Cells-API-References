---
title: "Clase NaryEquationNode"
linktitle: "NaryEquationNode"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Clase NaryEquationNode. Encapsula el objeto que representa naryequationnode en Go."
type: docs
weight: 200
url: /es/go-cpp/naryequationnode/
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
| [NewNaryEquationNode](./newnaryequationnode/) | Constructs from a parent object. |

## Methods

| Method | Description |
| --- | --- |
| [IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
| [IsHideSubscript](./ishidesubscript/) | Si se muestra el límite inferior |
| [SetIsHideSubscript](./setishidesubscript/) | Si se muestra el límite inferior |
| [IsHideSuperscript](./ishidesuperscript/) | Si se muestra el límite superior |
| [SetIsHideSuperscript](./setishidesuperscript/) | Si se muestra el límite superior |
| [GetLimitLocation](./getlimitlocation/) | Este atributo especifica la ubicación de los límites en operadores n-arios. Los límites pueden estar centrados arriba y abajo del operador n-ario, o posicionados justo a la derecha del operador. |
| [SetLimitLocation](./setlimitlocation/) | Este atributo especifica la ubicación de los límites en operadores n-arios. Los límites pueden estar centrados arriba y abajo del operador n-ario, o posicionados justo a la derecha del operador. |
| [GetNaryOperator](./getnaryoperator/) | un operador n-ario, p.ej. "∑". Se recomienda encarecidamente usar el atributo NaryOperatorType para establecer el operador n-ario. Use esta configuración de propiedad si no puede encontrar el carácter que necesita en un tipo conocido. |
| [SetNaryOperator](./setnaryoperator/) | un operador n-ario, p.ej. "∑". Se recomienda encarecidamente usar el atributo NaryOperatorType para establecer el operador n-ario. Use esta configuración de propiedad si no puede encontrar el carácter que necesita en un tipo conocido. |
| [GetNaryOperatorType](./getnaryoperatortype/) | un operador n-ario, p.ej. "∑" |
| [SetNaryOperatorType](./setnaryoperatortype/) | un operador n-ario, p.ej. "∑" |
| [GetNaryGrow](./getnarygrow/) | Este atributo especifica la propiedad de crecimiento de los operadores n-arios a nivel de documento. Cuando está desactivado, los operadores n-arios como integrales y sumas no crecen para coincidir con la altura de sus operandos. Cuando está activado, el operador n-ario crece verticalmente para coincidir con la altura de su operando. |
| [SetNaryGrow](./setnarygrow/) | Este atributo especifica la propiedad de crecimiento de los operadores n-arios a nivel de documento. Cuando está desactivado, los operadores n-arios como integrales y sumas no crecen para coincidir con la altura de sus operandos. Cuando está activado, el operador n-ario crece verticalmente para coincidir con la altura de su operando. |
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
| [NaryEquationNode_CreateNode](./naryequationnode_createnode/) | Create a node of the specified type. |
