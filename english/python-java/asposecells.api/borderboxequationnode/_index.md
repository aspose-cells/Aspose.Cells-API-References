---
title: "BorderBoxEquationNode Class"
linktitle: "BorderBoxEquationNode"
articleTitle: "BorderBoxEquationNode"
second_title: "Aspose.Cells for Python via Java"
description: "This class specifies the Border Box function, consisting of a border drawn around an equation."
type: docs
weight: 360
url: /python-java/asposecells.api/borderboxequationnode/
---

## BorderBoxEquationNode class

This class specifies the Border Box function, consisting of a border drawn around an equation.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [ParentNode](#parentnode) | EquationNode | Specifies the parent node of the current node |
| [Type](#type) | int | Represents the type of the node. The value of the property is TextNodeType integer constant. |
| [EquationType](#equationtype) | int | Get the equation type of the current node The value of the property is EquationNodeType integer constant. |
| [StartIndex](#startindex) | int | Gets the start index of the characters. |
| [Length](#length) | int | Gets the length of the characters. |
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

### BorderBoxEquationNode.ParentNode property {#parentnode}

Specifies the parent node of the current node

**Type:** EquationNode

### BorderBoxEquationNode.Type property {#type}

Represents the type of the node. The value of the property is TextNodeType integer constant.

**Type:** int

### BorderBoxEquationNode.EquationType property {#equationtype}

Get the equation type of the current node The value of the property is EquationNodeType integer constant.

**Type:** int

### BorderBoxEquationNode.StartIndex property {#startindex}

Gets the start index of the characters.

**Type:** int

### BorderBoxEquationNode.Length property {#length}

Gets the length of the characters.

**Type:** int

### BorderBoxEquationNode.Font property {#font}

Returns the font of this object.

**Type:** Font

### BorderBoxEquationNode.TextOptions property {#textoptions}

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
| equationType | int | A EquationNodeType value. Types of Equation Nodes |

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
| index | int | index value |
| equationType | int | A EquationNodeType value. Types of Equation Nodes |

**Returns:** If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.

### insertAfter(equationType) {#insertafter}

Inserts the specified node after the current node.

| Parameter | Type | Description |
| --- | --- | --- |
| equationType | int | A EquationNodeType value. Types of Equation Nodes |

**Returns:** If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.

### insertBefore(equationType) {#insertbefore}

Inserts the specified node before the current node.

| Parameter | Type | Description |
| --- | --- | --- |
| equationType | int | A EquationNodeType value. Types of Equation Nodes |

**Returns:** If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.

### getChild(index) {#getchild}

Returns the node at the specified index among the children of the current node.

| Parameter | Type | Description |
| --- | --- | --- |
| index | int | Index of the node |

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
| index | int | Index of the node |

### removeAllChildren() {#removeallchildren}

Removes all the child nodes of the current node.

### setWordArtStyle(style) {#setwordartstyle}

Sets the preset WordArt style.

Only for the text of shape/chart.

| Parameter | Type | Description |
| --- | --- | --- |
| style | int | A PresetWordArtStyle value. The preset WordArt style. |
