---
title: "PivotFilterCollection"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt eine Sammlung aller PivotFilters dar."
type: docs
url: /de/java/com.aspose.cells/pivotfiltercollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PivotFilterCollection extends CollectionBase
```

Stellt eine Sammlung aller PivotFilters dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add(int fieldIndex, int type)](#add-int-int-) | Fügt ein PivotFilter-Objekt zum angegebenen Typ hinzu |
| [add(Object o)](#add-java.lang.Object-) | Fügt ein Element zur CollectionBase-Instanz hinzu. |
| [addDateFilter(int baseFieldIndex, int type, DateTime dateTime1, DateTime dateTime2)](#addDateFilter-int-int-com.aspose.cells.DateTime-com.aspose.cells.DateTime-) | Filtert nach Datumseinstellung der Zeilen- oder Spalten-Pivotfeldes. |
| [addLabelFilter(int baseFieldIndex, int type, String label1, String label2)](#addLabelFilter-int-int-java.lang.String-java.lang.String-) | Filtert nach Beschriftungen des Zeilen- oder Spalten-Pivotfeldes. |
| [addTop10Filter(int baseFieldIndex, int valueFieldIndex, int type, boolean isTop, int itemCount)](#addTop10Filter-int-int-int-boolean-int-) | Filtert nach Werten des Daten-Pivotfeldes. |
| [addValueFilter(int baseFieldIndex, int valueFieldIndex, int type, double value1, double value2)](#addValueFilter-int-int-int-double-double-) | Filtert nach Werten des Daten-Pivotfeldes. |
| [clear()](#clear--) | Entfernt alle Objekte aus der CollectionBase-Instanz. |
| [clearFilter(int fieldIndex)](#clearFilter-int-) | Löscht PivotFilter aus dem angegebenen PivotField |
| [contains(Object o)](#contains-java.lang.Object-) | Gibt zurück, ob die Instanz dieses Objekt enthält |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Ruft das pivotfilter-Objekt am angegebenen Index ab. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ermittelt die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Bestimmt den Index eines bestimmten Elements in der CollectionBase-Instanz. |
| [iterator()](#iterator--) | Gibt einen Enumerator zurück, der die CollectionBase-Instanz durchläuft. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Entfernt das Element am angegebenen Index. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int fieldIndex, int type) {#add-int-int-}
```
public int add(int fieldIndex, int type)
```


Fügt ein PivotFilter-Objekt zum angegebenen Typ hinzu

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Methoden PivotFilterCollection.AddValueFilter(), AddTop10Filter(), AddLabelFilter() und AddDateFilter(). Diese Methode wird 12 Monate später, seit November 2024, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldIndex | int | der PivotField-Index |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). der PivotFilter-Typ |

**Returns:**
int - der Index des PivotFilter-Objekts in dieser PivotFilterCollection.
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
### addDateFilter(int baseFieldIndex, int type, DateTime dateTime1, DateTime dateTime2) {#addDateFilter-int-int-com.aspose.cells.DateTime-com.aspose.cells.DateTime-}
```
public PivotFilter addDateFilter(int baseFieldIndex, int type, DateTime dateTime1, DateTime dateTime2)
```


Filtert nach Datumseinstellung der Zeilen- oder Spalten-Pivotfeldes.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| baseFieldIndex | int | Der Index des Feldes in der Quelle. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Der Typ der zu filternden Daten. |
| dateTime1 | [DateTime](../../com.aspose.cells/datetime) | Das Datumslabel der Filterbedingung |
| dateTime2 | [DateTime](../../com.aspose.cells/datetime) | Das obere Datumslabel der Zwischenfilterbedingung |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### addLabelFilter(int baseFieldIndex, int type, String label1, String label2) {#addLabelFilter-int-int-java.lang.String-java.lang.String-}
```
public PivotFilter addLabelFilter(int baseFieldIndex, int type, String label1, String label2)
```


Filtert nach Beschriftungen des Zeilen- oder Spalten-Pivotfeldes.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| baseFieldIndex | int | Der Index des Feldes in der Quelle. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Der Typ der zu filternden Daten. |
| label1 | java.lang.String | Das Label der Filterbedingung |
| label2 | java.lang.String | Das obere Label der Zwischenfilterbedingung |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### addTop10Filter(int baseFieldIndex, int valueFieldIndex, int type, boolean isTop, int itemCount) {#addTop10Filter-int-int-int-boolean-int-}
```
public PivotFilter addTop10Filter(int baseFieldIndex, int valueFieldIndex, int type, boolean isTop, int itemCount)
```


Filtert nach Werten des Daten-Pivotfeldes.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| baseFieldIndex | int | Der Index des Feldes in der Quelle. |
| valueFieldIndex | int | Der Index des Datenfelds im Datenbereich. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Der Typ der Datenfilterung. Es können nur Count, Sum und Percent sein. |
| isTop | boolean | Gibt an, ob der Filter von oben oder unten ist. |
| itemCount | int | Die Elementanzahl |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### addValueFilter(int baseFieldIndex, int valueFieldIndex, int type, double value1, double value2) {#addValueFilter-int-int-int-double-double-}
```
public PivotFilter addValueFilter(int baseFieldIndex, int valueFieldIndex, int type, double value1, double value2)
```


Filtert nach Werten des Daten-Pivotfeldes.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| baseFieldIndex | int | Der Index des Feldes in der Quelle. |
| valueFieldIndex | int | Der Index des Wertefelds im Wertebereich. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Der Typ der zu filternden Daten. |
| value1 | double | Der Wert der Filterbedingung |
| value2 | double | Der obere Grenzwert der Zwischenfilterbedingung |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### clear() {#clear--}
```
public void clear()
```


Entfernt alle Objekte aus der CollectionBase-Instanz.

### clearFilter(int fieldIndex) {#clearFilter-int-}
```
public void clearFilter(int fieldIndex)
```


Löscht PivotFilter aus dem angegebenen PivotField

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldIndex | int | der PivotField-Index |

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
### get(int index) {#get-int-}
```
public PivotFilter get(int index)
```


Ruft das pivotfilter-Objekt am angegebenen Index ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int |  |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
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

