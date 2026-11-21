---
title: "OleObjectCollection"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar inbäddade OLE-objekt."
type: docs
url: /sv/java/com.aspose.cells/oleobjectcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class OleObjectCollection extends CollectionBase
```

Representerar inbäddade OLE-objekt.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(int topRow, int leftColumn, int height, int width, byte[] imageData)](#add-int-int-int-int-byte---) | Lägger till ett OleObject i samlingen. |
| [add(int topRow, int leftColumn, int height, int width, byte[] imageData, String linkedFile)](#add-int-int-int-int-byte---java.lang.String-) | Lägger till ett länkat OleObject i samlingen. |
| [add(Object o)](#add-java.lang.Object-) | Lägger till ett objekt i CollectionBase-instansen. |
| [clear()](#clear--) | Ta bort alla inbäddade OLE-objekt. |
| [contains(Object o)](#contains-java.lang.Object-) | Returnerar om instansen innehåller detta objekt |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Hämtar [OleObject](../../com.aspose.cells/oleobject)-elementet på det angivna indexet. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Hämtar antalet element som finns i CollectionBase-instansen. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Bestämmer indexet för ett specifikt objekt i CollectionBase-instansen. |
| [iterator()](#iterator--) | Returnerar en enumerator som itererar genom CollectionBase-instansen. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Tar bort elementet på det angivna indexet. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int topRow, int leftColumn, int height, int width, byte[] imageData) {#add-int-int-int-int-byte---}
```
public int add(int topRow, int leftColumn, int height, int width, byte[] imageData)
```


Lägger till ett OleObject i samlingen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | int | Övre vänstra radindex. |
| leftColumn | int | Övre vänstra kolumnindex. |
| höjd | int | Höjd för oleObject, i enheten pixel. |
| bredd | int | Bredd för oleObject, i enheten pixel. |
| imageData | byte[] | Bild av ole-objekt som bytearray. |

**Returns:**
int - [OleObject](../../com.aspose.cells/oleobject) objektindex.
### add(int topRow, int leftColumn, int height, int width, byte[] imageData, String linkedFile) {#add-int-int-int-int-byte---java.lang.String-}
```
public int add(int topRow, int leftColumn, int height, int width, byte[] imageData, String linkedFile)
```


Lägger till ett länkat OleObject i samlingen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | int | Övre vänstra radindex. |
| leftColumn | int | Övre vänstra kolumnindex. |
| höjd | int | Höjd för oleObject, i enheten pixel. |
| bredd | int | Bredd för oleObject, i enheten pixel. |
| imageData | byte[] | Bild av ole-objekt som bytearray. |
| linkedFile | java.lang.String |  |

**Returns:**
int - [OleObject](../../com.aspose.cells/oleobject) objektindex.
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
### clear() {#clear--}
```
public void clear()
```


Ta bort alla inbäddade OLE-objekt.

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
public OleObject get(int index)
```


Hämtar [OleObject](../../com.aspose.cells/oleobject)-elementet på det angivna indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Det nollbaserade indexet för elementet. |

**Returns:**
[OleObject](../../com.aspose.cells/oleobject) - The element at the specified index.
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


Tar bort elementet på det angivna indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Det angivna indexet. |

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

