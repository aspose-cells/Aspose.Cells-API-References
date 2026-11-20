---
title: "GridJsPermissionException"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет исключение доступа в режиме совместной работы. Сейчас доступно только в версии Java, в будущих версиях будет доступно в .NETython."
type: docs
url: /ru/java/com.aspose.gridjs/gridjspermissionexception/
---

**Inheritance:**
java.lang.Object, java.lang.Throwable, java.lang.Exception
```
public class GridJsPermissionException extends Exception
```

Представляет исключение разрешения в режиме совместной работы. Доступно только в версии Java сейчас, будет доступно в версиях .net/python в будущем.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [GridJsPermissionException(String operation, int requiredPermission, int currentPermission)](#GridJsPermissionException-java.lang.String-int-int-) | Создаёт исключение доступа |
| [GridJsPermissionException(String message, String operation, int requiredPermission, int currentPermission)](#GridJsPermissionException-java.lang.String-java.lang.String-int-int-) | Создаёт исключение доступа |
## Методы

| Метод | Описание |
| --- | --- |
| [addSuppressed(Throwable arg0)](#addSuppressed-java.lang.Throwable-) |  |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [fillInStackTrace()](#fillInStackTrace--) |  |
| [getCause()](#getCause--) |  |
| [getClass()](#getClass--) |  |
| [getCurrentPermission()](#getCurrentPermission--) | Получает текущий уровень доступа пользователя |
| [getLocalizedMessage()](#getLocalizedMessage--) |  |
| [getMessage()](#getMessage--) |  |
| [getOperation()](#getOperation--) | Получает операцию, которую попытались выполнить |
| [getRequiredPermission()](#getRequiredPermission--) | Получает требуемый уровень доступа для операции |
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


Создаёт исключение доступа

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| операция | java.lang.String | Операция, попытка выполнить |
| requiredPermission | int | [CoWorkUserPermission](../../com.aspose.gridjs/coworkuserpermission). Требуемый доступ для операции |
| currentPermission | int | [CoWorkUserPermission](../../com.aspose.gridjs/coworkuserpermission). Текущий доступ пользователя |

### GridJsPermissionException(String message, String operation, int requiredPermission, int currentPermission) {#GridJsPermissionException-java.lang.String-java.lang.String-int-int-}
```
public GridJsPermissionException(String message, String operation, int requiredPermission, int currentPermission)
```


Создаёт исключение доступа

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| сообщение | java.lang.String | Пользовательское сообщение об ошибке |
| операция | java.lang.String | Операция, попытка выполнить |
| requiredPermission | int | [CoWorkUserPermission](../../com.aspose.gridjs/coworkuserpermission). Требуемый доступ для операции |
| currentPermission | int | [CoWorkUserPermission](../../com.aspose.gridjs/coworkuserpermission). Текущий доступ пользователя |

### addSuppressed(Throwable arg0) {#addSuppressed-java.lang.Throwable-}
```
public final synchronized void addSuppressed(Throwable arg0)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | java.lang.Throwable |  |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Параметр | Тип | Описание |
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


Получает текущий уровень доступа пользователя

**Returns:**
int — [CoWorkUserPermission](../../com.aspose.gridjs/coworkuserpermission). Текущий уровень разрешений пользователя
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


Получает операцию, которую попытались выполнить

**Returns:**
java.lang.String — имя операции
### getRequiredPermission() {#getRequiredPermission--}
```
public int getRequiredPermission()
```


Получает требуемый уровень доступа для операции

**Returns:**
int — [CoWorkUserPermission](../../com.aspose.gridjs/coworkuserpermission). Требуемый уровень доступа
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
| Параметр | Тип | Описание |
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
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | java.io.PrintStream |  |

### printStackTrace(PrintWriter arg0) {#printStackTrace-java.io.PrintWriter-}
```
public void printStackTrace(PrintWriter arg0)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | java.io.PrintWriter |  |

### setStackTrace(StackTraceElement[] arg0) {#setStackTrace-java.lang.StackTraceElement---}
```
public void setStackTrace(StackTraceElement[] arg0)
```




**Parameters:**
| Параметр | Тип | Описание |
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
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

