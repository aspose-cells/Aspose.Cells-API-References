---
title: "RevisionCellComment"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt einen Revisionsdatensatz einer Zellkommentaränderung dar."
type: docs
url: /de/java/com.aspose.cells/revisioncellcomment/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionCellComment extends Revision
```

Stellt einen Revisionsdatensatz einer Zellkommentaränderung dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActionType()](#getActionType--) | Liefert den Aktionstyp der Revision. |
| [getCellName()](#getCellName--) | Liefert den Namen der Zelle. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Ermittelt den Spaltenindex, der einen Kommentar enthält. |
| [getId()](#getId--) | Ermittelt die Nummer dieser Revision. |
| [getNewLength()](#getNewLength--) | Ermittelt die Länge des Kommentars, bevor diese Revision vorgenommen wurde. |
| [getOldLength()](#getOldLength--) | Ermittelt die Länge des Kommentartexts, der in dieser Revision hinzugefügt wurde. |
| [getRow()](#getRow--) | Ermittelt den Zeilenindex, der einen Kommentar enthält. |
| [getType()](#getType--) | Liefert den Typ der Revision. |
| [getWorksheet()](#getWorksheet--) | Ermittelt das Arbeitsblatt. |
| [hashCode()](#hashCode--) |  |
| [isOldComment()](#isOldComment--) | Gibt an, ob es sich um einen alten Kommentar handelt. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCellName(String value)](#setCellName-java.lang.String-) | Liefert den Namen der Zelle. |
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


Liefert den Aktionstyp der Revision.

Siehe [RevisionActionType](../../com.aspose.cells/revisionactiontype).

**Returns:**
int
### getCellName() {#getCellName--}
```
public String getCellName()
```


Liefert den Namen der Zelle.

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumn() {#getColumn--}
```
public int getColumn()
```


Ermittelt den Spaltenindex, der einen Kommentar enthält.

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
### getNewLength() {#getNewLength--}
```
public int getNewLength()
```


Ermittelt die Länge des Kommentars, bevor diese Revision vorgenommen wurde.

**Returns:**
int
### getOldLength() {#getOldLength--}
```
public int getOldLength()
```


Ermittelt die Länge des Kommentartexts, der in dieser Revision hinzugefügt wurde.

**Returns:**
int
### getRow() {#getRow--}
```
public int getRow()
```


Ermittelt den Zeilenindex, der einen Kommentar enthält.

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
### isOldComment() {#isOldComment--}
```
public boolean isOldComment()
```


Gibt an, ob es sich um einen alten Kommentar handelt.

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




### setCellName(String value) {#setCellName-java.lang.String-}
```
public void setCellName(String value)
```


Liefert den Namen der Zelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

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

