##DelimiterEquationNode
This class specifies the delimiter equation consisting of opening and closing delimiters such as parentheses braces brackets and vertical bars and a component contained inside.
**Inheritance:**
java.lang.Object, [com.aspose.cells.FontSetting](../../com.aspose.cells/fontsetting), [com.aspose.cells.EquationNode](../../com.aspose.cells/equationnode)
```
public class DelimiterEquationNode extends EquationNode
```
This class specifies the delimiter equation, consisting of opening and closing delimiters (such as parentheses, braces, brackets, and vertical bars), and a component contained inside. The delimiter may have more than one component, with a designated separator character between each component.
## Methods
| Method | Description |
| --- | --- |
| [addChild(EquationNode node)](#addChild-com.aspose.cells.EquationNode-) | Inserts the specified node at the end of the current node's list of child nodes. |
| [addChild(int equationType)](#addChild-int-) | Insert a node of the specified type at the end of the child node list of the current node. |
| [createNode(int equationType, Workbook workbook, EquationNode parent)](#createNode-int-com.aspose.cells.Workbook-com.aspose.cells.EquationNode-) | Create a node of the specified type. |
| [equals(Object obj)](#equals-java.lang.Object-) | Determine whether the current equation node is equal to the specified node |
| [getBeginChar()](#getBeginChar--) | Delimiter beginning character. |
| [getChild(int index)](#getChild-int-) | Returns the node at the specified index among the children of the current node. |
| [getClass()](#getClass--) |  |
| [getDelimiterShape()](#getDelimiterShape--) | Specifies the shape of delimiters in the delimiter object. |
| [getEndChar()](#getEndChar--) | Delimiter ending character. |
| [getEquationType()](#getEquationType--) | Get the equation type of the current node |
| [getFont()](#getFont--) | Returns the font of this object. |
| [getLength()](#getLength--) | Gets the length of the characters. |
| [getNaryGrow()](#getNaryGrow--) |  |
| [getParentNode()](#getParentNode--) | Specifies the parent node of the current node |
| [getSeparatorChar()](#getSeparatorChar--) | Delimiter separator character. |
| [getStartIndex()](#getStartIndex--) | Gets the start index of the characters. |
| [getTextOptions()](#getTextOptions--) | Returns the text options. |
| [getType()](#getType--) | Represents the type of the node. |
| [hashCode()](#hashCode--) |  |
| [insertAfter(int equationType)](#insertAfter-int-) | Inserts the specified node after the current node. |
| [insertBefore(int equationType)](#insertBefore-int-) | Inserts the specified node before the current node. |
| [insertChild(int index, int equationType)](#insertChild-int-int-) | Inserts a node of the specified type at the specified index position in the current node's child node list. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove()](#remove--) | Removes itself from the parent. |
| [removeAllChildren()](#removeAllChildren--) | Removes all the child nodes of the current node. |
| [removeChild(EquationNode node)](#removeChild-com.aspose.cells.EquationNode-) | Removes the specified node from the current node's children. |
| [removeChild(int index)](#removeChild-int-) | Removes the node at the specified index from the current node's children. |
| [setBeginChar(String value)](#setBeginChar-java.lang.String-) | Delimiter beginning character. |
| [setDelimiterShape(int value)](#setDelimiterShape-int-) | Specifies the shape of delimiters in the delimiter object. |
| [setEndChar(String value)](#setEndChar-java.lang.String-) | Delimiter ending character. |
| [setNaryGrow(boolean value)](#setNaryGrow-boolean-) |  |
| [setParentNode(EquationNode value)](#setParentNode-com.aspose.cells.EquationNode-) | Specifies the parent node of the current node |
| [setSeparatorChar(String value)](#setSeparatorChar-java.lang.String-) | Delimiter separator character. |
| [setWordArtStyle(int style)](#setWordArtStyle-int-) | Sets the preset WordArt style. |
| [toLaTeX()](#toLaTeX--) | Convert this equtation to LaTeX expression. |
| [toMathML()](#toMathML--) | Convert this equtation to MathML expression. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addChild(EquationNode node) {#addChild-com.aspose.cells.EquationNode-}
```
public void addChild(EquationNode node)
```
Inserts the specified node at the end of the current node's list of child nodes.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| node | [EquationNode](../../com.aspose.cells/equationnode) | The specified node |
### addChild(int equationType) {#addChild-int-}
```
public EquationNode addChild(int equationType)
```
Insert a node of the specified type at the end of the child node list of the current node.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). Types of Equation Nodes |
**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### createNode(int equationType, Workbook workbook, EquationNode parent) {#createNode-int-com.aspose.cells.Workbook-com.aspose.cells.EquationNode-}
```
public static EquationNode createNode(int equationType, Workbook workbook, EquationNode parent)
```
Create a node of the specified type.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). Types of Equation Nodes |
| workbook | [Workbook](../../com.aspose.cells/workbook) | The workbook object associated with the equation |
| parent | [EquationNode](../../com.aspose.cells/equationnode) | The parent node where this node is located |
**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```
Determine whether the current equation node is equal to the specified node
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | The specified node |
**Returns:**
boolean -
### getBeginChar() {#getBeginChar--}
```
public String getBeginChar()
```
Delimiter beginning character.
**Remarks**
It should be noted that this property only accepts one character, and if multiple characters are passed in, only the first character is accepted.
**Returns:**
java.lang.String
### getChild(int index) {#getChild-int-}
```
public EquationNode getChild(int index)
```
Returns the node at the specified index among the children of the current node.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | Index of the node |
**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - Returns the corresponding node if the specified node exists, otherwise returns null.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getDelimiterShape() {#getDelimiterShape--}
```
public int getDelimiterShape()
```
Specifies the shape of delimiters in the delimiter object.
See [EquationDelimiterShapeType](../../com.aspose.cells/equationdelimitershapetype).
**Returns:**
int
### getEndChar() {#getEndChar--}
```
public String getEndChar()
```
Delimiter ending character.
**Remarks**
It should be noted that this property only accepts one character, and if multiple characters are passed in, only the first character is accepted.
**Returns:**
java.lang.String
### getEquationType() {#getEquationType--}
```
public int getEquationType()
```
Get the equation type of the current node
See [EquationNodeType](../../com.aspose.cells/equationnodetype).
**Returns:**
int
### getFont() {#getFont--}
```
public Font getFont()
```
Returns the font of this object.
**Returns:**
[Font](../../com.aspose.cells/font)
### getLength() {#getLength--}
```
public int getLength()
```
Gets the length of the characters.
**Returns:**
int
### getNaryGrow() {#getNaryGrow--}
```
public boolean getNaryGrow()
```
**Returns:**
boolean
### getParentNode() {#getParentNode--}
```
public EquationNode getParentNode()
```
Specifies the parent node of the current node
**Returns:**
[EquationNode](../../com.aspose.cells/equationnode)
### getSeparatorChar() {#getSeparatorChar--}
```
public String getSeparatorChar()
```
Delimiter separator character.
**Remarks**
It should be noted that this property only accepts one character, and if multiple characters are passed in, only the first character is accepted.
**Returns:**
java.lang.String
### getStartIndex() {#getStartIndex--}
```
public int getStartIndex()
```
Gets the start index of the characters.
**Returns:**
int
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```
Returns the text options.
**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getType() {#getType--}
```
public int getType()
```
Represents the type of the node.
See [TextNodeType](../../com.aspose.cells/textnodetype).
**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### insertAfter(int equationType) {#insertAfter-int-}
```
public EquationNode insertAfter(int equationType)
```
Inserts the specified node after the current node.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). Types of Equation Nodes |
**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### insertBefore(int equationType) {#insertBefore-int-}
```
public EquationNode insertBefore(int equationType)
```
Inserts the specified node before the current node.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). Types of Equation Nodes |
**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### insertChild(int index, int equationType) {#insertChild-int-int-}
```
public EquationNode insertChild(int index, int equationType)
```
Inserts a node of the specified type at the specified index position in the current node's child node list.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | index value |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). Types of Equation Nodes |
**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
### remove() {#remove--}
```
public void remove()
```
Removes itself from the parent.
### removeAllChildren() {#removeAllChildren--}
```
public void removeAllChildren()
```
Removes all the child nodes of the current node.
### removeChild(EquationNode node) {#removeChild-com.aspose.cells.EquationNode-}
```
public void removeChild(EquationNode node)
```
Removes the specified node from the current node's children.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| node | [EquationNode](../../com.aspose.cells/equationnode) | Node to be deleted. |
### removeChild(int index) {#removeChild-int-}
```
public void removeChild(int index)
```
Removes the node at the specified index from the current node's children.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | Index of the node |
### setBeginChar(String value) {#setBeginChar-java.lang.String-}
```
public void setBeginChar(String value)
```
Delimiter beginning character.
**Remarks**
It should be noted that this property only accepts one character, and if multiple characters are passed in, only the first character is accepted.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setDelimiterShape(int value) {#setDelimiterShape-int-}
```
public void setDelimiterShape(int value)
```
Specifies the shape of delimiters in the delimiter object.
See [EquationDelimiterShapeType](../../com.aspose.cells/equationdelimitershapetype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setEndChar(String value) {#setEndChar-java.lang.String-}
```
public void setEndChar(String value)
```
Delimiter ending character.
**Remarks**
It should be noted that this property only accepts one character, and if multiple characters are passed in, only the first character is accepted.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setNaryGrow(boolean value) {#setNaryGrow-boolean-}
```
public void setNaryGrow(boolean value)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setParentNode(EquationNode value) {#setParentNode-com.aspose.cells.EquationNode-}
```
public void setParentNode(EquationNode value)
```
Specifies the parent node of the current node
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [EquationNode](../../com.aspose.cells/equationnode) |  |
### setSeparatorChar(String value) {#setSeparatorChar-java.lang.String-}
```
public void setSeparatorChar(String value)
```
Delimiter separator character.
**Remarks**
It should be noted that this property only accepts one character, and if multiple characters are passed in, only the first character is accepted.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setWordArtStyle(int style) {#setWordArtStyle-int-}
```
public void setWordArtStyle(int style)
```
Sets the preset WordArt style.
**Remarks**
Only for the text of shape/chart.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | int | [PresetWordArtStyle](../../com.aspose.cells/presetwordartstyle). The preset WordArt style. |
### toLaTeX() {#toLaTeX--}
```
public String toLaTeX()
```
Convert this equtation to LaTeX expression.
**Returns:**
java.lang.String
### toMathML() {#toMathML--}
```
public String toMathML()
```
Convert this equtation to MathML expression.
**Returns:**
java.lang.String -
### toString() {#toString--}
```
public String toString()
```
**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```
### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |
