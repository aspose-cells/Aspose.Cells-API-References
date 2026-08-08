---
title: "DelimiterEquationNode"
linktitle: "DelimiterEquationNode"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "This class specifies the delimiter equation, consisting of opening and closing delimiters (such as parentheses, braces, brackets, and vertical bars), and a comp"
type: docs
weight: 1140
url: /nodejs/aspose.cells/delimiterequationnode/
---

## DelimiterEquationNode class

This class specifies the delimiter equation, consisting of opening and closing delimiters (such as parentheses, braces, brackets, and vertical bars), and a component contained inside. The delimiter may have more than one component, with a designated separator character between each component.

## Methods

| Name | Description |
| --- | --- |
| [addChild(equationType)](#addchild) | Insert a node of the specified type at the end of the child node list of the current node. |
| [addChild(node)](#addchild-1) | Inserts the specified node at the end of the current node's list of child nodes. |
| [equals(obj)](#equals) | Determine whether the current equation node is equal to the specified node |
| [getBeginChar()](#getbeginchar) | Delimiter beginning character. It should be noted that this property only accepts one character, and if multiple charact |
| [getChild(index)](#getchild) | Returns the node at the specified index among the children of the current node. |
| [getDelimiterShape()](#getdelimitershape) | Specifies the shape of delimiters in the delimiter object. The value of the property is EquationDelimiterShapeType integ |
| [getEndChar()](#getendchar) | Delimiter ending character. It should be noted that this property only accepts one character, and if multiple characters |
| [getEquationType()](#getequationtype) | Get the equation type of the current node The value of the property is EquationNodeType integer constant. |
| [getFont()](#getfont) | Returns the font of this object. |
| [getLength()](#getlength) | Gets the length of the characters. |
| [getNaryGrow()](#getnarygrow) | This property specifies the growth property of the delimiter at the document level. When off, the delimiter will not gro |
| [getParentNode()](#getparentnode) | Specifies the parent node of the current node |
| [getSeparatorChar()](#getseparatorchar) | Delimiter separator character. It should be noted that this property only accepts one character, and if multiple charact |
| [getStartIndex()](#getstartindex) | Gets the start index of the characters. |
| [getTextOptions()](#gettextoptions) | Returns the text options. |
| [getType()](#gettype) | Represents the type of the node. The value of the property is TextNodeType integer constant. |
| [insertAfter(equationType)](#insertafter) | Inserts the specified node after the current node. |
| [insertBefore(equationType)](#insertbefore) | Inserts the specified node before the current node. |
| [insertChild(index, equationType)](#insertchild) | Inserts a node of the specified type at the specified index position in the current node's child node list. |
| [remove()](#remove) | Removes itself from the parent. |
| [removeAllChildren()](#removeallchildren) | Removes all the child nodes of the current node. |
| [removeChild(node)](#removechild) | Removes the specified node from the current node's children. |
| [removeChild(index)](#removechild-1) | Removes the node at the specified index from the current node's children. |
| [setBeginChar()](#setbeginchar) | Delimiter beginning character. It should be noted that this property only accepts one character, and if multiple charact |
| [setDelimiterShape()](#setdelimitershape) | Specifies the shape of delimiters in the delimiter object. The value of the property is EquationDelimiterShapeType integ |
| [setEndChar()](#setendchar) | Delimiter ending character. It should be noted that this property only accepts one character, and if multiple characters |
| [setNaryGrow()](#setnarygrow) | This property specifies the growth property of the delimiter at the document level. When off, the delimiter will not gro |
| [setParentNode()](#setparentnode) | Specifies the parent node of the current node |
| [setSeparatorChar()](#setseparatorchar) | Delimiter separator character. It should be noted that this property only accepts one character, and if multiple charact |
| [setWordArtStyle(style)](#setwordartstyle) | Sets the preset WordArt style. Only for the text of shape/chart. |
| [toLaTeX()](#tolatex) |  |
| [toMathML()](#tomathml) |  |

### addChild(equationType) {#addchild}

Insert a node of the specified type at the end of the child node list of the current node.

| Parameter | Type | Description |
| --- | --- | --- |
| equationType | Number | EquationNodeType |

**Returns:** EquationNode — `EquationNode` If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.

### addChild(node) {#addchild-1}

Inserts the specified node at the end of the current node's list of child nodes.

| Parameter | Type | Description |
| --- | --- | --- |
| node | EquationNode | The specified node |

### equals(obj) {#equals}

Determine whether the current equation node is equal to the specified node

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | The specified node |

**Returns:** boolean — `boolean`

### getBeginChar() {#getbeginchar}

Delimiter beginning character. It should be noted that this property only accepts one character, and if multiple characters are passed in, only the first character is accepted.

### getChild(index) {#getchild}

Returns the node at the specified index among the children of the current node.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | Index of the node |

**Returns:** EquationNode — `EquationNode` Returns the corresponding node if the specified node exists, otherwise returns null.

### getDelimiterShape() {#getdelimitershape}

Specifies the shape of delimiters in the delimiter object. The value of the property is EquationDelimiterShapeType integer constant.

### getEndChar() {#getendchar}

Delimiter ending character. It should be noted that this property only accepts one character, and if multiple characters are passed in, only the first character is accepted.

### getEquationType() {#getequationtype}

Get the equation type of the current node The value of the property is EquationNodeType integer constant.

### getFont() {#getfont}

Returns the font of this object.

### getLength() {#getlength}

Gets the length of the characters.

### getNaryGrow() {#getnarygrow}

This property specifies the growth property of the delimiter at the document level. When off, the delimiter will not grow to match the size of its component height. When enabled, the delimiter grows vertically to match its component height.

### getParentNode() {#getparentnode}

Specifies the parent node of the current node

### getSeparatorChar() {#getseparatorchar}

Delimiter separator character. It should be noted that this property only accepts one character, and if multiple characters are passed in, only the first character is accepted.

### getStartIndex() {#getstartindex}

Gets the start index of the characters.

### getTextOptions() {#gettextoptions}

Returns the text options.

### getType() {#gettype}

Represents the type of the node. The value of the property is TextNodeType integer constant.

### insertAfter(equationType) {#insertafter}

Inserts the specified node after the current node.

| Parameter | Type | Description |
| --- | --- | --- |
| equationType | Number | EquationNodeType |

**Returns:** EquationNode — `EquationNode` If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.

### insertBefore(equationType) {#insertbefore}

Inserts the specified node before the current node.

| Parameter | Type | Description |
| --- | --- | --- |
| equationType | Number | EquationNodeType |

**Returns:** EquationNode — `EquationNode` If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.

### insertChild(index, equationType) {#insertchild}

Inserts a node of the specified type at the specified index position in the current node's child node list.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | index value |
| equationType | Number | EquationNodeType |

**Returns:** EquationNode — `EquationNode` If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.

### remove() {#remove}

Removes itself from the parent.

### removeAllChildren() {#removeallchildren}

Removes all the child nodes of the current node.

### removeChild(node) {#removechild}

Removes the specified node from the current node's children.

| Parameter | Type | Description |
| --- | --- | --- |
| node | EquationNode | Node to be deleted. |

### removeChild(index) {#removechild-1}

Removes the node at the specified index from the current node's children.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | Index of the node |

### setBeginChar() {#setbeginchar}

Delimiter beginning character. It should be noted that this property only accepts one character, and if multiple characters are passed in, only the first character is accepted.

### setDelimiterShape() {#setdelimitershape}

Specifies the shape of delimiters in the delimiter object. The value of the property is EquationDelimiterShapeType integer constant.

### setEndChar() {#setendchar}

Delimiter ending character. It should be noted that this property only accepts one character, and if multiple characters are passed in, only the first character is accepted.

### setNaryGrow() {#setnarygrow}

This property specifies the growth property of the delimiter at the document level. When off, the delimiter will not grow to match the size of its component height. When enabled, the delimiter grows vertically to match its component height.

### setParentNode() {#setparentnode}

Specifies the parent node of the current node

### setSeparatorChar() {#setseparatorchar}

Delimiter separator character. It should be noted that this property only accepts one character, and if multiple characters are passed in, only the first character is accepted.

### setWordArtStyle(style) {#setwordartstyle}

Sets the preset WordArt style. Only for the text of shape/chart.

| Parameter | Type | Description |
| --- | --- | --- |
| style | Number | PresetWordArtStyle |

### toLaTeX() {#tolatex}

### toMathML() {#tomathml}
