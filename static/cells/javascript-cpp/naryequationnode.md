##NaryEquationNode
This class specifies an nary operator equation consisting of an nary operator a base or operand and optional upper and lower bounds.
## NaryEquationNode class
This class specifies an n-ary operator equation consisting of an n-ary operator, a base (or operand), and optional upper and lower bounds.
```javascript
class NaryEquationNode extends EquationNode;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor(EquationNode)](#constructor-equationnode-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [isHideSubscript](#isHideSubscript--)| boolean | Whether to display the lower bound |
| [isHideSuperscript](#isHideSuperscript--)| boolean | Whether to display the upper bound |
| [limitLocation](#limitLocation--)| EquationLimitLocationType | This attribute specifies the location of limits in n-ary operators. Limits can be either centered above and below the n-ary operator, or positioned just to the right of the operator. |
| [naryOperator](#naryOperator--)| string | an n-ary operator.e.g "∑". It is strongly recommended to use attribute NaryOperatorType to set n-ary operator. Use this property setting if you cannot find the character you need in a known type. |
| [naryOperatorType](#naryOperatorType--)| EquationMathematicalOperatorType | an n-ary operator.e.g "∑" |
| [naryGrow](#naryGrow--)| boolean | This attribute specifies the growth property of n-ary operators at the document level. When off, n-ary operators such as integrals and summations do not grow to match the size of their operand height. When on, the n-ary operator grows vertically to match its operand height. |
| [startIndex](#startIndex--)| number | Readonly. Gets the start index of the characters. |
| [length](#length--)| number | Readonly. Gets the length of the characters. |
| [font](#font--)| Font | Readonly. Returns the font of this object. |
| [textOptions](#textOptions--)| TextOptions | Readonly. Returns the text options. |
| [parentNode](#parentNode--)| EquationNode | Specifies the parent node of the current node |
| [equationType](#equationType--)| EquationNodeType | Readonly. Get the equation type of the current node |
## Methods
| Method | Description |
| --- | --- |
| [setWordArtStyle(PresetWordArtStyle)](#setWordArtStyle-presetwordartstyle-)| Sets the preset WordArt style. |
| [toLaTeX()](#toLaTeX--)| Convert this equtation to LaTeX expression. |
| [toMathML()](#toMathML--)| Convert this equtation to MathML expression. |
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
| [equals(VObject)](#equals-vobject-)| Determine whether the current equation node is equal to the specified node |
| [getType()](#getType--)| Represents the type of the node. |
### constructor(EquationNode) {#constructor-equationnode-}
Constructs from a parent object convertible to this.
```javascript
constructor(obj: EquationNode);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | EquationNode | The parent object. |
### isHideSubscript {#isHideSubscript--}
Whether to display the lower bound
```javascript
isHideSubscript : boolean;
```
### isHideSuperscript {#isHideSuperscript--}
Whether to display the upper bound
```javascript
isHideSuperscript : boolean;
```
### limitLocation {#limitLocation--}
This attribute specifies the location of limits in n-ary operators. Limits can be either centered above and below the n-ary operator, or positioned just to the right of the operator.
```javascript
limitLocation : EquationLimitLocationType;
```
### naryOperator {#naryOperator--}
an n-ary operator.e.g "∑". It is strongly recommended to use attribute NaryOperatorType to set n-ary operator. Use this property setting if you cannot find the character you need in a known type.
```javascript
naryOperator : string;
```
**Remarks**
It should be noted that this property only accepts one character, and if multiple characters are passed in, only the first character is accepted.
### naryOperatorType {#naryOperatorType--}
an n-ary operator.e.g "∑"
```javascript
naryOperatorType : EquationMathematicalOperatorType;
```
### naryGrow {#naryGrow--}
This attribute specifies the growth property of n-ary operators at the document level. When off, n-ary operators such as integrals and summations do not grow to match the size of their operand height. When on, the n-ary operator grows vertically to match its operand height.
```javascript
naryGrow : boolean;
```
### startIndex {#startIndex--}
Readonly. Gets the start index of the characters.
```javascript
startIndex : number;
```
### length {#length--}
Readonly. Gets the length of the characters.
```javascript
length : number;
```
### font {#font--}
Readonly. Returns the font of this object.
```javascript
font : Font;
```
### textOptions {#textOptions--}
Readonly. Returns the text options.
```javascript
textOptions : TextOptions;
```
### parentNode {#parentNode--}
Specifies the parent node of the current node
```javascript
parentNode : EquationNode;
```
### equationType {#equationType--}
Readonly. Get the equation type of the current node
```javascript
equationType : EquationNodeType;
```
### setWordArtStyle(PresetWordArtStyle) {#setWordArtStyle-presetwordartstyle-}
Sets the preset WordArt style.
```javascript
setWordArtStyle(style: PresetWordArtStyle) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [PresetWordArtStyle](../presetwordartstyle/) | The preset WordArt style. |
**Remarks**
Only for the text of shape/chart.
### toLaTeX() {#toLaTeX--}
Convert this equtation to LaTeX expression.
```javascript
toLaTeX() : string;
```
### toMathML() {#toMathML--}
Convert this equtation to MathML expression.
```javascript
toMathML() : string;
```
### addChild(EquationNodeType) {#addChild-equationnodetype-}
Insert a node of the specified type at the end of the child node list of the current node.
```javascript
addChild(equationType: EquationNodeType) : EquationNode;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| equationType | [EquationNodeType](../equationnodetype/) | Types of Equation Nodes |
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
| node | [EquationNode](../equationnode/) | The specified node |
### insertChild(number, EquationNodeType) {#insertChild-number-equationnodetype-}
Inserts a node of the specified type at the specified index position in the current node's child node list.
```javascript
insertChild(index: number, equationType: EquationNodeType) : EquationNode;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | index value |
| equationType | [EquationNodeType](../equationnodetype/) | Types of Equation Nodes |
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
| equationType | [EquationNodeType](../equationnodetype/) | Types of Equation Nodes |
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
| equationType | [EquationNodeType](../equationnodetype/) | Types of Equation Nodes |
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
| node | [EquationNode](../equationnode/) | Node to be deleted. |
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
| equationType | [EquationNodeType](../equationnodetype/) | Types of Equation Nodes |
| workbook | [Workbook](../workbook/) | The workbook object associated with the equation |
| parent | [EquationNode](../equationnode/) | The parent node where this node is located |
**Returns**
If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### equals(VObject) {#equals-vobject-}
Determine whether the current equation node is equal to the specified node
```javascript
equals(obj: VObject) : boolean;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | VObject | The specified node |
### getType() {#getType--}
Represents the type of the node.
```javascript
getType() : TextNodeType;
```
**Returns**
[TextNodeType](../textnodetype/)
