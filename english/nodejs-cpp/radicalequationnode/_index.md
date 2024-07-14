---
title: RadicalEquationNode
second_title: Aspose.Cells for Node.js via C++ API Reference
description: This class specifies the radical equation consisting of an optional degree degEquationNodeType.Degree and a base.
type: docs
url: /nodejs-cpp/radicalequationnode/
---

## RadicalEquationNode class

This class specifies the radical equation, consisting of an optional degree deg(EquationNodeType.Degree) and a base.

```javascript
class RadicalEquationNode extends EquationNode;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(EquationNode)](#constructor-equationnode-)| Constructs from a parent object convertible to this. |

## Methods

| Method | Description |
| --- | --- |
| [isDegHide()](#isDegHide--)| Whether to hide the degree of radicals. |
| [setIsDegHide(boolean)](#setIsDegHide-boolean-)| Whether to hide the degree of radicals. |
| [getStartIndex()](#getStartIndex--)| Gets the start index of the characters. |
| [getLength()](#getLength--)| Gets the length of the characters. |
| [getFont()](#getFont--)| Returns the font of this object. |
| [getTextOptions()](#getTextOptions--)| Returns the text options. |
| [setWordArtStyle(PresetWordArtStyle)](#setWordArtStyle-presetwordartstyle-)| Sets the preset WordArt style. |
| [getParentNode()](#getParentNode--)| Specifies the parent node of the current node |
| [setParentNode(EquationNode)](#setParentNode-equationnode-)| Specifies the parent node of the current node |
| [getType()](#getType--)| Represents the type of the node. |
| [getEquationType()](#getEquationType--)| Get the equation type of the current node |
| [addChild(EquationNodeType)](#addChild-equationnodetype-)| Insert a node of the specified type at the end of the child node list of the current node. |
| [addChild(EquationNode)](#addChild-equationnode-)| Inserts the specified node at the end of the current node's list of child nodes. |
| [insertChild(number, EquationNodeType)](#insertChild-number-equationnodetype-)| Inserts a node of the specified type at the specified index position in the current node's child node list. |
| [insertAfter(EquationNodeType)](#insertAfter-equationnodetype-)| Inserts the specified node after the current node. |
| [insertBefore(EquationNodeType)](#insertBefore-equationnodetype-)| Inserts the specified node before the current node. |
| [getChild(number)](#getChild-number-)| Returns the node at the specified index among the children of the current node. |
| [remove()](#remove--)| Removes itself from the parent. |
| [removeChild(EquationNode)](#removeChild-equationnode-)| Removes the specified node from the current node's children. |
| [removeChild(number)](#removeChild-number-)| Removes the node at the specified index from the current node's children. |
| [removeAllChildren()](#removeAllChildren--)| Removes all the child nodes of the current node. |
| static [createNode(EquationNodeType, Workbook, EquationNode)](#createNode-equationnodetype-workbook-equationnode-)| Create a node of the specified type. |


### constructor(EquationNode) {#constructor-equationnode-}

Constructs from a parent object convertible to this.

```javascript
constructor(obj: EquationNode);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | EquationNode | The parent object. |

### isDegHide() {#isDegHide--}

Whether to hide the degree of radicals.

```javascript
isDegHide() : boolean;
```


### setIsDegHide(boolean) {#setIsDegHide-boolean-}

Whether to hide the degree of radicals.

```javascript
setIsDegHide(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getStartIndex() {#getStartIndex--}

Gets the start index of the characters.

```javascript
getStartIndex() : number;
```


### getLength() {#getLength--}

Gets the length of the characters.

```javascript
getLength() : number;
```


### getFont() {#getFont--}

Returns the font of this object.

```javascript
getFont() : Font;
```


**Returns**

[Font](./font/)

### getTextOptions() {#getTextOptions--}

Returns the text options.

```javascript
getTextOptions() : TextOptions;
```


**Returns**

[TextOptions](./textoptions/)

### setWordArtStyle(PresetWordArtStyle) {#setWordArtStyle-presetwordartstyle-}

Sets the preset WordArt style.

```javascript
setWordArtStyle(style: PresetWordArtStyle) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [PresetWordArtStyle](./presetwordartstyle/) | The preset WordArt style. |

