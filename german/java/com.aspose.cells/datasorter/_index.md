---
title: "DataSorter"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Zusammenfassende Beschreibung für DataSorter."
type: docs
url: /de/java/com.aspose.cells/datasorter/
---

**Inheritance:**
java.lang.Object
```
public class DataSorter
```

Zusammenfassende Beschreibung für DataSorter.

**Example**

```
         //Instantiate a new Workbook object.
         Workbook workbook = new Workbook("Book1.xls");
         //Get the workbook datasorter object.
         DataSorter sorter = workbook.getDataSorter();
         //Set the first order for datasorter object.
         sorter.setOrder1(com.aspose.cells.SortOrder.DESCENDING);
         //Define the first key.
         sorter.setKey1(0);
         //Set the second order for datasorter object.
         sorter.setOrder2(com.aspose.cells.SortOrder.ASCENDING);
         //Define the second key.
         sorter.setKey2(1);
         //Create a cells area (range).
         CellArea ca = new CellArea();
         //Specify the start row index.
         ca.StartRow = 0;
         //Specify the start column index.
         ca.StartColumn = 0;
         //Specify the last row index.
         ca.EndRow = 13;
         //Specify the last column index.
         ca.EndColumn = 1;
         //Sort data in the specified data range (A1:B14)
         sorter.sort(workbook.getWorksheets().get(0).getCells(), ca);
         //Save the excel file.
         workbook.save("outBook.xls");
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [addColorKey(int key, int type, int order, Color color)](#addColorKey-int-int-int-com.aspose.cells.Color-) | Fügt Farbsortierschlüssel hinzu. |
| [addKey(int key, int order)](#addKey-int-int-) | Fügt sortierten Spaltenindex und Sortierreihenfolge hinzu. |
| [addKey(int key, int type, int order, Object customList)](#addKey-int-int-int-java.lang.Object-) | Fügt sortierten Spaltenindex und Sortierreihenfolge mit benutzerdefinierter Sortierliste hinzu. |
| [addKey(int key, int order, String customList)](#addKey-int-int-java.lang.String-) | Fügt sortierten Spaltenindex und Sortierreihenfolge mit benutzerdefinierter Sortierliste hinzu. |
| [addKey(int key, int order, String[] customList)](#addKey-int-int-java.lang.String---) | Fügt sortierten Spaltenindex und Sortierreihenfolge mit benutzerdefinierter Sortierliste hinzu. |
| [clear()](#clear--) | Alle Einstellungen zurücksetzen. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCaseSensitive()](#getCaseSensitive--) | Ermittelt, ob beim Vergleichen von Zeichenketten die Groß-/Kleinschreibung berücksichtigt wird. |
| [getClass()](#getClass--) |  |
| [getKey1()](#getKey1--) | Stellt den ersten sortierten Spaltenindex dar (absolute Position, Spalte A ist 0, B ist 1, ...). |
| [getKey2()](#getKey2--) | Stellt den zweiten sortierten Spaltenindex dar (absolute Position, Spalte A ist 0, B ist 1, ...). |
| [getKey3()](#getKey3--) | Stellt den dritten sortierten Spaltenindex dar (absolute Position, Spalte A ist 0, B ist 1, ...). |
| [getKeys()](#getKeys--) | Ermittelt die Schlüsselliste des DataSorters. |
| [getOrder1()](#getOrder1--) | Stellt die Sortierreihenfolge des ersten Schlüssels dar. |
| [getOrder2()](#getOrder2--) | Stellt die Sortierreihenfolge des zweiten Schlüssels dar. |
| [getOrder3()](#getOrder3--) | Stellt die Sortierreihenfolge des dritten Schlüssels dar. |
| [getSortAsNumber()](#getSortAsNumber--) | Gibt an, ob alles, was wie eine Zahl aussieht, sortiert wird. |
| [getSortLeftToRight()](#getSortLeftToRight--) | True bedeutet, dass die Sortierrichtung von links nach rechts verläuft. |
| [hasHeaders()](#hasHeaders--) | Gibt an, ob der Bereich Überschriften enthält. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCaseSensitive(boolean value)](#setCaseSensitive-boolean-) | Legt fest, ob beim Vergleichen von Zeichenfolgen die Groß-/Kleinschreibung berücksichtigt wird. |
| [setHasHeaders(boolean value)](#setHasHeaders-boolean-) | Gibt an, ob der Bereich Überschriften enthält. |
| [setKey1(int value)](#setKey1-int-) | Stellt den ersten sortierten Spaltenindex dar (absolute Position, Spalte A ist 0, B ist 1, ...). |
| [setKey2(int value)](#setKey2-int-) | Stellt den zweiten sortierten Spaltenindex dar (absolute Position, Spalte A ist 0, B ist 1, ...). |
| [setKey3(int value)](#setKey3-int-) | Stellt den dritten sortierten Spaltenindex dar (absolute Position, Spalte A ist 0, B ist 1, ...). |
| [setOrder1(int value)](#setOrder1-int-) | Stellt die Sortierreihenfolge des ersten Schlüssels dar. |
| [setOrder2(int value)](#setOrder2-int-) | Stellt die Sortierreihenfolge des zweiten Schlüssels dar. |
| [setOrder3(int value)](#setOrder3-int-) | Stellt die Sortierreihenfolge des dritten Schlüssels dar. |
| [setSortAsNumber(boolean value)](#setSortAsNumber-boolean-) | Gibt an, ob alles, was wie eine Zahl aussieht, sortiert wird. |
| [setSortLeftToRight(boolean value)](#setSortLeftToRight-boolean-) | True bedeutet, dass die Sortierrichtung von links nach rechts verläuft. |
| [sort()](#sort--) | Sortiert die Daten im Bereich. |
| [sort(Cells cells, CellArea area)](#sort-com.aspose.cells.Cells-com.aspose.cells.CellArea-) | Sortiert die Daten des Bereichs. |
| [sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn)](#sort-com.aspose.cells.Cells-int-int-int-int-) | Sortiert die Daten des Bereichs. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addColorKey(int key, int type, int order, Color color) {#addColorKey-int-int-int-com.aspose.cells.Color-}
```
public void addColorKey(int key, int type, int order, Color color)
```


Fügt Farbsortierschlüssel hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Schlüssel | int | Der sortierte Spaltenindex (absolute Position, Spalte A ist 0, B ist 1, ...) |
| type | int | [SortOnType](../../com.aspose.cells/sortontype). Der sortierte Farbwerttyp. |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). Die Sortierreihenfolge. |
| color | [Color](../../com.aspose.cells/color) | Die benutzerdefinierte Sortierfarbe. |

### addKey(int key, int order) {#addKey-int-int-}
```
public void addKey(int key, int order)
```


Fügt sortierten Spaltenindex und Sortierreihenfolge hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Schlüssel | int | Der sortierte Spaltenindex (absolute Position, Spalte A ist 0, B ist 1, ...) |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). Die Sortierreihenfolge |

### addKey(int key, int type, int order, Object customList) {#addKey-int-int-int-java.lang.Object-}
```
public void addKey(int key, int type, int order, Object customList)
```


Fügt sortierten Spaltenindex und Sortierreihenfolge mit benutzerdefinierter Sortierliste hinzu.

**Remarks**

Wenn der Typ SortOnType.CellColor oder SortOnType.FontColor ist, ist die customList eine Farbe.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Schlüssel | int | Der sortierte Spaltenindex (absolute Position, Spalte A ist 0, B ist 1, ...) |
| type | int | [SortOnType](../../com.aspose.cells/sortontype). Der sortierte Werttyp. |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). Die Sortierreihenfolge. |
| customList | java.lang.Object | Die benutzerdefinierte Sortierliste. |

### addKey(int key, int order, String customList) {#addKey-int-int-java.lang.String-}
```
public void addKey(int key, int order, String customList)
```


Fügt sortierten Spaltenindex und Sortierreihenfolge mit benutzerdefinierter Sortierliste hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Schlüssel | int | Der sortierte Spaltenindex (absolute Position, Spalte A ist 0, B ist 1, ...) |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). Die Sortierreihenfolge. |
| customList | java.lang.String | Die benutzerdefinierte Sortierliste. |

### addKey(int key, int order, String[] customList) {#addKey-int-int-java.lang.String---}
```
public void addKey(int key, int order, String[] customList)
```


Fügt sortierten Spaltenindex und Sortierreihenfolge mit benutzerdefinierter Sortierliste hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Schlüssel | int | Der sortierte Spaltenindex (absolute Position, Spalte A ist 0, B ist 1, ...) |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). Die Sortierreihenfolge. |
| customList | java.lang.String[] | Die benutzerdefinierte Sortierliste. |

### clear() {#clear--}
```
public void clear()
```


Alle Einstellungen zurücksetzen.

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
### getCaseSensitive() {#getCaseSensitive--}
```
public boolean getCaseSensitive()
```


Ermittelt, ob beim Vergleichen von Zeichenketten die Groß-/Kleinschreibung berücksichtigt wird.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getKey1() {#getKey1--}
```
public int getKey1()
```


Stellt den ersten sortierten Spaltenindex dar (absolute Position, Spalte A ist 0, B ist 1, ...).

**Returns:**
int
### getKey2() {#getKey2--}
```
public int getKey2()
```


Stellt den zweiten sortierten Spaltenindex dar (absolute Position, Spalte A ist 0, B ist 1, ...).

**Returns:**
int
### getKey3() {#getKey3--}
```
public int getKey3()
```


Stellt den dritten sortierten Spaltenindex dar (absolute Position, Spalte A ist 0, B ist 1, ...).

**Returns:**
int
### getKeys() {#getKeys--}
```
public DataSorterKeyCollection getKeys()
```


Ermittelt die Schlüsselliste des DataSorters.

**Returns:**
[DataSorterKeyCollection](../../com.aspose.cells/datasorterkeycollection)
### getOrder1() {#getOrder1--}
```
public int getOrder1()
```


Stellt die Sortierreihenfolge des ersten Schlüssels dar.

Siehe [SortOrder](../../com.aspose.cells/sortorder).

**Returns:**
int
### getOrder2() {#getOrder2--}
```
public int getOrder2()
```


Stellt die Sortierreihenfolge des zweiten Schlüssels dar.

Siehe [SortOrder](../../com.aspose.cells/sortorder).

**Returns:**
int
### getOrder3() {#getOrder3--}
```
public int getOrder3()
```


Stellt die Sortierreihenfolge des dritten Schlüssels dar.

Siehe [SortOrder](../../com.aspose.cells/sortorder).

**Returns:**
int
### getSortAsNumber() {#getSortAsNumber--}
```
public boolean getSortAsNumber()
```


Gibt an, ob alles, was wie eine Zahl aussieht, sortiert wird.

**Returns:**
boolean
### getSortLeftToRight() {#getSortLeftToRight--}
```
public boolean getSortLeftToRight()
```


True bedeutet, dass die Sortierrichtung von links nach rechts verläuft. False bedeutet, dass die Sortierrichtung von oben nach unten verläuft. Der Standardwert ist false.

**Returns:**
boolean
### hasHeaders() {#hasHeaders--}
```
public boolean hasHeaders()
```


Gibt an, ob der Bereich Überschriften enthält.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setCaseSensitive(boolean value) {#setCaseSensitive-boolean-}
```
public void setCaseSensitive(boolean value)
```


Legt fest, ob beim Vergleichen von Zeichenfolgen die Groß-/Kleinschreibung berücksichtigt wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setHasHeaders(boolean value) {#setHasHeaders-boolean-}
```
public void setHasHeaders(boolean value)
```


Gibt an, ob der Bereich Überschriften enthält.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setKey1(int value) {#setKey1-int-}
```
public void setKey1(int value)
```


Stellt den ersten sortierten Spaltenindex dar (absolute Position, Spalte A ist 0, B ist 1, ...).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setKey2(int value) {#setKey2-int-}
```
public void setKey2(int value)
```


Stellt den zweiten sortierten Spaltenindex dar (absolute Position, Spalte A ist 0, B ist 1, ...).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setKey3(int value) {#setKey3-int-}
```
public void setKey3(int value)
```


Stellt den dritten sortierten Spaltenindex dar (absolute Position, Spalte A ist 0, B ist 1, ...).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setOrder1(int value) {#setOrder1-int-}
```
public void setOrder1(int value)
```


Stellt die Sortierreihenfolge des ersten Schlüssels dar.

Siehe [SortOrder](../../com.aspose.cells/sortorder).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setOrder2(int value) {#setOrder2-int-}
```
public void setOrder2(int value)
```


Stellt die Sortierreihenfolge des zweiten Schlüssels dar.

Siehe [SortOrder](../../com.aspose.cells/sortorder).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setOrder3(int value) {#setOrder3-int-}
```
public void setOrder3(int value)
```


Stellt die Sortierreihenfolge des dritten Schlüssels dar.

Siehe [SortOrder](../../com.aspose.cells/sortorder).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setSortAsNumber(boolean value) {#setSortAsNumber-boolean-}
```
public void setSortAsNumber(boolean value)
```


Gibt an, ob alles, was wie eine Zahl aussieht, sortiert wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSortLeftToRight(boolean value) {#setSortLeftToRight-boolean-}
```
public void setSortLeftToRight(boolean value)
```


True bedeutet, dass die Sortierrichtung von links nach rechts verläuft. False bedeutet, dass die Sortierrichtung von oben nach unten verläuft. Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### sort() {#sort--}
```
public int[] sort()
```


Sortiert die Daten im Bereich.

**Returns:**
int[] - die ursprünglichen Indizes (absolute Position, zum Beispiel ist Spalte A 0, B ist 1, ...) der sortierten Zeilen/Spalten. Wenn keine Zeilen/Spalten durch diesen Sortiervorgang verschoben werden müssen, wird null zurückgegeben.
### sort(Cells cells, CellArea area) {#sort-com.aspose.cells.Cells-com.aspose.cells.CellArea-}
```
public int[] sort(Cells cells, CellArea area)
```


Sortiert die Daten des Bereichs.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cells | [Cells](../../com.aspose.cells/cells) | Die Zellen enthalten den Datenbereich. |
| area | [CellArea](../../com.aspose.cells/cellarea) | Der zu sortierende Bereich |

**Returns:**
int[] - die ursprünglichen Indizes (absolute Position, zum Beispiel ist Spalte A 0, B ist 1, ...) der sortierten Zeilen/Spalten. Wenn keine Zeilen/Spalten durch diesen Sortiervorgang verschoben werden müssen, wird null zurückgegeben.
### sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn) {#sort-com.aspose.cells.Cells-int-int-int-int-}
```
public int[] sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn)
```


Sortiert die Daten des Bereichs.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cells | [Cells](../../com.aspose.cells/cells) | Die Zellen enthalten den Datenbereich. |
| startRow | int | Die Startzeile des Bereichs. |
| startColumn | int | Die Startspalte des Bereichs. |
| endRow | int | Die Endzeile des Bereichs. |
| endColumn | int | Die Endspalte des Bereichs. |

**Returns:**
int[] - die ursprünglichen Indizes (absolute Position, zum Beispiel ist Spalte A 0, B ist 1, ...) der sortierten Zeilen/Spalten. Wenn keine Zeilen/Spalten durch diesen Sortiervorgang verschoben werden müssen, wird null zurückgegeben.
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

