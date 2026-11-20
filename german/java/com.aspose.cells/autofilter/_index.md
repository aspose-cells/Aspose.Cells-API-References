---
title: "AutoFilter"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Autofilterung für das angegebene Arbeitsblatt dar."
type: docs
url: /de/java/com.aspose.cells/autofilter/
---

**Inheritance:**
java.lang.Object
```
public class AutoFilter
```

Stellt die Autofilterung für das angegebene Arbeitsblatt dar.

**Example**

```
         //Creating a file stream containing the Excel file to be opened
         //Instantiating a Workbook object
         Workbook workbook = new Workbook("template.xlsx");
         //Accessing the first worksheet in the Excel file
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Creating AutoFilter by giving the cells range of the heading row
         worksheet.getAutoFilter().setRange("A1:B1");
         //Filtering columns with specified values
         worksheet.getAutoFilter().filter(1, "Bananas");
         //Saving the modified Excel file.
         workbook.save("output.xls");
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [addDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second)](#addDateFilter-int-int-int-int-int-int-int-int-) | Fügt einen Datumsfilter hinzu. |
| [addFillColorFilter(int fieldIndex, int pattern, CellsColor foregroundColor, CellsColor backgroundColor)](#addFillColorFilter-int-int-com.aspose.cells.CellsColor-com.aspose.cells.CellsColor-) | Fügt einen Füllfarbenfilter hinzu. |
| [addFilter(int fieldIndex, String criteria)](#addFilter-int-java.lang.String-) | Fügt einen Filter für eine Filterspalte hinzu. |
| [addFontColorFilter(int fieldIndex, CellsColor color)](#addFontColorFilter-int-com.aspose.cells.CellsColor-) | Fügt einen Schriftfarbenfilter hinzu. |
| [addIconFilter(int fieldIndex, int iconSetType, int iconId)](#addIconFilter-int-int-int-) | Fügt einen Symbolfilter hinzu. |
| [custom(int fieldIndex, int operatorType1, Object criteria1)](#custom-int-int-java.lang.Object-) | Filtert eine Liste mit einem benutzerdefinierten Kriterium. |
| [custom(int fieldIndex, int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2)](#custom-int-int-java.lang.Object-boolean-int-java.lang.Object-) | Filtert eine Liste mit benutzerdefinierten Kriterien. |
| [dynamicFilter(int fieldIndex, int dynamicFilterType)](#dynamicFilter-int-int-) | Fügt einen dynamischen Filter hinzu. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filter(int fieldIndex, String criteria)](#filter-int-java.lang.String-) | Filtert eine Liste mit angegebenen Kriterien. |
| [filterTop10(int fieldIndex, boolean isTop, boolean isPercent, int itemCount)](#filterTop10-int-boolean-boolean-int-) | Filtert die Top‑10‑Elemente in der Liste |
| [getCellArea()](#getCellArea--) | Ruft den [CellArea](../../com.aspose.cells/cellarea) ab, auf den dieser AutoFilter angewendet wird. |
| [getCellArea(boolean refreshAppliedRange)](#getCellArea-boolean-) | Ruft den [CellArea](../../com.aspose.cells/cellarea) ab, auf den der angegebene AutoFilter angewendet wird. |
| [getClass()](#getClass--) |  |
| [getFilterColumns()](#getFilterColumns--) | Ruft die Sammlung der Filterspalten ab. |
| [getRange()](#getRange--) | Stellt den Bereich dar, auf den der angegebene AutoFilter angewendet wird. |
| [getShowFilterButton()](#getShowFilterButton--) | Gibt an, ob die AutoFilter‑Schaltfläche für diese Spalte sichtbar ist. |
| [getSorter()](#getSorter--) | Ruft den Datensortierer ab. |
| [hashCode()](#hashCode--) |  |
| [matchBlanks(int fieldIndex)](#matchBlanks-int-) | Alle leeren Zellen in der Liste abgleichen. |
| [matchNonBlanks(int fieldIndex)](#matchNonBlanks-int-) | Alle nicht-leeren Zellen in der Liste abgleichen. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refresh()](#refresh--) | Aktualisiert Autofilter, um Zeilen auszublenden oder einzublenden. |
| [refresh(boolean hideRows)](#refresh-boolean-) | Ruft die Indizes aller ausgeblendeten Zeilen ab. |
| [removeDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second)](#removeDateFilter-int-int-int-int-int-int-int-int-) | Entfernt einen Datumsfilter. |
| [removeFilter(int fieldIndex)](#removeFilter-int-) | Entfernt den spezifischen Filter. |
| [removeFilter(int fieldIndex, String criteria)](#removeFilter-int-java.lang.String-) | Entfernt einen Filter für eine Filterspalte. |
| [setRange(int row, int startColumn, int endColumn)](#setRange-int-int-int-) | Legt den Bereich fest, auf den der angegebene AutoFilter angewendet wird. |
| [setRange(String value)](#setRange-java.lang.String-) | Stellt den Bereich dar, auf den der angegebene AutoFilter angewendet wird. |
| [setShowFilterButton(boolean value)](#setShowFilterButton-boolean-) | Gibt an, ob die AutoFilter‑Schaltfläche für diese Spalte sichtbar ist. |
| [showAll()](#showAll--) | Alle Zeilen einblenden. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second) {#addDateFilter-int-int-int-int-int-int-int-int-}
```
public void addDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second)
```


Fügt einen Datumsfilter hinzu.

**Remarks**

Wenn DateTimeGroupingType Jahr ist, wirkt nur das Parameterjahr. Wenn DateTiemGroupingType Monat ist, wirken nur das Parameterjahr und der Monat.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldIndex | int | Der ganzzahlige Versatz des Feldes, auf dem Sie den Filter basieren möchten (vom linken Rand der Liste; das linkeste Feld ist Feld 0). |
| dateTimeGroupingType | int | [DateTimeGroupingType](../../com.aspose.cells/datetimegroupingtype). Der Gruppierungstyp |
| Jahr | int | Das Jahr. |
| Monat | int | Der Monat. |
| Tag | int | Der Tag. |
| Stunde | int | Die Stunde. |
| Minute | int | Die Minute. |
| Sekunde | int | Die Sekunde. |

### addFillColorFilter(int fieldIndex, int pattern, CellsColor foregroundColor, CellsColor backgroundColor) {#addFillColorFilter-int-int-com.aspose.cells.CellsColor-com.aspose.cells.CellsColor-}
```
public void addFillColorFilter(int fieldIndex, int pattern, CellsColor foregroundColor, CellsColor backgroundColor)
```


Fügt einen Füllfarbenfilter hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldIndex | int | Der ganzzahlige Versatz des Feldes, auf dem Sie den Filter basieren möchten (vom linken Rand der Liste; das linkeste Feld ist Feld 0). |
| pattern | int | [BackgroundType](../../com.aspose.cells/backgroundtype). Der Hintergrundmuster-Typ. |
| foregroundColor | [CellsColor](../../com.aspose.cells/cellscolor) | Die Vordergrundfarbe. |
| backgroundColor | [CellsColor](../../com.aspose.cells/cellscolor) | Die Hintergrundfarbe. |

### addFilter(int fieldIndex, String criteria) {#addFilter-int-java.lang.String-}
```
public void addFilter(int fieldIndex, String criteria)
```


Fügt einen Filter für eine Filterspalte hinzu.

**Remarks**

MS Excel 2007 unterstützt Mehrfachauswahl in einer Filterspalte.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldIndex | int | Der ganzzahlige Versatz des Feldes, auf dem Sie den Filter basieren möchten (vom linken Rand der Liste; das linkeste Feld ist Feld 0). |
| criteria | java.lang.String | Das angegebene Kriterium (ein String; zum Beispiel "101"). Es kann nur null sein oder einem der Zellenwerte in dieser Spalte entsprechen. |

### addFontColorFilter(int fieldIndex, CellsColor color) {#addFontColorFilter-int-com.aspose.cells.CellsColor-}
```
public void addFontColorFilter(int fieldIndex, CellsColor color)
```


Fügt einen Schriftfarbenfilter hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldIndex | int | Der ganzzahlige Versatz des Feldes, auf dem Sie den Filter basieren möchten (vom linken Rand der Liste; das linkeste Feld ist Feld 0). |
| color | [CellsColor](../../com.aspose.cells/cellscolor) | Das [CellsColor](../../com.aspose.cells/cellscolor) Objekt. |

### addIconFilter(int fieldIndex, int iconSetType, int iconId) {#addIconFilter-int-int-int-}
```
public void addIconFilter(int fieldIndex, int iconSetType, int iconId)
```


Fügt einen Symbolfilter hinzu.

**Remarks**

Unterstützt nur das Hinzufügen des Symbolfilters. Unterstützt nicht die Überprüfung, welche Zeile sichtbar ist, wenn der Filter ein Symbolfilter ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldIndex | int | Der ganzzahlige Versatz des Feldes, auf dem Sie den Filter basieren möchten (vom linken Rand der Liste; das linkeste Feld ist Feld 0). |
| iconSetType | int | [IconSetType](../../com.aspose.cells/iconsettype). Der Symbolsatztyp. |
| iconId | int | Die Symbol-ID. |

### custom(int fieldIndex, int operatorType1, Object criteria1) {#custom-int-int-java.lang.Object-}
```
public void custom(int fieldIndex, int operatorType1, Object criteria1)
```


Filtert eine Liste mit einem benutzerdefinierten Kriterium.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldIndex | int | Der ganzzahlige Versatz des Feldes, auf dem Sie den Filter basieren möchten (vom linken Rand der Liste; das linkeste Feld ist Feld 0). |
| operatorType1 | int | [FilterOperatorType](../../com.aspose.cells/filteroperatortype). Der Filteroperator-Typ |
| criteria1 | java.lang.Object | Das benutzerdefinierte Kriterium |

### custom(int fieldIndex, int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2) {#custom-int-int-java.lang.Object-boolean-int-java.lang.Object-}
```
public void custom(int fieldIndex, int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2)
```


Filtert eine Liste mit benutzerdefinierten Kriterien.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldIndex | int | Der ganzzahlige Versatz des Feldes, auf dem Sie den Filter basieren möchten (vom linken Rand der Liste; das linkeste Feld ist Feld 0). |
| operatorType1 | int | [FilterOperatorType](../../com.aspose.cells/filteroperatortype). Der Filteroperator-Typ |
| criteria1 | java.lang.Object | Das benutzerdefinierte Kriterium |
| isAnd | boolean |  |
| operatorType2 | int | [FilterOperatorType](../../com.aspose.cells/filteroperatortype). Der Filteroperator-Typ |
| criteria2 | java.lang.Object | Das benutzerdefinierte Kriterium |

### dynamicFilter(int fieldIndex, int dynamicFilterType) {#dynamicFilter-int-int-}
```
public void dynamicFilter(int fieldIndex, int dynamicFilterType)
```


Fügt einen dynamischen Filter hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldIndex | int | Der ganzzahlige Versatz des Feldes, auf dem Sie den Filter basieren möchten (vom linken Rand der Liste; das linkeste Feld ist Feld 0). |
| dynamicFilterType | int | [DynamicFilterType](../../com.aspose.cells/dynamicfiltertype). Dynamischer Filtertyp. |

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
### filter(int fieldIndex, String criteria) {#filter-int-java.lang.String-}
```
public void filter(int fieldIndex, String criteria)
```


Filtert eine Liste mit angegebenen Kriterien.

**Remarks**

Aspose.Cells entfernt alle anderen Filtereinstellungen für dieses Feld wie in MS Excel 97-2003.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldIndex | int | Der ganzzahlige Versatz des Feldes, auf dem Sie den Filter basieren möchten (vom linken Rand der Liste; das linkeste Feld ist Feld 0). |
| criteria | java.lang.String | Das angegebene Kriterium (ein String; zum Beispiel "101"). |

### filterTop10(int fieldIndex, boolean isTop, boolean isPercent, int itemCount) {#filterTop10-int-boolean-boolean-int-}
```
public void filterTop10(int fieldIndex, boolean isTop, boolean isPercent, int itemCount)
```


Filtert die Top‑10‑Elemente in der Liste

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldIndex | int | Der ganzzahlige Versatz des Feldes, auf dem Sie den Filter basieren möchten (vom linken Rand der Liste; das linkeste Feld ist Feld 0). |
| isTop | boolean | Gibt an, ob der Filter von oben oder unten ist. |
| isPercent | boolean | Gibt an, ob die Elemente Prozent oder Anzahl sind |
| itemCount | int | Die Elementanzahl |

### getCellArea() {#getCellArea--}
```
public CellArea getCellArea()
```


Ruft den [CellArea](../../com.aspose.cells/cellarea) ab, auf den dieser AutoFilter angewendet wird.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the area this filter applies to
### getCellArea(boolean refreshAppliedRange) {#getCellArea-boolean-}
```
public CellArea getCellArea(boolean refreshAppliedRange)
```


Ruft den [CellArea](../../com.aspose.cells/cellarea) ab, auf den der angegebene AutoFilter angewendet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| refreshAppliedRange | boolean | Ob der angewendete Bereich aktualisiert werden soll. Für den angewendeten Bereich des AutoFilters kann sich die letzte Zeile ändern, wenn sich die Zellen­daten ändern. Wenn dieses Flag true ist, wird die letzte Zeile des Bereichs basierend auf den aktuellen Zellen­daten neu berechnet. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the area this filter applies to
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFilterColumns() {#getFilterColumns--}
```
public FilterColumnCollection getFilterColumns()
```


Ruft die Sammlung der Filterspalten ab.

**Returns:**
[FilterColumnCollection](../../com.aspose.cells/filtercolumncollection)
### getRange() {#getRange--}
```
public String getRange()
```


Stellt den Bereich dar, auf den der angegebene AutoFilter angewendet wird.

**Returns:**
java.lang.String
### getShowFilterButton() {#getShowFilterButton--}
```
public boolean getShowFilterButton()
```


Gibt an, ob die AutoFilter‑Schaltfläche für diese Spalte sichtbar ist.

**Returns:**
boolean
### getSorter() {#getSorter--}
```
public DataSorter getSorter()
```


Ruft den Datensortierer ab.

**Returns:**
[DataSorter](../../com.aspose.cells/datasorter)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### matchBlanks(int fieldIndex) {#matchBlanks-int-}
```
public void matchBlanks(int fieldIndex)
```


Alle leeren Zellen in der Liste abgleichen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldIndex | int | Der ganzzahlige Versatz des Feldes, auf dem Sie den Filter basieren möchten (vom linken Rand der Liste; das linkeste Feld ist Feld 0). |

### matchNonBlanks(int fieldIndex) {#matchNonBlanks-int-}
```
public void matchNonBlanks(int fieldIndex)
```


Alle nicht-leeren Zellen in der Liste abgleichen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldIndex | int | Der ganzzahlige Versatz des Feldes, auf dem Sie den Filter basieren möchten (vom linken Rand der Liste; das linkeste Feld ist Feld 0). |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refresh() {#refresh--}
```
public int[] refresh()
```


Aktualisiert Autofilter, um Zeilen auszublenden oder einzublenden.

**Returns:**
int[] - Gibt alle Indizes der ausgeblendeten Zeilen zurück.
### refresh(boolean hideRows) {#refresh-boolean-}
```
public int[] refresh(boolean hideRows)
```


Ruft die Indizes aller ausgeblendeten Zeilen ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| hideRows | boolean | Wenn true, werden die gefilterten Zeilen ausgeblendet. |

**Returns:**
int[] - Gibt alle Indizes der ausgeblendeten Zeilen zurück.
### removeDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second) {#removeDateFilter-int-int-int-int-int-int-int-int-}
```
public void removeDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second)
```


Entfernt einen Datumsfilter.

**Remarks**

Wenn DateTimeGroupingType Jahr ist, wirkt nur das Parameterjahr. Wenn DateTiemGroupingType Monat ist, wirken nur das Parameterjahr und der Monat.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldIndex | int | Der ganzzahlige Versatz des Feldes, auf dem Sie den Filter basieren möchten (vom linken Rand der Liste; das linkeste Feld ist Feld 0). |
| dateTimeGroupingType | int | [DateTimeGroupingType](../../com.aspose.cells/datetimegroupingtype). Der Gruppierungstyp |
| Jahr | int | Das Jahr. |
| Monat | int | Der Monat. |
| Tag | int | Der Tag. |
| Stunde | int | Die Stunde. |
| Minute | int | Die Minute. |
| Sekunde | int | Die Sekunde. |

### removeFilter(int fieldIndex) {#removeFilter-int-}
```
public void removeFilter(int fieldIndex)
```


Entfernt den spezifischen Filter.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldIndex | int | Der spezifische Filterindex |

### removeFilter(int fieldIndex, String criteria) {#removeFilter-int-java.lang.String-}
```
public void removeFilter(int fieldIndex, String criteria)
```


Entfernt einen Filter für eine Filterspalte.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldIndex | int | Der ganzzahlige Versatz des Feldes, auf dem Sie den Filter basieren möchten (vom linken Rand der Liste; das linkeste Feld ist Feld 0). |
| criteria | java.lang.String | Das angegebene Kriterium (ein String; zum Beispiel "101"). Es kann nur null sein oder einem der Zellenwerte in dieser Spalte entsprechen. |

### setRange(int row, int startColumn, int endColumn) {#setRange-int-int-int-}
```
public void setRange(int row, int startColumn, int endColumn)
```


Legt den Bereich fest, auf den der angegebene AutoFilter angewendet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex. |
| startColumn | int | Startspaltenindex. |
| endColumn | int | Endspaltenindex. |

### setRange(String value) {#setRange-java.lang.String-}
```
public void setRange(String value)
```


Stellt den Bereich dar, auf den der angegebene AutoFilter angewendet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setShowFilterButton(boolean value) {#setShowFilterButton-boolean-}
```
public void setShowFilterButton(boolean value)
```


Gibt an, ob die AutoFilter‑Schaltfläche für diese Spalte sichtbar ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### showAll() {#showAll--}
```
public void showAll()
```


Alle Zeilen einblenden.

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

