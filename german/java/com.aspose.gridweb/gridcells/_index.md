---
title: "GridCells"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Kapselt eine Sammlung von Objekten."
type: docs
url: /de/java/com.aspose.gridweb/gridcells/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class GridCells implements Iterable
```

Kapselt eine Sammlung von [GridCell](../../com.aspose.gridweb/gridcell)-Objekten.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [cellIndexToName(int row, int column)](#cellIndexToName-int-int-) | Ermittelt den Zellenamen anhand seiner Zeilen‑ und Spaltenindizes. |
| [cellNameToIndex(String cellName, int row, int column)](#cellNameToIndex-java.lang.String-int-int-) | Ermittelt die Zeilen‑ und Spaltenindizes der Zelle gemäß ihrem Namen |
| [checkCell(int row, int column)](#checkCell-int-int-) | Ermittelt das [GridCell](../../com.aspose.gridweb/gridcell)-Element oder null am angegebenen Zeilen‑ und Spaltenindex der Zelle. |
| [checkColumn(int col)](#checkColumn-int-) | Ermittelt das [GridColumn](../../com.aspose.gridweb/gridcolumn)-Element oder null am angegebenen Spaltenindex. |
| [checkRow(int i)](#checkRow-int-) | Ermittelt das [GridRow](../../com.aspose.gridweb/gridrow)-Element oder null am angegebenen Zeilenindex der Zelle. |
| [clear()](#clear--) | Löscht alle Zellen in der Sammlung. |
| [clearContents(GridCellArea range)](#clearContents-com.aspose.gridweb.GridCellArea-) | Löscht den Inhalt eines Bereichs. |
| [clearContents(int startRow, int startColumn, int endRow, int endColumn)](#clearContents-int-int-int-int-) | Löscht den Inhalt eines Bereichs. |
| [clearFormats(GridCellArea range)](#clearFormats-com.aspose.gridweb.GridCellArea-) | Löscht die Formatierung eines Bereichs. |
| [clearFormats(int startRow, int startColumn, int endRow, int endColumn)](#clearFormats-int-int-int-int-) | Löscht die Formatierung eines Bereichs. |
| [clearRange(GridCellArea range)](#clearRange-com.aspose.gridweb.GridCellArea-) | Löscht Inhalt und Formatierung eines Bereichs. |
| [clearRange(int startRow, int startColumn, int endRow, int endColumn)](#clearRange-int-int-int-int-) | Löscht Inhalt und Formatierung eines Bereichs. |
| [columnIndexToName(int column)](#columnIndexToName-int-) | Ermittelt den Spaltennamen anhand des Spaltenindex. |
| [columnNameToIndex(String columnName)](#columnNameToIndex-java.lang.String-) | Ermittelt den Spaltenindex anhand des Spaltennamens. |
| [copyColumn(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex)](#copyColumn-com.aspose.gridweb.GridCells-int-int-) | Kopiert Daten und Formatierungen einer gesamten Spalte. |
| [copyColumns(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber)](#copyColumns-com.aspose.gridweb.GridCells-int-int-int-) | Kopiert Daten und Formatierungen einer gesamten Spalte. |
| [copyRow(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex)](#copyRow-com.aspose.gridweb.GridCells-int-int-) | Kopiert Daten und Formatierungen einer gesamten Zeile. |
| [copyRows(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)](#copyRows-com.aspose.gridweb.GridCells-int-int-int-) | Kopiert Daten und Formatierungen einiger ganzer Zeilen. |
| [deleteBlankColumns()](#deleteBlankColumns--) | Löscht alle leeren Spalten, die keine Daten enthalten. |
| [deleteBlankRows()](#deleteBlankRows--) | Löscht alle leeren Zeilen, die keine Daten enthalten. |
| [deleteColumn(int columnIndex)](#deleteColumn-int-) | Löscht eine Spalte. |
| [deleteColumn(int columnIndex, boolean updateReference)](#deleteColumn-int-boolean-) | Löscht eine Spalte. |
| [deleteColumns(int columnIndex, int totalColumns, boolean updateReference)](#deleteColumns-int-int-boolean-) | Löscht mehrere Spalten. |
| [deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType)](#deleteRange-int-int-int-int-int-) | Löscht einen Zellbereich und verschiebt Zellen gemäß der Verschiebeoption. |
| [deleteRow(int rowIndex)](#deleteRow-int-) | Löscht eine Zeile. |
| [deleteRows(int rowIndex, int totalRows)](#deleteRows-int-int-) | Löscht mehrere Zeilen. |
| [deleteRows(int rowIndex, int totalRows, boolean updateReference)](#deleteRows-int-int-boolean-) | Löscht mehrere Zeilen im Arbeitsblatt. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)](#exportArray-int-int-int-int-) | Exportiert Daten aus der [GridCells](../../com.aspose.gridweb/gridcells)-Sammlung in ein zweidimensionales Array-Objekt. |
| [get(int row, int column)](#get-int-int-) | Ruft das [GridCell](../../com.aspose.gridweb/gridcell)-Element am angegebenen Zeilenindex und Spaltenindex der Zelle ab. |
| [get(String cellName)](#get-java.lang.String-) | Ruft das [GridCell](../../com.aspose.gridweb/gridcell)-Element mit dem angegebenen Zellenamen ab. |
| [getCell(int row, int column)](#getCell-int-int-) | Ruft das [GridCell](../../com.aspose.gridweb/gridcell)-Element am angegebenen Zeilenindex und Spaltenindex der Zelle ab. |
| [getClass()](#getClass--) |  |
| [getColumnWidth(int column)](#getColumnWidth-int-) | Ermittelt die Breite der angegebenen Spalte |
| [getColumnWidthInch(int column)](#getColumnWidthInch-int-) | Ermittelt die Breite der angegebenen Spalte in Zoll. |
| [getColumnWidthPixel(int column)](#getColumnWidthPixel-int-) | Ermittelt die Breite der angegebenen Spalte in Pixel. |
| [getColumns()](#getColumns--) | Ruft die Sammlung von [GridColumn](../../com.aspose.gridweb/gridcolumn)-Objekten ab, die die einzelnen Spalten in diesem Arbeitsblatt darstellen. |
| [getCount()](#getCount--) | Ermittelt die Anzahl der Zellen. |
| [getFirstCell()](#getFirstCell--) | Ermittelt die erste Zelle in diesem Arbeitsblatt. |
| [getLastCell()](#getLastCell--) | Ermittelt die letzte Zelle in diesem Arbeitsblatt. |
| [getMaxColumn()](#getMaxColumn--) | Maximaler Spaltenindex einer Zelle, die Daten oder Formatierungen enthält. |
| [getMaxDataColumn()](#getMaxDataColumn--) | Maximaler Spaltenindex der Zelle, die Daten enthält. |
| [getMaxDataRow()](#getMaxDataRow--) | Maximaler Zeilenindex der Zelle, die Daten enthält. |
| [getMaxRow()](#getMaxRow--) | Maximaler Zeilenindex der Zelle, die Daten oder Stil enthält. |
| [getMergedCells()](#getMergedCells--) | Ermittelt die Sammlung zusammengeführter Zellen. |
| [getMinColumn()](#getMinColumn--) | Minimaler Spaltenindex der Zellen, die in der Sammlung instanziiert wurden (schließt die Spalte nicht ein, in der der Stil für die gesamte Spalte definiert ist, aber keine Zelle instanziiert wurde). |
| [getMinDataColumn()](#getMinDataColumn--) | Minimaler Spaltenindex der Zelle, die Daten enthält. |
| [getMinDataRow()](#getMinDataRow--) | Minimaler Zeilenindex der Zelle, die Daten enthält. |
| [getMinRow()](#getMinRow--) | Minimaler Zeilenindex der Zelle, die Daten oder Stil enthält. |
| [getRow(int i)](#getRow-int-) | Ruft das [GridRow](../../com.aspose.gridweb/gridrow)-Element am angegebenen Zeilenindex der Zelle ab. |
| [getRowEnumerator()](#getRowEnumerator--) | Ruft den Zeilen-Enumerator ab. |
| [getRowHeight(int row)](#getRowHeight-int-) | Ermittelt die Höhe einer angegebenen Zeile. |
| [getRowHeightInch(int row)](#getRowHeightInch-int-) | Ermittelt die Höhe einer angegebenen Zeile in der Einheit Zoll. |
| [getRowHeightPixel(int row)](#getRowHeightPixel-int-) | Ermittelt die Höhe einer angegebenen Zeile in der Einheit Pixel. |
| [getRowOutlineLevel(int rowIndex)](#getRowOutlineLevel-int-) | Ermittelt die Gliederungsebene der Zeile. |
| [getRows()](#getRows--) | Ruft die Sammlung von [GridRow](../../com.aspose.gridweb/gridrow)-Objekten ab, die die einzelnen Zeilen in diesem Arbeitsblatt darstellen. |
| [getStandardHeight()](#getStandardHeight--) | Ruft die Standardzeilenhöhe in diesem Arbeitsblatt in Punkten ab. |
| [getStandardHeightPixels()](#getStandardHeightPixels--) | Ruft die Standardzeilenhöhe in diesem Arbeitsblatt in Pixeln ab. |
| [getStandardWidth()](#getStandardWidth--) | Ermittelt die Standardspaltenbreite im Arbeitsblatt in Zeichen. |
| [getStandardWidthInch()](#getStandardWidthInch--) | Ermittelt die Standardspaltenbreite im Arbeitsblatt in der Einheit Zoll. |
| [getStandardWidthPixels()](#getStandardWidthPixels--) | Ermittelt die Standardspaltenbreite im Arbeitsblatt in der Einheit Pixel. |
| [getViewColumnWidthPixel(int column)](#getViewColumnWidthPixel-int-) | Ermittelt die Breite in verschiedenen Ansichtstypen. |
| [groupColumns(int firstIndex, int lastIndex)](#groupColumns-int-int-) | Gruppiert Spalten. |
| [groupColumns(int firstIndex, int lastIndex, boolean isHidden)](#groupColumns-int-int-boolean-) | Gruppiert Spalten. |
| [groupRows(int firstIndex, int lastIndex)](#groupRows-int-int-) | Gruppiert Zeilen. |
| [hashCode()](#hashCode--) |  |
| [hideColumn(int column)](#hideColumn-int-) | Blendet eine Spalte aus. |
| [hideRow(int row)](#hideRow-int-) | Blendet eine Zeile aus. |
| [insertColumn(int columnIndex)](#insertColumn-int-) | Fügt eine neue Spalte in das Arbeitsblatt ein. |
| [insertColumn(int columnIndex, boolean updateReference)](#insertColumn-int-boolean-) | Fügt eine neue Spalte in das Arbeitsblatt ein. |
| [insertColumns(int columnIndex, int totalColumns)](#insertColumns-int-int-) | Fügt mehrere Spalten in das Arbeitsblatt ein. |
| [insertColumns(int columnIndex, int totalColumns, boolean updateReference)](#insertColumns-int-int-boolean-) | Fügt mehrere Spalten in das Arbeitsblatt ein. |
| [insertRange(GridCellArea area, int shiftType)](#insertRange-com.aspose.gridweb.GridCellArea-int-) | Fügt einen Zellbereich ein und verschiebt Zellen gemäß der Verschiebungsoption. |
| [insertRange(GridCellArea area, int shiftNumber, int shiftType, boolean updateReference)](#insertRange-com.aspose.gridweb.GridCellArea-int-int-boolean-) | Fügt einen Zellbereich ein und verschiebt Zellen gemäß der Verschiebungsoption. |
| [insertRow(int rowIndex)](#insertRow-int-) | Fügt eine neue Zeile in das Arbeitsblatt ein. |
| [insertRows(int rowIndex, int totalRows)](#insertRows-int-int-) | Fügt mehrere Zeilen in das Arbeitsblatt ein. |
| [insertRows(int rowIndex, int totalRows, boolean updateReference)](#insertRows-int-int-boolean-) | Fügt mehrere Zeilen in das Arbeitsblatt ein. |
| [isBlankColumn(int columnIndex)](#isBlankColumn-int-) | Überprüft, ob die angegebene Spalte leer ist (enthält keine Daten). |
| [isColumnHidden(int columnIndex)](#isColumnHidden-int-) | Überprüft, ob eine Spalte am angegebenen Index ausgeblendet ist. |
| [isRowHidden(int rowIndex)](#isRowHidden-int-) | Überprüft, ob eine Zeile am angegebenen Index ausgeblendet ist. |
| [iterator()](#iterator--) | Ruft den Zeilen-Enumerator ab. |
| [merge(int firstRow, int firstColumn, int totalRows, int totalColumns)](#merge-int-int-int-int-) | Führt einen angegebenen Zellbereich zu einer einzelnen Zelle zusammen. |
| [moveRange(GridCellArea sourceArea, int destRow, int destColumn)](#moveRange-com.aspose.gridweb.GridCellArea-int-int-) | Verschiebt den Bereich. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeDuplicates(int startRow, int startColumn, int endRow, int endColumn)](#removeDuplicates-int-int-int-int-) | Entfernt doppelte Werte im Bereich. |
| [removeFormulas()](#removeFormulas--) | Entfernt alle Formeln und ersetzt sie durch den Ergebniswert. |
| [setBorders(int firstRow, int firstColumn, int rowNumber, int columnNumber, int position, WebBorderStyle borderStyle)](#setBorders-int-int-int-int-int-com.aspose.gridweb.WebBorderStyle-) | Setzt Rahmen für einen Zellenbereich. |
| [setColumnWidth(int column, double width)](#setColumnWidth-int-double-) | Setzt die Breite der angegebenen Spalte. |
| [setColumnWidthInch(int column, double inches)](#setColumnWidthInch-int-double-) | Setzt die Spaltenbreite in Zoll. |
| [setColumnWidthPixel(int column, int pixel)](#setColumnWidthPixel-int-int-) | Setzt die Spaltenbreite in Pixel. |
| [setRowHeight(int row, double height)](#setRowHeight-int-double-) | Setzt die Höhe der angegebenen Zeile. |
| [setRowHeightInch(int row, double inches)](#setRowHeightInch-int-double-) | Setzt die Zeilenhöhe in Zoll. |
| [setRowHeightPixel(int row, int pixels)](#setRowHeightPixel-int-int-) | Setzt die Zeilenhöhe in Pixeln. |
| [setRowOutlineLevel(int rowIndex, int outlineLevel)](#setRowOutlineLevel-int-int-) | Setzt die Gliederungsebene der Zeile. |
| [setStandardHeight(double value)](#setStandardHeight-double-) | Setzt die Standardzeilenhöhe in diesem Arbeitsblatt, in Punkten. |
| [setStandardHeightPixels(int value)](#setStandardHeightPixels-int-) | Setzt die Standardzeilenhöhe in diesem Arbeitsblatt, in Pixeln. |
| [setStandardWidth(double value)](#setStandardWidth-double-) | Setzt die Standardspaltenbreite im Arbeitsblatt in Zeichen. |
| [setStandardWidthInch(double value)](#setStandardWidthInch-double-) | Legt die Standardspaltenbreite im Arbeitsblatt fest, in der Einheit Zoll. |
| [setStandardWidthPixels(int value)](#setStandardWidthPixels-int-) | Legt die Standardspaltenbreite im Arbeitsblatt fest, in der Einheit Pixel. |
| [setStyle(int firstRow, int firstColumn, int rowNumber, int columnNumber, GridTableItemStyle style)](#setStyle-int-int-int-int-com.aspose.gridweb.GridTableItemStyle-) | Setzt den Stil für einen angegebenen Zellenbereich. |
| [setStyle(String cellRange, GridTableItemStyle style)](#setStyle-java.lang.String-com.aspose.gridweb.GridTableItemStyle-) | Setzt den Stil für einen angegebenen Zellenbereich. |
| [sort(int startRow, int startColumn, int rows, int columns, int index, boolean isAsending, boolean isCaseSensitive, boolean islefttoright)](#sort-int-int-int-int-int-boolean-boolean-boolean-) | Sortiert die Daten aufsteigend/absteigend von oben nach unten in einem Bereich eines Arbeitsblatts nach dem angegebenen Spaltenindex. |
| [sort(int startRow, int startColumn, int rows, int columns, int[] indexes, int[] orders, int orientation, boolean isCaseSensitive)](#sort-int-int-int-int-int---int---int-boolean-) | Sortiert die Daten aufsteigend/absteigend von oben nach unten in einem Bereich eines Arbeitsblatts nach dem angegebenen Spaltenindex. |
| [toString()](#toString--) |  |
| [unMerge(int firstRow, int firstColumn, int totalRows, int totalColumns)](#unMerge-int-int-int-int-) | Löst einen angegebenen Bereich zusammengeführter Zellen. |
| [ungroupColumns(int firstIndex, int lastIndex)](#ungroupColumns-int-int-) | Hebt die Gruppierung von Spalten auf. |
| [ungroupRows(int firstIndex, int lastIndex)](#ungroupRows-int-int-) | Hebt die Gruppierung von Zeilen auf. |
| [unhideColumn(int column, double width)](#unhideColumn-int-double-) | Blendet eine Spalte ein |
| [unhideRow(int row)](#unhideRow-int-) | Blendet eine Zeile ein. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### cellIndexToName(int row, int column) {#cellIndexToName-int-int-}
```
public static String cellIndexToName(int row, int column)
```


Ermittelt den Zellenamen anhand seiner Zeilen‑ und Spaltenindizes.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex. |
| Spalte | int | Spaltenindex. |

**Returns:**
java.lang.String - Name der Zelle.
### cellNameToIndex(String cellName, int row, int column) {#cellNameToIndex-java.lang.String-int-int-}
```
public static void cellNameToIndex(String cellName, int row, int column)
```


Ermittelt die Zeilen‑ und Spaltenindizes der Zelle gemäß ihrem Namen

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellName | java.lang.String | Name der Zelle. |
| Zeile | int | Ausgabezeilenindex |
| Spalte | int | Ausgabespaltenindex |

### checkCell(int row, int column) {#checkCell-int-int-}
```
public GridCell checkCell(int row, int column)
```


Ermittelt das [GridCell](../../com.aspose.gridweb/gridcell)-Element oder null am angegebenen Zeilen‑ und Spaltenindex der Zelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex |
| Spalte | int | Spaltenindex |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - Return GridCell object if a GridCell object exists. Return null if the GridCell does not exist.
### checkColumn(int col) {#checkColumn-int-}
```
public GridColumn checkColumn(int col)
```


Ermittelt das [GridColumn](../../com.aspose.gridweb/gridcolumn)-Element oder null am angegebenen Spaltenindex.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Spalte | int | Der Spaltenindex. |

**Returns:**
[GridColumn](../../com.aspose.gridweb/gridcolumn) - The Column object.
### checkRow(int i) {#checkRow-int-}
```
public GridRow checkRow(int i)
```


Ermittelt das [GridRow](../../com.aspose.gridweb/gridrow)-Element oder null am angegebenen Zeilenindex der Zelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| i | int | Zeilenindex |

**Returns:**
[GridRow](../../com.aspose.gridweb/gridrow) - Returns [GridRow](../../com.aspose.gridweb/gridrow) object If the row object does exist, otherwise returns null.
### clear() {#clear--}
```
public void clear()
```


Löscht alle Zellen in der Sammlung.

### clearContents(GridCellArea range) {#clearContents-com.aspose.gridweb.GridCellArea-}
```
public void clearContents(GridCellArea range)
```


Löscht den Inhalt eines Bereichs.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| range | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Zu löschender Bereich. |

### clearContents(int startRow, int startColumn, int endRow, int endColumn) {#clearContents-int-int-int-int-}
```
public void clearContents(int startRow, int startColumn, int endRow, int endColumn)
```


Löscht den Inhalt eines Bereichs.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | int | Startzeilenindex. |
| startColumn | int | Startspaltenindex. |
| endRow | int | Endzeilenindex. |
| endColumn | int | Endspaltenindex. |

### clearFormats(GridCellArea range) {#clearFormats-com.aspose.gridweb.GridCellArea-}
```
public void clearFormats(GridCellArea range)
```


Löscht die Formatierung eines Bereichs.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| range | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Zu löschender Bereich. |

### clearFormats(int startRow, int startColumn, int endRow, int endColumn) {#clearFormats-int-int-int-int-}
```
public void clearFormats(int startRow, int startColumn, int endRow, int endColumn)
```


Löscht die Formatierung eines Bereichs.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | int | Startzeilenindex. |
| startColumn | int | Startspaltenindex. |
| endRow | int | Endzeilenindex. |
| endColumn | int | Endspaltenindex. |

### clearRange(GridCellArea range) {#clearRange-com.aspose.gridweb.GridCellArea-}
```
public void clearRange(GridCellArea range)
```


Löscht Inhalt und Formatierung eines Bereichs.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| range | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Zu löschender Bereich. |

### clearRange(int startRow, int startColumn, int endRow, int endColumn) {#clearRange-int-int-int-int-}
```
public void clearRange(int startRow, int startColumn, int endRow, int endColumn)
```


Löscht Inhalt und Formatierung eines Bereichs.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | int | Startzeilenindex. |
| startColumn | int | Startspaltenindex. |
| endRow | int | Endzeilenindex. |
| endColumn | int | Endspaltenindex. |

### columnIndexToName(int column) {#columnIndexToName-int-}
```
public static String columnIndexToName(int column)
```


Ermittelt den Spaltennamen anhand des Spaltenindex.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Spalte | int | Spaltenindex. |

**Returns:**
java.lang.String - Name der Spalte.
### columnNameToIndex(String columnName) {#columnNameToIndex-java.lang.String-}
```
public static int columnNameToIndex(String columnName)
```


Ermittelt den Spaltenindex anhand des Spaltennamens.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnName | java.lang.String | Spaltenname. |

**Returns:**
int - Spaltenindex.
### copyColumn(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex) {#copyColumn-com.aspose.gridweb.GridCells-int-int-}
```
public void copyColumn(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex)
```


Kopiert Daten und Formatierungen einer gesamten Spalte.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceCells | [GridCells](../../com.aspose.gridweb/gridcells) | Das Source Cells-Objekt enthält Daten und Formatierungen zum Kopieren. |
| sourceColumnIndex | int | Quellspaltenindex. |
| destinationColumnIndex | int | Zielspaltenindex. |

### copyColumns(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber) {#copyColumns-com.aspose.gridweb.GridCells-int-int-int-}
```
public void copyColumns(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber)
```


Kopiert Daten und Formatierungen einer gesamten Spalte.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceCells | [GridCells](../../com.aspose.gridweb/gridcells) | Das Source Cells-Objekt enthält Daten und Formatierungen zum Kopieren. |
| sourceColumnIndex | int | Quellspaltenindex. |
| destinationColumnIndex | int | Zielspaltenindex. |
| columnNumber | int | Die kopierte Spaltennummer. |

### copyRow(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex) {#copyRow-com.aspose.gridweb.GridCells-int-int-}
```
public void copyRow(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex)
```


Kopiert Daten und Formatierungen einer gesamten Zeile.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceCells | [GridCells](../../com.aspose.gridweb/gridcells) | Das Source Cells-Objekt enthält Daten und Formatierungen zum Kopieren. |
| sourceRowIndex | int | Quellzeilenindex. |
| destinationRowIndex | int | Zielzeilenindex. |

### copyRows(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber) {#copyRows-com.aspose.gridweb.GridCells-int-int-int-}
```
public void copyRows(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)
```


Kopiert Daten und Formatierungen einiger ganzer Zeilen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceCells | [GridCells](../../com.aspose.gridweb/gridcells) | Das Source Cells-Objekt enthält Daten und Formatierungen zum Kopieren. |
| sourceRowIndex | int | Quellzeilenindex. |
| destinationRowIndex | int | Zielzeilenindex. |
| rowNumber | int | Die kopierte Zeilennummer. |

### deleteBlankColumns() {#deleteBlankColumns--}
```
public void deleteBlankColumns()
```


Löscht alle leeren Spalten, die keine Daten enthalten.

### deleteBlankRows() {#deleteBlankRows--}
```
public void deleteBlankRows()
```


Löscht alle leeren Zeilen, die keine Daten enthalten.

### deleteColumn(int columnIndex) {#deleteColumn-int-}
```
public void deleteColumn(int columnIndex)
```


Löscht eine Spalte.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnIndex | int | Spaltenindex. |

### deleteColumn(int columnIndex, boolean updateReference) {#deleteColumn-int-boolean-}
```
public void deleteColumn(int columnIndex, boolean updateReference)
```


Löscht eine Spalte.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnIndex | int | Spaltenindex. |
| updateReference | boolean | Gibt an, ob Verweise in anderen Arbeitsblättern aktualisiert werden. |

### deleteColumns(int columnIndex, int totalColumns, boolean updateReference) {#deleteColumns-int-int-boolean-}
```
public void deleteColumns(int columnIndex, int totalColumns, boolean updateReference)
```


Löscht mehrere Spalten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnIndex | int | Spaltenindex. |
| totalColumns | int | Anzahl der zu löschenden Spalten. |
| updateReference | boolean | Gibt an, ob Verweise in anderen Arbeitsblättern aktualisiert werden. |

### deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType) {#deleteRange-int-int-int-int-int-}
```
public void deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType)
```


Löscht einen Zellbereich und verschiebt Zellen gemäß der Verschiebeoption.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | int | Startzeilenindex. |
| startColumn | int | Startspaltenindex. |
| endRow | int | Endzeilenindex. |
| endColumn | int | Endspaltenindex. |
| shiftType | int | [GridShiftType](../../com.aspose.gridweb/gridshifttype). Zellenverschiebungsoption. |

### deleteRow(int rowIndex) {#deleteRow-int-}
```
public void deleteRow(int rowIndex)
```


Löscht eine Zeile.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowIndex | int | Zeilenindex. |

### deleteRows(int rowIndex, int totalRows) {#deleteRows-int-int-}
```
public boolean deleteRows(int rowIndex, int totalRows)
```


Löscht mehrere Zeilen.

**Remarks**

Wenn der gelöschte Bereich den oberen Teil (nicht das Ganze) der Tabelle (ListObject) enthält, kann der Bereich nicht gelöscht werden und es wird nichts unternommen. Es funktioniert wie in MS Excel.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowIndex | int | Der Index der ersten zu löschenden Zeile. |
| totalRows | int | Anzahl der zu löschenden Zeilen. |

**Returns:**
boolean
### deleteRows(int rowIndex, int totalRows, boolean updateReference) {#deleteRows-int-int-boolean-}
```
public boolean deleteRows(int rowIndex, int totalRows, boolean updateReference)
```


Löscht mehrere Zeilen im Arbeitsblatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowIndex | int | Zeilenindex. |
| totalRows | int | Anzahl der zu löschenden Zeilen. |
| updateReference | boolean | Gibt an, ob Verweise in anderen Arbeitsblättern aktualisiert werden. |

**Returns:**
boolean -
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
### exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns) {#exportArray-int-int-int-int-}
```
public Object[][] exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


