---
title: "SessionMode"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل وضع الجلسة للـ grid."
type: docs
url: /ar/java/com.aspose.gridweb/sessionmode/
---

**Inheritance:**
java.lang.Object
```
public final class SessionMode
```

يمثل وضع الجلسة للـ grid.
## حقول

| حقل | الوصف |
| --- | --- |
| [CUSTOM](#CUSTOM) | يستخدم حدث LoadCustomData لتحميل بيانات ورقة الشبكة يدويًا. |
| [FILE](#FILE) | يستخدم ملف النظام لتخزين/استعادة بيانات ورقة الشبكة تلقائيًا، يحتاج المستخدم إلى ضبط SessionStorePath لتحديد دليل الملف. |
| [SESSION](#SESSION) | يستخدم جلسة النظام لتخزين/استعادة بيانات ورقة الشبكة تلقائيًا. |
| [VIEW_STATE](#VIEW-STATE) | يستخدم viewstate الصفحة لتخزين/استعادة بيانات ورقة الشبكة تلقائيًا. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CUSTOM {#CUSTOM}
```
public static final int CUSTOM
```


يستخدم حدث LoadCustomData لتحميل بيانات ورقة الشبكة يدويًا. ويستخدم حدث SheetDataUpdated لحفظ بيانات ورقة الشبكة.

### FILE {#FILE}
```
public static final int FILE
```


يستخدم ملف النظام لتخزين/استعادة بيانات ورقة الشبكة تلقائيًا، يحتاج المستخدم إلى ضبط SessionStorePath لتحديد دليل الملف.

### SESSION {#SESSION}
```
public static final int SESSION
```


يستخدم جلسة النظام لتخزين/استعادة بيانات ورقة الشبكة تلقائيًا.

### VIEW_STATE {#VIEW-STATE}
```
public static final int VIEW_STATE
```


يستخدم viewstate الصفحة لتخزين/استعادة بيانات ورقة الشبكة تلقائيًا.

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

