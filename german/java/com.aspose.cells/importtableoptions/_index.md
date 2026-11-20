---
title: "ImportTableOptions"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Optionen für das Importieren von Daten in Zellen dar."
type: docs
url: /de/java/com.aspose.cells/importtableoptions/
---

**Inheritance:**
java.lang.Object
```
public class ImportTableOptions
```

Stellt die Optionen für das Importieren von Daten in Zellen dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [ImportTableOptions()](#ImportTableOptions--) | Erstellt die Standard-Importoptionen. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCheckMergedCells()](#getCheckMergedCells--) | Gibt an, ob zusammengeführte Zellen geprüft werden. |
| [getClass()](#getClass--) |  |
| [getColumnIndexes()](#getColumnIndexes--) | Ruft die Spalten (0‑basiert) ab, die aus der Datenquelle importiert werden sollen. Null bedeutet, dass alle Spalten importiert werden. |
| [getConvertGridStyle()](#getConvertGridStyle--) | Gibt an, ob der Stil der Grid-Ansicht auf Zellen angewendet wird. |
| [getConvertNumericData()](#getConvertNumericData--) | Ruft einen Wert ab, der angibt, ob der Zeichenfolgenwert in einen numerischen oder Datumswert konvertiert werden soll. |
| [getDateFormat()](#getDateFormat--) | Ruft das Datumsformat für Zellen mit importierten Datums‑Zeit‑Werten ab. |
| [getDefaultValues()](#getDefaultValues--) | Der Standardwert für den Wert in der Tabelle ist Null. |
| [getExportCaptionAsFieldName()](#getExportCaptionAsFieldName--) | Gibt an, ob die Beschriftung als Feldname exportiert wird. |
| [getInsertRows()](#getInsertRows--) | Gibt an, ob neue Zeilen für das Importieren von Daten­datensätzen hinzugefügt werden sollen. |
| [getNumberFormats()](#getNumberFormats--) | Ruft die Zahlenformate ab. |
| [getShiftFirstRowDown()](#getShiftFirstRowDown--) | Gibt an, ob die erste Zeile beim Einfügen von Zeilen nach unten verschoben wird. |
| [getStyles()](#getStyles--) | Ruft die Stile für jede Spalte der Tabelle ab. |
| [getTotalColumns()](#getTotalColumns--) | Ruft die Gesamtanzahl der zu importierenden Spalten aus der Datenquelle ab. -1 bedeutet, dass alle Zeilen der angegebenen Datenquelle importiert werden. |
| [getTotalRows()](#getTotalRows--) | Ruft die Gesamtanzahl der zu importierenden Zeilen aus der Datenquelle ab. -1 bedeutet, dass alle Zeilen der angegebenen Datenquelle importiert werden. |
| [hashCode()](#hashCode--) |  |
| [isFieldNameShown()](#isFieldNameShown--) | Gibt an, ob der Feldname importiert werden soll. |
| [isFormulas()](#isFormulas--) | Gibt an, ob die Daten Formeln sind. |
| [isHtmlString()](#isHtmlString--) | Gibt an, ob der Wert HTML‑Tags enthält. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCheckMergedCells(boolean value)](#setCheckMergedCells-boolean-) | Gibt an, ob zusammengeführte Zellen geprüft werden. |
| [setColumnIndexes(int[] value)](#setColumnIndexes-int---) | Legt die Spalten (0‑basiert) fest, die aus der Datenquelle importiert werden sollen. Null bedeutet, dass alle Spalten importiert werden. |
| [setConvertGridStyle(boolean value)](#setConvertGridStyle-boolean-) | Gibt an, ob der Stil der Grid-Ansicht auf Zellen angewendet wird. |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | Legt einen Wert fest, der angibt, ob der Zeichenfolgenwert in einen numerischen oder Datumswert konvertiert werden soll. |
| [setDateFormat(String value)](#setDateFormat-java.lang.String-) | Legt das Datumsformat für Zellen mit importierten Datums‑Zeit‑Werten fest. |
| [setDefaultValues(Object[] value)](#setDefaultValues-java.lang.Object---) | Der Standardwert für den Wert in der Tabelle ist Null. |
| [setExportCaptionAsFieldName(boolean value)](#setExportCaptionAsFieldName-boolean-) | Gibt an, ob die Beschriftung als Feldname exportiert wird. |
| [setFieldNameShown(boolean value)](#setFieldNameShown-boolean-) | Gibt an, ob der Feldname importiert werden soll. |
| [setFormulas(boolean[] value)](#setFormulas-boolean---) | Gibt an, ob die Daten Formeln sind. |
| [setHtmlString(boolean value)](#setHtmlString-boolean-) | Gibt an, ob der Wert HTML‑Tags enthält. |
| [setInsertRows(boolean value)](#setInsertRows-boolean-) | Gibt an, ob neue Zeilen für das Importieren von Daten­datensätzen hinzugefügt werden sollen. |
| [setNumberFormats(String[] value)](#setNumberFormats-java.lang.String---) | Legt die Zahlenformate fest. |
| [setShiftFirstRowDown(boolean value)](#setShiftFirstRowDown-boolean-) | Gibt an, ob die erste Zeile beim Einfügen von Zeilen nach unten verschoben wird. |
| [setStyles(Style[] value)](#setStyles-com.aspose.cells.Style---) | Legt die Stile für jede Spalte der Tabelle fest. |
| [setTotalColumns(int value)](#setTotalColumns-int-) | Legt die Gesamtanzahl der zu importierenden Spalten aus der Datenquelle fest. -1 bedeutet, dass alle Zeilen der angegebenen Datenquelle importiert werden. |
| [setTotalRows(int value)](#setTotalRows-int-) | Legt die Gesamtanzahl der zu importierenden Zeilen aus der Datenquelle fest. -1 bedeutet, dass alle Zeilen der angegebenen Datenquelle importiert werden. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ImportTableOptions() {#ImportTableOptions--}
```
public ImportTableOptions()
```


Erstellt die Standard-Importoptionen.

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
### getCheckMergedCells() {#getCheckMergedCells--}
```
public boolean getCheckMergedCells()
```


Gibt an, ob zusammengeführte Zellen geprüft werden.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnIndexes() {#getColumnIndexes--}
```
public int[] getColumnIndexes()
```


Ruft die Spalten (0‑basiert) ab, die aus der Datenquelle importiert werden sollen. Null bedeutet, dass alle Spalten importiert werden.

**Returns:**
int[]
### getConvertGridStyle() {#getConvertGridStyle--}
```
public boolean getConvertGridStyle()
```


Gibt an, ob der Stil der Grid-Ansicht auf Zellen angewendet wird.

**Returns:**
boolean
### getConvertNumericData() {#getConvertNumericData--}
```
public boolean getConvertNumericData()
```


Ruft einen Wert ab, der angibt, ob der Zeichenfolgenwert in einen numerischen oder Datumswert konvertiert werden soll.

**Returns:**
boolean
### getDateFormat() {#getDateFormat--}
```
public String getDateFormat()
```


Ruft das Datumsformat für Zellen mit importierten Datums‑Zeit‑Werten ab.

**Returns:**
java.lang.String
### getDefaultValues() {#getDefaultValues--}
```
public Object[] getDefaultValues()
```


Der Standardwert für den Wert in der Tabelle ist Null.

**Returns:**
java.lang.Object[]
### getExportCaptionAsFieldName() {#getExportCaptionAsFieldName--}
```
public boolean getExportCaptionAsFieldName()
```


Gibt an, ob die Beschriftung als Feldname exportiert wird.

**Remarks**

Funktioniert nur für DataTable.

**Returns:**
boolean
### getInsertRows() {#getInsertRows--}
```
public boolean getInsertRows()
```


Gibt an, ob neue Zeilen für das Importieren von Daten­datensätzen hinzugefügt werden sollen.

**Returns:**
boolean
### getNumberFormats() {#getNumberFormats--}
```
public String[] getNumberFormats()
```


Ruft die Zahlenformate ab.

**Returns:**
java.lang.String[]
### getShiftFirstRowDown() {#getShiftFirstRowDown--}
```
public boolean getShiftFirstRowDown()
```


Gibt an, ob die erste Zeile beim Einfügen von Zeilen nach unten verschoben wird.

**Returns:**
boolean
### getStyles() {#getStyles--}
```
public Style[] getStyles()
```


Ruft die Stile für jede Spalte der Tabelle ab.

**Returns:**
com.aspose.cells.Style[]
### getTotalColumns() {#getTotalColumns--}
```
public int getTotalColumns()
```


Ruft die Gesamtanzahl der zu importierenden Spalten aus der Datenquelle ab. -1 bedeutet, dass alle Zeilen der angegebenen Datenquelle importiert werden.

**Returns:**
int
### getTotalRows() {#getTotalRows--}
```
public int getTotalRows()
```


Ruft die Gesamtanzahl der zu importierenden Zeilen aus der Datenquelle ab. -1 bedeutet, dass alle Zeilen der angegebenen Datenquelle importiert werden.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isFieldNameShown() {#isFieldNameShown--}
```
public boolean isFieldNameShown()
```


Gibt an, ob der Feldname importiert werden soll.

**Returns:**
boolean
### isFormulas() {#isFormulas--}
```
public boolean[] isFormulas()
```


Gibt an, ob die Daten Formeln sind.

**Returns:**
boolean[]
### isHtmlString() {#isHtmlString--}
```
public boolean isHtmlString()
```


Gibt an, ob der Wert HTML‑Tags enthält.

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




### setCheckMergedCells(boolean value) {#setCheckMergedCells-boolean-}
```
public void setCheckMergedCells(boolean value)
```


Gibt an, ob zusammengeführte Zellen geprüft werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setColumnIndexes(int[] value) {#setColumnIndexes-int---}
```
public void setColumnIndexes(int[] value)
```


Legt die Spalten (0‑basiert) fest, die aus der Datenquelle importiert werden sollen. Null bedeutet, dass alle Spalten importiert werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int[] |  |

### setConvertGridStyle(boolean value) {#setConvertGridStyle-boolean-}
```
public void setConvertGridStyle(boolean value)
```


Gibt an, ob der Stil der Grid-Ansicht auf Zellen angewendet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```


Legt einen Wert fest, der angibt, ob der Zeichenfolgenwert in einen numerischen oder Datumswert konvertiert werden soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setDateFormat(String value) {#setDateFormat-java.lang.String-}
```
public void setDateFormat(String value)
```


Legt das Datumsformat für Zellen mit importierten Datums‑Zeit‑Werten fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setDefaultValues(Object[] value) {#setDefaultValues-java.lang.Object---}
```
public void setDefaultValues(Object[] value)
```


Der Standardwert für den Wert in der Tabelle ist Null.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.Object[] |  |

### setExportCaptionAsFieldName(boolean value) {#setExportCaptionAsFieldName-boolean-}
```
public void setExportCaptionAsFieldName(boolean value)
```


Gibt an, ob die Beschriftung als Feldname exportiert wird.

**Remarks**

Funktioniert nur für DataTable.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setFieldNameShown(boolean value) {#setFieldNameShown-boolean-}
```
public void setFieldNameShown(boolean value)
```


Gibt an, ob der Feldname importiert werden soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setFormulas(boolean[] value) {#setFormulas-boolean---}
```
public void setFormulas(boolean[] value)
```


Gibt an, ob die Daten Formeln sind.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean[] |  |

### setHtmlString(boolean value) {#setHtmlString-boolean-}
```
public void setHtmlString(boolean value)
```


Gibt an, ob der Wert HTML‑Tags enthält.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setInsertRows(boolean value) {#setInsertRows-boolean-}
```
public void setInsertRows(boolean value)
```


Gibt an, ob neue Zeilen für das Importieren von Daten­datensätzen hinzugefügt werden sollen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setNumberFormats(String[] value) {#setNumberFormats-java.lang.String---}
```
public void setNumberFormats(String[] value)
```


Legt die Zahlenformate fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String[] |  |

### setShiftFirstRowDown(boolean value) {#setShiftFirstRowDown-boolean-}
```
public void setShiftFirstRowDown(boolean value)
```


Gibt an, ob die erste Zeile beim Einfügen von Zeilen nach unten verschoben wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setStyles(Style[] value) {#setStyles-com.aspose.cells.Style---}
```
public void setStyles(Style[] value)
```


Legt die Stile für jede Spalte der Tabelle fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Style\[\]](../../com.aspose.cells/style) |  |

### setTotalColumns(int value) {#setTotalColumns-int-}
```
public void setTotalColumns(int value)
```


Legt die Gesamtanzahl der zu importierenden Spalten aus der Datenquelle fest. -1 bedeutet, dass alle Zeilen der angegebenen Datenquelle importiert werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setTotalRows(int value) {#setTotalRows-int-}
```
public void setTotalRows(int value)
```


Legt die Gesamtanzahl der zu importierenden Zeilen aus der Datenquelle fest. -1 bedeutet, dass alle Zeilen der angegebenen Datenquelle importiert werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

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

