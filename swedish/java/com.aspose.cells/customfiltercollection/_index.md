---
title: "CustomFilterCollection"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar de anpassade filtren."
type: docs
url: /sv/java/com.aspose.cells/customfiltercollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class CustomFilterCollection extends CollectionBase
```

Representerar de anpassade filtren.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [CustomFilterCollection()](#CustomFilterCollection--) | Skapar en ny instans. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Lägger till ett objekt i CollectionBase-instansen. |
| [clear()](#clear--) | Tar bort alla objekt från CollectionBase-instansen. |
| [contains(Object o)](#contains-java.lang.Object-) | Returnerar om instansen innehåller detta objekt |
| [custom(int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2)](#custom-int-java.lang.Object-boolean-int-java.lang.Object-) | Filtrerar en lista med anpassade kriterier. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Hämtar det anpassade filtret på det specifika indexet. |
| [getAnd()](#getAnd--) | Indikerar om de två kriterierna har ett "och"-förhållande. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Hämtar antalet element som finns i CollectionBase-instansen. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Bestämmer indexet för ett specifikt objekt i CollectionBase-instansen. |
| [iterator()](#iterator--) | Returnerar en enumerator som itererar genom CollectionBase-instansen. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Tar bort objektet på det angivna indexet. |
| [setAnd(boolean value)](#setAnd-boolean-) | Indikerar om de två kriterierna har ett "och"-förhållande. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CustomFilterCollection() {#CustomFilterCollection--}
```
public CustomFilterCollection()
```


Skapar en ny instans.

**Remarks**

OBS: Denna medlem är nu föråldrad. Istället, vänligen sätt FilterColumn.FilterType till FilterType.CustomFilters och hämta sedan FilterColumn.CustomFilters. Denna egenskap kommer att tas bort 12 månader senare från och med juni 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

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
### custom(int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2) {#custom-int-java.lang.Object-boolean-int-java.lang.Object-}
```
public void custom(int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2)
```


Filtrerar en lista med anpassade kriterier.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| operatorType1 | int | [FilterOperatorType](../../com.aspose.cells/filteroperatortype). Filteroperatortypen |
| criteria1 | java.lang.Object | Det anpassade kriteriet |
| isAnd | boolean |  |
| operatorType2 | int | [FilterOperatorType](../../com.aspose.cells/filteroperatortype). Filteroperatortypen |
| criteria2 | java.lang.Object | Det anpassade kriteriet |

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
public CustomFilter get(int index)
```


Hämtar det anpassade filtret på det specifika indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Indexet. |

**Returns:**
[CustomFilter](../../com.aspose.cells/customfilter) - 
### getAnd() {#getAnd--}
```
public boolean getAnd()
```


Indikerar om de två kriterierna har ett "och"-förhållande.

**Returns:**
boolean
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

### setAnd(boolean value) {#setAnd-boolean-}
```
public void setAnd(boolean value)
```


Indikerar om de två kriterierna har ett "och"-förhållande.

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

