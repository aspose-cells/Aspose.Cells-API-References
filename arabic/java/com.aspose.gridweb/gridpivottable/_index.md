---
title: "GridPivotTable"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل تقرير PivotTable على ورقة العمل."
type: docs
url: /ar/java/com.aspose.gridweb/gridpivottable/
---

**Inheritance:**
java.lang.Object
```
public class GridPivotTable
```

يمثل تقرير PivotTable على ورقة عمل. كائن PivotTable هو عضو في مجموعة [GridPivotTable](../../com.aspose.gridweb/gridpivottable). مجموعة PivotTables تحتوي على جميع كائنات PivotTable على عنصر التحكم.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [addFieldToArea(int fieldType, int baseFieldIndex)](#addFieldToArea-int-int-) | يضيف الحقل إلى المنطقة المحددة. |
| [addFieldToArea(int fieldType, String fieldName)](#addFieldToArea-int-java.lang.String-) | يضيف الحقل إلى المنطقة المحددة. |
| [calculateData()](#calculateData--) | يحسب بيانات pivottable إلى الخلايا. |
| [clearAllFields()](#clearAllFields--) | مسح جميع حقول pivot. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [fields(int fieldType)](#fields-int-) | يحصل على الحقول المحددة حسب نوع الحقل. |
| [fields(String fieldName)](#fields-java.lang.String-) | يحصل على الحقل المحدد باسم الحقل. |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshData()](#refreshData--) | يقوم بتحديث بيانات pivottable وإعداداته من مصدر البيانات الخاص به. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addFieldToArea(int fieldType, int baseFieldIndex) {#addFieldToArea-int-int-}
```
public int addFieldToArea(int fieldType, int baseFieldIndex)
```


يضيف الحقل إلى المنطقة المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldType | int | [GridPivotFieldType](../../com.aspose.gridweb/gridpivotfieldtype). نوع مساحة الحقول. |
| baseFieldIndex | int | فهرس الحقل في الحقول الأساسية. |

**Returns:**
int - موضع الحقل في الحقول المحددة.
### addFieldToArea(int fieldType, String fieldName) {#addFieldToArea-int-java.lang.String-}
```
public int addFieldToArea(int fieldType, String fieldName)
```


يضيف الحقل إلى المنطقة المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldType | int | [GridPivotFieldType](../../com.aspose.gridweb/gridpivotfieldtype). نوع مساحة الحقول. |
| fieldName | java.lang.String | الاسم في الحقول الأساسية. |

**Returns:**
int - موضع الحقل في الحقول المحددة. إذا لم يكن هناك حقل يحمل هذا الاسم، أعد -1.
### calculateData() {#calculateData--}
```
public void calculateData()
```


يحسب بيانات pivottable إلى الخلايا.

**Remarks**

قد لا تُعيد Cell.Value في نطاق pivot النتيجة الصحيحة إذا لم يتم استدعاء الطريقة. هذه الطريقة تحسب البيانات باستخدام ذاكرة تخزين مؤقت داخلية للـ pivot، وليس مصدر البيانات الأصلي. لذا إذا تم تغيير مصدر البيانات، يرجى استدعاء طريقة RefreshData() أولاً.

### clearAllFields() {#clearAllFields--}
```
public void clearAllFields()
```


مسح جميع حقول pivot.

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
### fields(int fieldType) {#fields-int-}
```
public GridPivotFieldCollection fields(int fieldType)
```


يحصل على الحقول المحددة حسب نوع الحقل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldType | int | [GridPivotFieldType](../../com.aspose.gridweb/gridpivotfieldtype). نوع الحقل. |

**Returns:**
[GridPivotFieldCollection](../../com.aspose.gridweb/gridpivotfieldcollection) - the specific fields
### fields(String fieldName) {#fields-java.lang.String-}
```
public GridPivotField fields(String fieldName)
```


يحصل على الحقل المحدد باسم الحقل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldName | java.lang.String | اسم الحقل. |

**Returns:**
[GridPivotField](../../com.aspose.gridweb/gridpivotfield) - the specific field
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
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




### refreshData() {#refreshData--}
```
public void refreshData()
```


يقوم بتحديث بيانات pivottable وإعداداته من مصدر البيانات الخاص به.

**Remarks**

سنقوم بجمع البيانات من مصدر البيانات إلى ذاكرة تخزين مؤقت للـ pivot، ثم حساب البيانات في الذاكرة إلى الخلايا. تُستخدم هذه الطريقة فقط لجمع جميع البيانات إلى ذاكرة تخزين مؤقت للـ pivot.

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

