---
title: "NameCollection"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar en samling av alla objekt i kalkylbladet."
type: docs
url: /sv/java/com.aspose.cells/namecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class NameCollection extends CollectionBase
```

Representerar en samling av alla [Name](../../com.aspose.cells/name)-objekt i kalkylbladet.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Lägger till ett objekt i CollectionBase-instansen. |
| [add(String text)](#add-java.lang.String-) | Definierar ett nytt namn. |
| [clear()](#clear--) | Ta bort alla definierade namn som inte refereras av formlerna och datakällan. |
| [contains(Object o)](#contains-java.lang.Object-) | Returnerar om instansen innehåller detta objekt |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filter(int type, int sheetIndex)](#filter-int-int-) | Hämtar alla definierade namn efter omfattning. |
| [get(int index)](#get-int-) | Hämtar [Name](../../com.aspose.cells/name)-elementet på det angivna indexet. |
| [get(String text)](#get-java.lang.String-) | Gets the [Name](../../com.aspose.cells/name)-elementet med det angivna namnet. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Hämtar antalet element som finns i CollectionBase-instansen. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Bestämmer indexet för ett specifikt objekt i CollectionBase-instansen. |
| [iterator()](#iterator--) | Returnerar en enumerator som itererar genom CollectionBase-instansen. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(String text)](#remove-java.lang.String-) | Ta bort namnet. |
| [remove(String[] names)](#remove-java.lang.String---) | Ta bort en array av namn. |
| [removeAt(int index)](#removeAt-int-) | Ta bort namnet på det specifika indexet. |
| [removeDuplicateNames()](#removeDuplicateNames--) | Ta bort de duplicerade definierade namnen. |
| [sort()](#sort--) | Sorterar definierade namn. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### add(String text) {#add-java.lang.String-}
```
public int add(String text)
```


Definierar ett nytt namn.

**Remarks**

Namnet får inte innehålla mellanslag och får inte se ut som cellreferenser.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| text | java.lang.String | Texten som ska användas som namn. |

**Returns:**
int - [Name](../../com.aspose.cells/name) objektindex.
### clear() {#clear--}
```
public void clear()
```


Ta bort alla definierade namn som inte refereras av formler och datakälla. Om det definierade namnet refereras, sätter vi bara Name.ReferTo till null och döljer dem.

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
### filter(int type, int sheetIndex) {#filter-int-int-}
```
public Name[] filter(int type, int sheetIndex)
```


Hämtar alla definierade namn efter omfattning.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| type | int | [NameScopeType](../../com.aspose.cells/namescopetype). Omfattningstypen. |
| sheetIndex | int | Bladindexet. Påverkar endast när omfattningstypen är [NameScopeType.WORKSHEET](../../com.aspose.cells/namescopetype\#WORKSHEET). |

**Returns:**
com.aspose.cells.Name[] -
### get(int index) {#get-int-}
```
public Name get(int index)
```


Hämtar [Name](../../com.aspose.cells/name)-elementet på det angivna indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Det nollbaserade indexet för elementet. |

**Returns:**
[Name](../../com.aspose.cells/name) - The element at the specified index.
### get(String text) {#get-java.lang.String-}
```
public Name get(String text)
```


Gets the [Name](../../com.aspose.cells/name)-elementet med det angivna namnet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| text | java.lang.String | Namnetext. |

**Returns:**
[Name](../../com.aspose.cells/name) - The element with the specified name.
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




### remove(String text) {#remove-java.lang.String-}
```
public void remove(String text)
```


Ta bort namnet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| text | java.lang.String | Namnetexten. |

### remove(String[] names) {#remove-java.lang.String---}
```
public void remove(String[] names)
```


Ta bort en array av namn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | java.lang.String[] | Texten för namnen. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Ta bort namnet på det specifika indexet.

**Remarks**

Se till att namnet inte refereras av andra formler innan metoden anropas. Och om namnet refereras är det bättre att sätta Name.RefersTo till null.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Index för namnet som ska tas bort. |

### removeDuplicateNames() {#removeDuplicateNames--}
```
public void removeDuplicateNames()
```


Ta bort de duplicerade definierade namnen.

### sort() {#sort--}
```
public void sort()
```


Sorterar definierade namn.

**Remarks**

Om du skapar ett stort antal namngivna områden i Excel-filen, anropa denna metod efter att alla namngivna områden har skapats och innan du sparar.

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

