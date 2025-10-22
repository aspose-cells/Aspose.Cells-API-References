##DelimiterEquationNode
This class specifies the delimiter equation consisting of opening and closing delimiters such as parentheses braces brackets and vertical bars and a component contained inside. The delimiter may have more than one component with a designated separator character between each component.
## DelimiterEquationNode class
This class specifies the delimiter equation, consisting of opening and closing delimiters (such as parentheses, braces, brackets, and vertical bars), and a component contained inside. The delimiter may have more than one component, with a designated separator character between each component.
```javascript
class DelimiterEquationNode extends EquationNode;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor(EquationNode)](#constructor-equationnode-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [beginChar](#beginChar--)| string | Delimiter beginning character. |
| [endChar](#endChar--)| string | Delimiter ending character. |
| [naryGrow](#naryGrow--)| boolean |  |
| [separatorChar](#separatorChar--)| string | Delimiter separator character. |
| [delimiterShape](#delimiterShape--)| EquationDelimiterShapeType | Specifies the shape of delimiters in the delimiter object. |
| [startIndex](#startIndex--)| number | Readonly. Gets the start index of the characters. |
| [length](#length--)| number | Readonly. Gets the length of the characters. |
| [font](#font--)| Font | Readonly. Returns the font of this object. |
| [textOptions](#textOptions--)| TextOptions | Readonly. Returns the text options. |
| [parentNode](#parentNode--)| EquationNode | Specifies the parent node of the current node |
| [equationType](#equationType--)| EquationNodeType | Readonly. Get the equation type of the current node |
## Methods
| Method | Description |
| --- | --- |
| [getBeginChar()](#getBeginChar--)| <b>@deprecated.</b> Please use the 'beginChar' property instead. Delimiter beginning character. |
| [setBeginChar(string)](#setBeginChar-string-)| <b>@deprecated.</b> Please use the 'beginChar' property instead. Delimiter beginning character. |
| [getEndChar()](#getEndChar--)| <b>@deprecated.</b> Please use the 'endChar' property instead. Delimiter ending character. |
| [setEndChar(string)](#setEndChar-string-)| <b>@deprecated.</b> Please use the 'endChar' property instead. Delimiter ending character. |
| [getNaryGrow()](#getNaryGrow--)| <b>@deprecated.</b> Please use the 'naryGrow' property instead. |
| [setNaryGrow(boolean)](#setNaryGrow-boolean-)| <b>@deprecated.</b> Please use the 'naryGrow' property instead. |
| [getSeparatorChar()](#getSeparatorChar--)| <b>@deprecated.</b> Please use the 'separatorChar' property instead. Delimiter separator character. |
| [setSeparatorChar(string)](#setSeparatorChar-string-)| <b>@deprecated.</b> Please use the 'separatorChar' property instead. Delimiter separator character. |
| [getDelimiterShape()](#getDelimiterShape--)| <b>@deprecated.</b> Please use the 'delimiterShape' property instead. Specifies the shape of delimiters in the delimiter object. |
| [setDelimiterShape(EquationDelimiterShapeType)](#setDelimiterShape-equationdelimitershapetype-)| <b>@deprecated.</b> Please use the 'delimiterShape' property instead. Specifies the shape of delimiters in the delimiter object. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getStartIndex()](#getStartIndex--)| <b>@deprecated.</b> Please use the 'startIndex' property instead. Gets the start index of the characters. |
| [getLength()](#getLength--)| <b>@deprecated.</b> Please use the 'length' property instead. Gets the length of the characters. |
| [getFont()](#getFont--)| <b>@deprecated.</b> Please use the 'font' property instead. Returns the font of this object. |
| [getTextOptions()](#getTextOptions--)| <b>@deprecated.</b> Please use the 'textOptions' property instead. Returns the text options. |
| [setWordArtStyle(PresetWordArtStyle)](#setWordArtStyle-presetwordartstyle-)| Sets the preset WordArt style. |
| [getParentNode()](#getParentNode--)| <b>@deprecated.</b> Please use the 'parentNode' property instead. Specifies the parent node of the current node |
| [setParentNode(EquationNode)](#setParentNode-equationnode-)| <b>@deprecated.</b> Please use the 'parentNode' property instead. Specifies the parent node of the current node |
| [getEquationType()](#getEquationType--)| <b>@deprecated.</b> Please use the 'equationType' property instead. Get the equation type of the current node |
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
| [equals(Object)](#equals-object-)| Determine whether the current equation node is equal to the specified node |
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
### beginChar {#beginChar--}
Delimiter beginning character.
```javascript
beginChar : string;
```
**Remarks**
It should be noted that this property only accepts one character, and if multiple characters are passed in, only the first character is accepted.
### endChar {#endChar--}
Delimiter ending character.
```javascript
endChar : string;
```
**Remarks**
It should be noted that this property only accepts one character, and if multiple characters are passed in, only the first character is accepted.
### naryGrow {#naryGrow--}
```javascript
naryGrow : boolean;
```
### separatorChar {#separatorChar--}
Delimiter separator character.
```javascript
separatorChar : string;
```
**Remarks**
It should be noted that this property only accepts one character, and if multiple characters are passed in, only the first character is accepted.
### delimiterShape {#delimiterShape--}
Specifies the shape of delimiters in the delimiter object.
```javascript
delimiterShape : EquationDelimiterShapeType;
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
### getBeginChar() {#getBeginChar--}
```javascript
getBeginChar() : string;
```
**Remarks**
It should be noted that this property only accepts one character, and if multiple characters are passed in, only the first character is accepted.
### setBeginChar(string) {#setBeginChar-string-}
```javascript
setBeginChar(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
**Remarks**
It should be noted that this property only accepts one character, and if multiple characters are passed in, only the first character is accepted.
### getEndChar() {#getEndChar--}
```javascript
getEndChar() : string;
```
**Remarks**
It should be noted that this property only accepts one character, and if multiple characters are passed in, only the first character is accepted.
### setEndChar(string) {#setEndChar-string-}
```javascript
setEndChar(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
**Remarks**
It should be noted that this property only accepts one character, and if multiple characters are passed in, only the first character is accepted.
### getNaryGrow() {#getNaryGrow--}
```javascript
getNaryGrow() : boolean;
```
### setNaryGrow(boolean) {#setNaryGrow-boolean-}
```javascript
setNaryGrow(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getSeparatorChar() {#getSeparatorChar--}
```javascript
getSeparatorChar() : string;
```
**Remarks**
It should be noted that this property only accepts one character, and if multiple characters are passed in, only the first character is accepted.
### setSeparatorChar(string) {#setSeparatorChar-string-}
```javascript
setSeparatorChar(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
**Remarks**
It should be noted that this property only accepts one character, and if multiple characters are passed in, only the first character is accepted.
### getDelimiterShape() {#getDelimiterShape--}
```javascript
getDelimiterShape() : EquationDelimiterShapeType;
```
**Returns**
[EquationDelimiterShapeType](../equationdelimitershapetype/)
### setDelimiterShape(EquationDelimiterShapeType) {#setDelimiterShape-equationdelimitershapetype-}
```javascript
setDelimiterShape(value: EquationDelimiterShapeType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [EquationDelimiterShapeType](../equationdelimitershapetype/) | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
### getStartIndex() {#getStartIndex--}
```javascript
getStartIndex() : number;
```
### getLength() {#getLength--}
```javascript
getLength() : number;
```
### getFont() {#getFont--}
```javascript
getFont() : Font;
```
**Returns**
[Font](../font/)
### getTextOptions() {#getTextOptions--}
```javascript
getTextOptions() : TextOptions;
```
**Returns**
[TextOptions](../textoptions/)
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
### getParentNode() {#getParentNode--}
```javascript
getParentNode() : EquationNode;
```
**Returns**
[EquationNode](../equationnode/)
### setParentNode(EquationNode) {#setParentNode-equationnode-}
```javascript
setParentNode(value: EquationNode) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [EquationNode](../equationnode/) | The value to set. |
### getEquationType() {#getEquationType--}
```javascript
getEquationType() : EquationNodeType;
```
**Returns**
[EquationNodeType](../equationnodetype/)
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
### equals(Object) {#equals-object-}
Determine whether the current equation node is equal to the specified node
```javascript
equals(obj: Object) : boolean;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | The specified node |
### getType() {#getType--}
Represents the type of the node.
```javascript
getType() : TextNodeType;
```
**Returns**
[TextNodeType](../textnodetype/)
