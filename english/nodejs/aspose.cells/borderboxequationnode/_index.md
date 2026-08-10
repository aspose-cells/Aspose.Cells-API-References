---
title: "BorderBoxEquationNode"
linktitle: "BorderBoxEquationNode"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "This class specifies the Border Box function, consisting of a border drawn around an equation."
type: docs
weight: 240
url: /nodejs/aspose.cells/borderboxequationnode/
---

## BorderBoxEquationNode class

This class specifies the Border Box function, consisting of a border drawn around an equation.

## Methods

| Name | Description |
| --- | --- |
| [addChild(equationType)](#addchild) | Insert a node of the specified type at the end of the child node list of the current node. |
| [addChild(node)](#addchild-1) | Inserts the specified node at the end of the current node's list of child nodes. |
| [equals(obj)](#equals) | Determine whether the current equation node is equal to the specified node |
| [getChild(index)](#getchild) | Returns the node at the specified index among the children of the current node. |
| [getEquationType()](#getequationtype) | Get the equation type of the current node The value of the property is EquationNodeType integer constant. |
| [getFont()](#getfont) | Returns the font of this object. |
| [getLength()](#getlength) | Gets the length of the characters. |
| [getParentNode()](#getparentnode) | Specifies the parent node of the current node |
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
| [setParentNode()](#setparentnode) | Specifies the parent node of the current node |
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

### getChild(index) {#getchild}

Returns the node at the specified index among the children of the current node.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | Index of the node |

**Returns:** EquationNode — `EquationNode` Returns the corresponding node if the specified node exists, otherwise returns null.

### getEquationType() {#getequationtype}

Get the equation type of the current node The value of the property is EquationNodeType integer constant.

### getFont() {#getfont}

Returns the font of this object.

### getLength() {#getlength}

Gets the length of the characters.

### getParentNode() {#getparentnode}

Specifies the parent node of the current node

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

### setParentNode() {#setparentnode}

Specifies the parent node of the current node

### setWordArtStyle(style) {#setwordartstyle}

Sets the preset WordArt style. Only for the text of shape/chart.

| Parameter | Type | Description |
| --- | --- | --- |
| style | Number | PresetWordArtStyle |

### toLaTeX() {#tolatex}

### toMathML() {#tomathml}
