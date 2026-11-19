---
title: "UnionRange"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل نطاق الاتحاد."
type: docs
url: /ar/java/com.aspose.cells/unionrange/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class UnionRange implements Iterable
```

يمثل نطاق الاتحاد.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | يطبق التنسيقات على نطاق كامل. |
| [copy(UnionRange range, PasteOptions options)](#copy-com.aspose.cells.UnionRange-com.aspose.cells.PasteOptions-) | نسخ النطاق باستخدام خيارات اللصق الخاصة. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCellCount()](#getCellCount--) | يحصل على عدد جميع الخلايا في النطاق. |
| [getClass()](#getClass--) |  |
| [getColumnCount()](#getColumnCount--) | يحصل على عدد الصفوف في النطاق. |
| [getFirstColumn()](#getFirstColumn--) | يحصل على فهرس العمود الأول في النطاق. |
| [getFirstRow()](#getFirstRow--) | يحصل على فهرس الصف الأول في النطاق. |
| [getHyperlinks()](#getHyperlinks--) | يحصل على جميع الروابط التشعبية في النطاق. |
| [getName()](#getName--) | يحصل على اسم النطاق. |
| [getRangeCount()](#getRangeCount--) | يحصل على عدد النطاقات. |
| [getRanges()](#getRanges--) | يحصل على جميع نطاقات الاتحاد. |
| [getRefersTo()](#getRefersTo--) | يحصل على ما يشير إليه النطاق. |
| [getRowCount()](#getRowCount--) | يحصل على عدد الصفوف في النطاق. |
| [getValue()](#getValue--) | يحصل على قيم النطاق. |
| [hasRange()](#hasRange--) | يشير إلى ما إذا كان لهذا نطاق. |
| [hashCode()](#hashCode--) |  |
| [intersect(Range[] ranges)](#intersect-com.aspose.cells.Range---) | يتقاطع مع نطاق آخر. |
| [intersect(UnionRange unionRange)](#intersect-com.aspose.cells.UnionRange-) | يتقاطع مع نطاق آخر. |
| [intersect(String range)](#intersect-java.lang.String-) | يتقاطع مع نطاق آخر. |
| [iterator()](#iterator--) | يحصل على المُعدِّد للخلايا في هذا النطاق. |
| [merge()](#merge--) | يجمع مجموعة من الخلايا في خلية واحدة. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putValue(String stringValue, boolean isConverted, boolean setStyle)](#putValue-java.lang.String-boolean-boolean-) | يضع قيمة في النطاق، إذا كان مناسبًا سيتم تحويل القيمة إلى نوع بيانات آخر وسيتم إعادة ضبط تنسيق الأرقام للخلية. |
| [setName(String value)](#setName-java.lang.String-) | يحدد اسم النطاق. |
| [setOutlineBorders(int borderStyle, Color borderColor)](#setOutlineBorders-int-com.aspose.cells.Color-) | يحدد الحدود الخارجية حول مجموعة من الخلايا بنفس نمط الحد واللون. |
| [setOutlineBorders(int[] borderStyles, Color[] borderColors)](#setOutlineBorders-int---com.aspose.cells.Color---) | يحدد حدودًا خارجية حول مجموعة من الخلايا. |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | يحدد نمط النطاق. |
| [setValue(Object value)](#setValue-java.lang.Object-) | يضبط قيم النطاق. |
| [toString()](#toString--) |  |
| [unMerge()](#unMerge--) | يفك دمج الخلايا المدمجة في هذا النطاق. |
| [union(Range[] ranges)](#union-com.aspose.cells.Range---) | اجمع النطاقات. |
| [union(UnionRange unionRange)](#union-com.aspose.cells.UnionRange-) | اجمع نطاقًا آخر. |
| [union(String range)](#union-java.lang.String-) | اجمع نطاقًا آخر. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


يطبق التنسيقات على نطاق كامل.

**Remarks**

كل خلية في هذا النطاق ستحتوي على كائن [Style](../../com.aspose.cells/style). لذا فإن هذه طريقة مستهلكة للذاكرة. يرجى استخدامها بحذر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | كائن النمط الذي سيتم تطبيقه. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | علامات تشير إلى خصائص التنسيق المطبقة. |

### copy(UnionRange range, PasteOptions options) {#copy-com.aspose.cells.UnionRange-com.aspose.cells.PasteOptions-}
```
public void copy(UnionRange range, PasteOptions options)
```


نسخ النطاق باستخدام خيارات اللصق الخاصة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| range | [UnionRange](../../com.aspose.cells/unionrange) | النطاق المصدر. |
| options | [PasteOptions](../../com.aspose.cells/pasteoptions) | خيارات اللصق الخاصة. |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getCellCount() {#getCellCount--}
```
public int getCellCount()
```


يحصل على عدد جميع الخلايا في النطاق.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


يحصل على عدد الصفوف في النطاق.

**Remarks**

يؤثر فقط عندما يحتوي على نطاق واحد فقط.

**Returns:**
int
### getFirstColumn() {#getFirstColumn--}
```
public int getFirstColumn()
```


يحصل على فهرس العمود الأول في النطاق.

**Remarks**

يؤثر فقط عندما يحتوي على نطاق واحد فقط.

**Returns:**
int
### getFirstRow() {#getFirstRow--}
```
public int getFirstRow()
```


يحصل على فهرس الصف الأول في النطاق.

**Remarks**

يؤثر فقط عندما يحتوي على نطاق واحد فقط.

**Returns:**
int
### getHyperlinks() {#getHyperlinks--}
```
public Hyperlink[] getHyperlinks()
```


يحصل على جميع الروابط التشعبية في النطاق.

**Returns:**
com.aspose.cells.Hyperlink[]
### getName() {#getName--}
```
public String getName()
```


يحصل على اسم النطاق.

**Remarks**

النطاق المسمى مدعوم. على سبيل المثال،

range.Name = "Sheet1!MyRange";

**Returns:**
java.lang.String
### getRangeCount() {#getRangeCount--}
```
public int getRangeCount()
```


يحصل على عدد النطاقات.

**Returns:**
int
### getRanges() {#getRanges--}
```
public Range[] getRanges()
```


يحصل على جميع نطاقات الاتحاد.

**Returns:**
com.aspose.cells.Range[]
### getRefersTo() {#getRefersTo--}
```
public String getRefersTo()
```


يحصل على ما يشير إليه النطاق.

**Returns:**
java.lang.String
### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


يحصل على عدد الصفوف في النطاق.

**Remarks**

يؤثر فقط عندما يحتوي على نطاق واحد فقط.

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


يحصل على قيم النطاق.

**Returns:**
java.lang.Object
### hasRange() {#hasRange--}
```
public boolean hasRange()
```


يشير إلى ما إذا كان لهذا نطاق.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### intersect(Range[] ranges) {#intersect-com.aspose.cells.Range---}
```
public UnionRange intersect(Range[] ranges)
```


يتقاطع مع نطاق آخر.

**Remarks**

إذا لم تتقاطع نطاقا الاتحاد الاثنين، تُرجع null.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| ranges | [Range\[\]](../../com.aspose.cells/range) | النطاق. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange)
### intersect(UnionRange unionRange) {#intersect-com.aspose.cells.UnionRange-}
```
public UnionRange intersect(UnionRange unionRange)
```


يتقاطع مع نطاق آخر.

**Remarks**

إذا لم تتقاطع نطاقا الاتحاد الاثنين، تُرجع null.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| unionRange | [UnionRange](../../com.aspose.cells/unionrange) | النطاق. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange)
### intersect(String range) {#intersect-java.lang.String-}
```
public UnionRange intersect(String range)
```


يتقاطع مع نطاق آخر.

**Remarks**

إذا لم تتقاطع نطاقا الاتحاد الاثنين، تُرجع null.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| نطاق | java.lang.String | النطاق. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange)
### iterator() {#iterator--}
```
public Iterator iterator()
```


يحصل على المُعدِّد للخلايا في هذا النطاق.

**Remarks**

عند تجوال العناصر باستخدام الـ Enumerator المُرجَع، يجب عدم تعديل مجموعة الخلايا (مثل العمليات التي قد تُنشئ خلية/صف جديد أو تحذف خلية/صف موجود). وإلا قد لا يتمكن الـ enumerator من تجوال جميع الخلايا بشكل صحيح (قد يتم تجوال بعض العناصر أكثر من مرة أو يتم تخطيها).

**Returns:**
java.util.Iterator - مُعدِّد الخلايا
### merge() {#merge--}
```
public void merge()
```


يجمع مجموعة من الخلايا في خلية واحدة.

**Remarks**

الإشارة إلى الخلية المدمجة عبر عنوان الخلية العليا اليسرى في النطاق.

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### putValue(String stringValue, boolean isConverted, boolean setStyle) {#putValue-java.lang.String-boolean-boolean-}
```
public void putValue(String stringValue, boolean isConverted, boolean setStyle)
```


يضع قيمة في النطاق، إذا كان مناسبًا سيتم تحويل القيمة إلى نوع بيانات آخر وسيتم إعادة ضبط تنسيق الأرقام للخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stringValue | java.lang.String | قيمة الإدخال |
| isConverted | boolean | True: تم التحويل إلى نوع بيانات آخر إذا كان مناسبًا. |
| setStyle | boolean | True: ضبط تنسيق الرقم على نمط الخلية عند التحويل إلى نوع بيانات آخر |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


يحدد اسم النطاق.

**Remarks**

النطاق المسمى مدعوم. على سبيل المثال،

range.Name = "Sheet1!MyRange";

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setOutlineBorders(int borderStyle, Color borderColor) {#setOutlineBorders-int-com.aspose.cells.Color-}
```
public void setOutlineBorders(int borderStyle, Color borderColor)
```


يحدد الحدود الخارجية حول مجموعة من الخلايا بنفس نمط الحد واللون.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). نمط الحد. |
| borderColor | [Color](../../com.aspose.cells/color) | لون الحد. |

### setOutlineBorders(int[] borderStyles, Color[] borderColors) {#setOutlineBorders-int---com.aspose.cells.Color---}
```
public void setOutlineBorders(int[] borderStyles, Color[] borderColors)
```


يحدد حدودًا خارجية حول مجموعة من الخلايا.

**Remarks**

يجب أن يكون طول كل من borderStyles و borderStyles هو 4. يجب أن يكون ترتيب borderStyles و borderStyles هو الأعلى، الأسفل، اليسار، اليمين.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| borderStyles | int[] | [CellBorderType](../../com.aspose.cells/cellbordertype). أنماط الحد. |
| borderColors | [Color\[\]](../../com.aspose.cells/color) | ألوان الحدود. |

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


يحدد نمط النطاق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | كائن Style. |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


يضبط قيم النطاق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.Object |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### unMerge() {#unMerge--}
```
public void unMerge()
```


يفك دمج الخلايا المدمجة في هذا النطاق.

### union(Range[] ranges) {#union-com.aspose.cells.Range---}
```
public UnionRange union(Range[] ranges)
```


اجمع النطاقات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| ranges | [Range\[\]](../../com.aspose.cells/range) | النطاقات. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - 
### union(UnionRange unionRange) {#union-com.aspose.cells.UnionRange-}
```
public UnionRange union(UnionRange unionRange)
```


اجمع نطاقًا آخر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| unionRange | [UnionRange](../../com.aspose.cells/unionrange) | النطاق. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - 
### union(String range) {#union-java.lang.String-}
```
public UnionRange union(String range)
```


اجمع نطاقًا آخر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| نطاق | java.lang.String | النطاق. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - 
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

