---
title: "PivotFieldCollection"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt eine Sammlung aller PivotField-Objekte in den verschiedenen Bereichen der Pivot-Tabelle dar."
type: docs
url: /de/java/com.aspose.cells/pivotfieldcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PivotFieldCollection extends CollectionBase
```

Stellt eine Sammlung aller PivotField-Objekte in den verschiedenen Bereichen der Pivot-Tabelle dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add(PivotField pivotField)](#add-com.aspose.cells.PivotField-) | Fügt ein PivotField-Objekt zu den spezifischen PivotFields-Typ hinzu. |
| [add(Object o)](#add-java.lang.Object-) | Fügt ein Element zur CollectionBase-Instanz hinzu. |
| [addByBaseIndex(int baseFieldIndex)](#addByBaseIndex-int-) | Fügt ein PivotField-Objekt zu den spezifischen PivotFields-Typ hinzu. |
| [clear()](#clear--) | Alle Felder der PivotFieldCollection löschen |
| [contains(Object o)](#contains-java.lang.Object-) | Gibt zurück, ob die Instanz dieses Objekt enthält |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Ermittelt das PivotField-Objekt am angegebenen Index. |
| [get(String name)](#get-java.lang.String-) | Ruft das PivotField-Objekt mit dem angegebenen Namen ab. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ermittelt die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente. |
| [getType()](#getType--) | Ruft den Typ von PivotFields ab. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Bestimmt den Index eines bestimmten Elements in der CollectionBase-Instanz. |
| [insert(int index, PivotField pivotField)](#insert-int-com.aspose.cells.PivotField-) | Fügt ein Pivot-Feld an einem bestimmten Index ein. |
| [iterator()](#iterator--) | Gibt einen Enumerator zurück, der die CollectionBase-Instanz durchläuft. |
| [move(int currPos, int destPos)](#move-int-int-) | Verschiebt das PivotField von der aktuellen Position zur Zielposition |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(PivotField pivotField)](#remove-com.aspose.cells.PivotField-) | Entfernt das Feld aus der aktuellen Region. |
| [removeAt(int index)](#removeAt-int-) | Entfernt das Feld anhand des Index. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(PivotField pivotField) {#add-com.aspose.cells.PivotField-}
```
public int add(PivotField pivotField)
```


Fügt ein PivotField-Objekt zu den spezifischen PivotFields-Typ hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivotField | [PivotField](../../com.aspose.cells/pivotfield) | ein PivotField-Objekt. |

**Returns:**
int - der Index des PivotField-Objekts in diesen PivotFields.
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Fügt ein Element zur CollectionBase-Instanz hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | Das Objekt, das zur CollectionBase-Instanz hinzugefügt werden soll. |

**Returns:**
int - Die Position, an der das neue Element eingefügt wurde.
### addByBaseIndex(int baseFieldIndex) {#addByBaseIndex-int-}
```
public int addByBaseIndex(int baseFieldIndex)
```


Fügt ein PivotField-Objekt zu den spezifischen PivotFields-Typ hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| baseFieldIndex | int | Feldindex in den Basis-PivotFields. |

**Returns:**
int - der Index des PivotField-Objekts in diesen PivotFields.
### clear() {#clear--}
```
public void clear()
```


Alle Felder der PivotFieldCollection löschen

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Gibt zurück, ob die Instanz dieses Objekt enthält

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | Testobjekt |

**Returns:**
boolean - Ob die Instanz dieses Objekt enthält
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
### get(int index) {#get-int-}
```
public PivotField get(int index)
```


Ermittelt das PivotField-Objekt am angegebenen Index.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int |  |

**Returns:**
[PivotField](../../com.aspose.cells/pivotfield)
### get(String name) {#get-java.lang.String-}
```
public PivotField get(String name)
```


Ruft das PivotField-Objekt mit dem angegebenen Namen ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String |  |

**Returns:**
[PivotField](../../com.aspose.cells/pivotfield)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


Ermittelt die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente.

**Returns:**
int - Die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente.
### getType() {#getType--}
```
public int getType()
```


Ruft den Typ von PivotFields ab.

Siehe [PivotFieldType](../../com.aspose.cells/pivotfieldtype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


Bestimmt den Index eines bestimmten Elements in der CollectionBase-Instanz.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | Bestimmt den Index eines bestimmten Elements in der CollectionBase-Instanz. |

**Returns:**
int - Der Index des Wertes, falls in der Liste gefunden; sonst -1.
### insert(int index, PivotField pivotField) {#insert-int-com.aspose.cells.PivotField-}
```
public void insert(int index, PivotField pivotField)
```


Fügt ein Pivot-Feld an einem bestimmten Index ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der Index. |
| pivotField | [PivotField](../../com.aspose.cells/pivotfield) | Das Feld. |

### iterator() {#iterator--}
```
public Iterator iterator()
```


Gibt einen Enumerator zurück, der die CollectionBase-Instanz durchläuft.

**Returns:**
java.util.Iterator - Ein Iterator für die CollectionBase-Instanz.
### move(int currPos, int destPos) {#move-int-int-}
```
public void move(int currPos, int destPos)
```


Verschiebt das PivotField von der aktuellen Position zur Zielposition

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| currPos | int | Aktuelle Position des PivotField basierend auf Null |
| destPos | int | Zielposition des PivotField basierend auf Null |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### remove(PivotField pivotField) {#remove-com.aspose.cells.PivotField-}
```
public void remove(PivotField pivotField)
```


Entfernt das Feld aus der aktuellen Region.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivotField | [PivotField](../../com.aspose.cells/pivotfield) |  |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Entfernt das Feld anhand des Index. Nur für Filter-, Zeilen-, Spalten- und Datenregion.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int |  |

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

