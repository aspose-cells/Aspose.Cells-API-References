---
title: "GridValidationCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "يحتوي على مجموعة من الكائنات."
type: docs
url: /ar/java/com.aspose.gridweb/gridvalidationcollection/
---

**Inheritance:**
java.lang.Object
```
public class GridValidationCollection
```

يحتوي على مجموعة من كائنات [GridValidation](../../com.aspose.gridweb/gridvalidation).
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add()](#add--) | أضف [GridValidation](../../com.aspose.gridweb/gridvalidation) إلى المجموعة. |
| [add(GridCellArea ca)](#add-com.aspose.gridweb.GridCellArea-) | يضيف تحققًا من البيانات إلى المجموعة. |
| [add(GridValidation validation)](#add-com.aspose.gridweb.GridValidation-) | أضف [GridValidation](../../com.aspose.gridweb/gridvalidation) إلى المجموعة. |
| [add(int row, int column)](#add-int-int-) | أضف [GridValidation](../../com.aspose.gridweb/gridvalidation) إلى المجموعة. يتم تطبيق التحقق على الخلية المحددة. |
| [add(String cellname)](#add-java.lang.String-) | أضف [GridValidation](../../com.aspose.gridweb/gridvalidation) إلى المجموعة. يتم تطبيق التحقق على الخلية المحددة. |
| [clear()](#clear--) | يمسح جميع عمليات التحقق. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | يحصل على عنصر [GridValidation](../../com.aspose.gridweb/gridvalidation) في الفهرس المحدد. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | يحصل على حجم المُعدد |
| [getValidationInCell(int row, int column)](#getValidationInCell-int-int-) | يحصل على التحقق المطبق على الخلية المعطاة. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | إزالة التحقق في الفهرس المحدد. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add() {#add--}
```
public GridValidation add()
```


أضف [GridValidation](../../com.aspose.gridweb/gridvalidation) إلى المجموعة.

**Remarks**

ملاحظة: هذا العضو أصبح الآن غير صالح. بدلاً من ذلك، يرجى استخدام طريقة GridValidationCollection.Add(row,col). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يناير 2015. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - [GridValidation](../../com.aspose.gridweb/gridvalidation) the added GridValidation instance.
### add(GridCellArea ca) {#add-com.aspose.gridweb.GridCellArea-}
```
public GridValidation add(GridCellArea ca)
```


يضيف تحققًا من البيانات إلى المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| ca | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | المنطقة التي تحتوي على هذا التحقق. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - [GridValidation](../../com.aspose.gridweb/gridvalidation) the validation.
### add(GridValidation validation) {#add-com.aspose.gridweb.GridValidation-}
```
public int add(GridValidation validation)
```


أضف [GridValidation](../../com.aspose.gridweb/gridvalidation) إلى المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| validation | [GridValidation](../../com.aspose.gridweb/gridvalidation) | كائن تحقق. |

**Returns:**
int - فهرس كائن [GridValidation](../../com.aspose.gridweb/gridvalidation).
### add(int row, int column) {#add-int-int-}
```
public GridValidation add(int row, int column)
```


أضف [GridValidation](../../com.aspose.gridweb/gridvalidation) إلى المجموعة. يتم تطبيق التحقق على الخلية المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | The row index. |
| عمود | int | The column index. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - [GridValidation](../../com.aspose.gridweb/gridvalidation) the added GridValidation instance.
### add(String cellname) {#add-java.lang.String-}
```
public GridValidation add(String cellname)
```


أضف [GridValidation](../../com.aspose.gridweb/gridvalidation) إلى المجموعة. يتم تطبيق التحقق على الخلية المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cellname | java.lang.String | اسم الخلية. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - [GridValidation](../../com.aspose.gridweb/gridvalidation) the added GridValidation instance.
### clear() {#clear--}
```
public void clear()
```


يمسح جميع عمليات التحقق.

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
public GridValidation get(int index)
```


يحصل على عنصر [GridValidation](../../com.aspose.gridweb/gridvalidation) في الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الفهرس الصفري للعنصر. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - The element at the specified index.
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


يحصل على حجم المُعدد

**Returns:**
int
### getValidationInCell(int row, int column) {#getValidationInCell-int-int-}
```
public GridValidation getValidationInCell(int row, int column)
```


يحصل على التحقق المطبق على الخلية المعطاة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | The row index. |
| عمود | int | The column index. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - Returns a [GridValidation](../../com.aspose.gridweb/gridvalidation) object or null if there is no validation for given cell
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
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


إزالة التحقق في الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الفهرس الصفري للعنصر. |

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

