---
title: "VbaModuleCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل قائمة"
type: docs
url: /ar/java/com.aspose.cells/vbamodulecollection/
---

**Inheritance:**
java.lang.Object، [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class VbaModuleCollection extends CollectionBase
```

يمثل قائمة الـ [VbaModule](../../com.aspose.cells/vbamodule)

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
          // Init VBA project.
         VbaProject vbaProject = workbook.getVbaProject(); 
         // Add a new module.
         vbaProject.getModules().add(VbaModuleType.CLASS, "test");
         //Saving the Excel file
         workbook.save("book1.xlsm");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(Worksheet sheet)](#add-com.aspose.cells.Worksheet-) | يضيف وحدة لورقة عمل. |
| [add(int type, String name)](#add-int-java.lang.String-) | يضيف وحدة. |
| [add(Object o)](#add-java.lang.Object-) | يضيف عنصرًا إلى مثيل CollectionBase. |
| [addDesignerStorage(String name, byte[] data)](#addDesignerStorage-java.lang.String-byte---) |  |
| [addUserForm(String name, String codes, byte[] designerStorage)](#addUserForm-java.lang.String-java.lang.String-byte---) | إدراج نموذج مستخدم في مشروع VBA. |
| [clear()](#clear--) | يزيل جميع الكائنات من مثيل CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | إرجاع ما إذا كان المثيل يحتوي على هذا الكائن |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | يحصل على [VbaModule](../../com.aspose.cells/vbamodule) في القائمة حسب الفهرس. |
| [get(String name)](#get-java.lang.String-) | يحصل على [VbaModule](../../com.aspose.cells/vbamodule) في القائمة حسب الاسم. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | يحصل على عدد العناصر الموجودة في مثيل CollectionBase. |
| [getDesignerStorage(String name)](#getDesignerStorage-java.lang.String-) | يمثل بيانات المصمم. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | يحدد فهرس عنصر محدد في مثيل CollectionBase. |
| [iterator()](#iterator--) | يرجع كائن تعداد يتنقل عبر مثيل CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Worksheet sheet)](#remove-com.aspose.cells.Worksheet-) | يزيل وحدة لورقة عمل. |
| [remove(String name)](#remove-java.lang.String-) | إزالة الوحدة حسب الاسم |
| [removeAt(int index)](#removeAt-int-) | يزيل العنصر في الفهرس المحدد. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Worksheet sheet) {#add-com.aspose.cells.Worksheet-}
```
public int add(Worksheet sheet)
```


يضيف وحدة لورقة عمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sheet | [Worksheet](../../com.aspose.cells/worksheet) | ورقة العمل |

**Returns:**
int -
### add(int type, String name) {#add-int-java.lang.String-}
```
public int add(int type, String name)
```


يضيف وحدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [VbaModuleType](../../com.aspose.cells/vbamoduletype). نوع الوحدة. |
| name | java.lang.String | اسم الوحدة. |

**Returns:**
int -
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
### addDesignerStorage(String name, byte[] data) {#addDesignerStorage-java.lang.String-byte---}
```
public void addDesignerStorage(String name, byte[] data)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String |  |
| بيانات | byte[] |  |

### addUserForm(String name, String codes, byte[] designerStorage) {#addUserForm-java.lang.String-java.lang.String-byte---}
```
public int addUserForm(String name, String codes, byte[] designerStorage)
```


إدراج نموذج مستخدم في مشروع VBA.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم نموذج المستخدم |
| الأكواد | java.lang.String | الأكواد لنموذج المستخدم |
| designerStorage | byte[] | إعدادات المصمم المتعلقة بنموذج المستخدم |

**Returns:**
int -
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
public VbaModule get(int index)
```


يحصل على [VbaModule](../../com.aspose.cells/vbamodule) في القائمة حسب الفهرس.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الفهرس. |

**Returns:**
[VbaModule](../../com.aspose.cells/vbamodule) - 
### get(String name) {#get-java.lang.String-}
```
public VbaModule get(String name)
```


يحصل على [VbaModule](../../com.aspose.cells/vbamodule) في القائمة حسب الاسم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم الوحدة. |

**Returns:**
[VbaModule](../../com.aspose.cells/vbamodule) - 
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
### getDesignerStorage(String name) {#getDesignerStorage-java.lang.String-}
```
public byte[] getDesignerStorage(String name)
```


يمثل بيانات المصمم.

**Remarks**

نحن لا ندعم تحليلها. فقط للنسخ.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
byte[]
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




### remove(Worksheet sheet) {#remove-com.aspose.cells.Worksheet-}
```
public void remove(Worksheet sheet)
```


يزيل وحدة لورقة عمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sheet | [Worksheet](../../com.aspose.cells/worksheet) | ورقة العمل |

### remove(String name) {#remove-java.lang.String-}
```
public void remove(String name)
```


إزالة الوحدة حسب الاسم

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String |  |

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

