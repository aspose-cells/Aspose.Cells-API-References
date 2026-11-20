---
title: "HorizontalPageBreakCollection"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Kapselt eine Sammlung von Objekten."
type: docs
url: /de/java/com.aspose.cells/horizontalpagebreakcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class HorizontalPageBreakCollection extends CollectionBase
```

Kapselt eine Sammlung von [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak)-Objekten.

**Example**

```
         Workbook excel = new Workbook();
 
         //Add a pagebreak at G5
         excel.getWorksheets().get(0).getHorizontalPageBreaks().add("G5");
         excel.getWorksheets().get(0).getVerticalPageBreaks().add("G5");
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add(int row)](#add-int-) | Fügt der Sammlung einen horizontalen Seitenumbruch hinzu. |
| [add(int row, int column)](#add-int-int-) | Fügt der Sammlung einen horizontalen Seitenumbruch hinzu. |
| [add(int row, int startColumn, int endColumn)](#add-int-int-int-) | Fügt der Sammlung einen horizontalen Seitenumbruch hinzu. |
| [add(Object o)](#add-java.lang.Object-) | Fügt ein Element zur CollectionBase-Instanz hinzu. |
| [add(String cellName)](#add-java.lang.String-) | Fügt der Sammlung einen horizontalen Seitenumbruch hinzu. |
| [clear()](#clear--) | Entfernt alle Objekte aus der CollectionBase-Instanz. |
| [contains(Object o)](#contains-java.lang.Object-) | Gibt zurück, ob die Instanz dieses Objekt enthält |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Liefert das [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak)-Element am angegebenen Index. |
| [get(String cellName)](#get-java.lang.String-) | Liefert das [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak)-Element mit dem angegebenen Zellnamen. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ermittelt die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Bestimmt den Index eines bestimmten Elements in der CollectionBase-Instanz. |
| [iterator()](#iterator--) | Gibt einen Enumerator zurück, der die CollectionBase-Instanz durchläuft. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Entfernt das HPageBreak-Element mit einem angegebenen Namen. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int row) {#add-int-}
```
public int add(int row)
```


Fügt der Sammlung einen horizontalen Seitenumbruch hinzu.

**Remarks**

Der Seitenumbruch wird oben links in der Zelle hinzugefügt. Bitte setzen Sie gleichzeitig einen horizontalen und einen vertikalen Seitenumbruch.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex der Zelle, nullbasiert. |

**Returns:**
int - Index des [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak)-Objekts.
### add(int row, int column) {#add-int-int-}
```
public int add(int row, int column)
```


Fügt der Sammlung einen horizontalen Seitenumbruch hinzu.

**Remarks**

Der Seitenumbruch wird oben links in der Zelle hinzugefügt. Bitte setzen Sie gleichzeitig einen horizontalen und einen vertikalen Seitenumbruch.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex der Zelle, nullbasiert. |
| Spalte | int | Spaltenindex der Zelle, nullbasiert. |

**Returns:**
int - Index des [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak)-Objekts.
### add(int row, int startColumn, int endColumn) {#add-int-int-int-}
```
public int add(int row, int startColumn, int endColumn)
```


Fügt der Sammlung einen horizontalen Seitenumbruch hinzu.

**Remarks**

Diese Methode wird verwendet, um einen horizontalen Seitenumbruch innerhalb eines Druckbereichs hinzuzufügen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex, nullbasiert. |
| startColumn | int | Startspaltenindex, nullbasiert. |
| endColumn | int | Endspaltenindex, nullbasiert. |

**Returns:**
int - Index des [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak)-Objekts.
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


Fügt der Sammlung einen horizontalen Seitenumbruch hinzu.

**Remarks**

Der Seitenumbruch wird oben links in der Zelle hinzugefügt. Bitte setzen Sie gleichzeitig einen horizontalen und einen vertikalen Seitenumbruch.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellName | java.lang.String | Zellenname. |

**Returns:**
int - Index des [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak)-Objekts.
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
public HorizontalPageBreak get(int index)
```


Liefert das [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak)-Element am angegebenen Index.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der nullbasierte Index des Elements. |

**Returns:**
[HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) - The element at the specified index.
### get(String cellName) {#get-java.lang.String-}
```
public HorizontalPageBreak get(String cellName)
```


Liefert das [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak)-Element mit dem angegebenen Zellnamen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellName | java.lang.String | Zellenname. |

**Returns:**
[HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) - The element with the specified cell name.
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


Entfernt das HPageBreak-Element mit einem angegebenen Namen.

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