Exportiert Daten aus der [GridCells](../../com.aspose.gridweb/gridcells)-Sammlung in ein zweidimensionales Array-Objekt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstRow | int | Die Zeilennummer der ersten zu exportierenden Zelle. |
| firstColumn | int | Die Spaltennummer der ersten zu exportierenden Zelle. |
| totalRows | int | Anzahl der zu exportierenden Zeilen |
| totalColumns | int | Anzahl der zu exportierenden Spalten |

**Returns:**
java.lang.Object[][] - Exportiertes Zellwert-Array-Objekt.
### get(int row, int column) {#get-int-int-}
```
public GridCell get(int row, int column)
```


Ruft das [GridCell](../../com.aspose.gridweb/gridcell)-Element am angegebenen Zeilenindex und Spaltenindex der Zelle ab.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         GridCells cells = GridWeb1.getWorkSheets().get(0).getCells();
         //Gets the cell at "A1"
         GridCell cell = cells.get(0, 0);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex. |
| Spalte | int | Spaltenindex. |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - The [GridCell](../../com.aspose.gridweb/gridcell) object.
### get(String cellName) {#get-java.lang.String-}
```
public GridCell get(String cellName)
```


Ruft das [GridCell](../../com.aspose.gridweb/gridcell)-Element mit dem angegebenen Zellenamen ab.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
          GridCells cells = GridWeb1.getWorkSheets().get(0).getCells();
          GridCell cell = cells.get("A1");	//Gets the cell at "A1"
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellName | java.lang.String | Zellname, einschließlich des Spaltenbuchstabens und der Zeilennummer, zum Beispiel A5. |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - A [GridCell](../../com.aspose.gridweb/gridcell) object
### getCell(int row, int column) {#getCell-int-int-}
```
public GridCell getCell(int row, int column)
```


