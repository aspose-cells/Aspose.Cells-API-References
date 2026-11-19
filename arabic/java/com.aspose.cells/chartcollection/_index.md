---
title: "ChartCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "يحتوي على مجموعة من الكائنات."
type: docs
url: /ar/java/com.aspose.cells/chartcollection/
---

**Inheritance:**
java.lang.Object، [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ChartCollection extends CollectionBase
```

يحتوي على مجموعة من كائنات [Chart](../../com.aspose.cells/chart).

**Example**

```
         Workbook workbook = new Workbook();
 
         ChartCollection charts = workbook.getWorksheets().get(0).getCharts();
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(byte[] data, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn)](#add-byte---java.lang.String-boolean-int-int-int-int-) | يضيف مخططًا باستخدام قالب مسبق. |
| [add(int type, int topRow, int leftColumn, int bottomRow, int rightColumn)](#add-int-int-int-int-int-) | يضيف مخططًا إلى المجموعة. |
| [add(int type, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn)](#add-int-java.lang.String-boolean-int-int-int-int-) | يضيف مخططًا إلى المجموعة. |
| [add(int type, String dataRange, int topRow, int leftColumn, int rightRow, int bottomColumn)](#add-int-java.lang.String-int-int-int-int-) | يضيف مخططًا إلى المجموعة. |
| [add(Object o)](#add-java.lang.Object-) | يضيف عنصرًا إلى مثيل CollectionBase. |
| [addFloatingChart(int type, int left, int top, int width, int height)](#addFloatingChart-int-int-int-int-int-) | يضيف مخططًا إلى المجموعة. |
| [clear()](#clear--) | امسح جميع المخططات. |
| [contains(Object o)](#contains-java.lang.Object-) | إرجاع ما إذا كان المثيل يحتوي على هذا الكائن |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | يحصل على عنصر [Chart](../../com.aspose.cells/chart) في الفهرس المحدد. |
| [get(String name)](#get-java.lang.String-) | يحصل على المخطط بالاسم. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | يحصل على عدد العناصر الموجودة في مثيل CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | يحدد فهرس عنصر محدد في مثيل CollectionBase. |
| [iterator()](#iterator--) | يرجع كائن تعداد يتنقل عبر مثيل CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Chart chart)](#remove-com.aspose.cells.Chart-) | إزالة المخطط المحدد. |
| [removeAt(int index)](#removeAt-int-) | إزالة مخطط في الفهرس المحدد. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(byte[] data, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn) {#add-byte---java.lang.String-boolean-int-int-int-int-}
```
public int add(byte[] data, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn)
```


يضيف مخططًا باستخدام قالب مسبق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| بيانات | byte[] | بيانات ملف قالب المخطط (.crtx). |
| dataRange | java.lang.String | يحدد نطاق البيانات للمخطط |
| isVertical | boolean | يحدد ما إذا كان سيتم رسم السلسلة من نطاق قيم الخلايا حسب الصف أو حسب العمود. |
| topRow | int | فهرس الصف العلوي الأيسر. |
| leftColumn | int | فهرس العمود العلوي الأيسر. |
| rightRow | int | فهرس الصف السفلي الأيمن. |
| bottomColumn | int | فهرس العمود السفلي الأيمن. |

**Returns:**
int - فهرس كائن [Chart](../../com.aspose.cells/chart).
### add(int type, int topRow, int leftColumn, int bottomRow, int rightColumn) {#add-int-int-int-int-int-}
```
public int add(int type, int topRow, int leftColumn, int bottomRow, int rightColumn)
```


يضيف مخططًا إلى المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [ChartType](../../com.aspose.cells/charttype). نوع المخطط |
| topRow | int | فهرس الصف العلوي الأيسر. |
| leftColumn | int | فهرس العمود العلوي الأيسر. |
| bottomRow | int | فهرس الصف السفلي الأيمن. |
| rightColumn | int | فهرس العمود السفلي الأيمن. |

**Returns:**
int - فهرس كائن [Chart](../../com.aspose.cells/chart).
### add(int type, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn) {#add-int-java.lang.String-boolean-int-int-int-int-}
```
public int add(int type, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn)
```


يضيف مخططًا إلى المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [ChartType](../../com.aspose.cells/charttype). نوع المخطط |
| dataRange | java.lang.String | يحدد نطاق البيانات للمخطط |
| isVertical | boolean | يحدد ما إذا كان سيتم رسم السلسلة من نطاق قيم الخلايا حسب الصف أو حسب العمود. |
| topRow | int | فهرس الصف العلوي الأيسر. |
| leftColumn | int | فهرس العمود العلوي الأيسر. |
| rightRow | int | فهرس الصف السفلي الأيمن. |
| bottomColumn | int | فهرس العمود السفلي الأيمن. |

**Returns:**
int - فهرس كائن [Chart](../../com.aspose.cells/chart).
### add(int type, String dataRange, int topRow, int leftColumn, int rightRow, int bottomColumn) {#add-int-java.lang.String-int-int-int-int-}
```
public int add(int type, String dataRange, int topRow, int leftColumn, int rightRow, int bottomColumn)
```


يضيف مخططًا إلى المجموعة.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهملًا. بدلاً من ذلك، يرجى استخدام خاصية [add(int,String,boolean,int,int,int,int)](../../com.aspose.cells/chartcollection\#add-int-String-boolean-int-int-int-int-). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مايو 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [ChartType](../../com.aspose.cells/charttype). نوع المخطط |
| dataRange | java.lang.String | يحدد نطاق البيانات للمخطط |
| topRow | int | فهرس الصف العلوي الأيسر. |
| leftColumn | int | فهرس العمود العلوي الأيسر. |
| rightRow | int | فهرس الصف السفلي الأيمن. |
| bottomColumn | int | فهرس العمود السفلي الأيمن. |

**Returns:**
int - فهرس كائن [Chart](../../com.aspose.cells/chart).
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
### addFloatingChart(int type, int left, int top, int width, int height) {#addFloatingChart-int-int-int-int-int-}
```
public int addFloatingChart(int type, int left, int top, int width, int height)
```


يضيف مخططًا إلى المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [ChartType](../../com.aspose.cells/charttype). نوع المخطط |
| يسار | int | الإزاحة الأفقية x إلى الزاوية |
| أعلى | int | الإزاحة العمودية y إلى الزاوية |
| العرض | int | عرض المخطط |
| الارتفاع | int | ارتفاع المخطط |

**Returns:**
int - فهرس كائن [Chart](../../com.aspose.cells/chart).
### clear() {#clear--}
```
public void clear()
```


امسح جميع المخططات.

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
public Chart get(int index)
```


يحصل على عنصر [Chart](../../com.aspose.cells/chart) في الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الفهرس الصفري للعنصر. |

**Returns:**
[Chart](../../com.aspose.cells/chart) - The element at the specified index.
### get(String name) {#get-java.lang.String-}
```
public Chart get(String name)
```


يحصل على المخطط بالاسم.

**Remarks**

اسم المخطط الافتراضي هو null. لذلك عليك تعيين اسم المخطط صراحةً.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم المخطط. |

**Returns:**
[Chart](../../com.aspose.cells/chart) - The chart.
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




### remove(Chart chart) {#remove-com.aspose.cells.Chart-}
```
public void remove(Chart chart)
```


إزالة المخطط المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| chart | [Chart](../../com.aspose.cells/chart) |  |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


إزالة مخطط في الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | فهرس المخطط. |

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

