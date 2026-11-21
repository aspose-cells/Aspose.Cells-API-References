---
title: "GridJsPermissionException"
second_title: "Aspose.Cells for Java API Referansı"
description: "İş birliği modunda izin istisnasını temsil eder. Şu anda yalnızca Java sürümünde mevcuttur, gelecekte .netython sürümünde de bulunacaktır."
type: docs
url: /tr/java/com.aspose.gridjs/gridjspermissionexception/
---

**Inheritance:**
java.lang.Object, java.lang.Throwable, java.lang.Exception
```
public class GridJsPermissionException extends Exception
```

İş birliği modunda izin istisnasını temsil eder. Şu anda yalnızca java sürümünde mevcuttur, gelecekte .net/python sürümünde de mevcut olacaktır.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [GridJsPermissionException(String operation, int requiredPermission, int currentPermission)](#GridJsPermissionException-java.lang.String-int-int-) | Bir izin istisnası oluşturur |
| [GridJsPermissionException(String message, String operation, int requiredPermission, int currentPermission)](#GridJsPermissionException-java.lang.String-java.lang.String-int-int-) | Bir izin istisnası oluşturur |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [addSuppressed(Throwable arg0)](#addSuppressed-java.lang.Throwable-) |  |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [fillInStackTrace()](#fillInStackTrace--) |  |
| [getCause()](#getCause--) |  |
| [getClass()](#getClass--) |  |
| [getCurrentPermission()](#getCurrentPermission--) | Kullanıcının mevcut izin seviyesini alır |
| [getLocalizedMessage()](#getLocalizedMessage--) |  |
| [getMessage()](#getMessage--) |  |
| [getOperation()](#getOperation--) | Yürütülmeye çalışılan işlemi alır |
| [getRequiredPermission()](#getRequiredPermission--) | İşlem için gereken izin seviyesini alır |
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


Bir izin istisnası oluşturur

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| işlem | java.lang.String | Yürütülmeye çalışılan işlem |
| requiredPermission | int | [CoWorkUserPermission](../../com.aspose.gridjs/coworkuserpermission). İşlem için gerekli izin |
| currentPermission | int | [CoWorkUserPermission](../../com.aspose.gridjs/coworkuserpermission). Mevcut kullanıcı izni |

### GridJsPermissionException(String message, String operation, int requiredPermission, int currentPermission) {#GridJsPermissionException-java.lang.String-java.lang.String-int-int-}
```
public GridJsPermissionException(String message, String operation, int requiredPermission, int currentPermission)
```


Bir izin istisnası oluşturur

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| mesaj | java.lang.String | Özel hata mesajı |
| işlem | java.lang.String | Yürütülmeye çalışılan işlem |
| requiredPermission | int | [CoWorkUserPermission](../../com.aspose.gridjs/coworkuserpermission). İşlem için gerekli izin |
| currentPermission | int | [CoWorkUserPermission](../../com.aspose.gridjs/coworkuserpermission). Mevcut kullanıcı izni |

### addSuppressed(Throwable arg0) {#addSuppressed-java.lang.Throwable-}
```
public final synchronized void addSuppressed(Throwable arg0)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | java.lang.Throwable |  |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametre | Tür | Açıklama |
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


Kullanıcının mevcut izin seviyesini alır

**Returns:**
int - [CoWorkUserPermission](../../com.aspose.gridjs/coworkuserpermission). Mevcut kullanıcı izin seviyesi
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


Yürütülmeye çalışılan işlemi alır

**Returns:**
java.lang.String - İşlem adı
### getRequiredPermission() {#getRequiredPermission--}
```
public int getRequiredPermission()
```


İşlem için gereken izin seviyesini alır

**Returns:**
int - [CoWorkUserPermission](../../com.aspose.gridjs/coworkuserpermission). Gerekli izin seviyesi
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
| Parametre | Tür | Açıklama |
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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | java.io.PrintStream |  |

### printStackTrace(PrintWriter arg0) {#printStackTrace-java.io.PrintWriter-}
```
public void printStackTrace(PrintWriter arg0)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | java.io.PrintWriter |  |

### setStackTrace(StackTraceElement[] arg0) {#setStackTrace-java.lang.StackTraceElement---}
```
public void setStackTrace(StackTraceElement[] arg0)
```




**Parameters:**
| Parametre | Tür | Açıklama |
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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

