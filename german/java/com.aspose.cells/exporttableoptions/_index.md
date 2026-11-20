---
title: "ExportTableOptions"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt alle Exporttabellenoptionen dar."
type: docs
url: /de/java/com.aspose.cells/exporttableoptions/
---

**Inheritance:**
java.lang.Object
```
public class ExportTableOptions
```

Stellt alle Exporttabellenoptionen dar.

**Remarks**

Wenn es spezielle Anforderungen beim Export gibt, z. B. das Ignorieren von Fehlerwerten, kann der Benutzer diese Klasse erweitern, um die entsprechenden APIs zu überschreiben und das Ziel zu erreichen.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [ExportTableOptions()](#ExportTableOptions--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllowDBNull()](#getAllowDBNull--) | Dieser Wert gibt an, ob DBNulls in dieser Tabelle erlaubt sind. |
| [getCheckMixedValueType()](#getCheckMixedValueType--) | False, Aspose.Cells setzt den Typ der DataColumn anhand des Wertetyps der ersten Zeile für bessere Leistung. |
| [getClass()](#getClass--) |  |
| [getExportAsHtmlString()](#getExportAsHtmlString--) | Exportiert den HTML-Stringwert der Zellen in die DataTable. |
| [getExportAsString()](#getExportAsString--) | Exportiert den Stringwert der Zellen in die DataTable. |
| [getExportColumnName()](#getExportColumnName--) | Gibt an, ob die Daten in der ersten Zeile in den Spaltennamen der DataTable exportiert werden. |
| [getFormatStrategy()](#getFormatStrategy--) | Ermittelt die Formatstrategie beim Export des Werts als Stringwert. |
| [getIndexes()](#getIndexes--) | Die Indizes von Spalten/Zeilen, die exportiert werden sollen. |
| [getPlotVisibleCells()](#getPlotVisibleCells--) | Exportiert nur sichtbare Zellen. |
| [getPlotVisibleColumns()](#getPlotVisibleColumns--) | Exportiert nur sichtbare Spalten. |
| [getPlotVisibleRows()](#getPlotVisibleRows--) | Exportiert nur sichtbare Zeilen. |
| [getRenameStrategy()](#getRenameStrategy--) | Strategie für doppelte Spaltennamen. |
| [getSkipErrorValue()](#getSkipErrorValue--) | Gibt an, ob ungültige Werte für die Spalte übersprungen werden. |
| [hashCode()](#hashCode--) |  |
| [isVertical()](#isVertical--) | True, wenn eine Zeile in der Arbeitsmappendatei eine Zeile in der DataTable darstellt. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [preprocessExportedValue(int cellRow, int cellColumn, CellValue value)](#preprocessExportedValue-int-int-com.aspose.cells.CellValue-) | Den Wert der aktuellen Zelle, die exportiert werden soll, vorverarbeiten. |
| [setAllowDBNull(boolean value)](#setAllowDBNull-boolean-) | Dieser Wert gibt an, ob DBNulls in dieser Tabelle erlaubt sind. |
| [setCheckMixedValueType(boolean value)](#setCheckMixedValueType-boolean-) | False, Aspose.Cells setzt den Typ der DataColumn anhand des Wertetyps der ersten Zeile für bessere Leistung. |
| [setExportAsHtmlString(boolean value)](#setExportAsHtmlString-boolean-) | Exportiert den HTML-Stringwert der Zellen in die DataTable. |
| [setExportAsString(boolean value)](#setExportAsString-boolean-) | Exportiert den Stringwert der Zellen in die DataTable. |
| [setExportColumnName(boolean value)](#setExportColumnName-boolean-) | Gibt an, ob die Daten in der ersten Zeile in den Spaltennamen der DataTable exportiert werden. |
| [setFormatStrategy(int value)](#setFormatStrategy-int-) | Legt die Formatstrategie fest, wenn der Wert als Zeichenfolge exportiert wird. |
| [setIndexes(int[] value)](#setIndexes-int---) | Die Indizes von Spalten/Zeilen, die exportiert werden sollen. |
| [setPlotVisibleCells(boolean value)](#setPlotVisibleCells-boolean-) | Exportiert nur sichtbare Zellen. |
| [setPlotVisibleColumns(boolean value)](#setPlotVisibleColumns-boolean-) | Exportiert nur sichtbare Spalten. |
| [setPlotVisibleRows(boolean value)](#setPlotVisibleRows-boolean-) | Exportiert nur sichtbare Zeilen. |
| [setRenameStrategy(int value)](#setRenameStrategy-int-) | Strategie für doppelte Spaltennamen. |
| [setSkipErrorValue(boolean value)](#setSkipErrorValue-boolean-) | Gibt an, ob ungültige Werte für die Spalte übersprungen werden. |
| [setVertical(boolean value)](#setVertical-boolean-) | True, wenn eine Zeile in der Arbeitsmappendatei eine Zeile in der DataTable darstellt. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ExportTableOptions() {#ExportTableOptions--}
```
public ExportTableOptions()
```


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
### getAllowDBNull() {#getAllowDBNull--}
```
public boolean getAllowDBNull()
```


Dieser Wert gibt an, ob DBNulls in dieser Tabelle erlaubt sind.

**Returns:**
boolean
### getCheckMixedValueType() {#getCheckMixedValueType--}
```
public boolean getCheckMixedValueType()
```


False, Aspose.Cells setzt den Typ der DataColumn anhand des Wertetyps der ersten Zeile aus Performancegründen. True, Aspose.Cells prüft, ob die Wertetypen in der Spalte gemischt sind, bevor der Typ der DataColumn festgelegt wird. Sind die Wertetypen gemischt, wird der Typ der DataColumn zu string.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getExportAsHtmlString() {#getExportAsHtmlString--}
```
public boolean getExportAsHtmlString()
```


Exportiert den HTML-Stringwert der Zellen in die DataTable.

**Returns:**
boolean
### getExportAsString() {#getExportAsString--}
```
public boolean getExportAsString()
```


Exportiert den Stringwert der Zellen in die DataTable.

**Returns:**
boolean
### getExportColumnName() {#getExportColumnName--}
```
public boolean getExportColumnName()
```


Gibt an, ob die Daten in der ersten Zeile zum Spaltennamen der DataTable exportiert werden. Der Standardwert ist false.

**Returns:**
boolean
### getFormatStrategy() {#getFormatStrategy--}
```
public int getFormatStrategy()
```


Ermittelt die Formatstrategie beim Export des Werts als Stringwert.

Siehe [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Remarks**

Der Standardwert ist [CellValueFormatStrategy.CELL\_STYLE](../../com.aspose.cells/cellvalueformatstrategy\#CELL-STYLE).

**Returns:**
int
### getIndexes() {#getIndexes--}
```
public int[] getIndexes()
```


Die Indizes von Spalten/Zeilen, die exportiert werden sollen.

**Returns:**
int[]
### getPlotVisibleCells() {#getPlotVisibleCells--}
```
public boolean getPlotVisibleCells()
```


Exportiert nur sichtbare Zellen.

**Returns:**
boolean
### getPlotVisibleColumns() {#getPlotVisibleColumns--}
```
public boolean getPlotVisibleColumns()
```


Exportiert nur sichtbare Spalten.

**Returns:**
boolean
### getPlotVisibleRows() {#getPlotVisibleRows--}
```
public boolean getPlotVisibleRows()
```


Exportiert nur sichtbare Zeilen.

**Returns:**
boolean
### getRenameStrategy() {#getRenameStrategy--}
```
public int getRenameStrategy()
```


Strategie für doppelte Spaltennamen.

Siehe [RenameStrategy](../../com.aspose.cells/renamestrategy).

**Returns:**
int
### getSkipErrorValue() {#getSkipErrorValue--}
```
public boolean getSkipErrorValue()
```


Gibt an, ob ungültige Werte für die Spalte übersprungen werden. Zum Beispiel, wenn der Spaltentyp decimal ist, der Wert größer als decimal.MaxValue ist und diese Eigenschaft true ist, wird keine Ausnahme mehr ausgelöst. Der Standardwert ist false.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isVertical() {#isVertical--}
```
public boolean isVertical()
```


True, wenn eine Zeile in der Arbeitsmappendatei eine Zeile in der DataTable darstellt. False, wenn eine Spalte in der Arbeitsmappendatei eine Zeile in der DataTable darstellt.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### preprocessExportedValue(int cellRow, int cellColumn, CellValue value) {#preprocessExportedValue-int-int-com.aspose.cells.CellValue-}
```
public boolean preprocessExportedValue(int cellRow, int cellColumn, CellValue value)
```


Den Wert der aktuellen Zelle, die exportiert werden soll, vorverarbeiten.

**Remarks**

Der Zeilen- und Spaltenindex ist der absolute Index der Zelle im Arbeitsblatt, nicht der Index in der exportierten Tabelle. Der Benutzer kann den Wert der aktuellen Zelle in der überschriebenen Implementierung dieser Methode prüfen; wenn die aktuelle Zelle durch einen anderen Typ und Wert ersetzt werden muss, sollte die Implementierung den erwarteten Typ und Wert im CellValue-Objekt setzen und true zurückgeben. Standardmäßig führt diese Methode nichts aus und gibt false zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellRow | int | der Zeilenindex der aktuellen Zelle |
| cellColumn | int | der Spaltenindex der Zelle |
| value | [CellValue](../../com.aspose.cells/cellvalue) | Wert und Typ der aktuellen Zelle |

**Returns:**
boolean – Ob die aktuelle Zelle durch einen anderen Typ und/oder Wert ersetzt wurde.
### setAllowDBNull(boolean value) {#setAllowDBNull-boolean-}
```
public void setAllowDBNull(boolean value)
```


Dieser Wert gibt an, ob DBNulls in dieser Tabelle erlaubt sind.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setCheckMixedValueType(boolean value) {#setCheckMixedValueType-boolean-}
```
public void setCheckMixedValueType(boolean value)
```


False, Aspose.Cells setzt den Typ der DataColumn anhand des Wertetyps der ersten Zeile aus Performancegründen. True, Aspose.Cells prüft, ob die Wertetypen in der Spalte gemischt sind, bevor der Typ der DataColumn festgelegt wird. Sind die Wertetypen gemischt, wird der Typ der DataColumn zu string.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setExportAsHtmlString(boolean value) {#setExportAsHtmlString-boolean-}
```
public void setExportAsHtmlString(boolean value)
```


Exportiert den HTML-Stringwert der Zellen in die DataTable.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setExportAsString(boolean value) {#setExportAsString-boolean-}
```
public void setExportAsString(boolean value)
```


Exportiert den Stringwert der Zellen in die DataTable.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setExportColumnName(boolean value) {#setExportColumnName-boolean-}
```
public void setExportColumnName(boolean value)
```


Gibt an, ob die Daten in der ersten Zeile zum Spaltennamen der DataTable exportiert werden. Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setFormatStrategy(int value) {#setFormatStrategy-int-}
```
public void setFormatStrategy(int value)
```


Legt die Formatstrategie fest, wenn der Wert als Zeichenfolge exportiert wird.

Siehe [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Remarks**

Der Standardwert ist [CellValueFormatStrategy.CELL\_STYLE](../../com.aspose.cells/cellvalueformatstrategy\#CELL-STYLE).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setIndexes(int[] value) {#setIndexes-int---}
```
public void setIndexes(int[] value)
```


Die Indizes von Spalten/Zeilen, die exportiert werden sollen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int[] |  |

### setPlotVisibleCells(boolean value) {#setPlotVisibleCells-boolean-}
```
public void setPlotVisibleCells(boolean value)
```


Exportiert nur sichtbare Zellen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setPlotVisibleColumns(boolean value) {#setPlotVisibleColumns-boolean-}
```
public void setPlotVisibleColumns(boolean value)
```


Exportiert nur sichtbare Spalten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setPlotVisibleRows(boolean value) {#setPlotVisibleRows-boolean-}
```
public void setPlotVisibleRows(boolean value)
```


Exportiert nur sichtbare Zeilen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setRenameStrategy(int value) {#setRenameStrategy-int-}
```
public void setRenameStrategy(int value)
```


Strategie für doppelte Spaltennamen.

Siehe [RenameStrategy](../../com.aspose.cells/renamestrategy).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setSkipErrorValue(boolean value) {#setSkipErrorValue-boolean-}
```
public void setSkipErrorValue(boolean value)
```


Gibt an, ob ungültige Werte für die Spalte übersprungen werden. Zum Beispiel, wenn der Spaltentyp decimal ist, der Wert größer als decimal.MaxValue ist und diese Eigenschaft true ist, wird keine Ausnahme mehr ausgelöst. Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setVertical(boolean value) {#setVertical-boolean-}
```
public void setVertical(boolean value)
```


True, wenn eine Zeile in der Arbeitsmappendatei eine Zeile in der DataTable darstellt. False, wenn eine Spalte in der Arbeitsmappendatei eine Zeile in der DataTable darstellt.

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

