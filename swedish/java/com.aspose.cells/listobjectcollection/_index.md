---
title: "ListObjectCollection"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar en samling av  objekt i kalkylbladet."
type: docs
url: /sv/java/com.aspose.cells/listobjectcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ListObjectCollection extends CollectionBase
```

Representerar en samling av [ListObject](../../com.aspose.cells/listobject) objekt i kalkylbladet.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders)](#add-int-int-int-int-boolean-) | Lägger till ett ListObject i kalkylbladet. |
| [add(Object o)](#add-java.lang.Object-) | Lägger till ett objekt i CollectionBase-instansen. |
| [add(String startCell, String endCell, boolean hasHeaders)](#add-java.lang.String-java.lang.String-boolean-) | Lägger till ett ListObject i kalkylbladet. |
| [clear()](#clear--) | Tar bort alla objekt från CollectionBase-instansen. |
| [contains(Object o)](#contains-java.lang.Object-) | Returnerar om instansen innehåller detta objekt |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Hämtar ListObject efter index. |
| [get(String tableName)](#get-java.lang.String-) | Hämtar ListObject efter angivet namn. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Hämtar antalet element som finns i CollectionBase-instansen. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Bestämmer indexet för ett specifikt objekt i CollectionBase-instansen. |
| [iterator()](#iterator--) | Returnerar en enumerator som itererar genom CollectionBase-instansen. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Ta bort [ListObject](../../com.aspose.cells/listobject) efter index. |
| [toString()](#toString--) |  |
| [updateColumnName()](#updateColumnName--) | Uppdatera alla kolumnnamn i tabellerna. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders) {#add-int-int-int-int-boolean-}
```
public int add(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders)
```


Lägger till ett ListObject i kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRad | int | Startraden för listintervallet. |
| startColumn | int | Startraden för listintervallet. |
| slutRad | int | Startraden för listintervallet. |
| endColumn | int | Startraden för listintervallet. |
| hasHeaders | boolean | Om intervallet har rubriker. |

**Returns:**
int - Indexet för det nya ListObject
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
### add(String startCell, String endCell, boolean hasHeaders) {#add-java.lang.String-java.lang.String-boolean-}
```
public int add(String startCell, String endCell, boolean hasHeaders)
```


Lägger till ett ListObject i kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startCell | java.lang.String | Startcellen för listintervallet. |
| endCell | java.lang.String | Slutcellen för listintervallet. |
| hasHeaders | boolean | Om intervallet har rubriker. |

**Returns:**
int - Indexet för det nya ListObject
### clear() {#clear--}
```
public void clear()
```


Tar bort alla objekt från CollectionBase-instansen.

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
public ListObject get(int index)
```


Hämtar ListObject efter index.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Indexet. |

**Returns:**
[ListObject](../../com.aspose.cells/listobject) - The ListObject
### get(String tableName) {#get-java.lang.String-}
```
public ListObject get(String tableName)
```


Hämtar ListObject efter angivet namn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| tableName | java.lang.String | ListObject namn. |

**Returns:**
[ListObject](../../com.aspose.cells/listobject) - The ListObject
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
### iterator() {#iterator--}
```
public Iterator iterator()
```


Returnerar en enumerator som itererar genom CollectionBase-instansen.

**Returns:**
java.util.Iterator - En iterator för CollectionBase-instansen.
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


Ta bort [ListObject](../../com.aspose.cells/listobject) efter index.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Indexet. |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### updateColumnName() {#updateColumnName--}
```
public void updateColumnName()
```


Uppdatera alla kolumnnamn i tabellerna.

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

