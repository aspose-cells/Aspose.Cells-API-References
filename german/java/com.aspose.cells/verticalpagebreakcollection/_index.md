---
title: "VerticalPageBreakCollection"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Kapselt eine Sammlung von Objekten."
type: docs
url: /de/java/com.aspose.cells/verticalpagebreakcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class VerticalPageBreakCollection extends CollectionBase
```

Kapselt eine Sammlung von [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak)-Objekten.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add(int column)](#add-int-) | Fügt der Sammlung einen vertikalen Seitenumbruch hinzu. |
| [add(int row, int column)](#add-int-int-) | Fügt der Sammlung einen vertikalen Seitenumbruch hinzu. |
| [add(int startRow, int endRow, int column)](#add-int-int-int-) | Fügt der Sammlung einen vertikalen Seitenumbruch hinzu. |
| [add(Object o)](#add-java.lang.Object-) | Fügt ein Element zur CollectionBase-Instanz hinzu. |
| [add(String cellName)](#add-java.lang.String-) | Fügt der Sammlung einen vertikalen Seitenumbruch hinzu. |
| [clear()](#clear--) | Entfernt alle Objekte aus der CollectionBase-Instanz. |
| [contains(Object o)](#contains-java.lang.Object-) | Gibt zurück, ob die Instanz dieses Objekt enthält |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Gibt das [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak)-Element am angegebenen Index zurück. |
| [get(String cellName)](#get-java.lang.String-) | Gibt das [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak)-Element mit dem angegebenen Zellnamen zurück. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ermittelt die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Bestimmt den Index eines bestimmten Elements in der CollectionBase-Instanz. |
| [iterator()](#iterator--) | Gibt einen Enumerator zurück, der die CollectionBase-Instanz durchläuft. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Entfernt das VPageBreak-Element mit einem angegebenen Namen. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int column) {#add-int-}
```
public int add(int column)
```


Fügt der Sammlung einen vertikalen Seitenumbruch hinzu.

**Remarks**

Der Seitenumbruch wird oben links in der Zelle hinzugefügt. Bitte setzen Sie gleichzeitig einen horizontalen und einen vertikalen Seitenumbruch.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Spalte | int | Spaltenindex der Zelle, nullbasiert. |

**Returns:**
int - [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) Objektindex.
### add(int row, int column) {#add-int-int-}
```
public int add(int row, int column)
```


Fügt der Sammlung einen vertikalen Seitenumbruch hinzu.

**Remarks**

Der Seitenumbruch wird oben links in der Zelle hinzugefügt. Bitte setzen Sie gleichzeitig einen horizontalen und einen vertikalen Seitenumbruch.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex der Zelle, nullbasiert. |
| Spalte | int | Spaltenindex der Zelle, nullbasiert. |

**Returns:**
int - [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) Objektindex.
### add(int startRow, int endRow, int column) {#add-int-int-int-}
```
public int add(int startRow, int endRow, int column)
```


Fügt der Sammlung einen vertikalen Seitenumbruch hinzu.

**Remarks**

Diese Methode wird verwendet, um einen vertikalen Seitenumbruch innerhalb eines Druckbereichs hinzuzufügen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | int | Startzeilenindex, nullbasiert. |
| endRow | int | Endzeilenindex, nullbasiert. |
| Spalte | int | Spaltenindex, nullbasiert. |

**Returns:**
int - [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) Objektindex.
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
### add(String cellName) {#add-java.lang.String-}
```
public int add(String cellName)
```


Fügt der Sammlung einen vertikalen Seitenumbruch hinzu.

**Remarks**

Der Seitenumbruch wird oben links in der Zelle hinzugefügt. Bitte setzen Sie gleichzeitig einen horizontalen und einen vertikalen Seitenumbruch.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellName | java.lang.String | Zellenname. |

**Returns:**
int - [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) Objektindex.
### clear() {#clear--}
```
public void clear()
```


Entfernt alle Objekte aus der CollectionBase-Instanz.

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
public VerticalPageBreak get(int index)
```


Gibt das [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak)-Element am angegebenen Index zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der nullbasierte Index des Elements. |

**Returns:**
[VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) - The element at the specified index.
### get(String cellName) {#get-java.lang.String-}
```
public VerticalPageBreak get(String cellName)
```


Gibt das [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak)-Element mit dem angegebenen Zellnamen zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellName | java.lang.String | Zellenname. |

**Returns:**
[VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) - The element with the specified cell name.
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
### iterator() {#iterator--}
```
public Iterator iterator()
```


Gibt einen Enumerator zurück, der die CollectionBase-Instanz durchläuft.

**Returns:**
java.util.Iterator - Ein Iterator für die CollectionBase-Instanz.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Entfernt das VPageBreak-Element mit einem angegebenen Namen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Elementindex, nullbasiert. |

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

