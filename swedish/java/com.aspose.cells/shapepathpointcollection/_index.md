---
title: "ShapePathPointCollection"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar alla formens sökvägspunkter."
type: docs
url: /sv/java/com.aspose.cells/shapepathpointcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ShapePathPointCollection extends CollectionBase
```

Representerar alla formens sökvägspunkter.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [ShapePathPointCollection()](#ShapePathPointCollection--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(int x, int y)](#add-int-int-) | Lägger till en banpunkt i enheten EMU. |
| [add(Object o)](#add-java.lang.Object-) | Lägger till ett objekt i CollectionBase-instansen. |
| [clear()](#clear--) | Tar bort alla objekt från CollectionBase-instansen. |
| [contains(Object o)](#contains-java.lang.Object-) | Returnerar om instansen innehåller detta objekt |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Hämtar banpunkt för formen efter index. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Hämtar antalet element som finns i CollectionBase-instansen. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Bestämmer indexet för ett specifikt objekt i CollectionBase-instansen. |
| [iterator()](#iterator--) | Returnerar en enumerator som itererar genom CollectionBase-instansen. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Tar bort objektet på det angivna indexet. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ShapePathPointCollection() {#ShapePathPointCollection--}
```
public ShapePathPointCollection()
```


### add(int x, int y) {#add-int-int-}
```
public int add(int x, int y)
```


Lägger till en banpunkt i enheten EMU.

**Remarks**

OBS: Den här medlemmen är nu föråldrad. Använd istället metoderna MoveTo,LineTo,CubicBezierTo och ArcTo i ShapePath. Denna metod kommer att tas bort 12 månader senare från och med augusti 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| x | int | x-koordinaten. |
| y | int | y-koordinaten. |

**Returns:**
int
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
public ShapePathPoint get(int index)
```


Hämtar banpunkt för formen efter index.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Indexet |

**Returns:**
[ShapePathPoint](../../com.aspose.cells/shapepathpoint) - Returns [ShapePathPoint](../../com.aspose.cells/shapepathpoint) object
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


Tar bort objektet på det angivna indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Det nollbaserade indexet för objektet som ska tas bort. |

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

