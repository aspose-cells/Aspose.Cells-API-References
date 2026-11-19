---
title: "CustomDocumentPropertyCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "مجموعة من خصائص المستند المخصصة."
type: docs
url: /ar/java/com.aspose.cells/customdocumentpropertycollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase), [com.aspose.cells.DocumentPropertyCollection](../../com.aspose.cells/documentpropertycollection)
```
public class CustomDocumentPropertyCollection extends DocumentPropertyCollection
```

مجموعة من خصائص المستند المخصصة.

**Remarks**

كل كائن يمثل خاصية مخصصة لوثيقة الحاوية.

**Example**

```
         //Instantiate a Workbook object
         Workbook workbook = new Workbook("book1.xls");
 
         //Retrieve a list of all custom document properties of the Excel file
         CustomDocumentPropertyCollection customProperties = workbook.getWorksheets().getCustomDocumentProperties();
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | يضيف عنصرًا إلى مثيل CollectionBase. |
| [add(String name, boolean value)](#add-java.lang.String-boolean-) | ينشئ خاصية مستند مخصصة جديدة من نوع البيانات **PropertyType.Boolean**. |
| [add(String name, DateTime value)](#add-java.lang.String-com.aspose.cells.DateTime-) | ينشئ خاصية مستند مخصصة جديدة من نوع البيانات **PropertyType.DateTime**. |
| [add(String name, double value)](#add-java.lang.String-double-) | ينشئ خاصية مستند مخصصة جديدة من نوع البيانات **PropertyType.Float**. |
| [add(String name, int value)](#add-java.lang.String-int-) | ينشئ خاصية مستند مخصصة جديدة من نوع البيانات **PropertyType.Number**. |
| [add(String name, String value)](#add-java.lang.String-java.lang.String-) | ينشئ خاصية مستند مخصصة جديدة من نوع البيانات **PropertyType.String**. |
| [addLinkToContent(String name, String source)](#addLinkToContent-java.lang.String-java.lang.String-) | ينشئ خاصية مستند مخصصة جديدة ترتبط بالمحتوى. |
| [clear()](#clear--) | يزيل جميع الكائنات من مثيل CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | إرجاع ما إذا كان المثيل يحتوي على هذا الكائن |
| [contains(String name)](#contains-java.lang.String-) | يرجع true إذا كان هناك خاصية بالاسم المحدد موجودة في المجموعة. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | يرجع كائن [DocumentProperty](../../com.aspose.cells/documentproperty) حسب الفهرس. |
| [get(String name)](#get-java.lang.String-) | يرجع كائن [DocumentProperty](../../com.aspose.cells/documentproperty) حسب اسم الخاصية. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | يحصل على عدد العناصر الموجودة في مثيل CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | يحدد فهرس عنصر محدد في مثيل CollectionBase. |
| [indexOf(String name)](#indexOf-java.lang.String-) | يحصل على فهرس الخاصية حسب الاسم. |
| [iterator()](#iterator--) | يرجع كائن تعداد يتنقل عبر مثيل CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(String name)](#remove-java.lang.String-) | يزيل خاصية بالاسم المحدد من المجموعة. |
| [removeAt(int index)](#removeAt-int-) | يزيل خاصية عند الفهرس المحدد. |
| [toString()](#toString--) |  |
| [updateLinkedPropertyValue()](#updateLinkedPropertyValue--) | يحدّث قيم جميع الخصائص المخصصة المرتبطة بالمحتوى (استخدم قيمة الخلية للنطاق المرتبط لتحديث قيمة الخاصية المخصصة). |
| [updateLinkedRange()](#updateLinkedRange--) | يحدّث جميع النطاقات المرتبطة بالخصائص المخصصة (استخدم قيمة خاصية المستند المخصصة لتحديث قيمة الخلية للنطاق المرتبط). |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### add(String name, boolean value) {#add-java.lang.String-boolean-}
```
public DocumentProperty add(String name, boolean value)
```


ينشئ خاصية مستند مخصصة جديدة من نوع البيانات **PropertyType.Boolean**.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم الخاصية. |
| القيمة | boolean | قيمة الخاصية. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
### add(String name, DateTime value) {#add-java.lang.String-com.aspose.cells.DateTime-}
```
public DocumentProperty add(String name, DateTime value)
```


ينشئ خاصية مستند مخصصة جديدة من نوع البيانات **PropertyType.DateTime**.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم الخاصية. |
| value | [DateTime](../../com.aspose.cells/datetime) | قيمة الخاصية. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
### add(String name, double value) {#add-java.lang.String-double-}
```
public DocumentProperty add(String name, double value)
```


ينشئ خاصية مستند مخصصة جديدة من نوع البيانات **PropertyType.Float**.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم الخاصية. |
| القيمة | double | قيمة الخاصية. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
### add(String name, int value) {#add-java.lang.String-int-}
```
public DocumentProperty add(String name, int value)
```


ينشئ خاصية مستند مخصصة جديدة من نوع البيانات **PropertyType.Number**.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم الخاصية. |
| القيمة | int | قيمة الخاصية. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
### add(String name, String value) {#add-java.lang.String-java.lang.String-}
```
public DocumentProperty add(String name, String value)
```


ينشئ خاصية مستند مخصصة جديدة من نوع البيانات **PropertyType.String**.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم الخاصية. |
| القيمة | java.lang.String | قيمة الخاصية. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
### addLinkToContent(String name, String source) {#addLinkToContent-java.lang.String-java.lang.String-}
```
public DocumentProperty addLinkToContent(String name, String source)
```


ينشئ خاصية مستند مخصصة جديدة ترتبط بالمحتوى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم الخاصية. |
| المصدر | java.lang.String | مصدر الخاصية. يجب أن يكون اسم النطاق المسمى. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
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
### contains(String name) {#contains-java.lang.String-}
```
public boolean contains(String name)
```


يرجع true إذا كان هناك خاصية بالاسم المحدد موجودة في المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم الخاصية غير حساس لحالة الأحرف. |

**Returns:**
boolean - True إذا كانت الخاصية موجودة في المجموعة؛ false خلاف ذلك.
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
public DocumentProperty get(int index)
```


