---
title: "ValidationCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل مجموعة التحقق من صحة البيانات."
type: docs
url: /ar/java/com.aspose.cells/validationcollection/
---

**Inheritance:**
java.lang.Object، [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ValidationCollection extends CollectionBase
```

يمثل مجموعة التحقق من صحة البيانات.

**Example**

```
         Workbook workbook = new Workbook();
         	ValidationCollection validations = workbook.getWorksheets().get(0).getValidations();
         CellArea area = CellArea.createCellArea(0, 0, 1, 1);
         Validation validation = validations.get(validations.add(area));
         validation.setType(com.aspose.cells.ValidationType.LIST);
         validation.setFormula1("a,b,c,d");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add()](#add--) | يضيف تحققًا من البيانات إلى المجموعة. |
| [add(CellArea ca)](#add-com.aspose.cells.CellArea-) | يضيف تحققًا من البيانات إلى المجموعة. |
| [add(Object o)](#add-java.lang.Object-) | يضيف عنصرًا إلى مثيل CollectionBase. |
| [clear()](#clear--) | يزيل جميع الكائنات من مثيل CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | إرجاع ما إذا كان المثيل يحتوي على هذا الكائن |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | يحصل على عنصر [Validation](../../com.aspose.cells/validation) في الفهرس المحدد. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | يحصل على عدد العناصر الموجودة في مثيل CollectionBase. |
| [getValidationInCell(int row, int column)](#getValidationInCell-int-int-) | يحصل على التحقق المطبق على الخلية المعطاة. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | يحدد فهرس عنصر محدد في مثيل CollectionBase. |
| [iterator()](#iterator--) | يرجع كائن تعداد يتنقل عبر مثيل CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeACell(int row, int column)](#removeACell-int-int-) | يزيل جميع إعدادات التحقق على الخلية. |
| [removeArea(CellArea ca)](#removeArea-com.aspose.cells.CellArea-) | يزيل جميع إعدادات التحقق على النطاق.. |
| [removeAt(int index)](#removeAt-int-) | يزيل العنصر في الفهرس المحدد. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add() {#add--}
```
public int add()
```


يضيف تحققًا من البيانات إلى المجموعة.

**Remarks**

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة ValidationCollection.Add(CellArea). سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ يناير 2015. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
int - فهرس كائن [Validation](../../com.aspose.cells/validation).
### add(CellArea ca) {#add-com.aspose.cells.CellArea-}
```
public int add(CellArea ca)
```


يضيف تحققًا من البيانات إلى المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | المنطقة التي تحتوي على هذا التحقق. |

**Returns:**
int - فهرس كائن [Validation](../../com.aspose.cells/validation).
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
### get(int index) {#get-int-}
```
public Validation get(int index)
```


يحصل على عنصر [Validation](../../com.aspose.cells/validation) في الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الفهرس الصفري للعنصر. |

**Returns:**
[Validation](../../com.aspose.cells/validation) - The element at the specified index.
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
### getValidationInCell(int row, int column) {#getValidationInCell-int-int-}
```
public Validation getValidationInCell(int row, int column)
```


يحصل على التحقق المطبق على الخلية المعطاة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | The row index. |
| عمود | int | The column index. |

**Returns:**
[Validation](../../com.aspose.cells/validation) - Returns a [Validation](../../com.aspose.cells/validation) object or null if there is no validation for given cell
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




### removeACell(int row, int column) {#removeACell-int-int-}
```
public void removeACell(int row, int column)
```


يزيل جميع إعدادات التحقق على الخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس الصف للخلية. |
| عمود | int | فهرس العمود للخلية. |

### removeArea(CellArea ca) {#removeArea-com.aspose.cells.CellArea-}
```
public void removeArea(CellArea ca)
```


يزيل جميع إعدادات التحقق على النطاق..

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | النطاق الذي يحتوي على إعدادات التحقق. |

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

