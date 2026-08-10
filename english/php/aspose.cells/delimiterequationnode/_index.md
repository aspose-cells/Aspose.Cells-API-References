---
title: "DelimiterEquationNode Class"
linktitle: "DelimiterEquationNode"
articleTitle: "DelimiterEquationNode"
second_title: "Aspose.Cells for PHP via Java"
description: "This class specifies the delimiter equation, consisting of opening and closing delimiters (such as parentheses, braces, brackets, and vertical bars), and a comp"
type: docs
weight: 1730
url: /php/aspose.cells/delimiterequationnode/
---

## DelimiterEquationNode class

This class specifies the delimiter equation, consisting of opening and closing delimiters (such as parentheses, braces, brackets, and vertical bars), and a component contained inside. The delimiter may have more than one component, with a designated separator character between each component.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [BeginChar](#beginchar) | String | Delimiter beginning character. It should be noted that this property only accepts one character, and if multiple charact |
| [EndChar](#endchar) | String | Delimiter ending character. It should be noted that this property only accepts one character, and if multiple characters |
| [NaryGrow](#narygrow) | boolean | This property specifies the growth property of the delimiter at the document level. When off, the delimiter will not gro |
| [SeparatorChar](#separatorchar) | String | Delimiter separator character. It should be noted that this property only accepts one character, and if multiple charact |
| [DelimiterShape](#delimitershape) | Number | Specifies the shape of delimiters in the delimiter object. The value of the property is EquationDelimiterShapeType integ |
| [ParentNode](#parentnode) | EquationNode | Specifies the parent node of the current node |
| [Type](#type) | Number | Represents the type of the node. The value of the property is TextNodeType integer constant. |
| [EquationType](#equationtype) | Number | Get the equation type of the current node The value of the property is EquationNodeType integer constant. |
| [StartIndex](#startindex) | Number | Gets the start index of the characters. |
| [Length](#length) | Number | Gets the length of the characters. |
| [Font](#font) | Font | Returns the font of this object. |
| [TextOptions](#textoptions) | TextOptions | Returns the text options. |

## Methods

| Name | Description |
| --- | --- |
| [equals](#equals) | Determine whether the current equation node is equal to the specified node |
| [toLaTeX](#tolatex) |  |
| [toMathML](#tomathml) |  |
| [addChild](#addchild) | Insert a node of the specified type at the end of the child node list of the current node. |
| [insertChild](#insertchild) | Inserts a node of the specified type at the specified index position in the current node's child node list. |
| [insertAfter](#insertafter) | Inserts the specified node after the current node. |
| [insertBefore](#insertbefore) | Inserts the specified node before the current node. |
| [getChild](#getchild) | Returns the node at the specified index among the children of the current node. |
| [remove](#remove) | Removes itself from the parent. |
| [removeChild](#removechild) | Removes the specified node from the current node's children. |
| [removeAllChildren](#removeallchildren) | Removes all the child nodes of the current node. |
| [setWordArtStyle](#setwordartstyle) | Sets the preset WordArt style.

Only for the text of shape/chart. |

### DelimiterEquationNode.BeginChar property {#beginchar}

Delimiter beginning character. It should be noted that this property only accepts one character, and if multiple characters are passed in, only the first character is accepted.

**Type:** String

### DelimiterEquationNode.EndChar property {#endchar}

Delimiter ending character. It should be noted that this property only accepts one character, and if multiple characters are passed in, only the first character is accepted.

**Type:** String

### DelimiterEquationNode.NaryGrow property {#narygrow}

This property specifies the growth property of the delimiter at the document level. When off, the delimiter will not grow to match the size of its component height. When enabled, the delimiter grows vertically to match its component height.

**Type:** boolean

### DelimiterEquationNode.SeparatorChar property {#separatorchar}

Delimiter separator character. It should be noted that this property only accepts one character, and if multiple characters are passed in, only the first character is accepted.

**Type:** String

### DelimiterEquationNode.DelimiterShape property {#delimitershape}

Specifies the shape of delimiters in the delimiter object. The value of the property is EquationDelimiterShapeType integer constant.

**Type:** Number

### DelimiterEquationNode.ParentNode property {#parentnode}

Specifies the parent node of the current node

**Type:** EquationNode

### DelimiterEquationNode.Type property {#type}

Represents the type of the node. The value of the property is TextNodeType integer constant.

**Type:** Number

### DelimiterEquationNode.EquationType property {#equationtype}

Get the equation type of the current node The value of the property is EquationNodeType integer constant.

**Type:** Number

### DelimiterEquationNode.StartIndex property {#startindex}

Gets the start index of the characters.

**Type:** Number

### DelimiterEquationNode.Length property {#length}

Gets the length of the characters.

**Type:** Number

### DelimiterEquationNode.Font property {#font}

Returns the font of this object.

**Type:** Font

### DelimiterEquationNode.TextOptions property {#textoptions}

Returns the text options.

**Type:** TextOptions

### equals(obj) {#equals}

Determine whether the current equation node is equal to the specified node

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | The specified node |

### toLaTeX() {#tolatex}

### toMathML() {#tomathml}

### addChild(equationType) (1 of 2) {#addchild}

Insert a node of the specified type at the end of the child node list of the current node.

| Parameter | Type | Description |
| --- | --- | --- |
| equationType | Number | A EquationNodeType value. Types of Equation Nodes |

**Returns:** If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.

---

### addChild(node) (2 of 2) {#addchild-1}

Inserts the specified node at the end of the current node's list of child nodes.

| Parameter | Type | Description |
| --- | --- | --- |
| node | EquationNode | The specified node |

### insertChild(index, equationType) {#insertchild}

Inserts a node of the specified type at the specified index position in the current node's child node list.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | index value |
| equationType | Number | A EquationNodeType value. Types of Equation Nodes |

**Returns:** If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.

### insertAfter(equationType) {#insertafter}

Inserts the specified node after the current node.

| Parameter | Type | Description |
| --- | --- | --- |
| equationType | Number | A EquationNodeType value. Types of Equation Nodes |

**Returns:** If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.

### insertBefore(equationType) {#insertbefore}

Inserts the specified node before the current node.

| Parameter | Type | Description |
| --- | --- | --- |
| equationType | Number | A EquationNodeType value. Types of Equation Nodes |

**Returns:** If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.

### getChild(index) {#getchild}

Returns the node at the specified index among the children of the current node.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | Index of the node |

**Returns:** Returns the corresponding node if the specified node exists, otherwise returns null.

### remove() {#remove}

Removes itself from the parent.

### removeChild(node) (1 of 2) {#removechild}

Removes the specified node from the current node's children.

| Parameter | Type | Description |
| --- | --- | --- |
| node | EquationNode | Node to be deleted. |

---

### removeChild(index) (2 of 2) {#removechild-1}

Removes the node at the specified index from the current node's children.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | Index of the node |

### removeAllChildren() {#removeallchildren}

Removes all the child nodes of the current node.

### setWordArtStyle(style) {#setwordartstyle}

Sets the preset WordArt style.

Only for the text of shape/chart.

| Parameter | Type | Description |
| --- | --- | --- |
| style | Number | A PresetWordArtStyle value. The preset WordArt style. |