يرجع كائن [DocumentProperty](../../com.aspose.cells/documentproperty) حسب الفهرس.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| index | int | الفهرس الصفري لـ [DocumentProperty](../../com.aspose.cells/documentproperty) المراد استرجاعه. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty)
### get(String name) {#get-java.lang.String-}
```
public DocumentProperty get(String name)
```


يرجع كائن [DocumentProperty](../../com.aspose.cells/documentproperty) حسب اسم الخاصية.

**Remarks**

يرجع null إذا لم يتم العثور على خاصية بالاسم المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم الخاصية غير حساس لحالة الأحرف المراد استرجاعه. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty)
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
### indexOf(String name) {#indexOf-java.lang.String-}
```
public int indexOf(String name)
```


يحصل على فهرس الخاصية حسب الاسم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم الخاصية غير حساس لحالة الأحرف. |

**Returns:**
int - الفهرس القائم على الصفر. قيمة سالبة إذا لم يتم العثور عليه.
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




### remove(String name) {#remove-java.lang.String-}
```
public void remove(String name)
```


يزيل خاصية بالاسم المحدد من المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم الخاصية غير حساس لحالة الأحرف. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


يزيل خاصية عند الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الفهرس القائم على الصفر. |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### updateLinkedPropertyValue() {#updateLinkedPropertyValue--}
```
public void updateLinkedPropertyValue()
```


يحدّث قيم جميع الخصائص المخصصة المرتبطة بالمحتوى (استخدم قيمة الخلية للنطاق المرتبط لتحديث قيمة الخاصية المخصصة).

### updateLinkedRange() {#updateLinkedRange--}
```
public void updateLinkedRange()
```


يحدّث جميع النطاقات المرتبطة بالخصائص المخصصة (استخدم قيمة خاصية المستند المخصصة لتحديث قيمة الخلية للنطاق المرتبط).

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

