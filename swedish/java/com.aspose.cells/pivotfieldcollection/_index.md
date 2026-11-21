---
title: "PivotFieldCollection"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar en samling av alla PivotField‑objekt i de olika regionerna i pivottabellen."
type: docs
url: /sv/java/com.aspose.cells/pivotfieldcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PivotFieldCollection extends CollectionBase
```

Representerar en samling av alla PivotField‑objekt i de olika regionerna i pivottabellen.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(PivotField pivotField)](#add-com.aspose.cells.PivotField-) | Lägger till ett PivotField Object till den specifika typen PivotFields. |
| [add(Object o)](#add-java.lang.Object-) | Lägger till ett objekt i CollectionBase-instansen. |
| [addByBaseIndex(int baseFieldIndex)](#addByBaseIndex-int-) | Lägger till ett PivotField Object till den specifika typen PivotFields. |
| [clear()](#clear--) | rensa alla fält i PivotFieldCollection |
| [contains(Object o)](#contains-java.lang.Object-) | Returnerar om instansen innehåller detta objekt |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Hämtar PivotField-objektet på det specifika indexet. |
| [get(String name)](#get-java.lang.String-) | Hämtar PivotField-objektet med det specifika namnet. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Hämtar antalet element som finns i CollectionBase-instansen. |
| [getType()](#getType--) | Hämtar typen för PivotFields. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Bestämmer indexet för ett specifikt objekt i CollectionBase-instansen. |
| [insert(int index, PivotField pivotField)](#insert-int-com.aspose.cells.PivotField-) | Infoga ett pivottfält på ett specifikt index. |
| [iterator()](#iterator--) | Returnerar en enumerator som itererar genom CollectionBase-instansen. |
| [move(int currPos, int destPos)](#move-int-int-) | Flyttar PivotField från aktuell position till destinationsposition |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(PivotField pivotField)](#remove-com.aspose.cells.PivotField-) | Tar bort fältet från den aktuella regionen. |
| [removeAt(int index)](#removeAt-int-) | Tar bort fältet efter indexet. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(PivotField pivotField) {#add-com.aspose.cells.PivotField-}
```
public int add(PivotField pivotField)
```


Lägger till ett PivotField Object till den specifika typen PivotFields.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivotField | [PivotField](../../com.aspose.cells/pivotfield) | ett PivotField-objekt. |

**Returns:**
int – indexet för PivotField-objektet i dessa PivotFields.
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Lägger till ett objekt i CollectionBase-instansen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| o | java.lang.Object | Objektet som ska läggas till i CollectionBase-instansen. |

**Returns:**
int - Positionen där det nya elementet infördes.
### addByBaseIndex(int baseFieldIndex) {#addByBaseIndex-int-}
```
public int addByBaseIndex(int baseFieldIndex)
```


Lägger till ett PivotField Object till den specifika typen PivotFields.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| baseFieldIndex | int | fältindex i de grundläggande PivotFields. |

**Returns:**
int – indexet för PivotField-objektet i dessa PivotFields.
### clear() {#clear--}
```
public void clear()
```


rensa alla fält i PivotFieldCollection

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Returnerar om instansen innehåller detta objekt

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| o | java.lang.Object | testobjekt |

**Returns:**
boolean - Om instansen innehåller detta objekt
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### get(int index) {#get-int-}
```
public PivotField get(int index)
```


Hämtar PivotField-objektet på det specifika indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int |  |

**Returns:**
[PivotField](../../com.aspose.cells/pivotfield)
### get(String name) {#get-java.lang.String-}
```
public PivotField get(String name)
```


Hämtar PivotField-objektet med det specifika namnet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String |  |

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


Hämtar antalet element som finns i CollectionBase-instansen.

**Returns:**
int - Antalet element som finns i CollectionBase-instansen.
### getType() {#getType--}
```
public int getType()
```


Hämtar typen för PivotFields.

Se [PivotFieldType](../../com.aspose.cells/pivotfieldtype).

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


Bestämmer indexet för ett specifikt objekt i CollectionBase-instansen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| o | java.lang.Object | Bestämmer indexet för ett specifikt objekt i CollectionBase-instansen. |

**Returns:**
int - Indexet för värdet om det hittas i listan; annars -1.
### insert(int index, PivotField pivotField) {#insert-int-com.aspose.cells.PivotField-}
```
public void insert(int index, PivotField pivotField)
```


Infoga ett pivottfält på ett specifikt index.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Indexet. |
| pivotField | [PivotField](../../com.aspose.cells/pivotfield) | Fältet. |

### iterator() {#iterator--}
```
public Iterator iterator()
```


Returnerar en enumerator som itererar genom CollectionBase-instansen.

**Returns:**
java.util.Iterator - En iterator för CollectionBase-instansen.
### move(int currPos, int destPos) {#move-int-int-}
```
public void move(int currPos, int destPos)
```


Flyttar PivotField från aktuell position till destinationsposition

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| currPos | int | Aktuell position för PivotField baserat på noll |
| destPos | int | Destinationsposition för PivotField baserat på noll |

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


Tar bort fältet från den aktuella regionen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivotField | [PivotField](../../com.aspose.cells/pivotfield) |  |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Tar bort fältet efter indexet. Endast för filter-, rad-, kolumn- och dataregion.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int |  |

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

