---
title: "NaryEquationNode"
second_title: "Aspose.Cells for Java API Reference"
description: "هذه الفئة تحدد معادلة عامل n-ary تتكون من عامل n-ary أساسي أو معامل وحدود علوية وسفلية اختيارية."
type: docs
url: /ar/java/com.aspose.cells/naryequationnode/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.FontSetting](../../com.aspose.cells/fontsetting), [com.aspose.cells.EquationNode](../../com.aspose.cells/equationnode)
```
public class NaryEquationNode extends EquationNode
```

هذه الفئة تحدد معادلة عامل n-ary تتكون من عامل n-ary، قاعدة (أو معامل)، وحدود عليا وسفلى اختيارية.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [addChild(EquationNode node)](#addChild-com.aspose.cells.EquationNode-) | يدرج العقدة المحددة في نهاية قائمة العقد الفرعية للعقدة الحالية. |
| [addChild(int equationType)](#addChild-int-) | أدرج عقدة من النوع المحدد في نهاية قائمة العقد الفرعية للعقدة الحالية. |
| [createNode(int equationType, Workbook workbook, EquationNode parent)](#createNode-int-com.aspose.cells.Workbook-com.aspose.cells.EquationNode-) | أنشئ عقدة من النوع المحدد. |
| [equals(Object obj)](#equals-java.lang.Object-) | حدد ما إذا كانت عقدة المعادلة الحالية مساوية للعقدة المحددة |
| [getChild(int index)](#getChild-int-) | يرجع العقدة الموجودة في الفهرس المحدد بين أبناء العقدة الحالية. |
| [getClass()](#getClass--) |  |
| [getEquationType()](#getEquationType--) | احصل على نوع المعادلة للعقدة الحالية |
| [getFont()](#getFont--) | يرجع الخط لهذا الكائن. |
| [getLength()](#getLength--) | يسترجع طول الأحرف. |
| [getLimitLocation()](#getLimitLocation--) | هذه الخاصية تحدد موقع الحدود في عوامل n-ary. |
| [getNaryGrow()](#getNaryGrow--) | هذه الخاصية تحدد خاصية النمو لعوامل n-ary على مستوى المستند. |
| [getNaryOperator()](#getNaryOperator--) | عامل n-ary. مثال: "\\u922d?. |
| [getNaryOperatorType()](#getNaryOperatorType--) | عامل n-ary. مثال: "\\u922d? |
| [getParentNode()](#getParentNode--) | يحدد العقدة الأصلية للعقدة الحالية |
| [getStartIndex()](#getStartIndex--) | يسترجع الفهرس الابتدائي للأحرف. |
| [getTextOptions()](#getTextOptions--) | يرجع خيارات النص. |
| [getType()](#getType--) | يمثل نوع العقدة. |
| [hashCode()](#hashCode--) |  |
| [insertAfter(int equationType)](#insertAfter-int-) | يدرج العقدة المحددة بعد العقدة الحالية. |
| [insertBefore(int equationType)](#insertBefore-int-) | يدرج العقدة المحددة قبل العقدة الحالية. |
| [insertChild(int index, int equationType)](#insertChild-int-int-) | يدرج عقدة من النوع المحدد في موضع الفهرس المحدد في قائمة العقد الفرعية للعقدة الحالية. |
| [isHideSubscript()](#isHideSubscript--) | ما إذا كان سيتم عرض الحد الأدنى |
| [isHideSuperscript()](#isHideSuperscript--) | ما إذا كان سيتم عرض الحد الأعلى |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove()](#remove--) | يزيل نفسه من العنصر الأب. |
| [removeAllChildren()](#removeAllChildren--) | يزيل جميع العقد الفرعية للعقدة الحالية. |
| [removeChild(EquationNode node)](#removeChild-com.aspose.cells.EquationNode-) | يزيل العقدة المحددة من أبناء العقدة الحالية. |
| [removeChild(int index)](#removeChild-int-) | يزيل العقدة الموجودة في الفهرس المحدد من أبناء العقدة الحالية. |
| [setHideSubscript(boolean value)](#setHideSubscript-boolean-) | ما إذا كان سيتم عرض الحد الأدنى |
| [setHideSuperscript(boolean value)](#setHideSuperscript-boolean-) | ما إذا كان سيتم عرض الحد الأعلى |
| [setLimitLocation(int value)](#setLimitLocation-int-) | هذه الخاصية تحدد موقع الحدود في عوامل n-ary. |
| [setNaryGrow(boolean value)](#setNaryGrow-boolean-) | هذه الخاصية تحدد خاصية النمو لعوامل n-ary على مستوى المستند. |
| [setNaryOperator(String value)](#setNaryOperator-java.lang.String-) | عامل n-ary. مثال: "\\u922d?. |
| [setNaryOperatorType(int value)](#setNaryOperatorType-int-) | عامل n-ary. مثال: "\\u922d? |
| [setParentNode(EquationNode value)](#setParentNode-com.aspose.cells.EquationNode-) | يحدد العقدة الأصلية للعقدة الحالية |
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
### getLimitLocation() {#getLimitLocation--}
```
public int getLimitLocation()
```


تحدد هذه السمة موقع الحدود في عوامل n-ary. يمكن أن تكون الحدود إما متمركزة فوق وتحت عامل n-ary، أو موضوعة مباشرةً إلى يمين العامل.

انظر [EquationLimitLocationType](../../com.aspose.cells/equationlimitlocationtype).

**Returns:**
int
### getNaryGrow() {#getNaryGrow--}
```
public boolean getNaryGrow()
```


تحدد هذه السمة خاصية النمو لعوامل n-ary على مستوى المستند. عندما تكون مُعطلة، لا تنمو عوامل n-ary مثل التكاملات والجمع لتطابق حجم ارتفاع المعامل الخاص بها. عندما تكون مفعلة، ينمو عامل n-ary عمودياً ليتطابق مع ارتفاع معاملاته.

**Returns:**
boolean
### getNaryOperator() {#getNaryOperator--}
```
public String getNaryOperator()
```


عامل n-ary operator. على سبيل المثال "\\u922d?. يُنصح بشدة باستخدام السمة NaryOperatorType لتعيين n-ary operator. استخدم إعداد الخاصية هذا إذا لم تتمكن من العثور على الحرف الذي تحتاجه في نوع معروف.

**Remarks**

يجب ملاحظة أن هذه الخاصية تقبل حرفًا واحدًا فقط، وإذا تم تمرير عدة أحرف، يُقبل الحرف الأول فقط.

**Returns:**
java.lang.String
### getNaryOperatorType() {#getNaryOperatorType--}
```
public int getNaryOperatorType()
```


عامل n-ary. مثال: "\\u922d?

انظر [EquationMathematicalOperatorType](../../com.aspose.cells/equationmathematicaloperatortype).

**Returns:**
int
### getParentNode() {#getParentNode--}
```
public EquationNode getParentNode()
```


يحدد العقدة الأصلية للعقدة الحالية

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode)
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
### isHideSubscript() {#isHideSubscript--}
```
public boolean isHideSubscript()
```


ما إذا كان سيتم عرض الحد الأدنى

**Returns:**
boolean
### isHideSuperscript() {#isHideSuperscript--}
```
public boolean isHideSuperscript()
```


ما إذا كان سيتم عرض الحد الأعلى

**Returns:**
boolean
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

### setHideSubscript(boolean value) {#setHideSubscript-boolean-}
```
public void setHideSubscript(boolean value)
```


ما إذا كان سيتم عرض الحد الأدنى

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setHideSuperscript(boolean value) {#setHideSuperscript-boolean-}
```
public void setHideSuperscript(boolean value)
```


ما إذا كان سيتم عرض الحد الأعلى

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setLimitLocation(int value) {#setLimitLocation-int-}
```
public void setLimitLocation(int value)
```


تحدد هذه السمة موقع الحدود في عوامل n-ary. يمكن أن تكون الحدود إما متمركزة فوق وتحت عامل n-ary، أو موضوعة مباشرةً إلى يمين العامل.

انظر [EquationLimitLocationType](../../com.aspose.cells/equationlimitlocationtype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setNaryGrow(boolean value) {#setNaryGrow-boolean-}
```
public void setNaryGrow(boolean value)
```


تحدد هذه السمة خاصية النمو لعوامل n-ary على مستوى المستند. عندما تكون مُعطلة، لا تنمو عوامل n-ary مثل التكاملات والجمع لتطابق حجم ارتفاع المعامل الخاص بها. عندما تكون مفعلة، ينمو عامل n-ary عمودياً ليتطابق مع ارتفاع معاملاته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setNaryOperator(String value) {#setNaryOperator-java.lang.String-}
```
public void setNaryOperator(String value)
```


عامل n-ary operator. على سبيل المثال "\\u922d?. يُنصح بشدة باستخدام السمة NaryOperatorType لتعيين n-ary operator. استخدم إعداد الخاصية هذا إذا لم تتمكن من العثور على الحرف الذي تحتاجه في نوع معروف.

**Remarks**

يجب ملاحظة أن هذه الخاصية تقبل حرفًا واحدًا فقط، وإذا تم تمرير عدة أحرف، يُقبل الحرف الأول فقط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setNaryOperatorType(int value) {#setNaryOperatorType-int-}
```
public void setNaryOperatorType(int value)
```


عامل n-ary. مثال: "\\u922d?

انظر [EquationMathematicalOperatorType](../../com.aspose.cells/equationmathematicaloperatortype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setParentNode(EquationNode value) {#setParentNode-com.aspose.cells.EquationNode-}
```
public void setParentNode(EquationNode value)
```


يحدد العقدة الأصلية للعقدة الحالية

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [EquationNode](../../com.aspose.cells/equationnode) |  |

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

