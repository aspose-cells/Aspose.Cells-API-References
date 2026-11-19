---
title: "PivotTableCreateOptions"
second_title: "Aspose.Cells for Java API Reference"
description: "خيارات إنشاء PivotTable جديد."
type: docs
url: /ar/java/com.aspose.cells/pivottablecreateoptions/
---

**Inheritance:**
java.lang.Object
```
public class PivotTableCreateOptions
```

خيارات إنشاء PivotTable جديد.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [PivotTableCreateOptions()](#PivotTableCreateOptions--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getTableName()](#getTableName--) | يحصل على اسم تقرير PivotTable الجديد. |
| [getUseSameSource()](#getUseSameSource--) | يحصل على قيمة تشير إلى ما إذا كان يجب مشاركة مصدر البيانات نفسه مع جداول PivotTable الموجودة. |
| [hashCode()](#hashCode--) |  |
| [isXlsClassic()](#isXlsClassic--) | يحصل على قيمة تشير إلى ما إذا كان يجب إنشاء PivotTable بنمط Excel 97-2003 الكلاسيكي. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setTableName(String value)](#setTableName-java.lang.String-) | يضبط اسم تقرير PivotTable الجديد. |
| [setUseSameSource(boolean value)](#setUseSameSource-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب مشاركة مصدر البيانات نفسه مع جداول PivotTable الموجودة. |
| [setXlsClassic(boolean value)](#setXlsClassic-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب إنشاء PivotTable بنمط Excel 97-2003 الكلاسيكي. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotTableCreateOptions() {#PivotTableCreateOptions--}
```
public PivotTableCreateOptions()
```


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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getTableName() {#getTableName--}
```
public String getTableName()
```


يحصل على اسم تقرير PivotTable الجديد.

**Remarks**

إذا لم يتم الضبط، سيتم تعيين اسم تلقائي.

**Returns:**
java.lang.String
### getUseSameSource() {#getUseSameSource--}
```
public boolean getUseSameSource()
```


يحصل على قيمة تشير إلى ما إذا كان يجب مشاركة مصدر البيانات نفسه مع جداول PivotTable الموجودة. القيمة الافتراضية هي true.

**Remarks**

عند ضبطها على true، يمكن لعدة جداول PivotTable إعادة استخدام مخزن Pivot واحد لتقليل استهلاك الذاكرة.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isXlsClassic() {#isXlsClassic--}
```
public boolean isXlsClassic()
```


يحصل على قيمة تشير إلى ما إذا كان يجب إنشاء PivotTable بنمط Excel 97-2003 الكلاسيكي.

**Remarks**

يستخدم PivotTable الكلاسيكي تخطيطًا وتنسيقًا قديمًا من Excel 97-2003. عندما لا يتم ضبطه صراحةً، يتم تحديد القيمة الافتراضية بناءً على تنسيق ملف دفتر العمل المستهدف.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setTableName(String value) {#setTableName-java.lang.String-}
```
public void setTableName(String value)
```


يضبط اسم تقرير PivotTable الجديد.

**Remarks**

إذا لم يتم الضبط، سيتم تعيين اسم تلقائي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setUseSameSource(boolean value) {#setUseSameSource-boolean-}
```
public void setUseSameSource(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب مشاركة مصدر البيانات نفسه مع جداول PivotTable الموجودة. القيمة الافتراضية هي true.

**Remarks**

عند ضبطها على true، يمكن لعدة جداول PivotTable إعادة استخدام مخزن Pivot واحد لتقليل استهلاك الذاكرة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setXlsClassic(boolean value) {#setXlsClassic-boolean-}
```
public void setXlsClassic(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب إنشاء PivotTable بنمط Excel 97-2003 الكلاسيكي.

**Remarks**

يستخدم PivotTable الكلاسيكي تخطيطًا وتنسيقًا قديمًا من Excel 97-2003. عندما لا يتم ضبطه صراحةً، يتم تحديد القيمة الافتراضية بناءً على تنسيق ملف دفتر العمل المستهدف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

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

