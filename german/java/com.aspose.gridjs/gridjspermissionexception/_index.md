---
title: "GridJsPermissionException"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt eine Berechtigungsausnahme im Kollaborationsmodus dar. Nur in der Java‑Version verfügbar, wird in Zukunft in .net/python‑Versionen verfügbar sein."
type: docs
url: /de/java/com.aspose.gridjs/gridjspermissionexception/
---

**Inheritance:**
java.lang.Object, java.lang.Throwable, java.lang.Exception
```
public class GridJsPermissionException extends Exception
```

Stellt die Berechtigungsausnahme im Kollaborationsmodus dar. Nur in der Java-Version verfügbar, wird in Zukunft in .net/python-Versionen verfügbar sein
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [GridJsPermissionException(String operation, int requiredPermission, int currentPermission)](#GridJsPermissionException-java.lang.String-int-int-) | Erstellt eine Berechtigungsausnahme |
| [GridJsPermissionException(String message, String operation, int requiredPermission, int currentPermission)](#GridJsPermissionException-java.lang.String-java.lang.String-int-int-) | Erstellt eine Berechtigungsausnahme |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [addSuppressed(Throwable arg0)](#addSuppressed-java.lang.Throwable-) |  |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [fillInStackTrace()](#fillInStackTrace--) |  |
| [getCause()](#getCause--) |  |
| [getClass()](#getClass--) |  |
| [getCurrentPermission()](#getCurrentPermission--) | Ermittelt das aktuelle Berechtigungsniveau des Benutzers |
| [getLocalizedMessage()](#getLocalizedMessage--) |  |
| [getMessage()](#getMessage--) |  |
| [getOperation()](#getOperation--) | Ermittelt die Operation, die ausgeführt werden sollte |
| [getRequiredPermission()](#getRequiredPermission--) | Ermittelt das für die Operation erforderliche Berechtigungsniveau |
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


Erstellt eine Berechtigungsausnahme

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Operation | java.lang.String | Versuchte auszuführende Operation |
| requiredPermission | int | [CoWorkUserPermission](../../com.aspose.gridjs/coworkuserpermission). Berechtigung, die für die Operation erforderlich ist |
| currentPermission | int | [CoWorkUserPermission](../../com.aspose.gridjs/coworkuserpermission). Aktuelle Benutzerberechtigung |

### GridJsPermissionException(String message, String operation, int requiredPermission, int currentPermission) {#GridJsPermissionException-java.lang.String-java.lang.String-int-int-}
```
public GridJsPermissionException(String message, String operation, int requiredPermission, int currentPermission)
```


Erstellt eine Berechtigungsausnahme

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Nachricht | java.lang.String | Benutzerdefinierte Fehlermeldung |
| Operation | java.lang.String | Versuchte auszuführende Operation |
| requiredPermission | int | [CoWorkUserPermission](../../com.aspose.gridjs/coworkuserpermission). Berechtigung, die für die Operation erforderlich ist |
| currentPermission | int | [CoWorkUserPermission](../../com.aspose.gridjs/coworkuserpermission). Aktuelle Benutzerberechtigung |

### addSuppressed(Throwable arg0) {#addSuppressed-java.lang.Throwable-}
```
public final synchronized void addSuppressed(Throwable arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | java.lang.Throwable |  |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
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


Ermittelt das aktuelle Berechtigungsniveau des Benutzers

**Returns:**
int - [CoWorkUserPermission](../../com.aspose.gridjs/coworkuserpermission). Aktuelle Berechtigungsstufe des Benutzers
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


Ermittelt die Operation, die ausgeführt werden sollte

**Returns:**
java.lang.String - Operationsname
### getRequiredPermission() {#getRequiredPermission--}
```
public int getRequiredPermission()
```


Ermittelt das für die Operation erforderliche Berechtigungsniveau

**Returns:**
int - [CoWorkUserPermission](../../com.aspose.gridjs/coworkuserpermission). Erforderliches Berechtigungsniveau
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
| Parameter | Typ | Beschreibung |
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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | java.io.PrintStream |  |

### printStackTrace(PrintWriter arg0) {#printStackTrace-java.io.PrintWriter-}
```
public void printStackTrace(PrintWriter arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | java.io.PrintWriter |  |

### setStackTrace(StackTraceElement[] arg0) {#setStackTrace-java.lang.StackTraceElement---}
```
public void setStackTrace(StackTraceElement[] arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

