---
title: "DocumentProperty"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل خاصية مستند مخصصة أو مدمجة."
type: docs
url: /ar/java/com.aspose.cells/documentproperty/
---

**Inheritance:**
java.lang.Object
```
public class DocumentProperty
```

يمثل خاصية مستند مخصصة أو مدمجة.

**Example**

```
         //Instantiate a Workbook object
         Workbook workbook = new Workbook("book1.xls");
 
         //Retrieve a list of all custom document properties of the Excel file
         DocumentPropertyCollection customProperties = workbook.getWorksheets().getCustomDocumentProperties();
 
         //Accessng a custom document property by using the property index
         DocumentProperty customProperty1 = customProperties.get(3);
 
         //Accessng a custom document property by using the property name
         DocumentProperty customProperty2 = customProperties.get("Owner");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getName()](#getName--) | يعيد اسم الخاصية. |
| [getSource()](#getSource--) | مصدر المحتوى المرتبط. |
| [getType()](#getType--) | يحصل على نوع البيانات للخاصية. |
| [getValue()](#getValue--) | يحصل على قيمة الخاصية. |
| [hashCode()](#hashCode--) |  |
| [isGeneratedName()](#isGeneratedName--) | يعيد true إذا لم يكن لهذه الخاصية اسم في تخزين OLE2 وتم إنشاء اسم فريد فقط لواجهة برمجة التطبيقات العامة. |
| [isLinkedToContent()](#isLinkedToContent--) | يشير إلى ما إذا كانت هذه الخاصية مرتبطة بالمحتوى |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setValue(Object value)](#setValue-java.lang.Object-) | يضبط قيمة الخاصية. |
| [toBool()](#toBool--) | يعيد قيمة الخاصية كقيمة منطقية (bool). |
| [toDateTime()](#toDateTime--) | يعيد قيمة الخاصية كـ DateTime في المنطقة الزمنية المحلية. |
| [toDouble()](#toDouble--) | يعيد قيمة الخاصية كـ double. |
| [toInt()](#toInt--) | يعيد قيمة الخاصية كـ integer. |
| [toString()](#toString--) | يعيد قيمة الخاصية كسلسلة. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getName() {#getName--}
```
public String getName()
```


يعيد اسم الخاصية.

**Returns:**
java.lang.String
### getSource() {#getSource--}
```
public String getSource()
```


مصدر المحتوى المرتبط.

**Returns:**
java.lang.String
### getType() {#getType--}
```
public int getType()
```


يحصل على نوع البيانات للخاصية.

انظر [PropertyType](../../com.aspose.cells/propertytype).

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


يحصل على قيمة الخاصية.

**Returns:**
java.lang.Object
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isGeneratedName() {#isGeneratedName--}
```
public boolean isGeneratedName()
```


يعيد true إذا لم يكن لهذه الخاصية اسم في تخزين OLE2 وتم إنشاء اسم فريد فقط لواجهة برمجة التطبيقات العامة.

**Returns:**
boolean
### isLinkedToContent() {#isLinkedToContent--}
```
public boolean isLinkedToContent()
```


يشير إلى ما إذا كانت هذه الخاصية مرتبطة بالمحتوى

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




### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


يضبط قيمة الخاصية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.Object |  |

### toBool() {#toBool--}
```
public boolean toBool()
```


يعيد قيمة الخاصية كقيمة منطقية (bool).

**Remarks**

يرمي استثناءً إذا لم يكن نوع الخاصية PropertyType.Boolean.

**Returns:**
boolean
### toDateTime() {#toDateTime--}
```
public DateTime toDateTime()
```


يعيد قيمة الخاصية كـ DateTime في المنطقة الزمنية المحلية.

**Remarks**

يرمي استثناءً إذا لم يكن نوع الخاصية PropertyType.Date.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### toDouble() {#toDouble--}
```
public double toDouble()
```


يعيد قيمة الخاصية كـ double.

**Remarks**

يرمي استثناءً إذا لم يكن نوع الخاصية PropertyType.Float.

**Returns:**
double
### toInt() {#toInt--}
```
public int toInt()
```


يعيد قيمة الخاصية كـ integer.

**Remarks**

يرمي استثناءً إذا لم يكن نوع الخاصية PropertyType.Number.

**Returns:**
int
### toString() {#toString--}
```
public String toString()
```


يعيد قيمة الخاصية كسلسلة.

**Remarks**

يقوم بتحويل خاصية رقمية باستخدام Object.ToString(). يحول خاصية منطقية إلى "Y" أو "N". يحول خاصية تاريخ إلى سلسلة تاريخ قصيرة.

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

