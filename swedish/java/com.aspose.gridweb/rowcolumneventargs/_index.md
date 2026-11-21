---
title: "RowColumnEventArgs"
second_title: "Aspose.Cells för Java API-referens"
description: "Tillhandahåller data för rad/kolumn‑händelser."
type: docs
url: /sv/java/com.aspose.gridweb/rowcolumneventargs/
---

**Inheritance:**
java.lang.Object
```
public class RowColumnEventArgs
```

Tillhandahåller data för rad/kolumn‑händelser.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgument()](#getArgument--) | Argumentet för händelsen. |
| [getClass()](#getClass--) |  |
| [getNum()](#getNum--) | Rad‑ eller kolumnnumret, börjar från noll. |
| [getType()](#getType--) | Rad‑ eller kolumntypen. |
| [hashCode()](#hashCode--) |  |
| [isCancel()](#isCancel--) | ska vi avbryta operationen. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [rejectOperation()](#rejectOperation--) | Anropa denna metod i RowDeleting/ColumnDeleting‑händelsehanterare för att avbryta raderingsoperationerna. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getArgument() {#getArgument--}
```
public Object getArgument()
```


Argumentet för händelsen.

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


Rad‑ eller kolumnnumret, börjar från noll.

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Rad‑ eller kolumntypen.

Se [RowColumnType](../../com.aspose.gridweb/rowcolumntype).

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


ska vi avbryta operationen.

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


Anropa denna metod i RowDeleting/ColumnDeleting‑händelsehanterare för att avbryta raderingsoperationerna.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

