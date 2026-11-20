---
title: "NameCollection"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt eine Sammlung aller Objekte im Tabellenblatt dar."
type: docs
url: /de/java/com.aspose.cells/namecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class NameCollection extends CollectionBase
```

Stellt eine Sammlung aller [Name](../../com.aspose.cells/name)-Objekte im Tabellenblatt dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Fügt ein Element zur CollectionBase-Instanz hinzu. |
| [add(String text)](#add-java.lang.String-) | Definiert einen neuen Namen. |
| [clear()](#clear--) | Entfernt alle definierten Namen, die von den Formeln und der Datenquelle nicht referenziert werden. |
| [contains(Object o)](#contains-java.lang.Object-) | Gibt zurück, ob die Instanz dieses Objekt enthält |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filter(int type, int sheetIndex)](#filter-int-int-) | Ruft alle definierten Namen nach Geltungsbereich ab. |
| [get(int index)](#get-int-) | Ruft das [Name](../../com.aspose.cells/name)-Element am angegebenen Index ab. |
| [get(String text)](#get-java.lang.String-) | Ruft das [Name](../../com.aspose.cells/name)-Element mit dem angegebenen Namen ab. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ermittelt die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Bestimmt den Index eines bestimmten Elements in der CollectionBase-Instanz. |
| [iterator()](#iterator--) | Gibt einen Enumerator zurück, der die CollectionBase-Instanz durchläuft. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(String text)](#remove-java.lang.String-) | Entfernt den Namen. |
| [remove(String[] names)](#remove-java.lang.String---) | Entfernt ein Array von Namen. |
| [removeAt(int index)](#removeAt-int-) | Entfernt den Namen am angegebenen Index. |
| [removeDuplicateNames()](#removeDuplicateNames--) | Entfernt die doppelten definierten Namen. |
| [sort()](#sort--) | Sortiert definierte Namen. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### add(String text) {#add-java.lang.String-}
```
public int add(String text)
```


Definiert einen neuen Namen.

**Remarks**

Der Name darf keine Leerzeichen enthalten und darf nicht wie Zellreferenzen aussehen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Text | java.lang.String | Der Text, der als Name verwendet werden soll. |

**Returns:**
int – [Name](../../com.aspose.cells/name)-Objektindex.
### clear() {#clear--}
```
public void clear()
```


Entfernt alle definierten Namen, die von den Formeln und der Datenquelle nicht referenziert werden. Wenn der definierte Name referenziert wird, setzen wir nur Name.ReferTo auf null und blenden ihn aus.

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
### filter(int type, int sheetIndex) {#filter-int-int-}
```
public Name[] filter(int type, int sheetIndex)
```


Ruft alle definierten Namen nach Geltungsbereich ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| type | int | [NameScopeType](../../com.aspose.cells/namescopetype). Der Geltungsbereichstyp. |
| sheetIndex | int | Der Blattindex. Wirkt nur, wenn der Geltungsbereichstyp [NameScopeType.WORKSHEET](../../com.aspose.cells/namescopetype\#WORKSHEET) ist. |

**Returns:**
com.aspose.cells.Name[] -
### get(int index) {#get-int-}
```
public Name get(int index)
```


Ruft das [Name](../../com.aspose.cells/name)-Element am angegebenen Index ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der nullbasierte Index des Elements. |

**Returns:**
[Name](../../com.aspose.cells/name) - The element at the specified index.
### get(String text) {#get-java.lang.String-}
```
public Name get(String text)
```


Ruft das [Name](../../com.aspose.cells/name)-Element mit dem angegebenen Namen ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Text | java.lang.String | Namentext. |

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




### remove(String text) {#remove-java.lang.String-}
```
public void remove(String text)
```


Entfernt den Namen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Text | java.lang.String | Der Namentext. |

### remove(String[] names) {#remove-java.lang.String---}
```
public void remove(String[] names)
```


Entfernt ein Array von Namen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Namen | java.lang.String[] | Der Text der Namen. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Entfernt den Namen am angegebenen Index.

**Remarks**

Bitte stellen Sie sicher, dass der Name nicht von anderen Formeln referenziert wird, bevor Sie die Methode aufrufen. Und wenn der Name referenziert wird, ist es besser, Name.RefersTo auf null zu setzen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Index des zu entfernenden Namens. |

### removeDuplicateNames() {#removeDuplicateNames--}
```
public void removeDuplicateNames()
```


Entfernt die doppelten definierten Namen.

### sort() {#sort--}
```
public void sort()
```


Sortiert definierte Namen.

**Remarks**

Wenn Sie eine große Anzahl benannter Bereiche in der Excel-Datei erstellen, rufen Sie diese Methode bitte auf, nachdem alle benannten Bereiche erstellt wurden und bevor Sie speichern.

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

