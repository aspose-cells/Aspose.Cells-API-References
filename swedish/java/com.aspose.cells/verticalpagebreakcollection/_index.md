---
title: "VerticalPageBreakCollection"
second_title: "Aspose.Cells för Java API-referens"
description: "Inkapslar en samling av objekt."
type: docs
url: /sv/java/com.aspose.cells/verticalpagebreakcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class VerticalPageBreakCollection extends CollectionBase
```

Inkapslar en samling av [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak)-objekt.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(int column)](#add-int-) | Lägger till ett vertikalt sidbryt i samlingen. |
| [add(int row, int column)](#add-int-int-) | Lägger till ett vertikalt sidbryt i samlingen. |
| [add(int startRow, int endRow, int column)](#add-int-int-int-) | Lägger till ett vertikalt sidbryt i samlingen. |
| [add(Object o)](#add-java.lang.Object-) | Lägger till ett objekt i CollectionBase-instansen. |
| [add(String cellName)](#add-java.lang.String-) | Lägger till ett vertikalt sidbryt i samlingen. |
| [clear()](#clear--) | Tar bort alla objekt från CollectionBase-instansen. |
| [contains(Object o)](#contains-java.lang.Object-) | Returnerar om instansen innehåller detta objekt |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Hämtar [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak)-elementet på det angivna indexet. |
| [get(String cellName)](#get-java.lang.String-) | Hämtar [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak)-elementet med det angivna cellnamnet. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Hämtar antalet element som finns i CollectionBase-instansen. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Bestämmer indexet för ett specifikt objekt i CollectionBase-instansen. |
| [iterator()](#iterator--) | Returnerar en enumerator som itererar genom CollectionBase-instansen. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Tar bort VPageBreak‑elementet med ett angivet namn. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int column) {#add-int-}
```
public int add(int column)
```


Lägger till ett vertikalt sidbryt i samlingen.

**Remarks**

Sidbryt läggs till i cellens övre vänstra hörn. Ställ in ett horisontellt sidbryt och ett vertikalt sidbryt samtidigt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kolumn | int | Cellkolumnindex, nollbaserad. |

**Returns:**
int - [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) objektindex.
### add(int row, int column) {#add-int-int-}
```
public int add(int row, int column)
```


Lägger till ett vertikalt sidbryt i samlingen.

**Remarks**

Sidbryt läggs till i cellens övre vänstra hörn. Ställ in ett horisontellt sidbryt och ett vertikalt sidbryt samtidigt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Cellradindex, nollbaserad. |
| kolumn | int | Cellkolumnindex, nollbaserad. |

**Returns:**
int - [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) objektindex.
### add(int startRow, int endRow, int column) {#add-int-int-int-}
```
public int add(int startRow, int endRow, int column)
```


Lägger till ett vertikalt sidbryt i samlingen.

**Remarks**

Denna metod används för att lägga till en vertikal sidbrytning inom ett utskriftsområde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRad | int | Startradindex, nollbaserad. |
| slutRad | int | Slutradindex, nollbaserad. |
| kolumn | int | Kolumnindex, nollbaserad. |

**Returns:**
int - [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) objektindex.
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
### add(String cellName) {#add-java.lang.String-}
```
public int add(String cellName)
```


Lägger till ett vertikalt sidbryt i samlingen.

**Remarks**

Sidbryt läggs till i cellens övre vänstra hörn. Ställ in ett horisontellt sidbryt och ett vertikalt sidbryt samtidigt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellNamn | java.lang.String | Cellnamn. |

**Returns:**
int - [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) objektindex.
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
public VerticalPageBreak get(int index)
```


Hämtar [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak)-elementet på det angivna indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Det nollbaserade indexet för elementet. |

**Returns:**
[VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) - The element at the specified index.
### get(String cellName) {#get-java.lang.String-}
```
public VerticalPageBreak get(String cellName)
```


Hämtar [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak)-elementet med det angivna cellnamnet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellNamn | java.lang.String | Cellnamn. |

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


Tar bort VPageBreak‑elementet med ett angivet namn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Elementindex, nollbaserad. |

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

