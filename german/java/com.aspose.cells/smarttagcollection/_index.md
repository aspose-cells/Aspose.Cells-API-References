---
title: "SmartTagCollection"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt alle SmartTags in der Zelle dar."
type: docs
url: /de/java/com.aspose.cells/smarttagcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class SmartTagCollection extends CollectionBase
```

Stellt alle SmartTags in der Zelle dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Fügt ein Element zur CollectionBase-Instanz hinzu. |
| [add(String uri, String name)](#add-java.lang.String-java.lang.String-) | Fügt ein Smart-Tag hinzu. |
| [clear()](#clear--) | Entfernt alle Objekte aus der CollectionBase-Instanz. |
| [contains(Object o)](#contains-java.lang.Object-) | Gibt zurück, ob die Instanz dieses Objekt enthält |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Liefert ein [SmartTag](../../com.aspose.cells/smarttag)-Objekt am angegebenen Index |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Liefert die Spalte der Zell‑Smart‑Tags. |
| [getCount()](#getCount--) | Ermittelt die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente. |
| [getRow()](#getRow--) | Liefert die Zeile der Zell‑Smart‑Tags. |
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
### add(String uri, String name) {#add-java.lang.String-java.lang.String-}
```
public int add(String uri, String name)
```


Fügt ein Smart-Tag hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| URI | java.lang.String | Gibt die Namespace-URI des Smart‑Tags an |
| Name | java.lang.String | Gibt den Namen des Smart‑Tags an. |

**Returns:**
int - Der Index des Smart‑Tags in der Liste.
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
public SmartTag get(int index)
```


Liefert ein [SmartTag](../../com.aspose.cells/smarttag)-Objekt am angegebenen Index

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der Index. |

**Returns:**
[SmartTag](../../com.aspose.cells/smarttag) - returns a [SmartTag](../../com.aspose.cells/smarttag) object.
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


Liefert die Spalte der Zell‑Smart‑Tags.

**Returns:**
int
### getCount() {#getCount--}
```
public int getCount()
```


Ermittelt die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente.

**Returns:**
int - Die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente.
### getRow() {#getRow--}
```
public int getRow()
```


Liefert die Zeile der Zell‑Smart‑Tags.

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

