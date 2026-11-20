---
title: "ReserveMissingPivotItemType"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt dar, wie fehlende Pivot-Elemente beibehalten werden."
type: docs
url: /de/java/com.aspose.cells/reservemissingpivotitemtype/
---

**Inheritance:**
java.lang.Object
```
public final class ReserveMissingPivotItemType
```

Stellt dar, wie fehlende Pivot-Elemente beibehalten werden.
## Felder

| Feld | Beschreibung |
| --- | --- |
| [ALL](#ALL) | Reserviert alle fehlenden Elemente. |
| [DEFAULT](#DEFAULT) | Entfernt alte fehlende Pivot-Elemente und reserviert gelöschte Elemente der neuen Datenquelle als fehlende Elemente. |
| [NONE](#NONE) | Entfernt alle fehlenden Pivot-Elemente. |
## Methoden

| Methode | Beschreibung |
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
### ALL {#ALL}
```
public static final int ALL
```


Reserviert alle fehlenden Elemente.

**Remarks**

In Excel bleiben die fehlenden Elemente, die beim ersten Aktualisieren der Pivot-Tabelle erzeugt wurden, erhalten, solange Excel nicht geschlossen ist, selbst wenn Sie wiederholt aktualisieren.

### DEFAULT {#DEFAULT}
```
public static final int DEFAULT
```


Entfernt alte fehlende Pivot-Elemente und reserviert gelöschte Elemente der neuen Datenquelle als fehlende Elemente.

### NONE {#NONE}
```
public static final int NONE
```


Entfernt alle fehlenden Pivot-Elemente.

**Remarks**

Die Reihenfolge der alten fehlenden Pivot-Elemente wird ignoriert.

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

