---
title: "CustomFilterCollection"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die benutzerdefinierten Filter dar."
type: docs
url: /de/java/com.aspose.cells/customfiltercollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class CustomFilterCollection extends CollectionBase
```

Stellt die benutzerdefinierten Filter dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [CustomFilterCollection()](#CustomFilterCollection--) | Erstellt eine neue Instanz. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Fügt ein Element zur CollectionBase-Instanz hinzu. |
| [clear()](#clear--) | Entfernt alle Objekte aus der CollectionBase-Instanz. |
| [contains(Object o)](#contains-java.lang.Object-) | Gibt zurück, ob die Instanz dieses Objekt enthält |
| [custom(int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2)](#custom-int-java.lang.Object-boolean-int-java.lang.Object-) | Filtert eine Liste mit benutzerdefinierten Kriterien. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Ruft den benutzerdefinierten Filter am angegebenen Index ab. |
| [getAnd()](#getAnd--) | Gibt an, ob die beiden Kriterien eine "und"-Beziehung haben. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ermittelt die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Bestimmt den Index eines bestimmten Elements in der CollectionBase-Instanz. |
| [iterator()](#iterator--) | Gibt einen Enumerator zurück, der die CollectionBase-Instanz durchläuft. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Entfernt das Element am angegebenen Index. |
| [setAnd(boolean value)](#setAnd-boolean-) | Gibt an, ob die beiden Kriterien eine "und"-Beziehung haben. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CustomFilterCollection() {#CustomFilterCollection--}
```
public CustomFilterCollection()
```


Erstellt eine neue Instanz.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Stattdessen setzen Sie bitte FilterColumn.FilterType auf FilterType.CustomFilters und rufen dann FilterColumn.CustomFilters ab. Diese Eigenschaft wird 12 Monate später, seit Juni 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Fügt ein Element zur CollectionBase-Instanz hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | Das Objekt, das zur CollectionBase-Instanz hinzugefügt werden soll. |

**Returns:**
int - Die Position, an der das neue Element eingefügt wurde.
### clear() {#clear--}
```
public void clear()
```


Entfernt alle Objekte aus der CollectionBase-Instanz.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Gibt zurück, ob die Instanz dieses Objekt enthält

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | Testobjekt |

**Returns:**
boolean - Ob die Instanz dieses Objekt enthält
### custom(int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2) {#custom-int-java.lang.Object-boolean-int-java.lang.Object-}
```
public void custom(int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2)
```


Filtert eine Liste mit benutzerdefinierten Kriterien.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| operatorType1 | int | [FilterOperatorType](../../com.aspose.cells/filteroperatortype). Der Filteroperator-Typ |
| criteria1 | java.lang.Object | Das benutzerdefinierte Kriterium |
| isAnd | boolean |  |
| operatorType2 | int | [FilterOperatorType](../../com.aspose.cells/filteroperatortype). Der Filteroperator-Typ |
| criteria2 | java.lang.Object | Das benutzerdefinierte Kriterium |

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
public CustomFilter get(int index)
```


Ruft den benutzerdefinierten Filter am angegebenen Index ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der Index. |

**Returns:**
[CustomFilter](../../com.aspose.cells/customfilter) - 
### getAnd() {#getAnd--}
```
public boolean getAnd()
```


Gibt an, ob die beiden Kriterien eine "und"-Beziehung haben.

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


Ermittelt die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente.

**Returns:**
int - Die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente.
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


Bestimmt den Index eines bestimmten Elements in der CollectionBase-Instanz.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | Bestimmt den Index eines bestimmten Elements in der CollectionBase-Instanz. |

**Returns:**
int - Der Index des Wertes, falls in der Liste gefunden; sonst -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Gibt einen Enumerator zurück, der die CollectionBase-Instanz durchläuft.

**Returns:**
java.util.Iterator - Ein Iterator für die CollectionBase-Instanz.
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


Entfernt das Element am angegebenen Index.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der nullbasierte Index des zu entfernenden Elements. |

### setAnd(boolean value) {#setAnd-boolean-}
```
public void setAnd(boolean value)
```


Gibt an, ob die beiden Kriterien eine "und"-Beziehung haben.

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

