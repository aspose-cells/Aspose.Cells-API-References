---
title: "MultipleFilterCollection"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Sammlung mehrerer Filter dar."
type: docs
url: /de/java/com.aspose.cells/multiplefiltercollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class MultipleFilterCollection implements Iterable
```

Stellt die Sammlung mehrerer Filter dar.

**Remarks**

HINWEIS: Diese Klasse ist jetzt veraltet. Verwenden Sie stattdessen [FilterValueCollection](../../com.aspose.cells/filtervaluecollection). Diese Eigenschaft wird 12 Monate später, seit Juni 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [MultipleFilterCollection()](#MultipleFilterCollection--) | Erstellt eine neue Instanz. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add(int type, int year, int month, int day)](#add-int-int-int-int-) | Fügt einen Datumsfilterkriterienwert hinzu. |
| [add(int type, int year, int month, int day, int hour, int minute, int second)](#add-int-int-int-int-int-int-int-) | Fügt einen Datum‑Uhrzeit‑Filterkriterienwert hinzu. |
| [add(String filter)](#add-java.lang.String-) | Fügt ein Beschriftungsfilterkriterium hinzu. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Liefert [DateTimeGroupItem](../../com.aspose.cells/datetimegroupitem) oder einen Zeichenkettenwert. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Liefert die Anzahl der Filterwerte. |
| [getMatchBlank()](#getMatchBlank--) | Gibt an, ob nach leeren Werten gefiltert werden soll. |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Erhalte den Enumerator für den Filterwert, |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setMatchBlank(boolean value)](#setMatchBlank-boolean-) | Gibt an, ob nach leeren Werten gefiltert werden soll. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### MultipleFilterCollection() {#MultipleFilterCollection--}
```
public MultipleFilterCollection()
```


Erstellt eine neue Instanz.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen FilterColumn.FilterType auf FilterType.MultipleFilters setzen und dann FilterColumn.MultipleFilters abrufen. Diese Eigenschaft wird 12 Monate später, seit Juni 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### add(int type, int year, int month, int day) {#add-int-int-int-int-}
```
public void add(int type, int year, int month, int day)
```


Fügt einen Datumsfilterkriterienwert hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| type | int | [DateTimeGroupingType](../../com.aspose.cells/datetimegroupingtype). Der Typ des Datumsfilters. |
| Jahr | int | Das Jahr. |
| Monat | int | Der Monat. |
| Tag | int | Der Tag. |

### add(int type, int year, int month, int day, int hour, int minute, int second) {#add-int-int-int-int-int-int-int-}
```
public void add(int type, int year, int month, int day, int hour, int minute, int second)
```


Fügt einen Datum‑Uhrzeit‑Filterkriterienwert hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| type | int | [DateTimeGroupingType](../../com.aspose.cells/datetimegroupingtype). Der Typ des Datumsfilters. |
| Jahr | int | Das Jahr. |
| Monat | int | Der Monat. |
| Tag | int | Der Tag. |
| Stunde | int | Die Stunde. |
| Minute | int | Die Minute. |
| Sekunde | int | Die Sekunde. |

### add(String filter) {#add-java.lang.String-}
```
public void add(String filter)
```


Fügt ein Beschriftungsfilterkriterium hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Filter | java.lang.String | Die Filterdaten. |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### get(int index) {#get-int-}
```
public Object get(int index)
```


Liefert [DateTimeGroupItem](../../com.aspose.cells/datetimegroupitem) oder einen Zeichenkettenwert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int |  |

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


Liefert die Anzahl der Filterwerte.

**Returns:**
int
### getMatchBlank() {#getMatchBlank--}
```
public boolean getMatchBlank()
```


Gibt an, ob nach leeren Werten gefiltert werden soll.

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


Erhalte den Enumerator für den Filterwert,

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


Gibt an, ob nach leeren Werten gefiltert werden soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

