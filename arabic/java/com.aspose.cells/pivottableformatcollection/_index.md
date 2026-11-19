---
title: "PivotTableFormatCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل مجموعة التنسيقات المطبقة على PivotTable."
type: docs
url: /ar/java/com.aspose.cells/pivottableformatcollection/
---

**Inheritance:**
java.lang.Object، [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PivotTableFormatCollection extends CollectionBase
```

يمثل مجموعة التنسيقات المطبقة على PivotTable.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add()](#add--) | أضف [PivotTableFormat](../../com.aspose.cells/pivottableformat). |
| [add(Object o)](#add-java.lang.Object-) | يضيف عنصرًا إلى مثيل CollectionBase. |
| [clear()](#clear--) | يزيل جميع الكائنات من مثيل CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | إرجاع ما إذا كان المثيل يحتوي على هذا الكائن |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [format(CellArea ca, Style style)](#format-com.aspose.cells.CellArea-com.aspose.cells.Style-) | يقوم بتنسيق المنطقة المحددة في PivotTable. |
| [format(PivotArea pivotArea, Style style)](#format-com.aspose.cells.PivotArea-com.aspose.cells.Style-) | يقوم بتنسيق المنطقة المحددة في PivotTable. |
| [format(int row, int column, Style style)](#format-int-int-com.aspose.cells.Style-) | يقوم بتنسيق الخلية في منطقة PivotTable |
| [formatArea(int axisType, int fieldPosition, int subtotalType, int selectionType, boolean isGrandRow, boolean isGrandColumn, Style style)](#formatArea-int-int-int-int-boolean-boolean-com.aspose.cells.Style-) | يقوم بتنسيق المنطقة المحددة. |
| [get(int index)](#get-int-) | يحصل على التنسيق حسب الفهرس. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | يحصل على عدد العناصر الموجودة في مثيل CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | يحدد فهرس عنصر محدد في مثيل CollectionBase. |
| [iterator()](#iterator--) | يرجع كائن تعداد يتنقل عبر مثيل CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | يزيل العنصر في الفهرس المحدد. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add() {#add--}
```
public int add()
```


أضف [PivotTableFormat](../../com.aspose.cells/pivottableformat).

**Returns:**
int - فهرس التنسيق الجديد.
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


يضيف عنصرًا إلى مثيل CollectionBase.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| o | java.lang.Object | الكائن لإضافته إلى مثيل CollectionBase. |

**Returns:**
int - الموضع الذي تم إدراج العنصر الجديد فيه.
### clear() {#clear--}
```
public void clear()
```


يزيل جميع الكائنات من مثيل CollectionBase.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


إرجاع ما إذا كان المثيل يحتوي على هذا الكائن

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| o | java.lang.Object | كائن اختبار |

**Returns:**
boolean - ما إذا كان المثيل يحتوي على هذا الكائن
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
### format(CellArea ca, Style style) {#format-com.aspose.cells.CellArea-com.aspose.cells.Style-}
```
public void format(CellArea ca, Style style)
```


يقوم بتنسيق المنطقة المحددة في PivotTable.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | نطاق الخلايا. |
| style | [Style](../../com.aspose.cells/style) | النمط |

### format(PivotArea pivotArea, Style style) {#format-com.aspose.cells.PivotArea-com.aspose.cells.Style-}
```
public void format(PivotArea pivotArea, Style style)
```


يقوم بتنسيق المنطقة المحددة في PivotTable.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| pivotArea | [PivotArea](../../com.aspose.cells/pivotarea) | منطقة عرض Pivot المحددة. |
| style | [Style](../../com.aspose.cells/style) | الإعداد المنسق. |

### format(int row, int column, Style style) {#format-int-int-com.aspose.cells.Style-}
```
public void format(int row, int column, Style style)
```


يقوم بتنسيق الخلية في منطقة PivotTable

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس الصف للخلية |
| عمود | int | فهرس العمود للخلية |
| style | [Style](../../com.aspose.cells/style) | النمط المستخدم لتنسيق الخلية |

### formatArea(int axisType, int fieldPosition, int subtotalType, int selectionType, boolean isGrandRow, boolean isGrandColumn, Style style) {#formatArea-int-int-int-int-boolean-boolean-com.aspose.cells.Style-}
```
public PivotTableFormat formatArea(int axisType, int fieldPosition, int subtotalType, int selectionType, boolean isGrandRow, boolean isGrandColumn, Style style)
```


يقوم بتنسيق المنطقة المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). المنطقة في PivotTable التي ينطبق عليها هذه القاعدة. |
| fieldPosition | int | موضع الحقل داخل المحور الذي تنطبق عليه هذه القاعدة. |
| subtotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). نوع مرشح الإجمالي الفرعي لحقل المحور. |
| selectionType | int | [PivotTableSelectionType](../../com.aspose.cells/pivottableselectiontype). يشير إلى كيفية تحديد البيانات. |
| isGrandRow | boolean | يشير إلى ما إذا كان يتم اختيار صفوف الإجمالي الكلي. |
| isGrandColumn | boolean | يشير إلى ما إذا كان يتم اختيار أعمدة الإجمالي الكلي. |
| style | [Style](../../com.aspose.cells/style) | النمط الذي يُطبق على منطقة جدول المحور. |

**Returns:**
[PivotTableFormat](../../com.aspose.cells/pivottableformat) - 
### get(int index) {#get-int-}
```
public PivotTableFormat get(int index)
```


يحصل على التنسيق حسب الفهرس.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الفهرس. |

**Returns:**
[PivotTableFormat](../../com.aspose.cells/pivottableformat) - 
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


يحصل على عدد العناصر الموجودة في مثيل CollectionBase.

**Returns:**
int - عدد العناصر الموجودة في مثيل CollectionBase.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


يحدد فهرس عنصر محدد في مثيل CollectionBase.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| o | java.lang.Object | يحدد فهرس عنصر محدد في مثيل CollectionBase. |

**Returns:**
int - فهرس القيمة إذا وجد في القائمة؛ وإلا -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


يرجع كائن تعداد يتنقل عبر مثيل CollectionBase.

**Returns:**
java.util.Iterator - كائن تكرار لمثيل CollectionBase.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


يزيل العنصر في الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الفهرس الصفري للعنصر المراد إزالته. |

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

