---
title: "RevisionCustomView"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt einen Revisionsdatensatz für das Hinzufügen oder Entfernen einer benutzerdefinierten Ansicht zur Arbeitsmappe dar"
type: docs
url: /de/java/com.aspose.cells/revisioncustomview/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionCustomView extends Revision
```

Stellt einen Revisionsdatensatz für das Hinzufügen oder Entfernen einer benutzerdefinierten Ansicht zur Arbeitsmappe dar
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActionType()](#getActionType--) | Liefert den Aktionstyp. |
| [getClass()](#getClass--) |  |
| [getGuid()](#getGuid--) | Liefert die global eindeutige Kennung der benutzerdefinierten Ansicht. |
| [getId()](#getId--) | Ermittelt die Nummer dieser Revision. |
| [getType()](#getType--) | Liefert den Typ der Revision. |
| [getWorksheet()](#getWorksheet--) | Ermittelt das Arbeitsblatt. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
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
### getActionType() {#getActionType--}
```
public int getActionType()
```


Liefert den Aktionstyp.

Siehe [RevisionActionType](../../com.aspose.cells/revisionactiontype).

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getGuid() {#getGuid--}
```
public UUID getGuid()
```


Liefert die global eindeutige Kennung der benutzerdefinierten Ansicht.

**Returns:**
java.util.UUID
### getId() {#getId--}
```
public int getId()
```


Ermittelt die Nummer dieser Revision.

**Remarks**

Null bedeutet, dass diese Revision keine ID enthält.

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Liefert den Typ der Revision.

Siehe [RevisionType](../../com.aspose.cells/revisiontype).

**Returns:**
int
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Ermittelt das Arbeitsblatt.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
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

