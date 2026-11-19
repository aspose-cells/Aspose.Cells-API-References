---
title: "GridJsPermissionException"
second_title: "Aspose.Cells for Java API 参考"
description: "表示协作模式下的权限异常。仅在 Java 版本中可用，未来将在 .netython 版本中提供。"
type: docs
url: /zh/java/com.aspose.gridjs/gridjspermissionexception/
---

**Inheritance:**
java.lang.Object, java.lang.Throwable, java.lang.Exception
```
public class GridJsPermissionException extends Exception
```

表示协作模式下的权限异常。目前仅在 Java 版本中可用，未来将在 .net/python 版本中提供。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [GridJsPermissionException(String operation, int requiredPermission, int currentPermission)](#GridJsPermissionException-java.lang.String-int-int-) | 构造一个权限异常 |
| [GridJsPermissionException(String message, String operation, int requiredPermission, int currentPermission)](#GridJsPermissionException-java.lang.String-java.lang.String-int-int-) | 构造一个权限异常 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [addSuppressed(Throwable arg0)](#addSuppressed-java.lang.Throwable-) |  |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [fillInStackTrace()](#fillInStackTrace--) |  |
| [getCause()](#getCause--) |  |
| [getClass()](#getClass--) |  |
| [getCurrentPermission()](#getCurrentPermission--) | 获取用户当前的权限级别 |
| [getLocalizedMessage()](#getLocalizedMessage--) |  |
| [getMessage()](#getMessage--) |  |
| [getOperation()](#getOperation--) | 获取尝试执行的操作 |
| [getRequiredPermission()](#getRequiredPermission--) | 获取操作所需的权限级别 |
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


构造一个权限异常

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 操作 | java.lang.String | 尝试执行的操作 |
| requiredPermission | int | [CoWorkUserPermission](../../com.aspose.gridjs/coworkuserpermission). 操作所需的权限 |
| currentPermission | int | [CoWorkUserPermission](../../com.aspose.gridjs/coworkuserpermission). 当前用户权限 |

### GridJsPermissionException(String message, String operation, int requiredPermission, int currentPermission) {#GridJsPermissionException-java.lang.String-java.lang.String-int-int-}
```
public GridJsPermissionException(String message, String operation, int requiredPermission, int currentPermission)
```


构造一个权限异常

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 消息 | java.lang.String | 自定义错误消息 |
| 操作 | java.lang.String | 尝试执行的操作 |
| requiredPermission | int | [CoWorkUserPermission](../../com.aspose.gridjs/coworkuserpermission). 操作所需的权限 |
| currentPermission | int | [CoWorkUserPermission](../../com.aspose.gridjs/coworkuserpermission). 当前用户权限 |

### addSuppressed(Throwable arg0) {#addSuppressed-java.lang.Throwable-}
```
public final synchronized void addSuppressed(Throwable arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | java.lang.Throwable |  |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
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


获取用户当前的权限级别

**Returns:**
int - [CoWorkUserPermission](../../com.aspose.gridjs/coworkuserpermission)。当前用户权限级别
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


获取尝试执行的操作

**Returns:**
java.lang.String - 操作名称
### getRequiredPermission() {#getRequiredPermission--}
```
public int getRequiredPermission()
```


获取操作所需的权限级别

**Returns:**
int - [CoWorkUserPermission](../../com.aspose.gridjs/coworkuserpermission). 所需权限级别
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
| 参数 | 类型 | 描述 |
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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | java.io.PrintStream |  |

### printStackTrace(PrintWriter arg0) {#printStackTrace-java.io.PrintWriter-}
```
public void printStackTrace(PrintWriter arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | java.io.PrintWriter |  |

### setStackTrace(StackTraceElement[] arg0) {#setStackTrace-java.lang.StackTraceElement---}
```
public void setStackTrace(StackTraceElement[] arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

