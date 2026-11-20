---
title: "CellWatchCollection"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Sammlung von Zellen in diesem Arbeitsblatt dar, die im Überwachungsfenster beobachtet werden."
type: docs
url: /de/java/com.aspose.cells/cellwatchcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class CellWatchCollection extends CollectionBase
```

Stellt die Sammlung von Zellen in diesem Arbeitsblatt dar, die im 'Watch-Fenster' überwacht werden.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         // Get the first Worksheet.
         Worksheet sheet = workbook.getWorksheets().get(0);
         // Add Cell Watch Item into the watch window
         sheet.getCellWatches().add("B2");
```
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [CellWatchCollection()](#CellWatchCollection--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add(int row, int column)](#add-int-int-) | Fügt [CellWatch](../../com.aspose.cells/cellwatch) mit einer Zeile und einer Spalte hinzu. |
| [add(Object o)](#add-java.lang.Object-) | Fügt ein Element zur CollectionBase-Instanz hinzu. |
| [add(String cellName)](#add-java.lang.String-) | Fügt [CellWatch](../../com.aspose.cells/cellwatch) mit dem Namen der Zelle hinzu. |
| [clear()](#clear--) | Entfernt alle Objekte aus der CollectionBase-Instanz. |
| [contains(Object o)](#contains-java.lang.Object-) | Gibt zurück, ob die Instanz dieses Objekt enthält |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Liest und setzt [CellWatch](../../com.aspose.cells/cellwatch) nach Index. |
| [get(String cellName)](#get-java.lang.String-) | Liest und setzt [CellWatch](../../com.aspose.cells/cellwatch) nach dem Namen der Zelle. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ermittelt die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Bestimmt den Index eines bestimmten Elements in der CollectionBase-Instanz. |
| [iterator()](#iterator--) | Gibt einen Enumerator zurück, der die CollectionBase-Instanz durchläuft. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Entfernt das Element am angegebenen Index. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CellWatchCollection() {#CellWatchCollection--}
```
public CellWatchCollection()
```


### add(int row, int column) {#add-int-int-}
```
public int add(int row, int column)
```


Fügt [CellWatch](../../com.aspose.cells/cellwatch) mit einer Zeile und einer Spalte hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Der Zeilenindex. |
| Spalte | int | Der Spaltenindex. |

**Returns:**
int - Gibt die Position dieses Elements in der Sammlung zurück.
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


Fügt [CellWatch](../../com.aspose.cells/cellwatch) mit dem Namen der Zelle hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellName | java.lang.String | Der Name der Zelle. |

**Returns:**
int -
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
public CellWatch get(int index)
```


Liest und setzt [CellWatch](../../com.aspose.cells/cellwatch) nach Index.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der Index. |

**Returns:**
[CellWatch](../../com.aspose.cells/cellwatch) - 
### get(String cellName) {#get-java.lang.String-}
```
public CellWatch get(String cellName)
```


Liest und setzt [CellWatch](../../com.aspose.cells/cellwatch) nach dem Namen der Zelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellName | java.lang.String | Der Name der Zelle. |

**Returns:**
[CellWatch](../../com.aspose.cells/cellwatch) - 
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


Entfernt das Element am angegebenen Index.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der nullbasierte Index des zu entfernenden Elements. |

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

