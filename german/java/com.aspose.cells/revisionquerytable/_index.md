---
title: "RevisionQueryTable"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt eine Revision einer Änderung des Abfrage-Tabellenfelds dar."
type: docs
url: /de/java/com.aspose.cells/revisionquerytable/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionQueryTable extends Revision
```

Stellt eine Revision einer Änderung des Abfrage-Tabellenfelds dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCellArea()](#getCellArea--) | Ermittelt den Speicherort der betroffenen Abfrage-Tabelle. |
| [getClass()](#getClass--) |  |
| [getFieldId()](#getFieldId--) | Ermittelt die ID des spezifischen Feldes der Abfrage-Tabelle, das entfernt wurde. |
| [getId()](#getId--) | Ermittelt die Nummer dieser Revision. |
| [getType()](#getType--) | Stellt den Typ der Revision dar. |
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
### getCellArea() {#getCellArea--}
```
public CellArea getCellArea()
```


Ermittelt den Speicherort der betroffenen Abfrage-Tabelle.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFieldId() {#getFieldId--}
```
public int getFieldId()
```


Ermittelt die ID des spezifischen Feldes der Abfrage-Tabelle, das entfernt wurde.

**Returns:**
int
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


Stellt den Typ der Revision dar.

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

