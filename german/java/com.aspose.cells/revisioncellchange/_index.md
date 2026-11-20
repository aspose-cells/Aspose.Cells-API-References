---
title: "RevisionCellChange"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Revision dar, die Zellen ändert."
type: docs
url: /de/java/com.aspose.cells/revisioncellchange/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionCellChange extends Revision
```

Stellt die Revision dar, die Zellen ändert.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCellName()](#getCellName--) | Liefert den Namen der Zelle. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Ermittelt den Spaltenindex der Zelle. |
| [getId()](#getId--) | Ermittelt die Nummer dieser Revision. |
| [getNewFormula()](#getNewFormula--) | Ruft die alte Formel ab. |
| [getNewStyle()](#getNewStyle--) | Ruft den neuen Stil der Zelle ab. |
| [getNewValue()](#getNewValue--) | Ruft den neuen Wert der Zelle ab. |
| [getOldFormula()](#getOldFormula--) | Ruft die alte Formel ab. |
| [getOldStyle()](#getOldStyle--) | Ruft den alten Stil der Zelle ab. |
| [getOldValue()](#getOldValue--) | Ruft den alten Wert der Zelle ab. |
| [getRow()](#getRow--) | Ermittelt den Zeilenindex der Zelle. |
| [getType()](#getType--) | Stellt den Typ der Revision dar. |
| [getWorksheet()](#getWorksheet--) | Ermittelt das Arbeitsblatt. |
| [hashCode()](#hashCode--) |  |
| [isNewFormatted()](#isNewFormatted--) | Gibt an, ob diese Zelle neu formatiert ist. |
| [isOldFormatted()](#isOldFormatted--) | Gibt an, ob diese Zelle bereits formatiert ist. |
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


Ermittelt den Spaltenindex der Zelle.

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
### getNewFormula() {#getNewFormula--}
```
public String getNewFormula()
```


Ruft die alte Formel ab.

**Returns:**
java.lang.String
### getNewStyle() {#getNewStyle--}
```
public Style getNewStyle()
```


Ruft den neuen Stil der Zelle ab.

**Returns:**
[Style](../../com.aspose.cells/style)
### getNewValue() {#getNewValue--}
```
public Object getNewValue()
```


Ruft den neuen Wert der Zelle ab.

**Returns:**
java.lang.Object
### getOldFormula() {#getOldFormula--}
```
public String getOldFormula()
```


Ruft die alte Formel ab.

**Returns:**
java.lang.String
### getOldStyle() {#getOldStyle--}
```
public Style getOldStyle()
```


Ruft den alten Stil der Zelle ab.

**Returns:**
[Style](../../com.aspose.cells/style)
### getOldValue() {#getOldValue--}
```
public Object getOldValue()
```


Ruft den alten Wert der Zelle ab.

**Returns:**
java.lang.Object
### getRow() {#getRow--}
```
public int getRow()
```


Ermittelt den Zeilenindex der Zelle.

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
### isNewFormatted() {#isNewFormatted--}
```
public boolean isNewFormatted()
```


Gibt an, ob diese Zelle neu formatiert ist.

**Returns:**
boolean
### isOldFormatted() {#isOldFormatted--}
```
public boolean isOldFormatted()
```


Gibt an, ob diese Zelle bereits formatiert ist.

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

