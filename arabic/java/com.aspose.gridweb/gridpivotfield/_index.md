---
title: "GridPivotField"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل حقلًا في تقرير جدول المحور."
type: docs
url: /ar/java/com.aspose.gridweb/gridpivotfield/
---

**Inheritance:**
java.lang.Object
```
public class GridPivotField
```

يمثل حقلًا في تقرير جدول المحور.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDisplayName()](#getDisplayName--) | يمثل اسم العرض لحقل PivotField. |
| [getFunction()](#getFunction--) | يمثل الدالة المستخدمة لتلخيص حقل بيانات PivotTable. |
| [getPosition()](#getPosition--) | يمثل فهرس PivotField في PivotFields. |
| [hashCode()](#hashCode--) |  |
| [hideItem(int index, boolean isHidden)](#hideItem-int-boolean-) | يحدد ما إذا كان PivotItem المحدد في حقل البيانات مخفيًا. |
| [hideItemByName(String name, boolean isHidden)](#hideItemByName-java.lang.String-boolean-) | يحدد ما إذا كان PivotItem المحدد في حقل البيانات مخفيًا. |
| [hideItemByValue(String value, boolean isHidden)](#hideItemByValue-java.lang.String-boolean-) | يحدد ما إذا كان PivotItem المحدد في حقل البيانات مخفيًا. |
| [isAscendSort()](#isAscendSort--) | يشير إلى ما إذا كان حقل PivotTable المحدد يتم فرزه تلقائيًا تصاعديًا. |
| [isAutoSort()](#isAutoSort--) | يشير إلى ما إذا كان حقل PivotTable المحدد يتم فرزه تلقائيًا. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAscendSort(boolean value)](#setAscendSort-boolean-) | يشير إلى ما إذا كان حقل PivotTable المحدد يتم فرزه تلقائيًا تصاعديًا. |
| [setAutoSort(boolean value)](#setAutoSort-boolean-) | يشير إلى ما إذا كان حقل PivotTable المحدد يتم فرزه تلقائيًا. |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | يمثل اسم العرض لحقل PivotField. |
| [setFunction(int value)](#setFunction-int-) | يمثل الدالة المستخدمة لتلخيص حقل بيانات PivotTable. |
| [setPosition(int value)](#setPosition-int-) | يمثل فهرس PivotField في PivotFields. |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


يمثل اسم العرض لحقل PivotField.

**Returns:**
java.lang.String
### getFunction() {#getFunction--}
```
public int getFunction()
```


يمثل الدالة المستخدمة لتلخيص حقل بيانات PivotTable.

انظر [GridPivotFieldFunction](../../com.aspose.gridweb/gridpivotfieldfunction).

**Returns:**
int
### getPosition() {#getPosition--}
```
public int getPosition()
```


يمثل فهرس PivotField في PivotFields.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### hideItem(int index, boolean isHidden) {#hideItem-int-boolean-}
```
public void hideItem(int index, boolean isHidden)
```


يحدد ما إذا كان PivotItem المحدد في حقل البيانات مخفيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | فهرس الـ pivotItem في الـ pivotField. |
| isHidden | boolean | ما إذا كان PivotItem المحدد مخفيًا |

### hideItemByName(String name, boolean isHidden) {#hideItemByName-java.lang.String-boolean-}
```
public void hideItemByName(String name, boolean isHidden)
```


يحدد ما إذا كان PivotItem المحدد في حقل البيانات مخفيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم الـpivotItem في الـpivotField. |
| isHidden | boolean | ما إذا كان PivotItem المحدد مخفيًا |

### hideItemByValue(String value, boolean isHidden) {#hideItemByValue-java.lang.String-boolean-}
```
public void hideItemByValue(String value, boolean isHidden)
```


يحدد ما إذا كان PivotItem المحدد في حقل البيانات مخفيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | قيمة الـpivotItem في الـpivotField. |
| isHidden | boolean | ما إذا كان PivotItem المحدد مخفيًا |

### isAscendSort() {#isAscendSort--}
```
public boolean isAscendSort()
```


يشير إلى ما إذا كان حقل PivotTable المحدد يتم فرزه تلقائيًا تصاعديًا.

**Returns:**
boolean
### isAutoSort() {#isAutoSort--}
```
public boolean isAutoSort()
```


يشير إلى ما إذا كان حقل PivotTable المحدد يتم فرزه تلقائيًا.

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




### setAscendSort(boolean value) {#setAscendSort-boolean-}
```
public void setAscendSort(boolean value)
```


يشير إلى ما إذا كان حقل PivotTable المحدد يتم فرزه تلقائيًا تصاعديًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAutoSort(boolean value) {#setAutoSort-boolean-}
```
public void setAutoSort(boolean value)
```


يشير إلى ما إذا كان حقل PivotTable المحدد يتم فرزه تلقائيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


يمثل اسم العرض لحقل PivotField.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setFunction(int value) {#setFunction-int-}
```
public void setFunction(int value)
```


يمثل الدالة المستخدمة لتلخيص حقل بيانات PivotTable.

انظر [GridPivotFieldFunction](../../com.aspose.gridweb/gridpivotfieldfunction).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setPosition(int value) {#setPosition-int-}
```
public void setPosition(int value)
```


يمثل فهرس PivotField في PivotFields.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

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

