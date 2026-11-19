---
title: "SparklineGroupCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "يحتوي على مجموعة من الكائنات."
type: docs
url: /ar/java/com.aspose.cells/sparklinegroupcollection/
---

**Inheritance:**
java.lang.Object، [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class SparklineGroupCollection extends CollectionBase
```

يحتوي على مجموعة من كائنات [SparklineGroup](../../com.aspose.cells/sparklinegroup).

**Example**

```
         Workbook book = new Workbook(); 
         Worksheet sheet = book.getWorksheets().get(0);
 
         sheet.getCells().get("A1").putValue(5);
         sheet.getCells().get("B1").putValue(2);
         sheet.getCells().get("C1").putValue(1);
         sheet.getCells().get("D1").putValue(3);
 
         // Define the CellArea
         CellArea ca = new CellArea();
         ca.StartColumn = 4;
         ca.EndColumn = 4;
         ca.StartRow = 0;
         ca.EndRow = 0;
 
         int idx = sheet.getSparklineGroups().add(com.aspose.cells.SparklineType.LINE, "A1:D1", false, ca);
         SparklineGroup group = sheet.getSparklineGroups().get(idx);
         group.getSparklines().add(sheet.getName() + "!A1:D1", 0, 4);
         book.save("output.xlsx", SaveFormat.XLSX);
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(int type)](#add-int-) | يضيف [SparklineGroup](../../com.aspose.cells/sparklinegroup) مع [Sparkline](../../com.aspose.cells/sparkline) إلى المجموعة. |
| [add(int type, String dataRange, boolean isVertical, CellArea locationRange)](#add-int-java.lang.String-boolean-com.aspose.cells.CellArea-) | يضيف [SparklineGroup](../../com.aspose.cells/sparklinegroup) مع بعض [Sparkline](../../com.aspose.cells/sparkline) إلى المجموعة. |
| [add(Object o)](#add-java.lang.Object-) | يضيف عنصرًا إلى مثيل CollectionBase. |
| [clear()](#clear--) | يزيل جميع الكائنات من مثيل CollectionBase. |
| [clearSparklineGroups(CellArea cellArea)](#clearSparklineGroups-com.aspose.cells.CellArea-) | يمسح مجموعات sparkline التي تتداخل مع منطقة من الخلايا. |
| [clearSparklines(CellArea cellArea)](#clearSparklines-com.aspose.cells.CellArea-) | يمسح sparklines الموجودة داخل منطقة من الخلايا. |
| [contains(Object o)](#contains-java.lang.Object-) | إرجاع ما إذا كان المثيل يحتوي على هذا الكائن |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | يحصل على عنصر [SparklineGroup](../../com.aspose.cells/sparklinegroup) في الفهرس المحدد. |
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
### add(int type) {#add-int-}
```
public int add(int type)
```


يضيف [SparklineGroup](../../com.aspose.cells/sparklinegroup) مع [Sparkline](../../com.aspose.cells/sparkline) إلى المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [SparklineType](../../com.aspose.cells/sparklinetype). يحدد نوع مجموعة Sparkline. |

**Returns:**
int - فهرس كائن [SparklineGroup](../../com.aspose.cells/sparklinegroup).
### add(int type, String dataRange, boolean isVertical, CellArea locationRange) {#add-int-java.lang.String-boolean-com.aspose.cells.CellArea-}
```
public int add(int type, String dataRange, boolean isVertical, CellArea locationRange)
```


يضيف [SparklineGroup](../../com.aspose.cells/sparklinegroup) مع بعض [Sparkline](../../com.aspose.cells/sparkline) إلى المجموعة.

**Remarks**

هذه الطريقة ستنشئ sparklines أيضًا. إذا كان  صحيحًا، يجب أن يكون عدد الصفوف في dataRange و locationRange متساويًا. إذا كان  خاطئًا، يجب أن يكون عدد الأعمدة في dataRange و locationRange متساويًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [SparklineType](../../com.aspose.cells/sparklinetype). يحدد نوع مجموعة Sparkline. |
| dataRange | java.lang.String | يحدد نطاق البيانات لمجموعة sparkline. |
| isVertical | boolean | يحدد ما إذا كان سيتم رسم sparklines من نطاق البيانات حسب الصف أو حسب العمود. |
| locationRange | [CellArea](../../com.aspose.cells/cellarea) | يحدد مكان وضع الخطوط الصغيرة. |

**Returns:**
int - فهرس كائن [SparklineGroup](../../com.aspose.cells/sparklinegroup).
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

### clearSparklineGroups(CellArea cellArea) {#clearSparklineGroups-com.aspose.cells.CellArea-}
```
public void clearSparklineGroups(CellArea cellArea)
```


يمسح مجموعات sparkline التي تتداخل مع منطقة من الخلايا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | يحدد منطقة الخلايا |

### clearSparklines(CellArea cellArea) {#clearSparklines-com.aspose.cells.CellArea-}
```
public void clearSparklines(CellArea cellArea)
```


يمسح sparklines الموجودة داخل منطقة من الخلايا.

**Remarks**

[SparklineGroup](../../com.aspose.cells/sparklinegroup) will be removed too if it does not contains any [Sparkline](../../com.aspose.cells/sparkline).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | يحدد منطقة الخلايا |

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
### get(int index) {#get-int-}
```
public SparklineGroup get(int index)
```


يحصل على عنصر [SparklineGroup](../../com.aspose.cells/sparklinegroup) في الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الفهرس الصفري للعنصر. |

**Returns:**
[SparklineGroup](../../com.aspose.cells/sparklinegroup) - The element at the specified index.
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

