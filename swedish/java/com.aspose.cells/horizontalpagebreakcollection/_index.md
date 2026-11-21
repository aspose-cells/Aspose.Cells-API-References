---
title: "HorizontalPageBreakCollection"
second_title: "Aspose.Cells för Java API-referens"
description: "Inkapslar en samling av objekt."
type: docs
url: /sv/java/com.aspose.cells/horizontalpagebreakcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class HorizontalPageBreakCollection extends CollectionBase
```

Inkapslar en samling av [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak)-objekt.

**Example**

```
         Workbook excel = new Workbook();
 
         //Add a pagebreak at G5
         excel.getWorksheets().get(0).getHorizontalPageBreaks().add("G5");
         excel.getWorksheets().get(0).getVerticalPageBreaks().add("G5");
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(int row)](#add-int-) | Lägger till ett horisontellt sidbryt i samlingen. |
| [add(int row, int column)](#add-int-int-) | Lägger till ett horisontellt sidbryt i samlingen. |
| [add(int row, int startColumn, int endColumn)](#add-int-int-int-) | Lägger till ett horisontellt sidbryt i samlingen. |
| [add(Object o)](#add-java.lang.Object-) | Lägger till ett objekt i CollectionBase-instansen. |
| [add(String cellName)](#add-java.lang.String-) | Lägger till ett horisontellt sidbryt i samlingen. |
| [clear()](#clear--) | Tar bort alla objekt från CollectionBase-instansen. |
| [contains(Object o)](#contains-java.lang.Object-) | Returnerar om instansen innehåller detta objekt |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Hämtar [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak)-elementet på det angivna indexet. |
| [get(String cellName)](#get-java.lang.String-) | Hämtar [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak)-elementet med det angivna cellnamnet. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Hämtar antalet element som finns i CollectionBase-instansen. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Bestämmer indexet för ett specifikt objekt i CollectionBase-instansen. |
| [iterator()](#iterator--) | Returnerar en enumerator som itererar genom CollectionBase-instansen. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Tar bort HPageBreak-elementet med ett angivet namn. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int row) {#add-int-}
```
public int add(int row)
```


Lägger till ett horisontellt sidbryt i samlingen.

**Remarks**

Sidbryt läggs till i cellens övre vänstra hörn. Ställ in ett horisontellt sidbryt och ett vertikalt sidbryt samtidigt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Cellradindex, nollbaserad. |

**Returns:**
int - [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak)-objektindex.
### add(int row, int column) {#add-int-int-}
```
public int add(int row, int column)
```


Lägger till ett horisontellt sidbryt i samlingen.

**Remarks**

Sidbryt läggs till i cellens övre vänstra hörn. Ställ in ett horisontellt sidbryt och ett vertikalt sidbryt samtidigt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Cellradindex, nollbaserad. |
| kolumn | int | Cellkolumnindex, nollbaserad. |

**Returns:**
int - [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak)-objektindex.
### add(int row, int startColumn, int endColumn) {#add-int-int-int-}
```
public int add(int row, int startColumn, int endColumn)
```


Lägger till ett horisontellt sidbryt i samlingen.

**Remarks**

Denna metod används för att lägga till ett horisontellt sidbryt inom ett utskriftsområde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindex, nollbaserat. |
| startColumn | int | Startkolumnindex, nollbaserat. |
| endColumn | int | Slutkolumnindex, nollbaserat. |

**Returns:**
int - [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak)-objektindex.
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


Lägger till ett horisontellt sidbryt i samlingen.

**Remarks**

Sidbryt läggs till i cellens övre vänstra hörn. Ställ in ett horisontellt sidbryt och ett vertikalt sidbryt samtidigt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellNamn | java.lang.String | Cellnamn. |

**Returns:**
int - [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak)-objektindex.
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
public HorizontalPageBreak get(int index)
```


Hämtar [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak)-elementet på det angivna indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Det nollbaserade indexet för elementet. |

**Returns:**
[HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) - The element at the specified index.
### get(String cellName) {#get-java.lang.String-}
```
public HorizontalPageBreak get(String cellName)
```


Hämtar [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak)-elementet med det angivna cellnamnet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellNamn | java.lang.String | Cellnamn. |

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


Tar bort HPageBreak-elementet med ett angivet namn.

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

