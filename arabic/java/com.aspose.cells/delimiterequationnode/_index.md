---
title: "DelimiterEquationNode"
second_title: "Aspose.Cells for Java API Reference"
description: "هذه الفئة تحدد معادلة الفاصل التي تتكون من الفواصل الافتتاحية والإغلاقية مثل الأقواس المعقوفة والأقواس المربعة والشرطات العمودية ومكوّن موجود بداخلها."
type: docs
url: /ar/java/com.aspose.cells/delimiterequationnode/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.FontSetting](../../com.aspose.cells/fontsetting), [com.aspose.cells.EquationNode](../../com.aspose.cells/equationnode)
```
public class DelimiterEquationNode extends EquationNode
```

هذه الفئة تحدد معادلة الفاصل، التي تتكون من الفواصل الافتتاحية والإغلاقية (مثل الأقواس، الأقواس المعقوفة، الأقواس المربعة، والشرطات العمودية)، ومكوّن موجود بداخلها. قد يحتوي الفاصل على أكثر من مكوّن، مع حرف فاصل مخصص بين كل مكوّن.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [addChild(EquationNode node)](#addChild-com.aspose.cells.EquationNode-) | يدرج العقدة المحددة في نهاية قائمة العقد الفرعية للعقدة الحالية. |
| [addChild(int equationType)](#addChild-int-) | أدرج عقدة من النوع المحدد في نهاية قائمة العقد الفرعية للعقدة الحالية. |
| [createNode(int equationType, Workbook workbook, EquationNode parent)](#createNode-int-com.aspose.cells.Workbook-com.aspose.cells.EquationNode-) | أنشئ عقدة من النوع المحدد. |
| [equals(Object obj)](#equals-java.lang.Object-) | حدد ما إذا كانت عقدة المعادلة الحالية مساوية للعقدة المحددة |
| [getBeginChar()](#getBeginChar--) | حرف بداية الفاصل. |
| [getChild(int index)](#getChild-int-) | يرجع العقدة الموجودة في الفهرس المحدد بين أبناء العقدة الحالية. |
| [getClass()](#getClass--) |  |
| [getDelimiterShape()](#getDelimiterShape--) | يحدد شكل الفواصل في كائن الفاصل. |
| [getEndChar()](#getEndChar--) | حرف نهاية الفاصل. |
| [getEquationType()](#getEquationType--) | احصل على نوع المعادلة للعقدة الحالية |
| [getFont()](#getFont--) | يرجع الخط لهذا الكائن. |
| [getLength()](#getLength--) | يسترجع طول الأحرف. |
| [getNaryGrow()](#getNaryGrow--) | يحدد ما إذا كان الفاصل يجب أن يتوسع ويتقلص تلقائيًا مع ارتفاع الصيغة. |
| [getParentNode()](#getParentNode--) | يحدد العقدة الأصلية للعقدة الحالية |
| [getSeparatorChar()](#getSeparatorChar--) | حرف فاصل الفاصل. |
| [getStartIndex()](#getStartIndex--) | يسترجع الفهرس الابتدائي للأحرف. |
| [getTextOptions()](#getTextOptions--) | يرجع خيارات النص. |
| [getType()](#getType--) | يمثل نوع العقدة. |
| [hashCode()](#hashCode--) |  |
| [insertAfter(int equationType)](#insertAfter-int-) | يدرج العقدة المحددة بعد العقدة الحالية. |
| [insertBefore(int equationType)](#insertBefore-int-) | يدرج العقدة المحددة قبل العقدة الحالية. |
| [insertChild(int index, int equationType)](#insertChild-int-int-) | يدرج عقدة من النوع المحدد في موضع الفهرس المحدد في قائمة العقد الفرعية للعقدة الحالية. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove()](#remove--) | يزيل نفسه من العنصر الأب. |
| [removeAllChildren()](#removeAllChildren--) | يزيل جميع العقد الفرعية للعقدة الحالية. |
| [removeChild(EquationNode node)](#removeChild-com.aspose.cells.EquationNode-) | يزيل العقدة المحددة من أبناء العقدة الحالية. |
| [removeChild(int index)](#removeChild-int-) | يزيل العقدة الموجودة في الفهرس المحدد من أبناء العقدة الحالية. |
| [setBeginChar(String value)](#setBeginChar-java.lang.String-) | حرف بداية الفاصل. |
| [setDelimiterShape(int value)](#setDelimiterShape-int-) | يحدد شكل الفواصل في كائن الفاصل. |
| [setEndChar(String value)](#setEndChar-java.lang.String-) | حرف نهاية الفاصل. |
| [setNaryGrow(boolean value)](#setNaryGrow-boolean-) | يحدد ما إذا كان الفاصل يجب أن يتوسع ويتقلص تلقائيًا مع ارتفاع الصيغة. |
| [setParentNode(EquationNode value)](#setParentNode-com.aspose.cells.EquationNode-) | يحدد العقدة الأصلية للعقدة الحالية |
| [setSeparatorChar(String value)](#setSeparatorChar-java.lang.String-) | حرف فاصل الفاصل. |
| [setWordArtStyle(int style)](#setWordArtStyle-int-) | يضبط نمط WordArt المحدد مسبقًا. |
| [toLaTeX()](#toLaTeX--) | حوّل هذه المعادلة إلى تعبير LaTeX. |
| [toMathML()](#toMathML--) | حوّل هذه المعادلة إلى تعبير MathML. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addChild(EquationNode node) {#addChild-com.aspose.cells.EquationNode-}
```
public void addChild(EquationNode node)
```


يدرج العقدة المحددة في نهاية قائمة العقد الفرعية للعقدة الحالية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| node | [EquationNode](../../com.aspose.cells/equationnode) | العقدة المحددة |

### addChild(int equationType) {#addChild-int-}
```
public EquationNode addChild(int equationType)
```


أدرج عقدة من النوع المحدد في نهاية قائمة العقد الفرعية للعقدة الحالية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). أنواع عقد المعادلة |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### createNode(int equationType, Workbook workbook, EquationNode parent) {#createNode-int-com.aspose.cells.Workbook-com.aspose.cells.EquationNode-}
```
public static EquationNode createNode(int equationType, Workbook workbook, EquationNode parent)
```


أنشئ عقدة من النوع المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). أنواع عقد المعادلة |
| workbook | [Workbook](../../com.aspose.cells/workbook) | كائن دفتر العمل المرتبط بالمعادلة |
| parent | [EquationNode](../../com.aspose.cells/equationnode) | العقدة الأب حيث توجد هذه العقدة |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


حدد ما إذا كانت عقدة المعادلة الحالية مساوية للعقدة المحددة

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| obj | java.lang.Object | العقدة المحددة |

**Returns:**
boolean -
### getBeginChar() {#getBeginChar--}
```
public String getBeginChar()
```


حرف بداية الفاصل.

**Remarks**

يجب ملاحظة أن هذه الخاصية تقبل حرفًا واحدًا فقط، وإذا تم تمرير عدة أحرف، يُقبل الحرف الأول فقط.

**Returns:**
java.lang.String
### getChild(int index) {#getChild-int-}
```
public EquationNode getChild(int index)
```


يرجع العقدة الموجودة في الفهرس المحدد بين أبناء العقدة الحالية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | فهرس العقدة |

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


يحدد شكل الفواصل في كائن الفاصل.

انظر [EquationDelimiterShapeType](../../com.aspose.cells/equationdelimitershapetype).

**Returns:**
int
### getEndChar() {#getEndChar--}
```
public String getEndChar()
```


حرف نهاية الفاصل.

**Remarks**

يجب ملاحظة أن هذه الخاصية تقبل حرفًا واحدًا فقط، وإذا تم تمرير عدة أحرف، يُقبل الحرف الأول فقط.

**Returns:**
java.lang.String
### getEquationType() {#getEquationType--}
```
public int getEquationType()
```


احصل على نوع المعادلة للعقدة الحالية

انظر [EquationNodeType](../../com.aspose.cells/equationnodetype).

**Returns:**
int
### getFont() {#getFont--}
```
public Font getFont()
```


يرجع الخط لهذا الكائن.

**Returns:**
[Font](../../com.aspose.cells/font)
### getLength() {#getLength--}
```
public int getLength()
```


يسترجع طول الأحرف.

**Returns:**
int
### getNaryGrow() {#getNaryGrow--}
```
public boolean getNaryGrow()
```


يحدد ما إذا كان الفاصل يجب أن يتوسع ويتقلص تلقائيًا مع ارتفاع الصيغة.

**Remarks**

هذه الخاصية تحدد خاصية النمو للفاصل على مستوى المستند. عندما تكون مُعطلة، لن يتوسع الفاصل لمطابقة حجم ارتفاع مكوّنه. عندما تكون مفعلة، يتوسع الفاصل عموديًا لمطابقة ارتفاع مكوّنه.

**Returns:**
boolean
### getParentNode() {#getParentNode--}
```
public EquationNode getParentNode()
```


يحدد العقدة الأصلية للعقدة الحالية

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode)
### getSeparatorChar() {#getSeparatorChar--}
```
public String getSeparatorChar()
```


حرف فاصل الفاصل.

**Remarks**

يجب ملاحظة أن هذه الخاصية تقبل حرفًا واحدًا فقط، وإذا تم تمرير عدة أحرف، يُقبل الحرف الأول فقط.

**Returns:**
java.lang.String
### getStartIndex() {#getStartIndex--}
```
public int getStartIndex()
```


يسترجع الفهرس الابتدائي للأحرف.

**Returns:**
int
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


يرجع خيارات النص.

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getType() {#getType--}
```
public int getType()
```


يمثل نوع العقدة.

انظر [TextNodeType](../../com.aspose.cells/textnodetype).

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


يدرج العقدة المحددة بعد العقدة الحالية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). أنواع عقد المعادلة |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### insertBefore(int equationType) {#insertBefore-int-}
```
public EquationNode insertBefore(int equationType)
```


يدرج العقدة المحددة قبل العقدة الحالية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). أنواع عقد المعادلة |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### insertChild(int index, int equationType) {#insertChild-int-int-}
```
public EquationNode insertChild(int index, int equationType)
```


يدرج عقدة من النوع المحدد في موضع الفهرس المحدد في قائمة العقد الفرعية للعقدة الحالية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | قيمة الفهرس |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). أنواع عقد المعادلة |

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


يزيل نفسه من العنصر الأب.

### removeAllChildren() {#removeAllChildren--}
```
public void removeAllChildren()
```


يزيل جميع العقد الفرعية للعقدة الحالية.

### removeChild(EquationNode node) {#removeChild-com.aspose.cells.EquationNode-}
```
public void removeChild(EquationNode node)
```


يزيل العقدة المحددة من أبناء العقدة الحالية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| node | [EquationNode](../../com.aspose.cells/equationnode) | العقدة التي سيتم حذفها. |

### removeChild(int index) {#removeChild-int-}
```
public void removeChild(int index)
```


يزيل العقدة الموجودة في الفهرس المحدد من أبناء العقدة الحالية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | فهرس العقدة |

### setBeginChar(String value) {#setBeginChar-java.lang.String-}
```
public void setBeginChar(String value)
```


حرف بداية الفاصل.

**Remarks**

يجب ملاحظة أن هذه الخاصية تقبل حرفًا واحدًا فقط، وإذا تم تمرير عدة أحرف، يُقبل الحرف الأول فقط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setDelimiterShape(int value) {#setDelimiterShape-int-}
```
public void setDelimiterShape(int value)
```


يحدد شكل الفواصل في كائن الفاصل.

انظر [EquationDelimiterShapeType](../../com.aspose.cells/equationdelimitershapetype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setEndChar(String value) {#setEndChar-java.lang.String-}
```
public void setEndChar(String value)
```


حرف نهاية الفاصل.

**Remarks**

يجب ملاحظة أن هذه الخاصية تقبل حرفًا واحدًا فقط، وإذا تم تمرير عدة أحرف، يُقبل الحرف الأول فقط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setNaryGrow(boolean value) {#setNaryGrow-boolean-}
```
public void setNaryGrow(boolean value)
```


يحدد ما إذا كان الفاصل يجب أن يتوسع ويتقلص تلقائيًا مع ارتفاع الصيغة.

**Remarks**

هذه الخاصية تحدد خاصية النمو للفاصل على مستوى المستند. عندما تكون مُعطلة، لن يتوسع الفاصل لمطابقة حجم ارتفاع مكوّنه. عندما تكون مفعلة، يتوسع الفاصل عموديًا لمطابقة ارتفاع مكوّنه.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setParentNode(EquationNode value) {#setParentNode-com.aspose.cells.EquationNode-}
```
public void setParentNode(EquationNode value)
```


يحدد العقدة الأصلية للعقدة الحالية

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [EquationNode](../../com.aspose.cells/equationnode) |  |

### setSeparatorChar(String value) {#setSeparatorChar-java.lang.String-}
```
public void setSeparatorChar(String value)
```


حرف فاصل الفاصل.

**Remarks**

يجب ملاحظة أن هذه الخاصية تقبل حرفًا واحدًا فقط، وإذا تم تمرير عدة أحرف، يُقبل الحرف الأول فقط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setWordArtStyle(int style) {#setWordArtStyle-int-}
```
public void setWordArtStyle(int style)
```


يضبط نمط WordArt المحدد مسبقًا.

**Remarks**

فقط لنص الشكل/المخطط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| style | int | [PresetWordArtStyle](../../com.aspose.cells/presetwordartstyle). نمط WordArt المحدد مسبقًا. |

### toLaTeX() {#toLaTeX--}
```
public String toLaTeX()
```


حوّل هذه المعادلة إلى تعبير LaTeX.

**Returns:**
java.lang.String
### toMathML() {#toMathML--}
```
public String toMathML()
```


حوّل هذه المعادلة إلى تعبير MathML.

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