**Remarks**

Only for the text of shape/chart.

### getParentNode() {#getParentNode--}

Specifies the parent node of the current node

```javascript
getParentNode() : EquationNode;
```


**Returns**

[EquationNode](./equationnode/)

### setParentNode(EquationNode) {#setParentNode-equationnode-}

Specifies the parent node of the current node

```javascript
setParentNode(value: EquationNode) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [EquationNode](./equationnode/) | The value to set. |

### getType() {#getType--}

Represents the type of the node.

```javascript
getType() : TextNodeType;
```


**Returns**

[TextNodeType](./textnodetype/)

### getEquationType() {#getEquationType--}

Get the equation type of the current node

```javascript
getEquationType() : EquationNodeType;
```


**Returns**

[EquationNodeType](./equationnodetype/)

### addChild(EquationNodeType) {#addChild-equationnodetype-}

Insert a node of the specified type at the end of the child node list of the current node.

```javascript
addChild(equationType: EquationNodeType) : EquationNode;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| equationType | [EquationNodeType](./equationnodetype/) | Types of Equation Nodes |

**Returns**

If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.

### addChild(EquationNode) {#addChild-equationnode-}

Inserts the specified node at the end of the current node's list of child nodes.

```javascript
addChild(node: EquationNode) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| node | [EquationNode](./equationnode/) | The specified node |

### insertChild(number, EquationNodeType) {#insertChild-number-equationnodetype-}

Inserts a node of the specified type at the specified index position in the current node's child node list.

```javascript
insertChild(index: number, equationType: EquationNodeType) : EquationNode;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | index value |
| equationType | [EquationNodeType](./equationnodetype/) | Types of Equation Nodes |

**Returns**

If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.

### insertAfter(EquationNodeType) {#insertAfter-equationnodetype-}

Inserts the specified node after the current node.

```javascript
insertAfter(equationType: EquationNodeType) : EquationNode;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| equationType | [EquationNodeType](./equationnodetype/) | Types of Equation Nodes |

**Returns**

If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.

### insertBefore(EquationNodeType) {#insertBefore-equationnodetype-}

Inserts the specified node before the current node.

```javascript
insertBefore(equationType: EquationNodeType) : EquationNode;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| equationType | [EquationNodeType](./equationnodetype/) | Types of Equation Nodes |

**Returns**

If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.

### getChild(number) {#getChild-number-}

Returns the node at the specified index among the children of the current node.

```javascript
getChild(index: number) : EquationNode;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | Index of the node |

**Returns**

Returns the corresponding node if the specified node exists, otherwise returns null.

### remove() {#remove--}

Removes itself from the parent.

```javascript
remove() : void;
```


### removeChild(EquationNode) {#removeChild-equationnode-}

Removes the specified node from the current node's children.

```javascript
removeChild(node: EquationNode) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| node | [EquationNode](./equationnode/) | Node to be deleted. |

### removeChild(number) {#removeChild-number-}

Removes the node at the specified index from the current node's children.

```javascript
removeChild(index: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | Index of the node |

### removeAllChildren() {#removeAllChildren--}

Removes all the child nodes of the current node.

```javascript
removeAllChildren() : void;
```


### createNode(EquationNodeType, Workbook, EquationNode) {#createNode-equationnodetype-workbook-equationnode-}

Create a node of the specified type.

```javascript
static createNode(equationType: EquationNodeType, workbook: Workbook, parent: EquationNode) : EquationNode;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| equationType | [EquationNodeType](./equationnodetype/) | Types of Equation Nodes |
| workbook | [Workbook](./workbook/) | The workbook object associated with the equation |
| parent | [EquationNode](./equationnode/) | The parent node where this node is located |

**Returns**

If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.


