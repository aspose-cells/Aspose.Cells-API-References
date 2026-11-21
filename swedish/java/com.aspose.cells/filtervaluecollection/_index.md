---
title: "FilterValueCollection"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar samlingen av flera filter."
type: docs
url: /sv/java/com.aspose.cells/filtervaluecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class FilterValueCollection extends CollectionBase
```

Representerar samlingen av flera filter.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(int type, int year, int month, int day)](#add-int-int-int-int-) | Lägger till ett datumfilterkriterievärde. |
| [add(int type, int year, int month, int day, int hour, int minute, int second)](#add-int-int-int-int-int-int-int-) | Lägger till ett datum‑tidsfilterkriterievärde. |
| [add(Object o)](#add-java.lang.Object-) | Lägger till ett objekt i CollectionBase-instansen. |
| [add(String filter)](#add-java.lang.String-) | Lägger till ett etikettfilterkriterium. |
| [clear()](#clear--) | Tar bort alla objekt från CollectionBase-instansen. |
| [contains(Object o)](#contains-java.lang.Object-) | Returnerar om instansen innehåller detta objekt |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Hämtar [FilterValue](../../com.aspose.cells/filtervalue) efter index. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Hämtar antalet element som finns i CollectionBase-instansen. |
| [getMatchBlank()](#getMatchBlank--) | Anger om man ska filtrera på tomma. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Bestämmer indexet för ett specifikt objekt i CollectionBase-instansen. |
| [iterator()](#iterator--) | Returnerar en enumerator som itererar genom CollectionBase-instansen. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Tar bort objektet på det angivna indexet. |
| [setMatchBlank(boolean value)](#setMatchBlank-boolean-) | Anger om man ska filtrera på tomma. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int type, int year, int month, int day) {#add-int-int-int-int-}
```
public void add(int type, int year, int month, int day)
```


Lägger till ett datumfilterkriterievärde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| type | int | [DateTimeGroupingType](../../com.aspose.cells/datetimegroupingtype). Typen av datumfilter. |
| år | int | Året. |
| månad | int | Månad. |
| dag | int | Dag. |

### add(int type, int year, int month, int day, int hour, int minute, int second) {#add-int-int-int-int-int-int-int-}
```
public void add(int type, int year, int month, int day, int hour, int minute, int second)
```


Lägger till ett datum‑tidsfilterkriterievärde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| type | int | [DateTimeGroupingType](../../com.aspose.cells/datetimegroupingtype). Typen av datumfilter. |
| år | int | Året. |
| månad | int | Månad. |
| dag | int | Dag. |
| timme | int | Timmen. |
| minut | int | Minuten. |
| sekund | int | Sekunden. |

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
### add(String filter) {#add-java.lang.String-}
```
public void add(String filter)
```


Lägger till ett etikettfilterkriterium.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filter | java.lang.String | Filterdata. |

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
public FilterValue get(int index)
```


Hämtar [FilterValue](../../com.aspose.cells/filtervalue) efter index.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int |  |

**Returns:**
[FilterValue](../../com.aspose.cells/filtervalue) - 
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
### getMatchBlank() {#getMatchBlank--}
```
public boolean getMatchBlank()
```


Anger om man ska filtrera på tomma.

**Returns:**
boolean
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

### setMatchBlank(boolean value) {#setMatchBlank-boolean-}
```
public void setMatchBlank(boolean value)
```


Anger om man ska filtrera på tomma.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

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

