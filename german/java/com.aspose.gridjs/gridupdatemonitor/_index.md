---
title: "GridUpdateMonitor"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Überwacht den Benutzer, um Änderungen der Aktualisierungsoperation zu verfolgen."
type: docs
url: /de/java/com.aspose.gridjs/gridupdatemonitor/
---

**Inheritance:**
java.lang.Object
```
public abstract class GridUpdateMonitor
```

Überwacht den Benutzer, um Änderungen der Aktualisierungsoperation zu verfolgen.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [GridUpdateMonitor()](#GridUpdateMonitor--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [afterUpdate(String op, String uid, ArrayList cells)](#afterUpdate-java.lang.String-java.lang.String-java.util.ArrayList-) | nach der Aktualisierungsoperation |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridUpdateMonitor() {#GridUpdateMonitor--}
```
public GridUpdateMonitor()
```


### afterUpdate(String op, String uid, ArrayList cells) {#afterUpdate-java.lang.String-java.lang.String-java.util.ArrayList-}
```
public abstract void afterUpdate(String op, String uid, ArrayList cells)
```


nach der Aktualisierungsoperation

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| op | java.lang.String | Die JSON-Zeichenfolge für die Aktualisierungsoperation |
| uid | java.lang.String | Die eindeutige ID für den Dateicache. |
| Zellen | java.util.ArrayList | Die Liste der aktualisierten Zellen, einschließlich Zellen, bei denen sich Stil, Wert oder Formel geändert hat |

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

