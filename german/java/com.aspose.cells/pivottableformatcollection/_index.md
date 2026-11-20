---
title: "PivotTableFormatCollection"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Sammlung von Formaten dar, die auf die PivotTable angewendet werden."
type: docs
url: /de/java/com.aspose.cells/pivottableformatcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PivotTableFormatCollection extends CollectionBase
```

Stellt die Sammlung von Formaten dar, die auf die PivotTable angewendet werden.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add()](#add--) | Füge ein [PivotTableFormat](../../com.aspose.cells/pivottableformat) hinzu. |
| [add(Object o)](#add-java.lang.Object-) | Fügt ein Element zur CollectionBase-Instanz hinzu. |
| [clear()](#clear--) | Entfernt alle Objekte aus der CollectionBase-Instanz. |
| [contains(Object o)](#contains-java.lang.Object-) | Gibt zurück, ob die Instanz dieses Objekt enthält |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [format(CellArea ca, Style style)](#format-com.aspose.cells.CellArea-com.aspose.cells.Style-) | Formatiert den ausgewählten Bereich der Pivot-Tabelle. |
| [format(PivotArea pivotArea, Style style)](#format-com.aspose.cells.PivotArea-com.aspose.cells.Style-) | Formatiert den ausgewählten Bereich der Pivot-Tabelle. |
| [format(int row, int column, Style style)](#format-int-int-com.aspose.cells.Style-) | Formatiert die Zelle im Pivot-Tabellenbereich |
| [formatArea(int axisType, int fieldPosition, int subtotalType, int selectionType, boolean isGrandRow, boolean isGrandColumn, Style style)](#formatArea-int-int-int-int-boolean-boolean-com.aspose.cells.Style-) | Formatiert den ausgewählten Bereich. |
| [get(int index)](#get-int-) | Ermittelt das Format anhand des Index. |
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
### add() {#add--}
```
public int add()
```


Füge ein [PivotTableFormat](../../com.aspose.cells/pivottableformat) hinzu.

**Returns:**
int - Der Index des neuen Formats.
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
### format(CellArea ca, Style style) {#format-com.aspose.cells.CellArea-com.aspose.cells.Style-}
```
public void format(CellArea ca, Style style)
```


Formatiert den ausgewählten Bereich der Pivot-Tabelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Der Bereich der Zellen. |
| style | [Style](../../com.aspose.cells/style) | Der Stil |

### format(PivotArea pivotArea, Style style) {#format-com.aspose.cells.PivotArea-com.aspose.cells.Style-}
```
public void format(PivotArea pivotArea, Style style)
```


Formatiert den ausgewählten Bereich der Pivot-Tabelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivotArea | [PivotArea](../../com.aspose.cells/pivotarea) | Der ausgewählte Pivot-Ansichtsbereich. |
| style | [Style](../../com.aspose.cells/style) | Die formatierte Einstellung. |

### format(int row, int column, Style style) {#format-int-int-com.aspose.cells.Style-}
```
public void format(int row, int column, Style style)
```


Formatiert die Zelle im Pivot-Tabellenbereich

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex der Zelle |
| Spalte | int | Spaltenindex der Zelle |
| style | [Style](../../com.aspose.cells/style) | Stil, der die Zelle formatieren soll |

### formatArea(int axisType, int fieldPosition, int subtotalType, int selectionType, boolean isGrandRow, boolean isGrandColumn, Style style) {#formatArea-int-int-int-int-boolean-boolean-com.aspose.cells.Style-}
```
public PivotTableFormat formatArea(int axisType, int fieldPosition, int subtotalType, int selectionType, boolean isGrandRow, boolean isGrandColumn, Style style)
```


Formatiert den ausgewählten Bereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Der Bereich der PivotTable, für den diese Regel gilt. |
| fieldPosition | int | Position des Feldes innerhalb der Achse, für die diese Regel gilt. |
| subtotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). Der Zwischensummen-Filtertyp des Pivot-Feldes |
| selectionType | int | [PivotTableSelectionType](../../com.aspose.cells/pivottableselectiontype). Gibt an, wie Daten ausgewählt werden. |
| isGrandRow | boolean | Gibt an, ob Gesamtsummen‑Zeilen ausgewählt werden. |
| isGrandColumn | boolean | Gibt an, ob Gesamtsummen‑Spalten ausgewählt werden. |
| style | [Style](../../com.aspose.cells/style) | Der Stil, der auf den Bereich der Pivot‑Tabelle angewendet wird. |

**Returns:**
[PivotTableFormat](../../com.aspose.cells/pivottableformat) - 
### get(int index) {#get-int-}
```
public PivotTableFormat get(int index)
```


Ermittelt das Format anhand des Index.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der Index. |

**Returns:**
[PivotTableFormat](../../com.aspose.cells/pivottableformat) - 
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