Ruft das [GridCell](../../com.aspose.gridweb/gridcell)-Element am angegebenen Zeilenindex und Spaltenindex der Zelle ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex |
| Spalte | int | Spaltenindex |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - Return Cell object
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnWidth(int column) {#getColumnWidth-int-}
```
public double getColumnWidth(int column)
```


Ermittelt die Breite der angegebenen Spalte

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Spalte | int | Spaltenindex |

**Returns:**
double - Breite der Spalte
### getColumnWidthInch(int column) {#getColumnWidthInch-int-}
```
public double getColumnWidthInch(int column)
```


Ermittelt die Breite der angegebenen Spalte in Zoll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Spalte | int | Spaltenindex |

**Returns:**
double - Breite der Spalte
### getColumnWidthPixel(int column) {#getColumnWidthPixel-int-}
```
public int getColumnWidthPixel(int column)
```


Ermittelt die Breite der angegebenen Spalte in Pixel.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Spalte | int | Spaltenindex |

**Returns:**
int – Breite der Spalte in der Normalansicht.
### getColumns() {#getColumns--}
```
public GridColumnCollection getColumns()
```


Ruft die Sammlung von [GridColumn](../../com.aspose.gridweb/gridcolumn)-Objekten ab, die die einzelnen Spalten in diesem Arbeitsblatt darstellen.

**Returns:**
[GridColumnCollection](../../com.aspose.gridweb/gridcolumncollection)
### getCount() {#getCount--}
```
public int getCount()
```


Ermittelt die Anzahl der Zellen.

**Returns:**
int
### getFirstCell() {#getFirstCell--}
```
public GridCell getFirstCell()
```


Ermittelt die erste Zelle in diesem Arbeitsblatt.

**Remarks**

Gibt null zurück, wenn im Arbeitsblatt keine Daten vorhanden sind.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getLastCell() {#getLastCell--}
```
public GridCell getLastCell()
```


Ermittelt die letzte Zelle in diesem Arbeitsblatt.

**Remarks**

Gibt null zurück, wenn im Arbeitsblatt keine Daten vorhanden sind.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getMaxColumn() {#getMaxColumn--}
```
public int getMaxColumn()
```


Maximaler Spaltenindex einer Zelle, die Daten oder Formatierungen enthält.

**Remarks**

Gibt -1 zurück, wenn kein Feld vorhanden ist.

**Returns:**
int
### getMaxDataColumn() {#getMaxDataColumn--}
```
public int getMaxDataColumn()
```


Maximaler Spaltenindex der Zelle, die Daten enthält.

**Remarks**

\-1 wird zurückgegeben, wenn kein Feld vorhanden ist, das Daten enthält. Diese Eigenschaft muss alle Zellen in einem Arbeitsblatt iterieren und prüfen, daher ist es ein zeitintensiver Vorgang und sollte nicht wiederholt aufgerufen werden.

**Returns:**
int
### getMaxDataRow() {#getMaxDataRow--}
```
public int getMaxDataRow()
```


Maximaler Zeilenindex der Zelle, die Daten enthält.

**Remarks**

Gibt -1 zurück, wenn kein Feld vorhanden ist, das Daten enthält.

**Returns:**
int
### getMaxRow() {#getMaxRow--}
```
public int getMaxRow()
```


Maximaler Zeilenindex der Zelle, die Daten oder Stil enthält.

**Remarks**

Gibt -1 zurück, wenn im Arbeitsblatt kein Feld vorhanden ist, das Daten oder Format enthält.

**Returns:**
int
### getMergedCells() {#getMergedCells--}
```
public ArrayList getMergedCells()
```


Ermittelt die Sammlung zusammengeführter Zellen.

**Remarks**

In dieser Sammlung ist jedes Element eine [GridCellArea](../../com.aspose.gridweb/gridcellarea)-Struktur, die einen Bereich zusammengeführter Zellen darstellt.

**Returns:**
java.util.ArrayList
### getMinColumn() {#getMinColumn--}
```
public int getMinColumn()
```


Minimaler Spaltenindex der Zellen, die in der Sammlung instanziiert wurden (schließt die Spalte nicht ein, in der der Stil für die gesamte Spalte definiert ist, aber keine Zelle instanziiert wurde).

**Returns:**
int
### getMinDataColumn() {#getMinDataColumn--}
```
public int getMinDataColumn()
```


Minimaler Spaltenindex der Zelle, die Daten enthält.

**Remarks**

\-1 wird zurückgegeben, wenn kein Feld vorhanden ist, das Daten enthält. Diese Eigenschaft muss alle Zellen in einem Arbeitsblatt iterieren und prüfen, daher ist es ein zeitintensiver Vorgang und sollte nicht wiederholt aufgerufen werden.

**Returns:**
int
### getMinDataRow() {#getMinDataRow--}
```
public int getMinDataRow()
```


Minimaler Zeilenindex der Zelle, die Daten enthält.

**Returns:**
int
### getMinRow() {#getMinRow--}
```
public int getMinRow()
```


Minimaler Zeilenindex der Zelle, die Daten oder Stil enthält.

**Returns:**
int
### getRow(int i) {#getRow-int-}
```
public GridRow getRow(int i)
```


Ruft das [GridRow](../../com.aspose.gridweb/gridrow)-Element am angegebenen Zeilenindex der Zelle ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| i | int | Zeilenindex |

**Returns:**
[GridRow](../../com.aspose.gridweb/gridrow) - the row object
### getRowEnumerator() {#getRowEnumerator--}
```
public Iterator getRowEnumerator()
```


Ruft den Zeilen-Enumerator ab.

**Returns:**
java.util.Iterator - Der Zeilen-Enumerator.
### getRowHeight(int row) {#getRowHeight-int-}
```
public double getRowHeight(int row)
```


Ermittelt die Höhe einer angegebenen Zeile.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex |

**Returns:**
double – Höhe der Zeile
### getRowHeightInch(int row) {#getRowHeightInch-int-}
```
public double getRowHeightInch(int row)
```


Ermittelt die Höhe einer angegebenen Zeile in der Einheit Zoll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex |

**Returns:**
double – Höhe der Zeile
### getRowHeightPixel(int row) {#getRowHeightPixel-int-}
```
public int getRowHeightPixel(int row)
```


Ermittelt die Höhe einer angegebenen Zeile in der Einheit Pixel.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex |

**Returns:**
int – Höhe der Zeile
### getRowOutlineLevel(int rowIndex) {#getRowOutlineLevel-int-}
```
public int getRowOutlineLevel(int rowIndex)
```


Ermittelt die Gliederungsebene der Zeile.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowIndex | int | Zeilenindex. |

**Returns:**
int - die Gliederungsebene.
### getRows() {#getRows--}
```
public GridRowCollection getRows()
```


Ruft die Sammlung von [GridRow](../../com.aspose.gridweb/gridrow)-Objekten ab, die die einzelnen Zeilen in diesem Arbeitsblatt darstellen.

**Returns:**
[GridRowCollection](../../com.aspose.gridweb/gridrowcollection)
### getStandardHeight() {#getStandardHeight--}
```
public double getStandardHeight()
```


Ruft die Standardzeilenhöhe in diesem Arbeitsblatt in Punkten ab.

**Returns:**
double
### getStandardHeightPixels() {#getStandardHeightPixels--}
```
public int getStandardHeightPixels()
```


Ruft die Standardzeilenhöhe in diesem Arbeitsblatt in Pixeln ab.

**Returns:**
int
### getStandardWidth() {#getStandardWidth--}
```
public double getStandardWidth()
```


Ermittelt die Standardspaltenbreite im Arbeitsblatt in Zeichen.

**Returns:**
double
### getStandardWidthInch() {#getStandardWidthInch--}
```
public double getStandardWidthInch()
```


Ermittelt die Standardspaltenbreite im Arbeitsblatt in der Einheit Zoll.

**Returns:**
double
### getStandardWidthPixels() {#getStandardWidthPixels--}
```
public int getStandardWidthPixels()
```


Ermittelt die Standardspaltenbreite im Arbeitsblatt in der Einheit Pixel.

**Returns:**
int
### getViewColumnWidthPixel(int column) {#getViewColumnWidthPixel-int-}
```
public int getViewColumnWidthPixel(int column)
```


Ermittelt die Breite in verschiedenen Ansichtstypen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Spalte | int | Der Spaltenindex. |

**Returns:**
int – die Spaltenbreite in Pixeln
### groupColumns(int firstIndex, int lastIndex) {#groupColumns-int-int-}
```
public void groupColumns(int firstIndex, int lastIndex)
```


Gruppiert Spalten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstIndex | int | Der erste Spaltenindex, der gruppiert werden soll. |
| lastIndex | int | Der letzte Spaltenindex, der gruppiert werden soll. |

### groupColumns(int firstIndex, int lastIndex, boolean isHidden) {#groupColumns-int-int-boolean-}
```
public void groupColumns(int firstIndex, int lastIndex, boolean isHidden)
```


Gruppiert Spalten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstIndex | int | Der erste Spaltenindex, der gruppiert werden soll. |
| lastIndex | int | Der letzte Spaltenindex, der gruppiert werden soll. |
| isHidden | boolean | Gibt an, ob die gruppierten Spalten ausgeblendet sind. |

### groupRows(int firstIndex, int lastIndex) {#groupRows-int-int-}
```
public void groupRows(int firstIndex, int lastIndex)
```


Gruppiert Zeilen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstIndex | int | Der erste Zeilenindex, der gruppiert werden soll. |
| lastIndex | int | Der letzte Zeilenindex, der gruppiert werden soll. |

### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### hideColumn(int column) {#hideColumn-int-}
```
public void hideColumn(int column)
```


Blendet eine Spalte aus.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Spalte | int | Spaltenindex. |

### hideRow(int row) {#hideRow-int-}
```
public void hideRow(int row)
```


Blendet eine Zeile aus.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex. |

### insertColumn(int columnIndex) {#insertColumn-int-}
```
public void insertColumn(int columnIndex)
```


Fügt eine neue Spalte in das Arbeitsblatt ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnIndex | int | Spaltenindex. |

### insertColumn(int columnIndex, boolean updateReference) {#insertColumn-int-boolean-}
```
public void insertColumn(int columnIndex, boolean updateReference)
```


Fügt eine neue Spalte in das Arbeitsblatt ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnIndex | int | Spaltenindex. |
| updateReference | boolean | Gibt an, ob Verweise in anderen Arbeitsblättern aktualisiert werden. |

### insertColumns(int columnIndex, int totalColumns) {#insertColumns-int-int-}
```
public void insertColumns(int columnIndex, int totalColumns)
```


Fügt mehrere Spalten in das Arbeitsblatt ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnIndex | int | Spaltenindex. |
| totalColumns | int | Die Anzahl der Spalten. |

### insertColumns(int columnIndex, int totalColumns, boolean updateReference) {#insertColumns-int-int-boolean-}
```
public void insertColumns(int columnIndex, int totalColumns, boolean updateReference)
```


Fügt mehrere Spalten in das Arbeitsblatt ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnIndex | int | Spaltenindex. |
| totalColumns | int | Die Anzahl der Spalten. |
| updateReference | boolean | Gibt an, ob Verweise in anderen Arbeitsblättern aktualisiert werden. |

### insertRange(GridCellArea area, int shiftType) {#insertRange-com.aspose.gridweb.GridCellArea-int-}
```
public void insertRange(GridCellArea area, int shiftType)
```


Fügt einen Zellbereich ein und verschiebt Zellen gemäß der Verschiebungsoption.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| area | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Verschiebebereich. |
| shiftType | int | [GridShiftType](../../com.aspose.gridweb/gridshifttype). Zellenverschiebungsoption. |

### insertRange(GridCellArea area, int shiftNumber, int shiftType, boolean updateReference) {#insertRange-com.aspose.gridweb.GridCellArea-int-int-boolean-}
```
public void insertRange(GridCellArea area, int shiftNumber, int shiftType, boolean updateReference)
```


Fügt einen Zellbereich ein und verschiebt Zellen gemäß der Verschiebungsoption.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| area | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Verschiebebereich. |
| shiftNumber | int | Anzahl der einzufügenden Zeilen oder Spalten. |
| shiftType | int | [GridShiftType](../../com.aspose.gridweb/gridshifttype). Zellenverschiebungsoption. |
| updateReference | boolean | Gibt an, ob Verweise in anderen Arbeitsblättern aktualisiert werden. |

### insertRow(int rowIndex) {#insertRow-int-}
```
public void insertRow(int rowIndex)
```


Fügt eine neue Zeile in das Arbeitsblatt ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowIndex | int | Zeilenindex. |

### insertRows(int rowIndex, int totalRows) {#insertRows-int-int-}
```
public void insertRows(int rowIndex, int totalRows)
```


Fügt mehrere Zeilen in das Arbeitsblatt ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowIndex | int | Zeilenindex. |
| totalRows | int | Anzahl der einzufügenden Zeilen. |

### insertRows(int rowIndex, int totalRows, boolean updateReference) {#insertRows-int-int-boolean-}
```
public void insertRows(int rowIndex, int totalRows, boolean updateReference)
```


Fügt mehrere Zeilen in das Arbeitsblatt ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowIndex | int | Zeilenindex. |
| totalRows | int | Anzahl der einzufügenden Zeilen. |
| updateReference | boolean | Gibt an, ob Verweise in anderen Arbeitsblättern aktualisiert werden. |

### isBlankColumn(int columnIndex) {#isBlankColumn-int-}
```
public boolean isBlankColumn(int columnIndex)
```


Überprüft, ob die angegebene Spalte leer ist (enthält keine Daten).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnIndex | int | der Spaltenindex |

**Returns:**
boolesch - wahr, wenn die angegebene Spalte keine Daten enthält
### isColumnHidden(int columnIndex) {#isColumnHidden-int-}
```
public boolean isColumnHidden(int columnIndex)
```


Überprüft, ob eine Spalte am angegebenen Index ausgeblendet ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnIndex | int | Spaltenindex |

**Returns:**
boolesch - wahr, wenn die Spalte ausgeblendet ist.
### isRowHidden(int rowIndex) {#isRowHidden-int-}
```
public boolean isRowHidden(int rowIndex)
```


Überprüft, ob eine Zeile am angegebenen Index ausgeblendet ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowIndex | int | Zeilenindex |

**Returns:**
boolesch - wahr, wenn die Zeile ausgeblendet ist
### iterator() {#iterator--}
```
public Iterator iterator()
```


Ruft den Zeilen-Enumerator ab.

**Returns:**
java.util.Iterator – Der Zeilen-Enumerator.
### merge(int firstRow, int firstColumn, int totalRows, int totalColumns) {#merge-int-int-int-int-}
```
public void merge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


Führt einen angegebenen Zellbereich zu einer einzelnen Zelle zusammen.

**Remarks**

Referenzieren Sie die zusammengeführte Zelle über die Adresse der oberen linken Zelle im Bereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstRow | int | Erste Zeile dieses Bereichs (nullbasiert) |
| firstColumn | int | Erste Spalte dieses Bereichs (nullbasiert) |
| totalRows | int | Anzahl der Zeilen (einsbasiert) |
| totalColumns | int | Anzahl der Spalten (beginnend bei 1) |

### moveRange(GridCellArea sourceArea, int destRow, int destColumn) {#moveRange-com.aspose.gridweb.GridCellArea-int-int-}
```
public void moveRange(GridCellArea sourceArea, int destRow, int destColumn)
```


Verschiebt den Bereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Der Bereich, der verschoben werden soll. |
| destRow | int | Die Zielzeile. |
| destColumn | int | Die Zielspalte. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeDuplicates(int startRow, int startColumn, int endRow, int endColumn) {#removeDuplicates-int-int-int-int-}
```
public void removeDuplicates(int startRow, int startColumn, int endRow, int endColumn)
```


Entfernt doppelte Werte im Bereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | int | Die Startzeile. |
| startColumn | int | Die Startspalte |
| endRow | int | Der Endzeilenindex. |
| endColumn | int | Der Endspaltenindex. |

### removeFormulas() {#removeFormulas--}
```
public void removeFormulas()
```


Entfernt alle Formeln und ersetzt sie durch den Ergebniswert.

### setBorders(int firstRow, int firstColumn, int rowNumber, int columnNumber, int position, WebBorderStyle borderStyle) {#setBorders-int-int-int-int-int-com.aspose.gridweb.WebBorderStyle-}
```
public void setBorders(int firstRow, int firstColumn, int rowNumber, int columnNumber, int position, WebBorderStyle borderStyle)
```


Setzt Rahmen für einen Zellenbereich.

**Example**

```
           GridWeb GridWeb1 = new GridWeb();
           WebBorderStyle borderStyle1 = new WebBorderStyle();
         	 GridWeb1.getWorkSheets().get(0).getCells().setBorders(0, 0, 5, 8, SetBorderPosition.OUTLINE, borderStyle1);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstRow | int | Die erste Zeilennummer des Bereichs (nullbasiert). |
| firstColumn | int | Die erste Spaltennummer des Bereichs (nullbasiert). |
| rowNumber | int | Die Zeilenanzahl. |
| columnNumber | int | Die Spaltenanzahl. |
| position | int | [SetBorderPosition](../../com.aspose.gridweb/setborderposition). Die Randposition. |
| borderStyle | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) | Der Randstil. |

### setColumnWidth(int column, double width) {#setColumnWidth-int-double-}
```
public void setColumnWidth(int column, double width)
```


Setzt die Breite der angegebenen Spalte.

**Remarks**

Um eine Spalte auszublenden, wird die Spaltenbreite auf Null gesetzt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Spalte | int | Spaltenindex. |
| Breite | double | Breite der Spalte. Die Spaltenbreite muss zwischen 0 und 255 liegen. |

### setColumnWidthInch(int column, double inches) {#setColumnWidthInch-int-double-}
```
public void setColumnWidthInch(int column, double inches)
```


Setzt die Spaltenbreite in Zoll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Spalte | int | Spaltenindex. |
| Zoll | double | Anzahl der Zoll. |

### setColumnWidthPixel(int column, int pixel) {#setColumnWidthPixel-int-int-}
```
public void setColumnWidthPixel(int column, int pixel)
```


Setzt die Spaltenbreite in Pixel.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Spalte | int | Spaltenindex. |
| Pixel | int | Anzahl der Pixel. |

### setRowHeight(int row, double height) {#setRowHeight-int-double-}
```
public void setRowHeight(int row, double height)
```


Setzt die Höhe der angegebenen Zeile.

**Remarks**

Um eine Zeile auszublenden, wird die Zeilenhöhe auf Null gesetzt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex. |
| Höhe | double | Höhe der Zeile. In Punkt angegeben. Sie sollte zwischen 0 und 409,5 liegen. |

### setRowHeightInch(int row, double inches) {#setRowHeightInch-int-double-}
```
public void setRowHeightInch(int row, double inches)
```


Setzt die Zeilenhöhe in Zoll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex. |
| Zoll | double | Anzahl der Zoll. Sie sollte zwischen 0 und 409.5/72 liegen. |

### setRowHeightPixel(int row, int pixels) {#setRowHeightPixel-int-int-}
```
public void setRowHeightPixel(int row, int pixels)
```


Setzt die Zeilenhöhe in Pixeln.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex. |
| Pixel | int | Anzahl der Pixel. |

### setRowOutlineLevel(int rowIndex, int outlineLevel) {#setRowOutlineLevel-int-int-}
```
public void setRowOutlineLevel(int rowIndex, int outlineLevel)
```


Setzt die Gliederungsebene der Zeile.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowIndex | int | Zeilenindex. |
| outlineLevel | int | Outline-Ebene. |

### setStandardHeight(double value) {#setStandardHeight-double-}
```
public void setStandardHeight(double value)
```


Setzt die Standardzeilenhöhe in diesem Arbeitsblatt, in Punkten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setStandardHeightPixels(int value) {#setStandardHeightPixels-int-}
```
public void setStandardHeightPixels(int value)
```


Setzt die Standardzeilenhöhe in diesem Arbeitsblatt, in Pixeln.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setStandardWidth(double value) {#setStandardWidth-double-}
```
public void setStandardWidth(double value)
```


Setzt die Standardspaltenbreite im Arbeitsblatt in Zeichen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setStandardWidthInch(double value) {#setStandardWidthInch-double-}
```
public void setStandardWidthInch(double value)
```


Legt die Standardspaltenbreite im Arbeitsblatt fest, in der Einheit Zoll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setStandardWidthPixels(int value) {#setStandardWidthPixels-int-}
```
public void setStandardWidthPixels(int value)
```


Legt die Standardspaltenbreite im Arbeitsblatt fest, in der Einheit Pixel.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setStyle(int firstRow, int firstColumn, int rowNumber, int columnNumber, GridTableItemStyle style) {#setStyle-int-int-int-int-com.aspose.gridweb.GridTableItemStyle-}
```
public void setStyle(int firstRow, int firstColumn, int rowNumber, int columnNumber, GridTableItemStyle style)
```


Setzt den Stil für einen angegebenen Zellenbereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstRow | int | Erste Zeile dieses Bereichs (nullbasiert) |
| firstColumn | int | Erste Spalte dieses Bereichs (nullbasiert) |
| rowNumber | int | Anzahl der Zeilen (einsbasiert) |
| columnNumber | int | Anzahl der Spalten (beginnend bei 1) |
| style | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | Das zu setzende Stilobjekt |

### setStyle(String cellRange, GridTableItemStyle style) {#setStyle-java.lang.String-com.aspose.gridweb.GridTableItemStyle-}
```
public void setStyle(String cellRange, GridTableItemStyle style)
```


Setzt den Stil für einen angegebenen Zellenbereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellRange | java.lang.String | Der Bereich der Zellnamen, z. B. "A1:D6" |
| style | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | Das zu setzende Stilobjekt |

### sort(int startRow, int startColumn, int rows, int columns, int index, boolean isAsending, boolean isCaseSensitive, boolean islefttoright) {#sort-int-int-int-int-int-boolean-boolean-boolean-}
```
public void sort(int startRow, int startColumn, int rows, int columns, int index, boolean isAsending, boolean isCaseSensitive, boolean islefttoright)
```


Sortiert die Daten von oben nach unten in einem Bereich eines Arbeitsblatts nach dem angegebenen Spaltenindex auf- bzw. absteigend. Sortiert die Daten von links nach rechts in einem Bereich eines Arbeitsblatts nach dem angegebenen Zeilenindex auf- bzw. absteigend.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         GridWeb1.getWorkSheets().get(0).getCells().sort(1,0,25,6,3,true,true,false);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | int | Die Zeilennummer der ersten zu sortierenden Zelle. |
| startColumn | int | Die Spaltennummer der ersten zu sortierenden Zelle. |
| rows | int | Anzahl der zu importierenden Zeilen. |
| Spalten | int | Anzahl der zu importierenden Spalten. |
| Index | int | Der Spaltenindex, der die Sortierspalte angibt. Wenn die Orientierung von oben nach unten ist, steht er für den Spaltenindex, der die Sortierspalte angibt. Wenn die Orientierung von links nach rechts ist, steht er für den Zeilenindex, der die Sortierreihen angibt. |
| isAsending | boolean | ob die Sortierreihenfolge aufsteigend ist. |
| isCaseSensitive | boolean | ob die Sortierung Groß-/Kleinschreibung beachtet. |
| islefttoright | boolean | ob die Sortierausrichtung von links nach rechts ist |

### sort(int startRow, int startColumn, int rows, int columns, int[] indexes, int[] orders, int orientation, boolean isCaseSensitive) {#sort-int-int-int-int-int---int---int-boolean-}
```
public void sort(int startRow, int startColumn, int rows, int columns, int[] indexes, int[] orders, int orientation, boolean isCaseSensitive)
```


Sortiert die Daten von oben nach unten in einem Bereich eines Arbeitsblatts nach dem angegebenen Spaltenindex auf- bzw. absteigend. Sortiert die Daten von links nach rechts in einem Bereich eines Arbeitsblatts nach dem angegebenen Zeilenindex auf- bzw. absteigend.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | int | Die Zeilennummer der ersten zu sortierenden Zelle. |
| startColumn | int | Die Spaltennummer der ersten zu sortierenden Zelle. |
| rows | int | Anzahl der zu importierenden Zeilen. |
| Spalten | int | Anzahl der zu importierenden Spalten. |
| indexes | int[] | Das Spaltenindex-Array, das die Sortierspalte angibt. Wenn die Orientierung von oben nach unten ist, steht es für den Spaltenindex, der die Sortierspalte angibt. Wenn die Orientierung von links nach rechts ist, steht es für den Zeilenindex, der die Sortierreihen angibt. |
| orders | int[] | [SortByOrder](../../com.aspose.gridweb/sortbyorder). das Sortierreihenfolge-Array. |
| orientation | int | [SortOrientation](../../com.aspose.gridweb/sortorientation). Sortierausrichtung |
| isCaseSensitive | boolean | ob die Sortierung Groß-/Kleinschreibung beachtet. |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### unMerge(int firstRow, int firstColumn, int totalRows, int totalColumns) {#unMerge-int-int-int-int-}
```
public void unMerge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


Löst einen angegebenen Bereich zusammengeführter Zellen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstRow | int | Erste Zeile dieses Bereichs (nullbasiert) |
| firstColumn | int | Erste Spalte dieses Bereichs (nullbasiert) |
| totalRows | int | Anzahl der Zeilen (einsbasiert) |
| totalColumns | int | Anzahl der Spalten (beginnend bei 1) |

### ungroupColumns(int firstIndex, int lastIndex) {#ungroupColumns-int-int-}
```
public void ungroupColumns(int firstIndex, int lastIndex)
```


Hebt die Gruppierung von Spalten auf.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstIndex | int | Der Index der ersten Spalte, die aufgelöst werden soll. |
| lastIndex | int | Der Index der letzten Spalte, die aufgelöst werden soll. |

### ungroupRows(int firstIndex, int lastIndex) {#ungroupRows-int-int-}
```
public void ungroupRows(int firstIndex, int lastIndex)
```


Hebt die Gruppierung von Zeilen auf.

**Remarks**

Entfernt nur äußere Gruppeninformationen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstIndex | int | Der Index der ersten Zeile, die aufgelöst werden soll. |
| lastIndex | int | Der Index der letzten Zeile, die aufgelöst werden soll. |

### unhideColumn(int column, double width) {#unhideColumn-int-double-}
```
public void unhideColumn(int column, double width)
```


Blendet eine Spalte ein

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Spalte | int | Spaltenindex. |
| Breite | double | Spaltenbreite..Die Spaltenbreite muss zwischen 0 und 255 liegen |

### unhideRow(int row) {#unhideRow-int-}
```
public void unhideRow(int row)
```


Blendet eine Zeile ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex. |

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

