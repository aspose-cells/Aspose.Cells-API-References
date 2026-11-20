---
title: "GridReferredArea"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt einen durch die Formel referenzierten Bereich dar."
type: docs
url: /de/java/com.aspose.gridjs/gridreferredarea/
---

**Inheritance:**
java.lang.Object
```
public class GridReferredArea
```

Stellt einen durch die Formel referenzierten Bereich dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getEndColumn()](#getEndColumn--) | Die Endspalte des Bereichs. |
| [getEndRow()](#getEndRow--) | Die Endzeile des Bereichs. |
| [getExternalFileName()](#getExternalFileName--) | Erhalte den externen Dateinamen, wenn dies eine externe Referenz ist. |
| [getSheetName()](#getSheetName--) | Gibt an, in welchem Blatt sich dies befindet |
| [getStartColumn()](#getStartColumn--) | Die Startspalte des Bereichs. |
| [getStartRow()](#getStartRow--) | Die Startzeile des Bereichs. |
| [getValue(int rowOffset, int colOffset)](#getValue-int-int-) | Ermittelt den Zellenwert mit dem angegebenen Versatz von der oberen linken Ecke dieses Bereichs. |
| [getValues()](#getValues--) | Ermittelt Zellwerte in diesem Bereich. |
| [hashCode()](#hashCode--) |  |
| [isArea()](#isArea--) | Gibt an, ob dies ein Bereich ist. |
| [isExternalLink()](#isExternalLink--) | Gibt an, ob dies ein externer Link ist. |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEndColumn() {#getEndColumn--}
```
public int getEndColumn()
```


Die Endspalte des Bereichs.

**Returns:**
int
### getEndRow() {#getEndRow--}
```
public int getEndRow()
```


Die Endzeile des Bereichs.

**Returns:**
int
### getExternalFileName() {#getExternalFileName--}
```
public String getExternalFileName()
```


Erhalte den externen Dateinamen, wenn dies eine externe Referenz ist.

**Returns:**
java.lang.String
### getSheetName() {#getSheetName--}
```
public String getSheetName()
```


Gibt an, in welchem Blatt sich dies befindet

**Returns:**
java.lang.String
### getStartColumn() {#getStartColumn--}
```
public int getStartColumn()
```


Die Startspalte des Bereichs.

**Returns:**
int
### getStartRow() {#getStartRow--}
```
public int getStartRow()
```


Die Startzeile des Bereichs.

**Returns:**
int
### getValue(int rowOffset, int colOffset) {#getValue-int-int-}
```
public Object getValue(int rowOffset, int colOffset)
```


Ermittelt den Zellenwert mit dem angegebenen Versatz von der oberen linken Ecke dieses Bereichs.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowOffset | int | Zeilenversatz von der Startzeile dieses Bereichs. |
| colOffset | int | Spaltenversatz von der Startzeile dieses Bereichs. |

**Returns:**
java.lang.Object - "\#REF!", wenn dieser Bereich ungültig ist; "\#N/A", wenn der angegebene Versatz außerhalb dieses Bereichs liegt; andernfalls wird der Zellenwert an der angegebenen Position zurückgegeben.
### getValues() {#getValues--}
```
public Object getValues()
```


Ermittelt Zellwerte in diesem Bereich.

**Returns:**
java.lang.Object - Wenn dieser Bereich ungültig ist, wird \"\\#REF!\" zurückgegeben; Wenn dieser Bereich eine einzelne Zelle ist, wird das Zellenwertobjekt zurückgegeben; Andernfalls wird ein Array mit allen Werten in diesem Bereich zurückgegeben.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isArea() {#isArea--}
```
public boolean isArea()
```


Gibt an, ob dies ein Bereich ist.

**Remarks**

Wenn dies kein Bereich ist, wirken nur StartRow und StartColumn.

**Returns:**
boolean
### isExternalLink() {#isExternalLink--}
```
public boolean isExternalLink()
```


Gibt an, ob dies ein externer Link ist.

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

