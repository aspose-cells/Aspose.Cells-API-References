---
title: "ConnectionParameter"
second_title: "Aspose.Cells for Java API Reference"
description: "يحدد الخصائص المتعلقة بأي معلمات تُستخدم مع اتصالات البيانات الخارجية. المعلمات صالحة لـ ODBC واستعلامات الويب."
type: docs
url: /ar/java/com.aspose.cells/connectionparameter/
---

**Inheritance:**
java.lang.Object
```
public class ConnectionParameter
```

يحدد الخصائص المتعلقة بأي معلمات تُستخدم مع اتصالات البيانات الخارجية. المعلمات صالحة لـ ODBC واستعلامات الويب.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCellReference()](#getCellReference--) | إشارة الخلية التي تحدد قيمة الخلية المستخدمة لمعلمة الاستعلام. |
| [getClass()](#getClass--) |  |
| [getName()](#getName--) | اسم المعلمة. |
| [getPrompt()](#getPrompt--) | سلسلة المطالبة للمعلمة. |
| [getRefreshOnChange()](#getRefreshOnChange--) | علامة تشير إلى ما إذا كان يجب تحديث الاستعلام تلقائيًا عندما يتغير محتوى الخلية التي توفر قيمة المعلمة. |
| [getSqlType()](#getSqlType--) | نوع بيانات SQL للمعلمة. |
| [getType()](#getType--) | نوع المعلمة المستخدمة. |
| [getValue()](#getValue--) | قيمة عددية غير صحيحة، قيمة صحيحة، قيمة نصية أو قيمة منطقية لاستخدامها كمعلمة استعلام. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCellReference(String value)](#setCellReference-java.lang.String-) | إشارة الخلية التي تحدد قيمة الخلية المستخدمة لمعلمة الاستعلام. |
| [setName(String value)](#setName-java.lang.String-) | اسم المعلمة. |
| [setPrompt(String value)](#setPrompt-java.lang.String-) | سلسلة المطالبة للمعلمة. |
| [setRefreshOnChange(boolean value)](#setRefreshOnChange-boolean-) | علامة تشير إلى ما إذا كان يجب تحديث الاستعلام تلقائيًا عندما يتغير محتوى الخلية التي توفر قيمة المعلمة. |
| [setSqlType(int value)](#setSqlType-int-) | نوع بيانات SQL للمعلمة. |
| [setType(int value)](#setType-int-) | نوع المعلمة المستخدمة. |
| [setValue(Object value)](#setValue-java.lang.Object-) | قيمة عددية غير صحيحة، قيمة صحيحة، قيمة نصية أو قيمة منطقية لاستخدامها كمعلمة استعلام. |
| [toString()](#toString--) |  |
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
### getCellReference() {#getCellReference--}
```
public String getCellReference()
```


إشارة الخلية التي تحدد قيمة الخلية المستخدمة لمعلمة الاستعلام. تُستخدم فقط عندما يكون parameterType هو cell.

**Returns:**
java.lang.String
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


اسم المعلمة.

**Returns:**
java.lang.String
### getPrompt() {#getPrompt--}
```
public String getPrompt()
```


سلسلة المطالبة للمعلمة. تُعرض على مستخدم الجدول مع واجهة إدخال لجمع قيمة المعلمة قبل تحديث البيانات الخارجية. تُستخدم فقط عندما يكون parameterType = prompt.

**Returns:**
java.lang.String
### getRefreshOnChange() {#getRefreshOnChange--}
```
public boolean getRefreshOnChange()
```


علامة تشير إلى ما إذا كان يجب تحديث الاستعلام تلقائيًا عندما يتغير محتوى الخلية التي توفر قيمة المعلمة. إذا كان true، يتم تحديث البيانات الخارجية باستخدام قيمة المعلمة الجديدة في كل مرة يحدث فيها تغيير. إذا كان false، يتم تحديث البيانات الخارجية فقط عند طلب المستخدم أو عندما يُحدث حدث آخر (مثال: فتح المصنف).

**Returns:**
boolean
### getSqlType() {#getSqlType--}
```
public int getSqlType()
```


نوع بيانات SQL للمعلمة. صالح فقط لمصادر ODBC.

انظر [SqlDataType](../../com.aspose.cells/sqldatatype).

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


نوع المعلمة المستخدمة. إذا كان parameterType=value، فستُستخدم القيمة من boolean أو double أو integer أو string. في هذه الحالة، يُتوقع تحديد أحد \{boolean, double, integer, or string\} فقط.

انظر [ConnectionParameterType](../../com.aspose.cells/connectionparametertype).

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


قيمة عددية غير صحيحة، قيمة صحيحة، قيمة نصية أو قيمة منطقية لاستخدامها كمعلمة استعلام. تُستخدم فقط عندما يكون parameterType هو value.

**Returns:**
java.lang.Object
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




### setCellReference(String value) {#setCellReference-java.lang.String-}
```
public void setCellReference(String value)
```


إشارة الخلية التي تحدد قيمة الخلية المستخدمة لمعلمة الاستعلام. تُستخدم فقط عندما يكون parameterType هو cell.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


اسم المعلمة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setPrompt(String value) {#setPrompt-java.lang.String-}
```
public void setPrompt(String value)
```


سلسلة المطالبة للمعلمة. تُعرض على مستخدم الجدول مع واجهة إدخال لجمع قيمة المعلمة قبل تحديث البيانات الخارجية. تُستخدم فقط عندما يكون parameterType = prompt.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setRefreshOnChange(boolean value) {#setRefreshOnChange-boolean-}
```
public void setRefreshOnChange(boolean value)
```


علامة تشير إلى ما إذا كان يجب تحديث الاستعلام تلقائيًا عندما يتغير محتوى الخلية التي توفر قيمة المعلمة. إذا كان true، يتم تحديث البيانات الخارجية باستخدام قيمة المعلمة الجديدة في كل مرة يحدث فيها تغيير. إذا كان false، يتم تحديث البيانات الخارجية فقط عند طلب المستخدم أو عندما يُحدث حدث آخر (مثال: فتح المصنف).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSqlType(int value) {#setSqlType-int-}
```
public void setSqlType(int value)
```


نوع بيانات SQL للمعلمة. صالح فقط لمصادر ODBC.

انظر [SqlDataType](../../com.aspose.cells/sqldatatype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


نوع المعلمة المستخدمة. إذا كان parameterType=value، فستُستخدم القيمة من boolean أو double أو integer أو string. في هذه الحالة، يُتوقع تحديد أحد \{boolean, double, integer, or string\} فقط.

انظر [ConnectionParameterType](../../com.aspose.cells/connectionparametertype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


قيمة عددية غير صحيحة، قيمة صحيحة، قيمة نصية أو قيمة منطقية لاستخدامها كمعلمة استعلام. تُستخدم فقط عندما يكون parameterType هو value.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.Object |  |

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

