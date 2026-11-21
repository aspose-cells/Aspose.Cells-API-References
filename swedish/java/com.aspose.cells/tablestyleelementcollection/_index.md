---
title: "TableStyleElementCollection"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar alla element i tabellstilen."
type: docs
url: /sv/java/com.aspose.cells/tablestyleelementcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class TableStyleElementCollection extends CollectionBase
```

Representerar alla element i tabellstilen.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(int type)](#add-int-) | Lägger till ett element. |
| [add(Object o)](#add-java.lang.Object-) | Lägger till ett objekt i CollectionBase-instansen. |
| [clear()](#clear--) | Tar bort alla objekt från CollectionBase-instansen. |
| [contains(Object o)](#contains-java.lang.Object-) | Returnerar om instansen innehåller detta objekt |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Hämtar ett element i tabellstilen efter index. |
| [getByTableStyleElementType(int type)](#getByTableStyleElementType-int-) | Hämtar elementet i tabellstilen efter elementtypen. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Hämtar antalet element som finns i CollectionBase-instansen. |
| [getTableStyleElementWithIndex(int index)](#getTableStyleElementWithIndex-int-) | Hämtar ett element i tabellstilen efter index. |
| [getTableStyleElementWithType(int type)](#getTableStyleElementWithType-int-) | Hämtar elementet i tabellstilen efter elementtypen. |
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
### add(int type) {#add-int-}
```
public int add(int type)
```


Lägger till ett element.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| type | int | [TableStyleElementType](../../com.aspose.cells/tablestyleelementtype). Typen av elementet |

**Returns:**
int - Returnerar elementets index i listan.
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
public TableStyleElement get(int index)
```


Hämtar ett element i tabellstilen efter index.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Indexet. |

**Returns:**
[TableStyleElement](../../com.aspose.cells/tablestyleelement) - Returns [TableStyleElement](../../com.aspose.cells/tablestyleelement) object
### getByTableStyleElementType(int type) {#getByTableStyleElementType-int-}
```
public TableStyleElement getByTableStyleElementType(int type)
```


Hämtar elementet i tabellstilen efter elementtypen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| type | int | [TableStyleElementType](../../com.aspose.cells/tablestyleelementtype). Elementtypen. |

**Returns:**
[TableStyleElement](../../com.aspose.cells/tablestyleelement) - Returns [TableStyleElement](../../com.aspose.cells/tablestyleelement) object
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
### getTableStyleElementWithIndex(int index) {#getTableStyleElementWithIndex-int-}
```
public TableStyleElement getTableStyleElementWithIndex(int index)
```


Hämtar ett element i tabellstilen efter index.

**Remarks**

OBS: Detta medlem är nu föråldrad. Använd i stället **Aspose.Cells.Tables.TableStyleElementCollection.this[int index]**-egenskapen. Denna egenskap kommer att tas bort 12 månader senare sedan JANUARY 2012. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int |  |

**Returns:**
[TableStyleElement](../../com.aspose.cells/tablestyleelement)
### getTableStyleElementWithType(int type) {#getTableStyleElementWithType-int-}
```
public TableStyleElement getTableStyleElementWithType(int type)
```


Hämtar elementet i tabellstilen efter elementtypen.

**Remarks**

OBS: Detta medlem är nu föråldrad. Använd i stället **Aspose.Cells.Tables.TableStyleElementCollection.this[TableStyleElementType type]**-egenskapen. Denna egenskap kommer att tas bort 12 månader senare sedan JANUARY 2012. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | int |  |

**Returns:**
[TableStyleElement](../../com.aspose.cells/tablestyleelement)
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

