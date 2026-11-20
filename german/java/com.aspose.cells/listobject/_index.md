---
title: "ListObject"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt eine Tabelle in einem Arbeitsblatt dar."
type: docs
url: /de/java/com.aspose.cells/listobject/
---

**Inheritance:**
java.lang.Object
```
public class ListObject
```

Stellt eine Tabelle in einem Arbeitsblatt dar.

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         for (int i = 0; i  ? i++)
         {
         cells.get(0,i).putValue(CellsHelper.columnIndexToName(i));
          }
         for (int row = 1; row  ? row++)
         {
          for (int column = 0; column  ? column++)
         {
         cells.get(row, column).putValue(row * column);
          }
          }
         ListObjectCollection tables = workbook.getWorksheets().get(0).getListObjects();
         int index = tables.add(0, 0, 9, 4, true);
         ListObject table = tables.get(0);
         table.setShowTotals(true);
         table.getListColumns().get(4).setTotalsCalculation(com.aspose.cells.TotalsCalculation.SUM);
         workbook.save("Book1.xlsx");
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [applyStyleToRange()](#applyStyleToRange--) | Wendet den Tabellenstil auf den Bereich an. |
| [convertToRange()](#convertToRange--) | Konvertiert die Tabelle in einen Bereich. |
| [convertToRange(TableToRangeOptions options)](#convertToRange-com.aspose.cells.TableToRangeOptions-) | Konvertiert die Tabelle in einen Bereich. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filter()](#filter--) | Filtert die Tabelle. |
| [getAlternativeDescription()](#getAlternativeDescription--) | Ruft die alternative Beschreibung ab. |
| [getAlternativeText()](#getAlternativeText--) | Ruft den alternativen Text ab. |
| [getAutoFilter()](#getAutoFilter--) | Ruft den AutoFilter dieser Tabelle ab. |
| [getClass()](#getClass--) |  |
| [getComment()](#getComment--) | Ruft den Kommentar der Tabelle ab. |
| [getDataRange()](#getDataRange--) | Ruft den Datenbereich der Tabelle ab. |
| [getDataSourceType()](#getDataSourceType--) | Ruft den Typ der Datenquelle der Tabelle ab. |
| [getDisplayName()](#getDisplayName--) | Ruft den Anzeigenamen der Tabelle ab. |
| [getEndColumn()](#getEndColumn--) | Ruft die Endspalte des Bereichs ab. |
| [getEndRow()](#getEndRow--) | Ruft die Endzeile des Bereichs ab. |
| [getListColumns()](#getListColumns--) | Ruft die [ListColumn](../../com.aspose.cells/listcolumn)-Liste dieser Tabelle ab. |
| [getQueryTable()](#getQueryTable--) | Ruft die verknüpfte QueryTable ab. |
| [getShowHeaderRow()](#getShowHeaderRow--) | Ermittelt, ob diese Tabelle die Kopfzeile anzeigt. |
| [getShowTableStyleColumnStripes()](#getShowTableStyleColumnStripes--) | Gibt an, ob Spaltenstreifenformatierung angewendet wird. |
| [getShowTableStyleFirstColumn()](#getShowTableStyleFirstColumn--) | Gibt an, ob die erste Spalte in der Tabelle den angewendeten Stil hat. |
| [getShowTableStyleLastColumn()](#getShowTableStyleLastColumn--) | Gibt an, ob die letzte Spalte in der Tabelle den angewendeten Stil hat. |
| [getShowTableStyleRowStripes()](#getShowTableStyleRowStripes--) | Gibt an, ob Zeilenstreifenformatierung angewendet wird. |
| [getShowTotals()](#getShowTotals--) | Ermittelt, ob diese Tabelle die Gesamtsumme‑Zeile anzeigt. |
| [getStartColumn()](#getStartColumn--) | Ruft die Startspalte des Bereichs ab. |
| [getStartRow()](#getStartRow--) | Ermittelt die Startzeile des Bereichs. |
| [getTableStyleName()](#getTableStyleName--) | Ermittelt den Namen des Tabellenstils. |
| [getTableStyleType()](#getTableStyleType--) | Ermittelt den integrierten Tabellenstil. |
| [getXmlMap()](#getXmlMap--) | Ermittelt ein [getXmlMap()](../../com.aspose.cells/listobject\#getXmlMap--) für diese Liste. |
| [hasAutoFilter()](#hasAutoFilter--) | Gibt an, ob ein Auto-Filter auf diese Tabelle angewendet wird. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putCellFormula(int rowOffset, int columnOffset, String formula)](#putCellFormula-int-int-java.lang.String-) | Setzt die Formel in die Zelle der Tabelle. |
| [putCellFormula(int rowOffset, int columnOffset, String formula, boolean isTotalsRowFormula)](#putCellFormula-int-int-java.lang.String-boolean-) | Setzt die Formel in die Zelle der Tabelle. |
| [putCellValue(int rowOffset, int columnOffset, Object value)](#putCellValue-int-int-java.lang.Object-) | Setzt den Wert in die Zelle. |
| [putCellValue(int rowOffset, int columnOffset, Object value, boolean isTotalsRowLabel)](#putCellValue-int-int-java.lang.Object-boolean-) | Setzt den Wert in die Zelle. |
| [removeAutoFilter()](#removeAutoFilter--) | Entfernt den Auto-Filter, der auf diese Tabelle angewendet wurde. |
| [resize(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders)](#resize-int-int-int-int-boolean-) | Ändert die Größe des Bereichs des Listobjekts. |
| [setAlternativeDescription(String value)](#setAlternativeDescription-java.lang.String-) | Legt die alternative Beschreibung fest. |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | Legt den alternativen Text fest. |
| [setComment(String value)](#setComment-java.lang.String-) | Legt den Kommentar der Tabelle fest. |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | Legt den Anzeigenamen der Tabelle fest. |
| [setHasAutoFilter(boolean value)](#setHasAutoFilter-boolean-) | Gibt an, ob ein Auto-Filter auf diese Tabelle angewendet wird. |
| [setShowHeaderRow(boolean value)](#setShowHeaderRow-boolean-) | Legt fest, ob diese Tabelle die Kopfzeile anzeigt. |
| [setShowTableStyleColumnStripes(boolean value)](#setShowTableStyleColumnStripes-boolean-) | Gibt an, ob Spaltenstreifenformatierung angewendet wird. |
| [setShowTableStyleFirstColumn(boolean value)](#setShowTableStyleFirstColumn-boolean-) | Gibt an, ob die erste Spalte in der Tabelle den angewendeten Stil hat. |
| [setShowTableStyleLastColumn(boolean value)](#setShowTableStyleLastColumn-boolean-) | Gibt an, ob die letzte Spalte in der Tabelle den angewendeten Stil hat. |
| [setShowTableStyleRowStripes(boolean value)](#setShowTableStyleRowStripes-boolean-) | Gibt an, ob Zeilenstreifenformatierung angewendet wird. |
| [setShowTotals(boolean value)](#setShowTotals-boolean-) | Legt fest, ob diese Tabelle die Gesamtsummen‑Zeile anzeigt. |
| [setTableStyleName(String value)](#setTableStyleName-java.lang.String-) | Legt den Namen des Tabellenstils fest. |
| [setTableStyleType(int value)](#setTableStyleType-int-) | Ermittelt den integrierten Tabellenstil. |
| [toString()](#toString--) |  |
| [updateColumnName()](#updateColumnName--) | Aktualisiert die Namen aller Listenspalten in den Zellen der Tabelle. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyStyleToRange() {#applyStyleToRange--}
```
public void applyStyleToRange()
```


Wendet den Tabellenstil auf den Bereich an.

### convertToRange() {#convertToRange--}
```
public void convertToRange()
```


Konvertiert die Tabelle in einen Bereich.

### convertToRange(TableToRangeOptions options) {#convertToRange-com.aspose.cells.TableToRangeOptions-}
```
public void convertToRange(TableToRangeOptions options)
```


Konvertiert die Tabelle in einen Bereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| options | [TableToRangeOptions](../../com.aspose.cells/tabletorangeoptions) | Die Optionen beim Konvertieren einer Tabelle in einen Bereich. |

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
### filter() {#filter--}
```
public AutoFilter filter()
```


Filtert die Tabelle.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Stattdessen bitte die Eigenschaft ListObject.HasAutoFilter setzen./// Diese Eigenschaft wird 12 Monate nach Oktober 2025 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Returns:**
[AutoFilter](../../com.aspose.cells/autofilter)
### getAlternativeDescription() {#getAlternativeDescription--}
```
public String getAlternativeDescription()
```


Ruft die alternative Beschreibung ab.

**Returns:**
java.lang.String
### getAlternativeText() {#getAlternativeText--}
```
public String getAlternativeText()
```


Ruft den alternativen Text ab.

**Returns:**
java.lang.String
### getAutoFilter() {#getAutoFilter--}
```
public AutoFilter getAutoFilter()
```


Ruft den AutoFilter dieser Tabelle ab.

**Remarks**

Es funktioniert nur, wenn [hasAutoFilter()](../../com.aspose.cells/listobject\#hasAutoFilter--) false ist.

**Returns:**
[AutoFilter](../../com.aspose.cells/autofilter)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getComment() {#getComment--}
```
public String getComment()
```


Ruft den Kommentar der Tabelle ab.

**Returns:**
java.lang.String
### getDataRange() {#getDataRange--}
```
public Range getDataRange()
```


Ruft den Datenbereich der Tabelle ab.

**Returns:**
[Range](../../com.aspose.cells/range)
### getDataSourceType() {#getDataSourceType--}
```
public int getDataSourceType()
```


Ruft den Typ der Datenquelle der Tabelle ab.

Siehe [TableDataSourceType](../../com.aspose.cells/tabledatasourcetype).

**Returns:**
int
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Ruft den Anzeigenamen der Tabelle ab.

**Returns:**
java.lang.String
### getEndColumn() {#getEndColumn--}
```
public int getEndColumn()
```


Ruft die Endspalte des Bereichs ab.

**Returns:**
int
### getEndRow() {#getEndRow--}
```
public int getEndRow()
```


Ruft die Endzeile des Bereichs ab.

**Returns:**
int
### getListColumns() {#getListColumns--}
```
public ListColumnCollection getListColumns()
```


Ruft die [ListColumn](../../com.aspose.cells/listcolumn)-Liste dieser Tabelle ab.

**Returns:**
[ListColumnCollection](../../com.aspose.cells/listcolumncollection)
### getQueryTable() {#getQueryTable--}
```
public QueryTable getQueryTable()
```


Ruft die verknüpfte QueryTable ab.

**Returns:**
[QueryTable](../../com.aspose.cells/querytable)
### getShowHeaderRow() {#getShowHeaderRow--}
```
public boolean getShowHeaderRow()
```


Ermittelt, ob diese Tabelle die Kopfzeile anzeigt.

**Returns:**
boolean
### getShowTableStyleColumnStripes() {#getShowTableStyleColumnStripes--}
```
public boolean getShowTableStyleColumnStripes()
```


Gibt an, ob Spaltenstreifenformatierung angewendet wird.

**Returns:**
boolean
### getShowTableStyleFirstColumn() {#getShowTableStyleFirstColumn--}
```
public boolean getShowTableStyleFirstColumn()
```


Gibt an, ob die erste Spalte in der Tabelle den angewendeten Stil hat.

**Returns:**
boolean
### getShowTableStyleLastColumn() {#getShowTableStyleLastColumn--}
```
public boolean getShowTableStyleLastColumn()
```


Gibt an, ob die letzte Spalte in der Tabelle den angewendeten Stil hat.

**Returns:**
boolean
### getShowTableStyleRowStripes() {#getShowTableStyleRowStripes--}
```
public boolean getShowTableStyleRowStripes()
```


Gibt an, ob Zeilenstreifenformatierung angewendet wird.

**Returns:**
boolean
### getShowTotals() {#getShowTotals--}
```
public boolean getShowTotals()
```


Ermittelt, ob diese Tabelle die Gesamtsumme‑Zeile anzeigt.

**Returns:**
boolean
### getStartColumn() {#getStartColumn--}
```
public int getStartColumn()
```


Ruft die Startspalte des Bereichs ab.

**Returns:**
int
### getStartRow() {#getStartRow--}
```
public int getStartRow()
```


Ermittelt die Startzeile des Bereichs.

**Returns:**
int
### getTableStyleName() {#getTableStyleName--}
```
public String getTableStyleName()
```


Ermittelt den Namen des Tabellenstils.

**Returns:**
java.lang.String
### getTableStyleType() {#getTableStyleType--}
```
public int getTableStyleType()
```


Ermittelt den integrierten Tabellenstil.

Siehe [TableStyleType](../../com.aspose.cells/tablestyletype).

**Example**

```
         Workbook workbook = new Workbook("Book1.xlsx");
         ListObjectCollection tables = workbook.getWorksheets().get(0).getListObjects();
         int index = tables.add(0, 0, 9, 4, true);
         ListObject table = tables.get(0);
         table.setTableStyleType(TableStyleType.TABLE_STYLE_DARK_2);
          workbook.save("TableStyle.xlsx");
```

**Returns:**
int
### getXmlMap() {#getXmlMap--}
```
public XmlMap getXmlMap()
```


Ermittelt ein [getXmlMap()](../../com.aspose.cells/listobject\#getXmlMap--) für diese Liste.

**Returns:**
[XmlMap](../../com.aspose.cells/xmlmap)
### hasAutoFilter() {#hasAutoFilter--}
```
public boolean hasAutoFilter()
```


Gibt an, ob ein Auto-Filter auf diese Tabelle angewendet wird.

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




### putCellFormula(int rowOffset, int columnOffset, String formula) {#putCellFormula-int-int-java.lang.String-}
```
public void putCellFormula(int rowOffset, int columnOffset, String formula)
```


Setzt die Formel in die Zelle der Tabelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowOffset | int | Der Zeilenversatz in der Tabelle. |
| columnOffset | int | Der Spaltenversatz in der Tabelle. |
| formula | java.lang.String | Die Formel der Zelle. |

### putCellFormula(int rowOffset, int columnOffset, String formula, boolean isTotalsRowFormula) {#putCellFormula-int-int-java.lang.String-boolean-}
```
public void putCellFormula(int rowOffset, int columnOffset, String formula, boolean isTotalsRowFormula)
```


Setzt die Formel in die Zelle der Tabelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowOffset | int | Der Zeilenversatz in der Tabelle. |
| columnOffset | int | Der Spaltenversatz in der Tabelle. |
| formula | java.lang.String | Die Formel der Zelle. |
| isTotalsRowFormula | boolean |  |

### putCellValue(int rowOffset, int columnOffset, Object value) {#putCellValue-int-int-java.lang.Object-}
```
public void putCellValue(int rowOffset, int columnOffset, Object value)
```


Setzt den Wert in die Zelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowOffset | int | Der Zeilenversatz in der Tabelle. |
| columnOffset | int | Der Spaltenversatz in der Tabelle. |
| Wert | java.lang.Object | Der Zellenwert. |

### putCellValue(int rowOffset, int columnOffset, Object value, boolean isTotalsRowLabel) {#putCellValue-int-int-java.lang.Object-boolean-}
```
public void putCellValue(int rowOffset, int columnOffset, Object value, boolean isTotalsRowLabel)
```


Setzt den Wert in die Zelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowOffset | int | Der Zeilenversatz in der Tabelle. |
| columnOffset | int | Der Spaltenversatz in der Tabelle. |
| Wert | java.lang.Object | Der Zellenwert. |
| isTotalsRowLabel | boolean | Gibt an, ob es sich um eine Bezeichnung für die Gesamtsumme‑Zeile handelt, funktioniert nur für die Gesamtsumme‑Zeile. Wenn False und diese Zeile eine Gesamtsumme‑Zeile ist, wird eine neue Zeile eingefügt. |

### removeAutoFilter() {#removeAutoFilter--}
```
public void removeAutoFilter()
```


Entfernt den Auto-Filter, der auf diese Tabelle angewendet wurde.

### resize(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders) {#resize-int-int-int-int-boolean-}
```
public void resize(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders)
```


Ändert die Größe des Bereichs des Listobjekts.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | int | Der Startzeilenindex des neuen Bereichs. |
| startColumn | int | Der Startspaltenindex des neuen Bereichs. |
| endRow | int | Der Endzeilenindex des neuen Bereichs. |
| endColumn | int | Der Endspaltenindex des neuen Bereichs. |
| hasHeaders | boolean | Ob diese Tabelle Kopfzeilen hat. |

### setAlternativeDescription(String value) {#setAlternativeDescription-java.lang.String-}
```
public void setAlternativeDescription(String value)
```


Legt die alternative Beschreibung fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setAlternativeText(String value) {#setAlternativeText-java.lang.String-}
```
public void setAlternativeText(String value)
```


Legt den alternativen Text fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setComment(String value) {#setComment-java.lang.String-}
```
public void setComment(String value)
```


Legt den Kommentar der Tabelle fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


Legt den Anzeigenamen der Tabelle fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setHasAutoFilter(boolean value) {#setHasAutoFilter-boolean-}
```
public void setHasAutoFilter(boolean value)
```


Gibt an, ob ein Auto-Filter auf diese Tabelle angewendet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowHeaderRow(boolean value) {#setShowHeaderRow-boolean-}
```
public void setShowHeaderRow(boolean value)
```


Legt fest, ob diese Tabelle die Kopfzeile anzeigt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowTableStyleColumnStripes(boolean value) {#setShowTableStyleColumnStripes-boolean-}
```
public void setShowTableStyleColumnStripes(boolean value)
```


Gibt an, ob Spaltenstreifenformatierung angewendet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowTableStyleFirstColumn(boolean value) {#setShowTableStyleFirstColumn-boolean-}
```
public void setShowTableStyleFirstColumn(boolean value)
```


Gibt an, ob die erste Spalte in der Tabelle den angewendeten Stil hat.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowTableStyleLastColumn(boolean value) {#setShowTableStyleLastColumn-boolean-}
```
public void setShowTableStyleLastColumn(boolean value)
```


Gibt an, ob die letzte Spalte in der Tabelle den angewendeten Stil hat.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowTableStyleRowStripes(boolean value) {#setShowTableStyleRowStripes-boolean-}
```
public void setShowTableStyleRowStripes(boolean value)
```


Gibt an, ob Zeilenstreifenformatierung angewendet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowTotals(boolean value) {#setShowTotals-boolean-}
```
public void setShowTotals(boolean value)
```


Legt fest, ob diese Tabelle die Gesamtsummen‑Zeile anzeigt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setTableStyleName(String value) {#setTableStyleName-java.lang.String-}
```
public void setTableStyleName(String value)
```


Legt den Namen des Tabellenstils fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setTableStyleType(int value) {#setTableStyleType-int-}
```
public void setTableStyleType(int value)
```


Ermittelt den integrierten Tabellenstil.

Siehe [TableStyleType](../../com.aspose.cells/tablestyletype).

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
### updateColumnName() {#updateColumnName--}
```
public void updateColumnName()
```


Aktualisiert die Namen aller Listenspalten in den Zellen der Tabelle.

**Remarks**

Der Wert der Zellen in der Kopfzeile der Tabelle muss mit dem Namen der ListColumn übereinstimmen; Cell.PutValue ändert den Namen der ListColumn aus Leistungsgründen nicht automatisch.

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

