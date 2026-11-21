---
title: "MultipleFilterCollection"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar samlingen av flera filter."
type: docs
url: /sv/java/com.aspose.cells/multiplefiltercollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class MultipleFilterCollection implements Iterable
```

Representerar samlingen av flera filter.

**Remarks**

OBS: Denna klass är nu föråldrad. Använd istället [FilterValueCollection](../../com.aspose.cells/filtervaluecollection). Denna egenskap kommer att tas bort 12 månader senare från och med juni 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [MultipleFilterCollection()](#MultipleFilterCollection--) | Skapar en ny instans. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(int type, int year, int month, int day)](#add-int-int-int-int-) | Lägger till ett datumfilterkriterievärde. |
| [add(int type, int year, int month, int day, int hour, int minute, int second)](#add-int-int-int-int-int-int-int-) | Lägger till ett datum‑tidsfilterkriterievärde. |
| [add(String filter)](#add-java.lang.String-) | Lägger till ett etikettfilterkriterium. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Hämtar [DateTimeGroupItem](../../com.aspose.cells/datetimegroupitem) eller ett strängvärde. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Hämtar antalet filtervärden. |
| [getMatchBlank()](#getMatchBlank--) | Anger om man ska filtrera på tomma. |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Hämta enumeratorn för filtervärdet, |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setMatchBlank(boolean value)](#setMatchBlank-boolean-) | Anger om man ska filtrera på tomma. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### MultipleFilterCollection() {#MultipleFilterCollection--}
```
public MultipleFilterCollection()
```


Skapar en ny instans.

**Remarks**

OBS: Detta medlem är nu föråldrad. Ställ istället in FilterColumn.FilterType till FilterType.MultipleFilters och hämta sedan FilterColumn.MultipleFilters. Denna egenskap kommer att tas bort 12 månader senare från och med juni 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

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

### add(String filter) {#add-java.lang.String-}
```
public void add(String filter)
```


Lägger till ett etikettfilterkriterium.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filter | java.lang.String | Filterdata. |

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
public Object get(int index)
```


Hämtar [DateTimeGroupItem](../../com.aspose.cells/datetimegroupitem) eller ett strängvärde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int |  |

**Returns:**
java.lang.Object - 
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


Hämtar antalet filtervärden.

**Returns:**
int
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
### iterator() {#iterator--}
```
public Iterator iterator()
```


Hämta enumeratorn för filtervärdet,

**Returns:**
java.util.Iterator -
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




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

