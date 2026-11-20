---
title: "RowColumnEventArgs"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt Daten für Zeilen-/Spaltenereignisse bereit."
type: docs
url: /de/java/com.aspose.gridweb/rowcolumneventargs/
---

**Inheritance:**
java.lang.Object
```
public class RowColumnEventArgs
```

Stellt Daten für Zeilen-/Spaltenereignisse bereit.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgument()](#getArgument--) | Das Argument des Ereignisses. |
| [getClass()](#getClass--) |  |
| [getNum()](#getNum--) | Die Zeilen‑ oder Spaltennummer, beginnend bei Null. |
| [getType()](#getType--) | Der Zeilen‑ oder Spaltentyp. |
| [hashCode()](#hashCode--) |  |
| [isCancel()](#isCancel--) | Soll die Operation abgebrochen werden. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [rejectOperation()](#rejectOperation--) | Rufen Sie diese Methode in RowDeleting/ColumnDeleting-Ereignishandlern auf, um die Löschvorgänge abzubrechen. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getArgument() {#getArgument--}
```
public Object getArgument()
```


Das Argument des Ereignisses.

**Returns:**
java.lang.Object
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getNum() {#getNum--}
```
public int getNum()
```


Die Zeilen‑ oder Spaltennummer, beginnend bei Null.

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Der Zeilen‑ oder Spaltentyp.

Siehe [RowColumnType](../../com.aspose.gridweb/rowcolumntype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCancel() {#isCancel--}
```
public boolean isCancel()
```


Soll die Operation abgebrochen werden.

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




### rejectOperation() {#rejectOperation--}
```
public void rejectOperation()
```


Rufen Sie diese Methode in RowDeleting/ColumnDeleting-Ereignishandlern auf, um die Löschvorgänge abzubrechen.

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

