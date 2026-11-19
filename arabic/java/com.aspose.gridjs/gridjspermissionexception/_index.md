---
title: "GridJsPermissionException"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل استثناء الإذن في وضع التعاون. متاح فقط في نسخة Java الآن وسيكون متاحًا في نسخة .netython في المستقبل."
type: docs
url: /ar/java/com.aspose.gridjs/gridjspermissionexception/
---

**Inheritance:**
java.lang.Object, java.lang.Throwable, java.lang.Exception
```
public class GridJsPermissionException extends Exception
```

يمثل استثناء الإذن في وضع التعاون. متاح فقط في نسخة جافا الآن، وسيكون متاحًا في نسخة .net/python في المستقبل.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [GridJsPermissionException(String operation, int requiredPermission, int currentPermission)](#GridJsPermissionException-java.lang.String-int-int-) | ينشئ استثناء صلاحية |
| [GridJsPermissionException(String message, String operation, int requiredPermission, int currentPermission)](#GridJsPermissionException-java.lang.String-java.lang.String-int-int-) | ينشئ استثناء صلاحية |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [addSuppressed(Throwable arg0)](#addSuppressed-java.lang.Throwable-) |  |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [fillInStackTrace()](#fillInStackTrace--) |  |
| [getCause()](#getCause--) |  |
| [getClass()](#getClass--) |  |
| [getCurrentPermission()](#getCurrentPermission--) | يحصل على مستوى الإذن الحالي للمستخدم |
| [getLocalizedMessage()](#getLocalizedMessage--) |  |
| [getMessage()](#getMessage--) |  |
| [getOperation()](#getOperation--) | يحصل على العملية التي تم محاولة تنفيذها |
| [getRequiredPermission()](#getRequiredPermission--) | يحصل على مستوى الإذن المطلوب للعملية |
| [getStackTrace()](#getStackTrace--) |  |
| [getSuppressed()](#getSuppressed--) |  |
| [hashCode()](#hashCode--) |  |
| [initCause(Throwable arg0)](#initCause-java.lang.Throwable-) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [printStackTrace()](#printStackTrace--) |  |
| [printStackTrace(PrintStream arg0)](#printStackTrace-java.io.PrintStream-) |  |
| [printStackTrace(PrintWriter arg0)](#printStackTrace-java.io.PrintWriter-) |  |
| [setStackTrace(StackTraceElement[] arg0)](#setStackTrace-java.lang.StackTraceElement---) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridJsPermissionException(String operation, int requiredPermission, int currentPermission) {#GridJsPermissionException-java.lang.String-int-int-}
```
public GridJsPermissionException(String operation, int requiredPermission, int currentPermission)
```


ينشئ استثناء صلاحية

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عملية | java.lang.String | العملية التي تم محاولة تنفيذها |
| requiredPermission | int | [CoWorkUserPermission](../../com.aspose.gridjs/coworkuserpermission). الإذن المطلوب للعملية |
| currentPermission | int | [CoWorkUserPermission](../../com.aspose.gridjs/coworkuserpermission). إذن المستخدم الحالي |

### GridJsPermissionException(String message, String operation, int requiredPermission, int currentPermission) {#GridJsPermissionException-java.lang.String-java.lang.String-int-int-}
```
public GridJsPermissionException(String message, String operation, int requiredPermission, int currentPermission)
```


ينشئ استثناء صلاحية

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| رسالة | java.lang.String | رسالة خطأ مخصصة |
| عملية | java.lang.String | العملية التي تم محاولة تنفيذها |
| requiredPermission | int | [CoWorkUserPermission](../../com.aspose.gridjs/coworkuserpermission). الإذن المطلوب للعملية |
| currentPermission | int | [CoWorkUserPermission](../../com.aspose.gridjs/coworkuserpermission). إذن المستخدم الحالي |

### addSuppressed(Throwable arg0) {#addSuppressed-java.lang.Throwable-}
```
public final synchronized void addSuppressed(Throwable arg0)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | java.lang.Throwable |  |

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
### fillInStackTrace() {#fillInStackTrace--}
```
public synchronized Throwable fillInStackTrace()
```




**Returns:**
java.lang.Throwable
### getCause() {#getCause--}
```
public synchronized Throwable getCause()
```




**Returns:**
java.lang.Throwable
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCurrentPermission() {#getCurrentPermission--}
```
public int getCurrentPermission()
```


يحصل على مستوى الإذن الحالي للمستخدم

**Returns:**
int - [CoWorkUserPermission](../../com.aspose.gridjs/coworkuserpermission). مستوى صلاحية المستخدم الحالي
### getLocalizedMessage() {#getLocalizedMessage--}
```
public String getLocalizedMessage()
```




**Returns:**
java.lang.String
### getMessage() {#getMessage--}
```
public String getMessage()
```




**Returns:**
java.lang.String
### getOperation() {#getOperation--}
```
public String getOperation()
```


يحصل على العملية التي تم محاولة تنفيذها

**Returns:**
java.lang.String - اسم العملية
### getRequiredPermission() {#getRequiredPermission--}
```
public int getRequiredPermission()
```


يحصل على مستوى الإذن المطلوب للعملية

**Returns:**
int - [CoWorkUserPermission](../../com.aspose.gridjs/coworkuserpermission). مستوى الإذن المطلوب
### getStackTrace() {#getStackTrace--}
```
public StackTraceElement[] getStackTrace()
```




**Returns:**
java.lang.StackTraceElement[]
### getSuppressed() {#getSuppressed--}
```
public final synchronized Throwable[] getSuppressed()
```




**Returns:**
java.lang.Throwable[]
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### initCause(Throwable arg0) {#initCause-java.lang.Throwable-}
```
public synchronized Throwable initCause(Throwable arg0)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | java.lang.Throwable |  |

**Returns:**
java.lang.Throwable
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### printStackTrace() {#printStackTrace--}
```
public void printStackTrace()
```




### printStackTrace(PrintStream arg0) {#printStackTrace-java.io.PrintStream-}
```
public void printStackTrace(PrintStream arg0)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | java.io.PrintStream |  |

### printStackTrace(PrintWriter arg0) {#printStackTrace-java.io.PrintWriter-}
```
public void printStackTrace(PrintWriter arg0)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | java.io.PrintWriter |  |

### setStackTrace(StackTraceElement[] arg0) {#setStackTrace-java.lang.StackTraceElement---}
```
public void setStackTrace(StackTraceElement[] arg0)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | java.lang.StackTraceElement[] |  |

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

