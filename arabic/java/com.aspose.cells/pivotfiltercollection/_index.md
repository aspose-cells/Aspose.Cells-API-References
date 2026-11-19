---
title: "PivotFilterCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل مجموعة جميع PivotFilters."
type: docs
url: /ar/java/com.aspose.cells/pivotfiltercollection/
---

**Inheritance:**
java.lang.Object، [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PivotFilterCollection extends CollectionBase
```

يمثل مجموعة جميع PivotFilters.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(int fieldIndex, int type)](#add-int-int-) | يضيف كائن PivotFilter إلى النوع المحدد |
| [add(Object o)](#add-java.lang.Object-) | يضيف عنصرًا إلى مثيل CollectionBase. |
| [addDateFilter(int baseFieldIndex, int type, DateTime dateTime1, DateTime dateTime2)](#addDateFilter-int-int-com.aspose.cells.DateTime-com.aspose.cells.DateTime-) | يفلتر حسب إعداد التاريخ لحقل محور الصف أو العمود. |
| [addLabelFilter(int baseFieldIndex, int type, String label1, String label2)](#addLabelFilter-int-int-java.lang.String-java.lang.String-) | يفلتر حسب عناوين حقل محور الصف أو العمود. |
| [addTop10Filter(int baseFieldIndex, int valueFieldIndex, int type, boolean isTop, int itemCount)](#addTop10Filter-int-int-int-boolean-int-) | يفلتر حسب قيم حقل محور البيانات. |
| [addValueFilter(int baseFieldIndex, int valueFieldIndex, int type, double value1, double value2)](#addValueFilter-int-int-int-double-double-) | يفلتر حسب قيم حقل محور البيانات. |
| [clear()](#clear--) | يزيل جميع الكائنات من مثيل CollectionBase. |
| [clearFilter(int fieldIndex)](#clearFilter-int-) | امسح PivotFilter من حقل PivotField المحدد |
| [contains(Object o)](#contains-java.lang.Object-) | إرجاع ما إذا كان المثيل يحتوي على هذا الكائن |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | يسترجع كائن pivotfilter في الفهرس المحدد. |
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
### add(int fieldIndex, int type) {#add-int-int-}
```
public int add(int fieldIndex, int type)
```


يضيف كائن PivotFilter إلى النوع المحدد

**Remarks**

ملاحظة: هذه الطريقة الآن مهجورة. بدلاً من ذلك، يرجى استخدام طرق PivotFilterCollection.AddValueFilter()،AddTop10Filter()،AddLabelFilter() وAddDateFilter(). سيتم إزالة هذه الطريقة بعد 12 شهرًا اعتبارًا من نوفمبر 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldIndex | int | فهرس PivotField |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). نوع PivotFilter |

**Returns:**
int - فهرس كائن PivotFilter في هذه PivotFilterCollection.
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
### addDateFilter(int baseFieldIndex, int type, DateTime dateTime1, DateTime dateTime2) {#addDateFilter-int-int-com.aspose.cells.DateTime-com.aspose.cells.DateTime-}
```
public PivotFilter addDateFilter(int baseFieldIndex, int type, DateTime dateTime1, DateTime dateTime2)
```


يفلتر حسب إعداد التاريخ لحقل محور الصف أو العمود.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| baseFieldIndex | int | فهرس الحقل في المصدر. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). نوع تصفية البيانات. |
| dateTime1 | [DateTime](../../com.aspose.cells/datetime) | تسمية التاريخ لشرط الفلترة |
| dateTime2 | [DateTime](../../com.aspose.cells/datetime) | تسمية التاريخ الحد الأعلى لشرط الفلترة بين |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### addLabelFilter(int baseFieldIndex, int type, String label1, String label2) {#addLabelFilter-int-int-java.lang.String-java.lang.String-}
```
public PivotFilter addLabelFilter(int baseFieldIndex, int type, String label1, String label2)
```


يفلتر حسب عناوين حقل محور الصف أو العمود.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| baseFieldIndex | int | فهرس الحقل في المصدر. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). نوع تصفية البيانات. |
| label1 | java.lang.String | تسمية شرط الفلترة |
| label2 | java.lang.String | العلامة العليا لشرط الفلتر بين |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### addTop10Filter(int baseFieldIndex, int valueFieldIndex, int type, boolean isTop, int itemCount) {#addTop10Filter-int-int-int-boolean-int-}
```
public PivotFilter addTop10Filter(int baseFieldIndex, int valueFieldIndex, int type, boolean isTop, int itemCount)
```


يفلتر حسب قيم حقل محور البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| baseFieldIndex | int | فهرس الحقل في المصدر. |
| valueFieldIndex | int | فهرس حقل البيانات في منطقة البيانات. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). نوع تصفية البيانات. يمكن أن يكون فقط Count,Sum و Percent. |
| isTop | boolean | يشير إلى ما إذا كان الفلتر من الأعلى أو الأسفل |
| itemCount | int | عدد العناصر |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### addValueFilter(int baseFieldIndex, int valueFieldIndex, int type, double value1, double value2) {#addValueFilter-int-int-int-double-double-}
```
public PivotFilter addValueFilter(int baseFieldIndex, int valueFieldIndex, int type, double value1, double value2)
```


يفلتر حسب قيم حقل محور البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| baseFieldIndex | int | فهرس الحقل في المصدر. |
| valueFieldIndex | int | فهرس حقل القيمة في منطقة القيمة. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). نوع تصفية البيانات. |
| value1 | double | قيمة شرط الفلتر |
| value2 | double | القيمة العليا لشرط الفلتر بين |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### clear() {#clear--}
```
public void clear()
```


يزيل جميع الكائنات من مثيل CollectionBase.

### clearFilter(int fieldIndex) {#clearFilter-int-}
```
public void clearFilter(int fieldIndex)
```


امسح PivotFilter من حقل PivotField المحدد

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldIndex | int | فهرس PivotField |

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
public PivotFilter get(int index)
```


يسترجع كائن pivotfilter في الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int |  |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
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

