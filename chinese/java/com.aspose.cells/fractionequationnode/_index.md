---
title: "FractionEquationNode"
second_title: "Aspose.Cells for Java API 参考"
description: "此类指定由分子和分母通过分数线分隔的分数方程。"
type: docs
url: /zh/java/com.aspose.cells/fractionequationnode/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.FontSetting](../../com.aspose.cells/fontsetting), [com.aspose.cells.EquationNode](../../com.aspose.cells/equationnode)
```
public class FractionEquationNode extends EquationNode
```

此类指定分数方程，由通过分数线分隔的分子和分母组成。分数线可以是水平的或对角的，取决于分数属性。分数方程还用于表示堆叠函数，该函数将一个元素放置在另一个元素之上，且没有分数线。
## 方法

| 方法 | 描述 |
| --- | --- |
| [addChild(EquationNode node)](#addChild-com.aspose.cells.EquationNode-) | 在当前节点的子节点列表末尾插入指定节点。 |
| [addChild(int equationType)](#addChild-int-) | 在当前节点的子节点列表末尾插入指定类型的节点。 |
| [createNode(int equationType, Workbook workbook, EquationNode parent)](#createNode-int-com.aspose.cells.Workbook-com.aspose.cells.EquationNode-) | 创建指定类型的节点。 |
| [equals(Object obj)](#equals-java.lang.Object-) | 确定当前方程节点是否等于指定节点 |
| [getChild(int index)](#getChild-int-) | 返回当前节点子节点中指定索引处的节点。 |
| [getClass()](#getClass--) |  |
| [getEquationType()](#getEquationType--) | 获取当前节点的方程类型 |
| [getFont()](#getFont--) | 返回此对象的字体。 |
| [getFractionType()](#getFractionType--) | 此项指定分数的类型；默认是 'Bar'。 |
| [getLength()](#getLength--) | 获取字符的长度。 |
| [getParentNode()](#getParentNode--) | 指定当前节点的父节点 |
| [getStartIndex()](#getStartIndex--) | 获取字符的起始索引。 |
| [getTextOptions()](#getTextOptions--) | 返回文本选项。 |
| [getType()](#getType--) | 表示节点的类型。 |
| [hashCode()](#hashCode--) |  |
| [insertAfter(int equationType)](#insertAfter-int-) | 在当前节点之后插入指定节点。 |
| [insertBefore(int equationType)](#insertBefore-int-) | 在当前节点之前插入指定节点。 |
| [insertChild(int index, int equationType)](#insertChild-int-int-) | 在当前节点的子节点列表中指定索引位置插入指定类型的节点。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove()](#remove--) | 从父节点中移除自身。 |
| [removeAllChildren()](#removeAllChildren--) | 移除当前节点的所有子节点。 |
| [removeChild(EquationNode node)](#removeChild-com.aspose.cells.EquationNode-) | 从当前节点的子节点中移除指定节点。 |
| [removeChild(int index)](#removeChild-int-) | 从当前节点的子节点中移除指定索引处的节点。 |
| [setFractionType(int value)](#setFractionType-int-) | 此项指定分数的类型；默认是 'Bar'。 |
| [setParentNode(EquationNode value)](#setParentNode-com.aspose.cells.EquationNode-) | 指定当前节点的父节点 |
| [setWordArtStyle(int style)](#setWordArtStyle-int-) | 设置预设的 WordArt 样式。 |
| [toLaTeX()](#toLaTeX--) | 将此等式转换为 LaTeX 表达式. |
| [toMathML()](#toMathML--) | 将此等式转换为 MathML 表达式. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addChild(EquationNode node) {#addChild-com.aspose.cells.EquationNode-}
```
public void addChild(EquationNode node)
```


在当前节点的子节点列表末尾插入指定节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| node | [EquationNode](../../com.aspose.cells/equationnode) | 指定的节点 |

### addChild(int equationType) {#addChild-int-}
```
public EquationNode addChild(int equationType)
```


在当前节点的子节点列表末尾插入指定类型的节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). 方程节点的类型 |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### createNode(int equationType, Workbook workbook, EquationNode parent) {#createNode-int-com.aspose.cells.Workbook-com.aspose.cells.EquationNode-}
```
public static EquationNode createNode(int equationType, Workbook workbook, EquationNode parent)
```


创建指定类型的节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). 方程节点的类型 |
| workbook | [Workbook](../../com.aspose.cells/workbook) | 与该方程关联的工作簿对象 |
| parent | [EquationNode](../../com.aspose.cells/equationnode) | 此节点所在的父节点 |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


确定当前方程节点是否等于指定节点

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj | java.lang.Object | 指定的节点 |

**Returns:**
boolean -
### getChild(int index) {#getChild-int-}
```
public EquationNode getChild(int index)
```


返回当前节点子节点中指定索引处的节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 节点的索引 |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - Returns the corresponding node if the specified node exists, otherwise returns null.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEquationType() {#getEquationType--}
```
public int getEquationType()
```


获取当前节点的方程类型

参见 [EquationNodeType](../../com.aspose.cells/equationnodetype).

**Returns:**
int
### getFont() {#getFont--}
```
public Font getFont()
```


返回此对象的字体。

**Returns:**
[Font](../../com.aspose.cells/font)
### getFractionType() {#getFractionType--}
```
public int getFractionType()
```


此项指定分数的类型；默认是 'Bar'。

参见 [EquationFractionType](../../com.aspose.cells/equationfractiontype)。

**Returns:**
int
### getLength() {#getLength--}
```
public int getLength()
```


获取字符的长度。

**Returns:**
int
### getParentNode() {#getParentNode--}
```
public EquationNode getParentNode()
```


指定当前节点的父节点

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode)
### getStartIndex() {#getStartIndex--}
```
public int getStartIndex()
```


获取字符的起始索引。

**Returns:**
int
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


返回文本选项。

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getType() {#getType--}
```
public int getType()
```


表示节点的类型。

参见 [TextNodeType](../../com.aspose.cells/textnodetype).

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


在当前节点之后插入指定节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). 方程节点的类型 |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### insertBefore(int equationType) {#insertBefore-int-}
```
public EquationNode insertBefore(int equationType)
```


在当前节点之前插入指定节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). 方程节点的类型 |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### insertChild(int index, int equationType) {#insertChild-int-int-}
```
public EquationNode insertChild(int index, int equationType)
```


在当前节点的子节点列表中指定索引位置插入指定类型的节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 索引值 |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). 方程节点的类型 |

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


从父节点中移除自身。

### removeAllChildren() {#removeAllChildren--}
```
public void removeAllChildren()
```


移除当前节点的所有子节点。

### removeChild(EquationNode node) {#removeChild-com.aspose.cells.EquationNode-}
```
public void removeChild(EquationNode node)
```


从当前节点的子节点中移除指定节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| node | [EquationNode](../../com.aspose.cells/equationnode) | 待删除的节点. |

### removeChild(int index) {#removeChild-int-}
```
public void removeChild(int index)
```


从当前节点的子节点中移除指定索引处的节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 节点的索引 |

### setFractionType(int value) {#setFractionType-int-}
```
public void setFractionType(int value)
```


此项指定分数的类型；默认是 'Bar'。

参见 [EquationFractionType](../../com.aspose.cells/equationfractiontype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setParentNode(EquationNode value) {#setParentNode-com.aspose.cells.EquationNode-}
```
public void setParentNode(EquationNode value)
```


指定当前节点的父节点

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [EquationNode](../../com.aspose.cells/equationnode) |  |

### setWordArtStyle(int style) {#setWordArtStyle-int-}
```
public void setWordArtStyle(int style)
```


设置预设的 WordArt 样式。

**Remarks**

仅适用于形状/图表的文本.

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| style | int | [PresetWordArtStyle](../../com.aspose.cells/presetwordartstyle). 预设的 WordArt 样式. |

### toLaTeX() {#toLaTeX--}
```
public String toLaTeX()
```


将此等式转换为 LaTeX 表达式.

**Returns:**
java.lang.String
### toMathML() {#toMathML--}
```
public String toMathML()
```


将此等式转换为 MathML 表达式.

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

