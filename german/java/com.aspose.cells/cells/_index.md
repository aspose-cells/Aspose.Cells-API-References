---
title: "Cells"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Kapselt eine Sammlung von zellenrelevanten Objekten, wie   ...etc."
type: docs
url: /de/java/com.aspose.cells/cells/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Cells implements Iterable
```

Kapselt eine Sammlung von zellenrelevanten Objekten, wie [Cell](../../com.aspose.cells/cell), [Row](../../com.aspose.cells/row), ...etc.

**Remarks**

**Example**

```
         Workbook excel = new Workbook();
         	Cells cells = excel.getWorksheets().get(0).getCells();
 
         	//Set default row height
         	cells.setStandardHeight(20);
         	//Set row height
         	cells.setRowHeight(2, 20.5);
 
         	//Set default colum width
         	cells.setStandardWidth(15);
         	//Set column width
         	cells.setColumnWidth(3, 12.57);
 
         	//Merge cells
         	cells.merge(5, 4, 2, 2);
 
         	//Put values to cells
         	cells.get(0, 0).putValue(true);
         	cells.get(0, 1).putValue(1);
         	cells.get(0, 2).putValue("abc");
 
         //Export data
         Object[][] arr = cells.exportArray(0, 0, 10, 10);
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [addRange(Range rangeObject)](#addRange-com.aspose.cells.Range-) | Fügt einen Bereichsobjektverweis zu Zellen hinzu. |
| [applyColumnStyle(int column, Style style, StyleFlag flag)](#applyColumnStyle-int-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Wendet Formate für eine gesamte Spalte an. |
| [applyRowStyle(int row, Style style, StyleFlag flag)](#applyRowStyle-int-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Wendet Formate für eine gesamte Zeile an. |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Wendet Formate für ein gesamtes Arbeitsblatt an. |
| [checkCell(int row, int column)](#checkCell-int-int-) | Liefert das [Cell](../../com.aspose.cells/cell)‑Element oder null am angegebenen Zeilen‑ und Spaltenindex der Zelle. |
| [checkColumn(int columnIndex)](#checkColumn-int-) | Liefert das [Column](../../com.aspose.cells/column)‑Element oder null am angegebenen Spaltenindex. |
| [checkRow(int row)](#checkRow-int-) | Liefert das [Row](../../com.aspose.cells/row)‑Element oder null am angegebenen Zeilenindex der Zelle. |
| [clear()](#clear--) | Löscht alle Daten des Arbeitsblatts. |
| [clearContents(CellArea range)](#clearContents-com.aspose.cells.CellArea-) | Löscht den Inhalt eines Bereichs. |
| [clearContents(int startRow, int startColumn, int endRow, int endColumn)](#clearContents-int-int-int-int-) | Löscht den Inhalt eines Bereichs. |
| [clearFormats(CellArea range)](#clearFormats-com.aspose.cells.CellArea-) | Löscht die Formatierung eines Bereichs. |
| [clearFormats(int startRow, int startColumn, int endRow, int endColumn)](#clearFormats-int-int-int-int-) | Löscht die Formatierung eines Bereichs. |
| [clearMergedCells()](#clearMergedCells--) | Löscht alle zusammengeführten Bereiche. |
| [clearRange(CellArea range)](#clearRange-com.aspose.cells.CellArea-) | Löscht Inhalt und Formatierung eines Bereichs. |
| [clearRange(int startRow, int startColumn, int endRow, int endColumn)](#clearRange-int-int-int-int-) | Löscht Inhalt und Formatierung eines Bereichs. |
| [convertStringToNumericValue()](#convertStringToNumericValue--) | Konvertiert alle Zeichenkettendaten im Arbeitsblatt, falls möglich, in numerische Werte. |
| [copyColumn(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex)](#copyColumn-com.aspose.cells.Cells-int-int-) | Kopiert Daten und Formate einer gesamten Spalte. |
| [copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber)](#copyColumns-com.aspose.cells.Cells-int-int-int-) | Kopiert Daten und Formate mehrerer Spalten. |
| [copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber, PasteOptions pasteOptions)](#copyColumns-com.aspose.cells.Cells-int-int-int-com.aspose.cells.PasteOptions-) | Kopiert Daten und Formate einer gesamten Spalte. |
| [copyColumns(Cells sourceCells, int sourceColumnIndex, int sourceTotalColumns, int destinationColumnIndex, int destinationTotalColumns)](#copyColumns-com.aspose.cells.Cells-int-int-int-int-) | Kopiert Daten und Formate aller Spalten. |
| [copyRow(Cells sourceCells, int sourceRowIndex, int destinationRowIndex)](#copyRow-com.aspose.cells.Cells-int-int-) | Kopiert Daten und Formate einer gesamten Zeile. |
| [copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)](#copyRows-com.aspose.cells.Cells-int-int-int-) | Kopiert Daten und Formate mehrerer ganzer Zeilen. |
| [copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions)](#copyRows-com.aspose.cells.Cells-int-int-int-com.aspose.cells.CopyOptions-) | Kopiert Daten und Formate mehrerer ganzer Zeilen. |
| [copyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions)](#copyRows-com.aspose.cells.Cells-int-int-int-com.aspose.cells.CopyOptions-com.aspose.cells.PasteOptions-) | Kopiert Daten und Formate mehrerer ganzer Zeilen. |
| [createRange(int firstIndex, int number, boolean isVertical)](#createRange-int-int-boolean-) | Erstellt ein [Range](../../com.aspose.cells/range)-Objekt aus Zeilen von Zellen oder Spalten von Zellen. |
| [createRange(int firstRow, int firstColumn, int totalRows, int totalColumns)](#createRange-int-int-int-int-) | Erstellt ein [Range](../../com.aspose.cells/range)-Objekt aus einem Zellbereich. |
| [createRange(String address)](#createRange-java.lang.String-) | Erstellt ein [Range](../../com.aspose.cells/range)-Objekt aus einer Bereichsadresse. |
| [createRange(String upperLeftCell, String lowerRightCell)](#createRange-java.lang.String-java.lang.String-) | Erstellt ein [Range](../../com.aspose.cells/range)-Objekt aus einem Zellbereich. |
| [deleteBlankColumns()](#deleteBlankColumns--) | Löscht alle leeren Spalten, die keine Daten enthalten. |
| [deleteBlankColumns(DeleteOptions options)](#deleteBlankColumns-com.aspose.cells.DeleteOptions-) | Löscht alle leeren Spalten, die keine Daten enthalten. |
| [deleteBlankRows()](#deleteBlankRows--) | Löscht alle leeren Zeilen, die keine Daten oder andere Objekte enthalten. |
| [deleteBlankRows(DeleteOptions options)](#deleteBlankRows-com.aspose.cells.DeleteOptions-) | Löscht alle leeren Zeilen, die keine Daten oder einige spezielle Objekte wie sichtbare Kommentare, Pivot‑Tabellen enthalten. |
| [deleteColumn(int columnIndex)](#deleteColumn-int-) | Löscht eine Spalte. |
| [deleteColumn(int columnIndex, boolean updateReference)](#deleteColumn-int-boolean-) | Löscht eine Spalte. |
| [deleteColumns(int columnIndex, int totalColumns, boolean updateReference)](#deleteColumns-int-int-boolean-) | Löscht mehrere Spalten. |
| [deleteColumns(int columnIndex, int totalColumns, DeleteOptions options)](#deleteColumns-int-int-com.aspose.cells.DeleteOptions-) | Löscht mehrere Spalten. |
| [deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType)](#deleteRange-int-int-int-int-int-) | Löscht einen Zellbereich und verschiebt Zellen gemäß der Verschiebeoption. |
| [deleteRow(int rowIndex)](#deleteRow-int-) | Löscht eine Zeile. |
| [deleteRow(int rowIndex, boolean updateReference)](#deleteRow-int-boolean-) | Löscht eine Zeile. |
| [deleteRows(int rowIndex, int totalRows)](#deleteRows-int-int-) | Löscht mehrere Zeilen. |
| [deleteRows(int rowIndex, int totalRows, boolean updateReference)](#deleteRows-int-int-boolean-) | Löscht mehrere Zeilen im Arbeitsblatt. |
| [deleteRows(int rowIndex, int totalRows, DeleteOptions options)](#deleteRows-int-int-com.aspose.cells.DeleteOptions-) | Löscht mehrere Zeilen im Arbeitsblatt. |
| [dispose()](#dispose--) | Führt anwendungsspezifische Aufgaben aus, die mit dem Freigeben, Freisetzen oder Zurücksetzen nicht verwalteter Ressourcen verbunden sind. |
| [endCellInColumn(int columnIndex)](#endCellInColumn-int-) | Gibt die letzte Zelle in dieser Spalte zurück. |
| [endCellInColumn(int startRow, int endRow, int startColumn, int endColumn)](#endCellInColumn-int-int-int-int-) | Gibt die letzte Zelle mit maximalem Spaltenindex in diesem Bereich zurück. |
| [endCellInRow(int rowIndex)](#endCellInRow-int-) | Gibt die letzte Zelle in dieser Zeile zurück. |
| [endCellInRow(int startRow, int endRow, int startColumn, int endColumn)](#endCellInRow-int-int-int-int-) | Gibt die letzte Zelle mit maximalem Zeilenindex in diesem Bereich zurück. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)](#exportArray-int-int-int-int-) | Exportiert Daten aus der [Cells](../../com.aspose.cells/cells)-Sammlung in ein zweidimensionales Array‑Objekt. |
| [exportTypeArray(int firstRow, int firstColumn, int totalRows, int totalColumns)](#exportTypeArray-int-int-int-int-) | Exportiert den Zellwerttyp aus der [Cells](../../com.aspose.cells/cells)-Sammlung in ein zweidimensionales Array‑Objekt. |
| [find(Object what, Cell previousCell)](#find-java.lang.Object-com.aspose.cells.Cell-) | Findet die Zelle, die das Eingabeobjekt enthält. |
| [find(Object what, Cell previousCell, FindOptions findOptions)](#find-java.lang.Object-com.aspose.cells.Cell-com.aspose.cells.FindOptions-) | Findet die Zelle, die das Eingabeobjekt enthält. |
| [get(int row, int column)](#get-int-int-) | Gibt das [Cell](../../com.aspose.cells/cell)-Element am angegebenen Zeilen‑ und Spaltenindex zurück. |
| [get(String cellName)](#get-java.lang.String-) | Gibt das [Cell](../../com.aspose.cells/cell)-Element mit dem angegebenen Zellenamen zurück. |
| [getCellDisplayStyle(int row, int column)](#getCellDisplayStyle-int-int-) | Gibt den Anzeigestil der angegebenen Zelle zurück. |
| [getCellDisplayStyle(int row, int column, int adjacentBorders)](#getCellDisplayStyle-int-int-int-) | Gibt den Anzeigestil der angegebenen Zelle zurück. |
| [getCellStyle(int row, int column)](#getCellStyle-int-int-) | Gibt den Stil der angegebenen Zelle zurück. |
| [getCellsWithPlaceInCellPicture()](#getCellsWithPlaceInCellPicture--) | Gibt alle Zellen zurück, die ein eingebettetes Bild enthalten. |
| [getClass()](#getClass--) |  |
| [getColumnOriginalWidthPoint(int column)](#getColumnOriginalWidthPoint-int-) | Ermittelt die ursprüngliche Höhe der Spalte in Punkt, wenn die Spalte ausgeblendet ist |
| [getColumnWidth(int column)](#getColumnWidth-int-) | Ermittelt die Breite(in Zeichen) der angegebenen Spalte in der Normalansicht |
| [getColumnWidth(int column, boolean isOriginal, int unitType)](#getColumnWidth-int-boolean-int-) | Ermittelt die Spaltenbreite. |
| [getColumnWidthInch(int column)](#getColumnWidthInch-int-) | Ermittelt die Breite der angegebenen Spalte in der Normalansicht, in Zoll. |
| [getColumnWidthPixel(int column)](#getColumnWidthPixel-int-) | Ermittelt die Breite der angegebenen Spalte in der Normalansicht, in Pixel. |
| [getColumnWidthPixel(int column, boolean original)](#getColumnWidthPixel-int-boolean-) | Ermittelt die Breite der angegebenen Spalte in der Normalansicht, in Pixel. |
| [getColumns()](#getColumns--) | Ermittelt die Sammlung von [Column](../../com.aspose.cells/column)-Objekten, die die einzelnen Spalten in diesem Arbeitsblatt darstellen. |
| [getCount()](#getCount--) | Ermittelt die Gesamtanzahl der instanziierten Cell-Objekte. |
| [getCountLarge()](#getCountLarge--) | Ermittelt die Gesamtanzahl der instanziierten Cell-Objekte. |
| [getDependents(boolean isAll, int row, int column)](#getDependents-boolean-int-int-) | Erhalte alle Zellen, die auf die bestimmte Zelle verweisen. |
| [getDependentsInCalculation(int row, int column, boolean recursive)](#getDependentsInCalculation-int-int-boolean-) | Ermittelt alle Zellen, deren berechnetes Ergebnis von einer bestimmten Zelle abhängt. |
| [getFirstCell()](#getFirstCell--) | Ermittelt die erste Zelle in diesem Arbeitsblatt. |
| [getFirstDataRow(int column)](#getFirstDataRow-int-) | Ermittelt den Index der ersten Zeile der Zelle, die Daten in der angegebenen Spalte enthält. |
| [getGroupedColumnOutlineLevel(int columnIndex)](#getGroupedColumnOutlineLevel-int-) | Ermittelt die Gliederungsebene (nullbasiert) der Spalte. |
| [getGroupedRowOutlineLevel(int rowIndex)](#getGroupedRowOutlineLevel-int-) | Ermittelt die Gliederungsebene (nullbasiert) der Zeile. |
| [getLastCell()](#getLastCell--) | Ermittelt die letzte Zelle in diesem Arbeitsblatt. |
| [getLastDataRow(int column)](#getLastDataRow-int-) | Ermittelt den Index der letzten Zeile der Zelle, die Daten in der angegebenen Spalte enthält. |
| [getMaxColumn()](#getMaxColumn--) | Maximaler Spaltenindex jener Zellen, die in der Sammlung instanziiert wurden (schließt die Spalte nicht ein, für die ein Stil für die gesamte Spalte definiert ist, aber in der keine Zelle instanziiert wurde). |
| [getMaxDataColumn()](#getMaxDataColumn--) | Maximaler Spaltenindex der Zelle, die Daten enthält. |
| [getMaxDataRow()](#getMaxDataRow--) | Maximaler Zeilenindex der Zelle, die Daten enthält. |
| [getMaxDisplayRange()](#getMaxDisplayRange--) | Ermittelt den maximalen Bereich, der Daten, zusammengeführte Zellen und Formen enthält. |
| [getMaxGroupedColumnOutlineLevel()](#getMaxGroupedColumnOutlineLevel--) | Ermittelt die maximale gruppierte Spalten-Gliederungsebene (nullbasiert). |
| [getMaxGroupedRowOutlineLevel()](#getMaxGroupedRowOutlineLevel--) | Ermittelt die maximale gruppierte Zeilen-Gliederungsebene (nullbasiert). |
| [getMaxRow()](#getMaxRow--) | Maximaler Zeilenindex der Zelle, die Daten oder Stil enthält. |
| [getMemorySetting()](#getMemorySetting--) | Ermittelt die Speicherverbrauchsoption für diese Zellen. |
| [getMergedAreas()](#getMergedAreas--) | Ermittelt alle zusammengeführten Zellen. |
| [getMergedCells()](#getMergedCells--) | Ermittelt die Sammlung zusammengeführter Zellen. |
| [getMinColumn()](#getMinColumn--) | Minimaler Spaltenindex der Zellen, die in der Sammlung instanziiert wurden (schließt die Spalte nicht ein, in der der Stil für die gesamte Spalte definiert ist, aber keine Zelle instanziiert wurde). |
| [getMinDataColumn()](#getMinDataColumn--) | Minimaler Spaltenindex der Zelle, die Daten enthält. |
| [getMinDataRow()](#getMinDataRow--) | Minimaler Zeilenindex der Zelle, die Daten enthält. |
| [getMinRow()](#getMinRow--) | Minimaler Zeilenindex der Zelle, die Daten oder Stil enthält. |
| [getMultiThreadReading()](#getMultiThreadReading--) | Ermittelt, ob das Zellen-Datenmodell das Multi‑Thread‑Lesen unterstützen soll. |
| [getOdsCellFields()](#getOdsCellFields--) | Ermittelt die Liste der Felder von ods. |
| [getPreserveString()](#getPreserveString--) | Ermittelt einen Wert, der angibt, ob alle Arbeitsblattwerte als Zeichenfolgen erhalten bleiben. |
| [getRanges()](#getRanges--) | Ermittelt die Sammlung von [Range](../../com.aspose.cells/range)-Objekten, die zur Laufzeit erstellt werden. |
| [getRowEnumerator()](#getRowEnumerator--) | Ermittelt den Zeilen‑Enumerator. |
| [getRowHeight(int row)](#getRowHeight-int-) | Ermittelt die Höhe einer angegebenen Zeile in der Einheit Punkte. |
| [getRowHeight(int row, boolean isOriginal, int unitType)](#getRowHeight-int-boolean-int-) | Ermittelt die Zeilenhöhe. |
| [getRowHeightInch(int row)](#getRowHeightInch-int-) | Ermittelt die Höhe einer angegebenen Zeile in der Einheit Zoll. |
| [getRowHeightPixel(int row)](#getRowHeightPixel-int-) | Ermittelt die Höhe einer angegebenen Zeile in der Einheit Pixel. |
| [getRowOriginalHeightPoint(int row)](#getRowOriginalHeightPoint-int-) | Ermittelt die ursprüngliche Zeilenhöhe in der Einheit Punkt, wenn die Zeile ausgeblendet ist. |
| [getRows()](#getRows--) | Ermittelt die Sammlung von [Row](../../com.aspose.cells/row)-Objekten, die die einzelnen Zeilen in diesem Arbeitsblatt darstellen. |
| [getStandardHeight()](#getStandardHeight--) | Ermittelt die Standardzeilenhöhe in diesem Arbeitsblatt in der Einheit Punkte. |
| [getStandardHeightInch()](#getStandardHeightInch--) | Ermittelt die Standardzeilenhöhe in diesem Arbeitsblatt in der Einheit Zoll. |
| [getStandardHeightPixels()](#getStandardHeightPixels--) | Ermittelt die Standardzeilenhöhe in diesem Arbeitsblatt in der Einheit Pixel. |
| [getStandardWidth()](#getStandardWidth--) | Ermittelt die Standardspaltenbreite im Arbeitsblatt in der Einheit Zeichen. |
| [getStandardWidthInch()](#getStandardWidthInch--) | Ermittelt die Standardspaltenbreite im Arbeitsblatt in der Einheit Zoll. |
| [getStandardWidthPixels()](#getStandardWidthPixels--) | Ermittelt die Standardspaltenbreite im Arbeitsblatt in der Einheit Pixel. |
| [getStyle()](#getStyle--) | Ermittelt den Standardstil des Arbeitsblatts. |
| [getViewColumnWidthPixel(int column)](#getViewColumnWidthPixel-int-) | Ermittelt die Breite in verschiedenen Ansichtstypen. |
| [getViewRowHeight(int row)](#getViewRowHeight-int-) | Ermittelt die Höhe einer angegebenen Zeile. |
| [getViewRowHeightInch(int row)](#getViewRowHeightInch-int-) | Ermittelt die Höhe einer angegebenen Zeile in der Einheit Zoll. |
| [groupColumns(int firstIndex, int lastIndex)](#groupColumns-int-int-) | Gruppiert Spalten. |
| [groupColumns(int firstIndex, int lastIndex, boolean isHidden)](#groupColumns-int-int-boolean-) | Gruppiert Spalten. |
| [groupRows(int firstIndex, int lastIndex)](#groupRows-int-int-) | Gruppiert Zeilen. |
| [groupRows(int firstIndex, int lastIndex, boolean isHidden)](#groupRows-int-int-boolean-) | Gruppiert Zeilen. |
| [hashCode()](#hashCode--) |  |
| [hideColumn(int column)](#hideColumn-int-) | Blendet eine Spalte aus. |
| [hideColumns(int column, int totalColumns)](#hideColumns-int-int-) | Mehrere Spalten ausblenden. |
| [hideGroupDetail(boolean isVertical, int index)](#hideGroupDetail-boolean-int-) | Klappt die gruppierten Zeilen/Spalten zusammen. |
| [hideRow(int row)](#hideRow-int-) | Blendet eine Zeile aus. |
| [hideRows(int row, int totalRows)](#hideRows-int-int-) | Mehrere Zeilen ausblenden. |
| [importArray(double[] doubleArray, int firstRow, int firstColumn, boolean isVertical)](#importArray-double---int-int-boolean-) | Importiert ein Array von Double in ein Arbeitsblatt. |
| [importArray(double[][] doubleArray, int firstRow, int firstColumn)](#importArray-double-----int-int-) | Importiert ein zweidimensionales Array von Double in ein Arbeitsblatt. |
| [importArray(int[] intArray, int firstRow, int firstColumn, boolean isVertical)](#importArray-int---int-int-boolean-) | Importiert ein Array von Integer in ein Arbeitsblatt. |
| [importArray(int[][] intArray, int firstRow, int firstColumn)](#importArray-int-----int-int-) | Importiert ein zweidimensionales Array von Integer in ein Arbeitsblatt. |
| [importArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical)](#importArray-java.lang.String---int-int-boolean-) | Importiert ein Array von String in ein Arbeitsblatt. |
| [importArray(String[][] stringArray, int firstRow, int firstColumn)](#importArray-java.lang.String-----int-int-) | Importiert ein zweidimensionales Array von String in ein Arbeitsblatt. |
| [importArrayList(ArrayList arrayList, int firstRow, int firstColumn, boolean isVertical)](#importArrayList-java.util.ArrayList-int-int-boolean-) | Importiert eine ArrayList von Daten in ein Arbeitsblatt. |
| [importCSV(InputStream stream, TxtLoadOptions options, int firstRow, int firstColumn)](#importCSV-java.io.InputStream-com.aspose.cells.TxtLoadOptions-int-int-) | Importiere eine CSV-Datei in die Zellen. |
| [importCSV(InputStream stream, String splitter, boolean convertNumericData, int firstRow, int firstColumn)](#importCSV-java.io.InputStream-java.lang.String-boolean-int-int-) | Importiere eine CSV-Datei in die Zellen. |
| [importCSV(String fileName, TxtLoadOptions options, int firstRow, int firstColumn)](#importCSV-java.lang.String-com.aspose.cells.TxtLoadOptions-int-int-) | Importiere eine CSV-Datei in die Zellen. |
| [importCSV(String fileName, String splitter, boolean convertNumericData, int firstRow, int firstColumn)](#importCSV-java.lang.String-java.lang.String-boolean-int-int-) | Importiere eine CSV-Datei in die Zellen. |
| [importCustomObjects(Collection list, int firstRow, int firstColumn, ImportTableOptions options)](#importCustomObjects-java.util.Collection-int-int-com.aspose.cells.ImportTableOptions-) | Importiert benutzerdefinierte Objekte. |
| [importCustomObjects(Collection list, String[] propertyNames, boolean isPropertyNameShown, int firstRow, int firstColumn, int rowNumber, boolean insertRows, String dateFormatString, boolean convertStringToNumber)](#importCustomObjects-java.util.Collection-java.lang.String---boolean-int-int-int-boolean-java.lang.String-boolean-) | Importiert benutzerdefinierte Objekte. |
| [importData(ICellsDataTable table, int firstRow, int firstColumn, ImportTableOptions options)](#importData-com.aspose.cells.ICellsDataTable-int-int-com.aspose.cells.ImportTableOptions-) | Importiere Daten aus einer benutzerdefinierten Datentabelle. |
| [importFormulaArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical)](#importFormulaArray-java.lang.String---int-int-boolean-) | Importiert ein Array von Formeln in ein Arbeitsblatt. |
| [importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical)](#importObjectArray-java.lang.Object---int-int-boolean-) | Importiert ein Array von Daten in ein Arbeitsblatt. |
| [importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical, int skip)](#importObjectArray-java.lang.Object---int-int-boolean-int-) | Importiert ein Array von Daten in ein Arbeitsblatt. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown)](#importResultSet-java.sql.ResultSet-int-int-boolean-) | Importiert Daten aus einem ResultSet-Objekt in das Arbeitsblatt. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber)](#importResultSet-java.sql.ResultSet-int-int-boolean-java.lang.String-boolean-) | Importiert Daten aus einem ResultSet-Objekt in das Arbeitsblatt. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, ImportTableOptions options)](#importResultSet-java.sql.ResultSet-int-int-com.aspose.cells.ImportTableOptions-) | Importiert Daten aus einem ResultSet-Objekt in das Arbeitsblatt. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown)](#importResultSet-java.sql.ResultSet-int-int-int-int-boolean-) | Importiert Daten aus einem ResultSet-Objekt in das Arbeitsblatt. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber)](#importResultSet-java.sql.ResultSet-int-int-int-int-boolean-java.lang.String-boolean-) | Importiert Daten aus einem ResultSet-Objekt in das Arbeitsblatt. |
| [importResultSet(ResultSet rs, String startCell, boolean isFieldNameShown)](#importResultSet-java.sql.ResultSet-java.lang.String-boolean-) | Importiert Daten aus einem ResultSet-Objekt in das Arbeitsblatt. |
| [importResultSet(ResultSet rs, String startCell, ImportTableOptions options)](#importResultSet-java.sql.ResultSet-java.lang.String-com.aspose.cells.ImportTableOptions-) | Importiert Daten aus einem ResultSet-Objekt in das Arbeitsblatt. |
| [importResultSet(ResultSet rs, String startCell, int rowNum, int columnNum, boolean isFieldNameShown)](#importResultSet-java.sql.ResultSet-java.lang.String-int-int-boolean-) | Importiert Daten aus einem ResultSet-Objekt in das Arbeitsblatt. |
| [importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn)](#importTwoDimensionArray-java.lang.Object-----int-int-) | Importiert ein zweidimensionales Array von Daten in ein Arbeitsblatt. |
| [importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn, boolean convertStringToNumber)](#importTwoDimensionArray-java.lang.Object-----int-int-boolean-) | Importiert ein zweidimensionales Array von Daten in ein Arbeitsblatt. |
| [importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, boolean convertStringToNumber)](#importTwoDimensionArray-java.lang.Object-----java.lang.Object-----int-int-boolean-) | Importiert ein zweidimensionales Array von Daten in ein Arbeitsblatt. |
| [importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, TxtLoadOptions opts)](#importTwoDimensionArray-java.lang.Object-----java.lang.Object-----int-int-com.aspose.cells.TxtLoadOptions-) | Importiert ein zweidimensionales Array von Daten in ein Arbeitsblatt. |
| [insertColumn(int columnIndex)](#insertColumn-int-) | Fügt eine neue Spalte in das Arbeitsblatt ein. |
| [insertColumn(int columnIndex, boolean updateReference)](#insertColumn-int-boolean-) | Fügt eine neue Spalte in das Arbeitsblatt ein. |
| [insertColumns(int columnIndex, int totalColumns)](#insertColumns-int-int-) | Fügt mehrere Spalten in das Arbeitsblatt ein. |
| [insertColumns(int columnIndex, int totalColumns, boolean updateReference)](#insertColumns-int-int-boolean-) | Fügt mehrere Spalten in das Arbeitsblatt ein. |
| [insertColumns(int columnIndex, int totalColumns, InsertOptions options)](#insertColumns-int-int-com.aspose.cells.InsertOptions-) | Fügt mehrere Spalten in das Arbeitsblatt ein. |
| [insertCutCells(Range cutRange, int row, int column, int shiftType)](#insertCutCells-com.aspose.cells.Range-int-int-int-) | Einfügen des ausgeschnittenen Bereichs. |
| [insertRange(CellArea area, int shiftType)](#insertRange-com.aspose.cells.CellArea-int-) | Fügt einen Zellbereich ein und verschiebt Zellen gemäß der Verschiebungsoption. |
| [insertRange(CellArea area, int shiftNumber, int shiftType)](#insertRange-com.aspose.cells.CellArea-int-int-) | Fügt einen Zellbereich ein und verschiebt Zellen gemäß der Verschiebungsoption. |
| [insertRange(CellArea area, int shiftNumber, int shiftType, boolean updateReference)](#insertRange-com.aspose.cells.CellArea-int-int-boolean-) | Fügt einen Zellbereich ein und verschiebt Zellen gemäß der Verschiebungsoption. |
| [insertRow(int rowIndex)](#insertRow-int-) | Fügt eine neue Zeile in das Arbeitsblatt ein. |
| [insertRows(int rowIndex, int totalRows)](#insertRows-int-int-) | Fügt mehrere Zeilen in das Arbeitsblatt ein. |
| [insertRows(int rowIndex, int totalRows, boolean updateReference)](#insertRows-int-int-boolean-) | Fügt mehrere Zeilen in das Arbeitsblatt ein. |
| [insertRows(int rowIndex, int totalRows, InsertOptions options)](#insertRows-int-int-com.aspose.cells.InsertOptions-) | Fügt mehrere Zeilen in das Arbeitsblatt ein. |
| [isBlankColumn(int columnIndex)](#isBlankColumn-int-) | Überprüft, ob die angegebene Spalte leer ist (enthält keine Daten). |
| [isColumnHidden(int columnIndex)](#isColumnHidden-int-) | Überprüft, ob eine Spalte am angegebenen Index ausgeblendet ist. |
| [isDefaultColumnHidden()](#isDefaultColumnHidden--) |  |
| [isDefaultRowHeightMatched()](#isDefaultRowHeightMatched--) | Zeigt an, dass Zeilenhöhe und Standard‑Schriftgröße übereinstimmen. |
| [isDefaultRowHidden()](#isDefaultRowHidden--) | Zeigt an, ob die Zeile standardmäßig ausgeblendet ist. |
| [isDeletingRangeEnabled(int startRow, int startColumn, int totalRows, int totalColumns)](#isDeletingRangeEnabled-int-int-int-int-) | Überprüft, ob der Bereich gelöscht werden kann. |
| [isRowHidden(int rowIndex)](#isRowHidden-int-) | Überprüft, ob eine Zeile am angegebenen Index ausgeblendet ist. |
| [iterator()](#iterator--) | Gibt den Zellen‑Enumerator zurück. |
| [linkToXmlMap(String mapName, int row, int column, String path)](#linkToXmlMap-java.lang.String-int-int-java.lang.String-) | Link zu einer XML‑Zuordnung. |
| [merge(int firstRow, int firstColumn, int totalRows, int totalColumns)](#merge-int-int-int-int-) | Führt einen angegebenen Zellbereich zu einer einzelnen Zelle zusammen. |
| [merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean mergeConflict)](#merge-int-int-int-int-boolean-) | Führt einen angegebenen Zellbereich zu einer einzelnen Zelle zusammen. |
| [merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean checkConflict, boolean mergeConflict)](#merge-int-int-int-int-boolean-boolean-) | Führt einen angegebenen Zellbereich zu einer einzelnen Zelle zusammen. |
| [moveRange(CellArea sourceArea, int destRow, int destColumn)](#moveRange-com.aspose.cells.CellArea-int-int-) | Verschiebt den Bereich. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeDuplicates()](#removeDuplicates--) | Entfernt doppelte Zeilen im Blatt. |
| [removeDuplicates(int startRow, int startColumn, int endRow, int endColumn)](#removeDuplicates-int-int-int-int-) | Entfernt doppelte Werte im Bereich. |
| [removeDuplicates(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders, int[] columnOffsets)](#removeDuplicates-int-int-int-int-boolean-int---) | Entfernt doppelte Daten des Bereichs. |
| [removeFormulas()](#removeFormulas--) | Entfernt alle Formeln und ersetzt sie durch den Ergebniswert. |
| [retrieveSubtotalSetting(CellArea ca)](#retrieveSubtotalSetting-com.aspose.cells.CellArea-) | Ruft die Zwischensummen‑Einstellung des Bereichs ab. |
| [setColumnWidth(int column, double width)](#setColumnWidth-int-double-) | Setzt die Breite der angegebenen Spalte in der Normalansicht. |
| [setColumnWidthInch(int column, double inches)](#setColumnWidthInch-int-double-) | Setzt die Spaltenbreite in Zoll in der Normalansicht. |
| [setColumnWidthPixel(int column, int pixels)](#setColumnWidthPixel-int-int-) | Setzt die Spaltenbreite in Pixeln in der Normalansicht. |
| [setDefaultColumnHidden(boolean value)](#setDefaultColumnHidden-boolean-) |  |
| [setDefaultRowHeightMatched(boolean value)](#setDefaultRowHeightMatched-boolean-) | Zeigt an, dass Zeilenhöhe und Standard‑Schriftgröße übereinstimmen. |
| [setDefaultRowHidden(boolean value)](#setDefaultRowHidden-boolean-) | Zeigt an, ob die Zeile standardmäßig ausgeblendet ist. |
| [setMemorySetting(int value)](#setMemorySetting-int-) | Setzt die Speicherverbrauchs‑Option für diese Zellen. |
| [setMultiThreadReading(boolean value)](#setMultiThreadReading-boolean-) | Legt fest, ob das Zellen‑Datenmodell das Lesen mit mehreren Threads unterstützen soll. |
| [setPreserveString(boolean value)](#setPreserveString-boolean-) | Setzt einen Wert, der angibt, ob alle Arbeitsblattwerte als Zeichenfolgen erhalten bleiben. |
| [setRowHeight(int row, double height)](#setRowHeight-int-double-) | Setzt die Höhe der angegebenen Zeile. |
| [setRowHeightInch(int row, double inches)](#setRowHeightInch-int-double-) | Setzt die Zeilenhöhe in Zoll. |
| [setRowHeightPixel(int row, int pixels)](#setRowHeightPixel-int-int-) | Setzt die Zeilenhöhe in Pixeln. |
| [setStandardHeight(double value)](#setStandardHeight-double-) | Legt die Standardzeilenhöhe in diesem Arbeitsblatt fest, in der Einheit Punkte. |
| [setStandardHeightInch(double value)](#setStandardHeightInch-double-) | Legt die Standardzeilenhöhe in diesem Arbeitsblatt fest, in der Einheit Zoll. |
| [setStandardHeightPixels(int value)](#setStandardHeightPixels-int-) | Legt die Standardzeilenhöhe in diesem Arbeitsblatt fest, in der Einheit Pixel. |
| [setStandardWidth(double value)](#setStandardWidth-double-) | Legt die Standardspaltenbreite im Arbeitsblatt fest, in der Einheit Zeichen. |
| [setStandardWidthInch(double value)](#setStandardWidthInch-double-) | Legt die Standardspaltenbreite im Arbeitsblatt fest, in der Einheit Zoll. |
| [setStandardWidthPixels(int value)](#setStandardWidthPixels-int-) | Legt die Standardspaltenbreite im Arbeitsblatt fest, in der Einheit Pixel. |
| [setStyle(Style value)](#setStyle-com.aspose.cells.Style-) | Legt den Standardstil des Arbeitsblatts fest. |
| [setViewColumnWidthPixel(int column, int pixels)](#setViewColumnWidthPixel-int-int-) | Legt die Spaltenbreite in verschiedenen Ansichten fest. |
| [showGroupDetail(boolean isVertical, int index)](#showGroupDetail-boolean-int-) | Erweitert die gruppierten Zeilen/Spalten. |
| [subtotal(CellArea ca, int groupBy, int function, int[] totalList)](#subtotal-com.aspose.cells.CellArea-int-int-int---) | Erstellt Zwischensummen für den Bereich. |
| [subtotal(CellArea ca, int groupBy, int function, int[] totalList, boolean replace, boolean pageBreaks, boolean summaryBelowData)](#subtotal-com.aspose.cells.CellArea-int-int-int---boolean-boolean-boolean-) | Erstellt Zwischensummen für den Bereich. |
| [textToColumns(int row, int column, int totalRows, TxtLoadOptions options)](#textToColumns-int-int-int-com.aspose.cells.TxtLoadOptions-) | Teilt den Inhalt in der angegebenen Spalte in mehrere Spalten auf.. |
| [toString()](#toString--) |  |
| [unMerge(int firstRow, int firstColumn, int totalRows, int totalColumns)](#unMerge-int-int-int-int-) | Löst einen angegebenen Bereich zusammengeführter Zellen. |
| [ungroupColumns(int firstIndex, int lastIndex)](#ungroupColumns-int-int-) | Hebt die Gruppierung von Spalten auf. |
| [ungroupRows(int firstIndex, int lastIndex)](#ungroupRows-int-int-) | Hebt die Gruppierung von Zeilen auf. |
| [ungroupRows(int firstIndex, int lastIndex, boolean isAll)](#ungroupRows-int-int-boolean-) | Hebt die Gruppierung von Zeilen auf. |
| [unhideColumn(int column, double width)](#unhideColumn-int-double-) | Blendet eine Spalte ein |
| [unhideColumns(int column, int totalColumns, double width)](#unhideColumns-int-int-double-) | Blendet mehrere Spalten ein. |
| [unhideRow(int row, double height)](#unhideRow-int-double-) | Blendet eine Zeile ein. |
| [unhideRows(int row, int totalRows, double height)](#unhideRows-int-int-double-) | Blendet die ausgeblendeten Zeilen ein. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addRange(Range rangeObject) {#addRange-com.aspose.cells.Range-}
```
public void addRange(Range rangeObject)
```


Fügt einen Bereichsobjektverweis zu Zellen hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rangeObject | [Range](../../com.aspose.cells/range) | Das Bereichsobjekt wird in den Zellen enthalten sein |

### applyColumnStyle(int column, Style style, StyleFlag flag) {#applyColumnStyle-int-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyColumnStyle(int column, Style style, StyleFlag flag)
```


Wendet Formate für eine gesamte Spalte an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Spalte | int | Der Spaltenindex. |
| style | [Style](../../com.aspose.cells/style) | Das Stilobjekt, das angewendet wird. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Flags, die angewandte Formatierungseigenschaften anzeigen. |

### applyRowStyle(int row, Style style, StyleFlag flag) {#applyRowStyle-int-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyRowStyle(int row, Style style, StyleFlag flag)
```


Wendet Formate für eine gesamte Zeile an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Der Zeilenindex. |
| style | [Style](../../com.aspose.cells/style) | Das Stilobjekt, das angewendet wird. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Flags, die angewandte Formatierungseigenschaften anzeigen. |

### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


Wendet Formate für ein gesamtes Arbeitsblatt an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Das Stilobjekt, das angewendet wird. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Flags, die angewandte Formatierungseigenschaften anzeigen. |

### checkCell(int row, int column) {#checkCell-int-int-}
```
public Cell checkCell(int row, int column)
```


Liefert das [Cell](../../com.aspose.cells/cell)‑Element oder null am angegebenen Zeilen‑ und Spaltenindex der Zelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex |
| Spalte | int | Spaltenindex |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Return Cell object if a Cell object exists. Return null if the cell does not exist.
### checkColumn(int columnIndex) {#checkColumn-int-}
```
public Column checkColumn(int columnIndex)
```


Liefert das [Column](../../com.aspose.cells/column)‑Element oder null am angegebenen Spaltenindex.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnIndex | int | Der Spaltenindex. |

**Returns:**
[Column](../../com.aspose.cells/column) - The Column object.
### checkRow(int row) {#checkRow-int-}
```
public Row checkRow(int row)
```


Liefert das [Row](../../com.aspose.cells/row)‑Element oder null am angegebenen Zeilenindex der Zelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex |

**Returns:**
[Row](../../com.aspose.cells/row) - Returns [Row](../../com.aspose.cells/row) object If the row object does exist, otherwise returns null.
### clear() {#clear--}
```
public void clear()
```


Löscht alle Daten des Arbeitsblatts.

### clearContents(CellArea range) {#clearContents-com.aspose.cells.CellArea-}
```
public void clearContents(CellArea range)
```


Löscht den Inhalt eines Bereichs.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| range | [CellArea](../../com.aspose.cells/cellarea) | Zu löschender Bereich. |

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

### clearFormats(CellArea range) {#clearFormats-com.aspose.cells.CellArea-}
```
public void clearFormats(CellArea range)
```


Löscht die Formatierung eines Bereichs.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| range | [CellArea](../../com.aspose.cells/cellarea) | Zu löschender Bereich. |

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

### clearMergedCells() {#clearMergedCells--}
```
public void clearMergedCells()
```


Löscht alle zusammengeführten Bereiche.

### clearRange(CellArea range) {#clearRange-com.aspose.cells.CellArea-}
```
public void clearRange(CellArea range)
```


Löscht Inhalt und Formatierung eines Bereichs.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| range | [CellArea](../../com.aspose.cells/cellarea) | Zu löschender Bereich. |

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

### convertStringToNumericValue() {#convertStringToNumericValue--}
```
public void convertStringToNumericValue()
```


Konvertiert alle Zeichenkettendaten im Arbeitsblatt, falls möglich, in numerische Werte.

### copyColumn(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex) {#copyColumn-com.aspose.cells.Cells-int-int-}
```
public void copyColumn(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex)
```


Kopiert Daten und Formate einer gesamten Spalte.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | Das Quellzellen-Objekt enthält Daten und Formate zum Kopieren. |
| sourceColumnIndex | int | Quellspaltenindex. |
| destinationColumnIndex | int | Zielspaltenindex. |

### copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber) {#copyColumns-com.aspose.cells.Cells-int-int-int-}
```
public void copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber)
```


Kopiert Daten und Formate mehrerer Spalten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | Das Quellzellen-Objekt enthält Daten und Formate zum Kopieren. |
| sourceColumnIndex | int | Quellspaltenindex. |
| destinationColumnIndex | int | Zielspaltenindex. |
| columnNumber | int | Die kopierte Spaltennummer. |

### copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber, PasteOptions pasteOptions) {#copyColumns-com.aspose.cells.Cells-int-int-int-com.aspose.cells.PasteOptions-}
```
public void copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber, PasteOptions pasteOptions)
```


Kopiert Daten und Formate einer gesamten Spalte.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | Das Quellzellen-Objekt enthält Daten und Formate zum Kopieren. |
| sourceColumnIndex | int | Quellspaltenindex. |
| destinationColumnIndex | int | Zielspaltenindex. |
| columnNumber | int | Die kopierte Spaltennummer. |
| pasteOptions | [PasteOptions](../../com.aspose.cells/pasteoptions) | die Optionen für das Einfügen. |

### copyColumns(Cells sourceCells, int sourceColumnIndex, int sourceTotalColumns, int destinationColumnIndex, int destinationTotalColumns) {#copyColumns-com.aspose.cells.Cells-int-int-int-int-}
```
public void copyColumns(Cells sourceCells, int sourceColumnIndex, int sourceTotalColumns, int destinationColumnIndex, int destinationTotalColumns)
```


Kopiert Daten und Formate aller Spalten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | Das Quellzellen-Objekt enthält Daten und Formate zum Kopieren. |
| sourceColumnIndex | int | Quellspaltenindex. |
| sourceTotalColumns | int | Die Anzahl der Quellspalten. |
| destinationColumnIndex | int | Zielspaltenindex. |
| destinationTotalColumns | int | Die Anzahl der Zielspalten. |

### copyRow(Cells sourceCells, int sourceRowIndex, int destinationRowIndex) {#copyRow-com.aspose.cells.Cells-int-int-}
```
public void copyRow(Cells sourceCells, int sourceRowIndex, int destinationRowIndex)
```


Kopiert Daten und Formate einer gesamten Zeile.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | Das Quellzellen-Objekt enthält Daten und Formate zum Kopieren. |
| sourceRowIndex | int | Quellzeilenindex. |
| destinationRowIndex | int | Zielzeilenindex. |

### copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber) {#copyRows-com.aspose.cells.Cells-int-int-int-}
```
public void copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)
```


Kopiert Daten und Formate mehrerer ganzer Zeilen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | Das Quellzellen-Objekt enthält Daten und Formate zum Kopieren. |
| sourceRowIndex | int | Quellzeilenindex. |
| destinationRowIndex | int | Zielzeilenindex. |
| rowNumber | int | Die kopierte Zeilennummer. |

### copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions) {#copyRows-com.aspose.cells.Cells-int-int-int-com.aspose.cells.CopyOptions-}
```
public void copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions)
```


Kopiert Daten und Formate mehrerer ganzer Zeilen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | Das Quellzellen-Objekt enthält Daten und Formate zum Kopieren. |
| sourceRowIndex | int | Quellzeilenindex. |
| destinationRowIndex | int | Zielzeilenindex. |
| rowNumber | int | Die kopierte Zeilennummer. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | Die Kopieroptionen. |

### copyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions) {#copyRows-com.aspose.cells.Cells-int-int-int-com.aspose.cells.CopyOptions-com.aspose.cells.PasteOptions-}
```
public void copyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions)
```


Kopiert Daten und Formate mehrerer ganzer Zeilen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceCells0 | [Cells](../../com.aspose.cells/cells) | Das Quellzellen-Objekt enthält Daten und Formate zum Kopieren. |
| sourceRowIndex | int | Quellzeilenindex. |
| destinationRowIndex | int | Zielzeilenindex. |
| rowNumber | int | Die kopierte Zeilennummer. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | Die Kopieroptionen. |
| pasteOptions | [PasteOptions](../../com.aspose.cells/pasteoptions) | die Optionen für das Einfügen. |

### createRange(int firstIndex, int number, boolean isVertical) {#createRange-int-int-boolean-}
```
public Range createRange(int firstIndex, int number, boolean isVertical)
```


Erstellt ein [Range](../../com.aspose.cells/range)-Objekt aus Zeilen von Zellen oder Spalten von Zellen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstIndex | int | Erster Zeilenindex oder erster Spaltenindex, nullbasiert. |
| Nummer | int | Gesamtzahl der Zeilen oder Spalten, einsbasiert. |
| isVertical | boolean | Wahr - Bereich aus Spalten von Zellen erstellt. Falsch - Bereich aus Zeilen von Zellen erstellt. |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object.
### createRange(int firstRow, int firstColumn, int totalRows, int totalColumns) {#createRange-int-int-int-int-}
```
public Range createRange(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


Erstellt ein [Range](../../com.aspose.cells/range)-Objekt aus einem Zellbereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstRow | int | Erste Zeile dieses Bereichs |
| firstColumn | int | Erste Spalte dieses Bereichs |
| totalRows | int | Anzahl der Zeilen |
| totalColumns | int | Anzahl der Spalten |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object
### createRange(String address) {#createRange-java.lang.String-}
```
public Range createRange(String address)
```


Erstellt ein [Range](../../com.aspose.cells/range)-Objekt aus einer Bereichsadresse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Adresse | java.lang.String | Die Adresse des Bereichs. |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object
### createRange(String upperLeftCell, String lowerRightCell) {#createRange-java.lang.String-java.lang.String-}
```
public Range createRange(String upperLeftCell, String lowerRightCell)
```


Erstellt ein [Range](../../com.aspose.cells/range)-Objekt aus einem Zellbereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| upperLeftCell | java.lang.String | Name der oberen linken Zelle. |
| lowerRightCell | java.lang.String | Name der unteren rechten Zelle. |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object
### deleteBlankColumns() {#deleteBlankColumns--}
```
public void deleteBlankColumns()
```


Löscht alle leeren Spalten, die keine Daten enthalten.

### deleteBlankColumns(DeleteOptions options) {#deleteBlankColumns-com.aspose.cells.DeleteOptions-}
```
public void deleteBlankColumns(DeleteOptions options)
```


Löscht alle leeren Spalten, die keine Daten enthalten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| options | [DeleteOptions](../../com.aspose.cells/deleteoptions) | Die Optionen zum Löschen des Bereichs. |

### deleteBlankRows() {#deleteBlankRows--}
```
public void deleteBlankRows()
```


Löscht alle leeren Zeilen, die keine Daten oder andere Objekte enthalten.

### deleteBlankRows(DeleteOptions options) {#deleteBlankRows-com.aspose.cells.DeleteOptions-}
```
public void deleteBlankRows(DeleteOptions options)
```


Löscht alle leeren Zeilen, die keine Daten oder einige spezielle Objekte wie sichtbare Kommentare, Pivot‑Tabellen enthalten.

**Remarks**

Für leere Zeilen, die gelöscht werden sollen, ist es nicht nur erforderlich, dass [Row.isBlank()](../../com.aspose.cells/row\#isBlank--) wahr ist, sondern es darf auch kein sichtbarer Kommentar für irgendeine Zelle in diesen Zeilen definiert sein und keine Pivot-Tabelle, deren Bereich sich mit ihnen überschneidet.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| options | [DeleteOptions](../../com.aspose.cells/deleteoptions) | Die Optionen zum Löschen des Bereichs. |

### deleteColumn(int columnIndex) {#deleteColumn-int-}
```
public void deleteColumn(int columnIndex)
```


Löscht eine Spalte.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnIndex | int | Index der zu löschenden Spalte. |

### deleteColumn(int columnIndex, boolean updateReference) {#deleteColumn-int-boolean-}
```
public void deleteColumn(int columnIndex, boolean updateReference)
```


Löscht eine Spalte.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnIndex | int | Index der zu löschenden Spalte. |
| updateReference | boolean | Gibt an, ob Referenzen in anderen Arbeitsblättern aktualisiert werden. |

### deleteColumns(int columnIndex, int totalColumns, boolean updateReference) {#deleteColumns-int-int-boolean-}
```
public void deleteColumns(int columnIndex, int totalColumns, boolean updateReference)
```


Löscht mehrere Spalten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnIndex | int | Index der ersten zu löschenden Spalte. |
| totalColumns | int | Anzahl der zu löschenden Spalten. |
| updateReference | boolean | Gibt an, ob Referenzen in anderen Arbeitsblättern aktualisiert werden. |

### deleteColumns(int columnIndex, int totalColumns, DeleteOptions options) {#deleteColumns-int-int-com.aspose.cells.DeleteOptions-}
```
public void deleteColumns(int columnIndex, int totalColumns, DeleteOptions options)
```


Löscht mehrere Spalten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnIndex | int | Index der ersten zu löschenden Spalte. |
| totalColumns | int | Anzahl der zu löschenden Spalten. |
| options | [DeleteOptions](../../com.aspose.cells/deleteoptions) | Optionen für den Löschvorgang |

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
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). Option zum Verschieben von Zellen. |

### deleteRow(int rowIndex) {#deleteRow-int-}
```
public void deleteRow(int rowIndex)
```


Löscht eine Zeile.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowIndex | int | Index der zu löschenden Zeile. |

### deleteRow(int rowIndex, boolean updateReference) {#deleteRow-int-boolean-}
```
public void deleteRow(int rowIndex, boolean updateReference)
```


Löscht eine Zeile.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowIndex | int | Index der zu löschenden Zeile. |
| updateReference | boolean | Gibt an, ob Referenzen in anderen Arbeitsblättern aktualisiert werden. |

### deleteRows(int rowIndex, int totalRows) {#deleteRows-int-int-}
```
public boolean deleteRows(int rowIndex, int totalRows)
```


Löscht mehrere Zeilen.

**Remarks**

Wenn der gelöschte Bereich den oberen Teil (nicht das Ganze) der Tabelle (ListObject) enthält, kann der Bereich nicht gelöscht werden und es wird nichts unternommen. Es funktioniert auf die gleiche Weise wie in MS Excel.

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
| rowIndex | int | Index der ersten zu löschenden Zeile. |
| totalRows | int | Anzahl der zu löschenden Zeilen. |
| updateReference | boolean | Gibt an, ob Referenzen in anderen Arbeitsblättern aktualisiert werden. |

**Returns:**
boolean -
### deleteRows(int rowIndex, int totalRows, DeleteOptions options) {#deleteRows-int-int-com.aspose.cells.DeleteOptions-}
```
public boolean deleteRows(int rowIndex, int totalRows, DeleteOptions options)
```


Löscht mehrere Zeilen im Arbeitsblatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowIndex | int | Index der ersten zu löschenden Zeile. |
| totalRows | int | Anzahl der zu löschenden Zeilen. |
| options | [DeleteOptions](../../com.aspose.cells/deleteoptions) | Optionen für den Löschvorgang |

**Returns:**
boolean -
### dispose() {#dispose--}
```
public void dispose()
```


Führt anwendungsspezifische Aufgaben aus, die mit dem Freigeben, Freisetzen oder Zurücksetzen nicht verwalteter Ressourcen verbunden sind.

### endCellInColumn(int columnIndex) {#endCellInColumn-int-}
```
public Cell endCellInColumn(int columnIndex)
```


Gibt die letzte Zelle in dieser Spalte zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnIndex | int | Spaltenindex. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### endCellInColumn(int startRow, int endRow, int startColumn, int endColumn) {#endCellInColumn-int-int-int-int-}
```
public Cell endCellInColumn(int startRow, int endRow, int startColumn, int endColumn)
```


Gibt die letzte Zelle mit maximalem Spaltenindex in diesem Bereich zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | int | Startzeilenindex. |
| endRow | int | Endzeilenindex. |
| startColumn | int | Startspaltenindex. |
| endColumn | int | Endspaltenindex. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### endCellInRow(int rowIndex) {#endCellInRow-int-}
```
public Cell endCellInRow(int rowIndex)
```


Gibt die letzte Zelle in dieser Zeile zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowIndex | int | Zeilenindex. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### endCellInRow(int startRow, int endRow, int startColumn, int endColumn) {#endCellInRow-int-int-int-int-}
```
public Cell endCellInRow(int startRow, int endRow, int startColumn, int endColumn)
```


Gibt die letzte Zelle mit maximalem Zeilenindex in diesem Bereich zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | int | Startzeilenindex. |
| endRow | int | Endzeilenindex. |
| startColumn | int | Startspaltenindex. |
| endColumn | int | Endspaltenindex. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
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


Exportiert Daten aus der [Cells](../../com.aspose.cells/cells)-Sammlung in ein zweidimensionales Array‑Objekt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstRow | int | Die Zeilennummer der ersten zu exportierenden Zelle. |
| firstColumn | int | Die Spaltennummer der ersten zu exportierenden Zelle. |
| totalRows | int | Anzahl der zu exportierenden Zeilen |
| totalColumns | int | Anzahl der zu exportierenden Spalten |

**Returns:**
java.lang.Object[][] - Exportiertes Zellwert-Array-Objekt.
### exportTypeArray(int firstRow, int firstColumn, int totalRows, int totalColumns) {#exportTypeArray-int-int-int-int-}
```
public int[][] exportTypeArray(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


Exportiert den Zellwerttyp aus der [Cells](../../com.aspose.cells/cells)-Sammlung in ein zweidimensionales Array‑Objekt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstRow | int | Die Zeilennummer der ersten zu exportierenden Zelle. |
| firstColumn | int | Die Spaltennummer der ersten zu exportierenden Zelle. |
| totalRows | int | Anzahl der zu exportierenden Zeilen. |
| totalColumns | int | Anzahl der zu exportierenden Spalten. |

**Returns:**
int[][] - [CellValueType](../../com.aspose.cells/cellvaluetype). Exportiertes Array-Objekt, das Zellwerttypen darstellt.
### find(Object what, Cell previousCell) {#find-java.lang.Object-com.aspose.cells.Cell-}
```
public Cell find(Object what, Cell previousCell)
```


Findet die Zelle, die das Eingabeobjekt enthält.

**Remarks**

Gibt null (Nichts) zurück, wenn keine Zelle gefunden wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| was | java.lang.Object | Das zu suchende Objekt. Der Typ sollte int,double,DateTime,string,bool sein. |
| previousCell | [Cell](../../com.aspose.cells/cell) | Vorherige Zelle mit demselben Objekt. Dieser Parameter kann auf null gesetzt werden, wenn von Anfang an gesucht wird. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### find(Object what, Cell previousCell, FindOptions findOptions) {#find-java.lang.Object-com.aspose.cells.Cell-com.aspose.cells.FindOptions-}
```
public Cell find(Object what, Cell previousCell, FindOptions findOptions)
```


Findet die Zelle, die das Eingabeobjekt enthält.

**Remarks**

Gibt null (Nichts) zurück, wenn keine Zelle gefunden wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| was | java.lang.Object | Das zu suchende Objekt. Der Typ sollte int,double,DateTime,string,bool sein. |
| previousCell | [Cell](../../com.aspose.cells/cell) | Vorherige Zelle mit demselben Objekt. Dieser Parameter kann auf null gesetzt werden, wenn von Anfang an gesucht wird. |
| findOptions | [FindOptions](../../com.aspose.cells/findoptions) | Suchoptionen |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### get(int row, int column) {#get-int-int-}
```
public Cell get(int row, int column)
```


Gibt das [Cell](../../com.aspose.cells/cell)-Element am angegebenen Zeilen‑ und Spaltenindex zurück.

**Example**

```
         Workbook excel = new Workbook();
         Cells cells = excel.getWorksheets().get(0).getCells();
         Cell cell = cells.get(0, 0);	//Gets the cell at "A1"
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex. |
| Spalte | int | Spaltenindex. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - The [Cell](../../com.aspose.cells/cell) object.
### get(String cellName) {#get-java.lang.String-}
```
public Cell get(String cellName)
```


Gibt das [Cell](../../com.aspose.cells/cell)-Element mit dem angegebenen Zellenamen zurück.

**Example**

```
         Workbook excel = new Workbook();
         Cells cells = excel.getWorksheets().get(0).getCells();
         Cell cell = cells.get("A1");	//Gets the cell at "A1"
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellName | java.lang.String | Zellname, einschließlich des Spaltenbuchstabens und der Zeilennummer, zum Beispiel A5. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - A [Cell](../../com.aspose.cells/cell) object
### getCellDisplayStyle(int row, int column) {#getCellDisplayStyle-int-int-}
```
public Style getCellDisplayStyle(int row, int column)
```


Gibt den Anzeigestil der angegebenen Zelle zurück.

**Remarks**

Entspricht [Cell.getDisplayStyle()](../../com.aspose.cells/cell\#getDisplayStyle--), und ebenso bei Verwendung von [BorderType.SIDE\_BORDERS](../../com.aspose.cells/bordertype\#SIDE-BORDERS) für [getCellDisplayStyle(int,int,int)](../../com.aspose.cells/cells\#getCellDisplayStyle-int-int-int-).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex der angegebenen Zelle |
| Spalte | int | Spalte der angegebenen Zelle |

**Returns:**
[Style](../../com.aspose.cells/style) - the display style of given cell.
### getCellDisplayStyle(int row, int column, int adjacentBorders) {#getCellDisplayStyle-int-int-int-}
```
public Style getCellDisplayStyle(int row, int column, int adjacentBorders)
```


Gibt den Anzeigestil der angegebenen Zelle zurück.

**Remarks**

Wenn die Zelle auch von anderen Einstellungen wie bedingter Formatierung, Listobjekten usw. betroffen ist, kann der Anzeigestil von [getCellStyle(int,int)](../../com.aspose.cells/cells\#getCellStyle-int-int-) abweichen. Da diese Einstellungen auch auf leere (nicht vorhandene) Zellen angewendet werden können, vermeidet die Verwendung dieser Methode die Instanziierung dieser leeren Zellen, sodass die Leistung besser ist, als die Cell‑Instanz aus Cells zu holen und anschließend [Cell.getDisplayStyle(int)](../../com.aspose.cells/cell\#getDisplayStyle-int-) aufzurufen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex der angegebenen Zelle |
| Spalte | int | Spalte der angegebenen Zelle |
| adjacentBorders | int | [BorderType](../../com.aspose.cells/bordertype). Gibt an, welche Rahmen überprüft und an die Rahmen benachbarter Zellen angepasst werden müssen. Bitte siehe die Beschreibung desselben Parameters von [Cell.getDisplayStyle(int)](../../com.aspose.cells/cell\#getDisplayStyle-int-). |

**Returns:**
[Style](../../com.aspose.cells/style) - the display style of given cell.
### getCellStyle(int row, int column) {#getCellStyle-int-int-}
```
public Style getCellStyle(int row, int column)
```


Gibt den Stil der angegebenen Zelle zurück.

**Remarks**

Der zurückgegebene Stil ist nur der für die Zelle festgelegte oder von Zeile/Spalte der Zelle vererbte Stil und enthält nicht die durch andere Einstellungen wie bedingte Formatierungen angewendeten Eigenschaften.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex |
| Spalte | int | Spalte |

**Returns:**
[Style](../../com.aspose.cells/style) - the style of given cell.
### getCellsWithPlaceInCellPicture() {#getCellsWithPlaceInCellPicture--}
```
public Iterator getCellsWithPlaceInCellPicture()
```


Gibt alle Zellen zurück, die ein eingebettetes Bild enthalten.

**Remarks**

Wenn in diesem Arbeitsblatt kein Bild mit der Einstellung "Place in Cell" vorhanden ist, wird null zurückgegeben.

**Returns:**
java.util.Iterator – Aufzählung, um alle Cell‑Objekte zu enumerieren, die ein eingebettetes Bild enthalten
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnOriginalWidthPoint(int column) {#getColumnOriginalWidthPoint-int-}
```
public double getColumnOriginalWidthPoint(int column)
```


Ermittelt die ursprüngliche Höhe der Spalte in Punkt, wenn die Spalte ausgeblendet ist

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Bitte verwenden Sie stattdessen die Methode Cells.GetColumnWidth(int, bool, CellsUnitType). Diese Methode wird 12 Monate nach April 2024 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Spalte | int | Der Zeilenindex. |

**Returns:**
double – Breite der Spalte in der Normalansicht.
### getColumnWidth(int column) {#getColumnWidth-int-}
```
public double getColumnWidth(int column)
```


Ermittelt die Breite(in Zeichen) der angegebenen Spalte in der Normalansicht

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Spalte | int | Spaltenindex |

**Returns:**
double – Breite der Spalte. Bei Tabellenkalkulationen wird die Spaltenbreite als Anzahl der Zeichen der maximalen Ziffernbreite der Zahlen 0~9 gemessen, wie sie in der Schriftart des Normalstils dargestellt werden.
### getColumnWidth(int column, boolean isOriginal, int unitType) {#getColumnWidth-int-boolean-int-}
```
public double getColumnWidth(int column, boolean isOriginal, int unitType)
```


Ermittelt die Spaltenbreite.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Spalte | int | Der Spaltenindex. |
| isOriginal | boolean | Gibt an, ob die ursprüngliche Breite abgerufen wird. |
| unitType | int | [CellsUnitType](../../com.aspose.cells/cellsunittype). |

**Returns:**
double -
### getColumnWidthInch(int column) {#getColumnWidthInch-int-}
```
public double getColumnWidthInch(int column)
```


Ermittelt die Breite der angegebenen Spalte in der Normalansicht, in Zoll.

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Bitte verwenden Sie stattdessen die Methode Cells.GetColumnWidth(int, bool, CellsUnitType). Diese Methode wird 12 Monate nach April 2024 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Spalte | int | Spaltenindex |

**Returns:**
double – Breite der Spalte in der Normalansicht.
### getColumnWidthPixel(int column) {#getColumnWidthPixel-int-}
```
public int getColumnWidthPixel(int column)
```


Ermittelt die Breite der angegebenen Spalte in der Normalansicht, in Pixel.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Spalte | int | Spaltenindex |

**Returns:**
int – Breite der Spalte in der Normalansicht.
### getColumnWidthPixel(int column, boolean original) {#getColumnWidthPixel-int-boolean-}
```
public int getColumnWidthPixel(int column, boolean original)
```


Ermittelt die Breite der angegebenen Spalte in der Normalansicht, in Pixel.

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Bitte verwenden Sie stattdessen die Methode Cells.GetColumnWidth(int, bool, CellsUnitType). Diese Methode wird 12 Monate nach April 2024 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Spalte | int | Spaltenindex |
| original | boolean | Gibt an, ob die ursprüngliche Breite zurückgegeben wird, selbst wenn die Spalte ausgeblendet ist |

**Returns:**
int – Breite der Spalte in der Normalansicht.
### getColumns() {#getColumns--}
```
public ColumnCollection getColumns()
```


Ermittelt die Sammlung von [Column](../../com.aspose.cells/column)-Objekten, die die einzelnen Spalten in diesem Arbeitsblatt darstellen.

**Returns:**
[ColumnCollection](../../com.aspose.cells/columncollection)
### getCount() {#getCount--}
```
public int getCount()
```


Ermittelt die Gesamtanzahl der instanziierten Cell-Objekte.

**Returns:**
int
### getCountLarge() {#getCountLarge--}
```
public long getCountLarge()
```


Ermittelt die Gesamtanzahl der instanziierten Cell-Objekte.

**Returns:**
long
### getDependents(boolean isAll, int row, int column) {#getDependents-boolean-int-int-}
```
public Cell[] getDependents(boolean isAll, int row, int column)
```


Erhalte alle Zellen, die auf die bestimmte Zelle verweisen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isAll | boolean | Gibt an, ob andere Arbeitsblätter überprüft werden sollen |
| Zeile | int | Der Zeilenindex. |
| Spalte | int | Der Spaltenindex. |

**Returns:**
com.aspose.cells.Cell[] -
### getDependentsInCalculation(int row, int column, boolean recursive) {#getDependentsInCalculation-int-int-boolean-}
```
public Iterator getDependentsInCalculation(int row, int column, boolean recursive)
```


Ermittelt alle Zellen, deren berechnetes Ergebnis von einer bestimmten Zelle abhängt.

**Remarks**

Um diese Methode zu verwenden, stellen Sie bitte sicher, dass das Arbeitsbuch für [FormulaSettings.getEnableCalculationChain()](../../aspose.cells/formulasettings\#getEnableCalculationChain--) auf true gesetzt wurde und mit dieser Einstellung vollständig berechnet ist. Wenn es keine Formelbezüge zu dieser Zelle gibt, wird null zurückgegeben. Weitere Details und ein Beispiel finden Sie unter [Cell.getDependentsInCalculation(boolean)](../../com.aspose.cells/cell\#getDependentsInCalculation-boolean-).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex der spezifischen Zelle |
| Spalte | int | Spaltenindex der spezifischen Zelle. |
| rekursiv | boolean | Ob jene Abhängigkeiten zurückgegeben werden, die nicht direkt auf die spezifische Zelle verweisen, sondern auf andere Blätter dieser Zelle. |

**Returns:**
java.util.Iterator - Aufzählung, um alle abhängigen (Zellobjekte) zu enumerieren
### getFirstCell() {#getFirstCell--}
```
public Cell getFirstCell()
```


Ermittelt die erste Zelle in diesem Arbeitsblatt.

**Remarks**

Gibt null zurück, wenn im Arbeitsblatt keine Daten vorhanden sind.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getFirstDataRow(int column) {#getFirstDataRow-int-}
```
public int getFirstDataRow(int column)
```


Ermittelt den Index der ersten Zeile der Zelle, die Daten in der angegebenen Spalte enthält.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Spalte | int | Spaltenindex. |

**Returns:**
int - erster Zeilenindex.
### getGroupedColumnOutlineLevel(int columnIndex) {#getGroupedColumnOutlineLevel-int-}
```
public int getGroupedColumnOutlineLevel(int columnIndex)
```


Ermittelt die Gliederungsebene (nullbasiert) der Spalte.

**Remarks**

Wenn die Spalte nicht gruppiert ist, wird null zurückgegeben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnIndex | int | Der Spaltenindex |

**Returns:**
int - Die Gliederungsebene der Spalte
### getGroupedRowOutlineLevel(int rowIndex) {#getGroupedRowOutlineLevel-int-}
```
public int getGroupedRowOutlineLevel(int rowIndex)
```


Ermittelt die Gliederungsebene (nullbasiert) der Zeile.

**Remarks**

Wenn die Zeile nicht gruppiert ist, wird null zurückgegeben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowIndex | int | Der Zeilenindex. |

**Returns:**
int - Die Gliederungsebene (nullbasiert) der Zeile.
### getLastCell() {#getLastCell--}
```
public Cell getLastCell()
```


Ermittelt die letzte Zelle in diesem Arbeitsblatt.

**Remarks**

Gibt null zurück, wenn im Arbeitsblatt keine Daten vorhanden sind.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getLastDataRow(int column) {#getLastDataRow-int-}
```
public int getLastDataRow(int column)
```


Ermittelt den Index der letzten Zeile der Zelle, die Daten in der angegebenen Spalte enthält.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Spalte | int | Spaltenindex. |

**Returns:**
int - letzter Zeilenindex.
### getMaxColumn() {#getMaxColumn--}
```
public int getMaxColumn()
```


Maximaler Spaltenindex jener Zellen, die in der Sammlung instanziiert wurden (schließt die Spalte nicht ein, für die ein Stil für die gesamte Spalte definiert ist, aber in der keine Zelle instanziiert wurde).

**Remarks**

Gibt -1 zurück, wenn keine Zelle instanziiert wurde.

**Returns:**
int
### getMaxDataColumn() {#getMaxDataColumn--}
```
public int getMaxDataColumn()
```


Maximaler Spaltenindex der Zelle, die Daten enthält.

**Remarks**

\-1 wird zurückgegeben, wenn keine Zelle Daten enthält. Diese Eigenschaft muss alle Zellen in einem Arbeitsblatt dynamisch iterieren und prüfen, daher ist es ein zeitaufwändiger Vorgang und sollte nicht wiederholt aufgerufen werden, z. B. direkt als Bedingung in einer Schleife verwendet.

**Returns:**
int
### getMaxDataRow() {#getMaxDataRow--}
```
public int getMaxDataRow()
```


Maximaler Zeilenindex der Zelle, die Daten enthält.

**Remarks**

Gibt -1 zurück, wenn keine Zelle Daten enthält. Diese Eigenschaft muss Zellen und Zeilen dynamisch iterieren und prüfen, daher ist es ein zeitaufwändiger Vorgang und sollte nicht wiederholt aufgerufen werden, z. B. direkt als Bedingung in einer Schleife verwendet.

**Returns:**
int
### getMaxDisplayRange() {#getMaxDisplayRange--}
```
public Range getMaxDisplayRange()
```


Ermittelt den maximalen Bereich, der Daten, zusammengeführte Zellen und Formen enthält.

**Remarks**

Gibt null zurück, wenn das Arbeitsblatt leer ist, seit Aspose.Cells 21.5.2.

**Returns:**
[Range](../../com.aspose.cells/range)
### getMaxGroupedColumnOutlineLevel() {#getMaxGroupedColumnOutlineLevel--}
```
public int getMaxGroupedColumnOutlineLevel()
```


Ermittelt die maximale gruppierte Spalten-Gliederungsebene (nullbasiert).

**Returns:**
int - Die maximale gruppierte Spalten-Gliederungsebene (nullbasiert)
### getMaxGroupedRowOutlineLevel() {#getMaxGroupedRowOutlineLevel--}
```
public int getMaxGroupedRowOutlineLevel()
```


Ermittelt die maximale gruppierte Zeilen-Gliederungsebene (nullbasiert).

**Returns:**
int - Die maximale gruppierte Zeilen-Gliederungsebene (nullbasiert)
### getMaxRow() {#getMaxRow--}
```
public int getMaxRow()
```


Maximaler Zeilenindex der Zelle, die Daten oder Stil enthält.

**Remarks**

Gibt -1 zurück, wenn im Arbeitsblatt keine Zelle Daten oder Stil enthält. Diese Eigenschaft muss Zellen und Zeilen dynamisch iterieren und prüfen, daher ist es ein zeitaufwändiger Vorgang und sollte nicht wiederholt aufgerufen werden, z. B. direkt als Bedingung in einer Schleife verwendet.

**Returns:**
int
### getMemorySetting() {#getMemorySetting--}
```
public int getMemorySetting()
```


Ermittelt die Speicherverbrauchsoption für diese Zellen.

Siehe [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

Bemerkenswerte Grenzen und empfohlene Vorgänge für einige Modi:

| Modus | Bemerkungen | Unterstützt |
| ------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------- |
| [MemorySetting.MEMORY\_PREFERENCE](../../com.aspose.cells/memorysetting\#MEMORY-PREFERENCE) | Cells data will be maintained in compact format to decrease the memory cost. On other hand, the compact data also may cause higher time cost, especially when updating the cells data, or accessing cells/rows randomly | v8.0.0 |
|  | [MemorySetting.FILE\_CACHE](../../com.aspose.cells/memorysetting\#FILE-CACHE) | Wenn dieser Modus für ein beliebiges Arbeitsblatt in einer Arbeitsmappe verwendet wird, sollte am Ende der Arbeit [Workbook.dispose()](../../com.aspose.cells/workbook\#dispose--) aufgerufen werden, um alle Ressourcen wie die temporären Dateien freizugeben. |
 
Zufälliger Zugriff auf Zellen führt zu schlechter Leistung, weil Daten zufällig und wiederholt gelesen/aktualisiert werden müssen (so wird der Zeiger in der Datei entsprechend geändert und I/O‑Operationen werden wiederholt benötigt). Wenn möglich, greifen Sie bitte immer sequenziell auf die Daten zu (Zeile für Zeile).
 
Wenn die Daten einer Zeile/einer Zelle geändert werden, können die Daten anderer Zellen/Zeilen ebenfalls beeinflusst werden (z. B. werden die Daten verschoben/umgelagert, um ausreichend Platz für die geänderten Daten zu schaffen). Daher erfordert jede Änderung aller Daten die Synchronisation anderer vorhandener Objekte (wie Zeilen‑ oder Zellenobjekte). Um eine bessere Leistung zu erzielen, sollten Sie nicht mehrere Zeilen/Zellen gleichzeitig beibehalten. Die Verarbeitung nacheinander reduziert die Datensynchronisation und verbessert die Leistung ein wenig. | v25.7     |

**Returns:**
int
### getMergedAreas() {#getMergedAreas--}
```
public CellArea[] getMergedAreas()
```


Ermittelt alle zusammengeführten Zellen.

**Returns:**
com.aspose.cells.CellArea[]
### getMergedCells() {#getMergedCells--}
```
public ArrayList getMergedCells()
```


Ermittelt die Sammlung zusammengeführter Zellen.

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Methode Cells.GetMergedAreas(). Diese Methode wird 12 Monate später, seit November 2023, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Returns:**
java.util.ArrayList
### getMinColumn() {#getMinColumn--}
```
public int getMinColumn()
```


Minimaler Spaltenindex der Zellen, die in der Sammlung instanziiert wurden (schließt die Spalte nicht ein, in der der Stil für die gesamte Spalte definiert ist, aber keine Zelle instanziiert wurde).

**Remarks**

Diese Eigenschaft muss Zellen und Zeilen dynamisch iterieren und prüfen, daher ist es ein zeitaufwändiger Vorgang und sollte nicht wiederholt aufgerufen werden, zum Beispiel indem sie direkt als Bedingung in einer Schleife verwendet wird.

**Returns:**
int
### getMinDataColumn() {#getMinDataColumn--}
```
public int getMinDataColumn()
```


Minimaler Spaltenindex der Zelle, die Daten enthält.

**Remarks**

\-1 wird zurückgegeben, wenn keine Zelle Daten enthält. Diese Eigenschaft muss alle Zellen in einem Arbeitsblatt dynamisch iterieren und prüfen, daher ist es ein zeitaufwändiger Vorgang und sollte nicht wiederholt aufgerufen werden, z. B. direkt als Bedingung in einer Schleife verwendet.

**Returns:**
int
### getMinDataRow() {#getMinDataRow--}
```
public int getMinDataRow()
```


Minimaler Zeilenindex der Zelle, die Daten enthält.

**Remarks**

Gibt -1 zurück, wenn keine Zelle Daten enthält. Diese Eigenschaft muss Zellen und Zeilen dynamisch iterieren und prüfen, daher ist es ein zeitaufwändiger Vorgang und sollte nicht wiederholt aufgerufen werden, z. B. direkt als Bedingung in einer Schleife verwendet.

**Returns:**
int
### getMinRow() {#getMinRow--}
```
public int getMinRow()
```


Minimaler Zeilenindex der Zelle, die Daten oder Stil enthält.

**Remarks**

Diese Eigenschaft muss Zellen und Zeilen dynamisch iterieren und prüfen, daher ist es ein zeitaufwändiger Vorgang und sollte nicht wiederholt aufgerufen werden, zum Beispiel indem sie direkt als Bedingung in einer Schleife verwendet wird.

**Returns:**
int
### getMultiThreadReading() {#getMultiThreadReading--}
```
public boolean getMultiThreadReading()
```


Ermittelt, ob das Zellen-Datenmodell Multi‑Thread‑Lesen unterstützen soll. Der Standardwert dieser Eigenschaft ist false.

**Remarks**

Wenn mehrere Threads gleichzeitig Row/Cell‑Objekte in dieser Sammlung lesen, sollte diese Eigenschaft auf true gesetzt werden, sonst können unerwartete Ergebnisse entstehen. Die Unterstützung von Multi‑Thread‑Lesen kann die Leistung beim Zugriff auf Row/Cell‑Objekte aus dieser Sammlung beeinträchtigen. Bitte beachten Sie, dass einige Funktionen Multi‑Thread‑Lesen nicht unterstützen, wie z. B. das Formatieren von Werten (durch [Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--), [Cell.getDisplayStringValue()](../../com.aspose.cells/cell\#getDisplayStringValue--), usw.). Daher können diese APIs selbst bei auf true gesetzter Eigenschaft weiterhin unerwartete Ergebnisse beim Multi‑Thread‑Lesen liefern.

**Returns:**
boolean
### getOdsCellFields() {#getOdsCellFields--}
```
public OdsCellFieldCollection getOdsCellFields()
```


Ermittelt die Liste der Felder von ods.

**Returns:**
[OdsCellFieldCollection](../../com.aspose.cells/odscellfieldcollection)
### getPreserveString() {#getPreserveString--}
```
public boolean getPreserveString()
```


Ermittelt einen Wert, der angibt, ob alle Arbeitsblattwerte als Zeichenfolgen erhalten bleiben. Der Standardwert ist false.

**Returns:**
boolean
### getRanges() {#getRanges--}
```
public RangeCollection getRanges()
```


Ermittelt die Sammlung von [Range](../../com.aspose.cells/range)-Objekten, die zur Laufzeit erstellt werden.

**Returns:**
[RangeCollection](../../com.aspose.cells/rangecollection)
### getRowEnumerator() {#getRowEnumerator--}
```
public Iterator getRowEnumerator()
```


Ermittelt den Zeilen‑Enumerator.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode RowCollection.GetEnumerator(). Diese Methode wird 12 Monate nach Mai 2023 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Returns:**
java.util.Iterator – Der Zeilen‑Enumerator.
### getRowHeight(int row) {#getRowHeight-int-}
```
public double getRowHeight(int row)
```


Ermittelt die Höhe einer angegebenen Zeile in der Einheit Punkte.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex |

**Returns:**
double – Höhe der Zeile
### getRowHeight(int row, boolean isOriginal, int unitType) {#getRowHeight-int-boolean-int-}
```
public double getRowHeight(int row, boolean isOriginal, int unitType)
```


Ermittelt die Zeilenhöhe.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Der Zeilenindex. |
| isOriginal | boolean | Gibt an, ob die ursprüngliche Zeilenhöhe oder 0 für eine ausgeblendete Zeile zurückgegeben wird. |
| unitType | int | [CellsUnitType](../../com.aspose.cells/cellsunittype). Einheitstyp des zurückgegebenen Höhenwerts |

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
### getRowOriginalHeightPoint(int row) {#getRowOriginalHeightPoint-int-}
```
public double getRowOriginalHeightPoint(int row)
```


Ermittelt die ursprüngliche Zeilenhöhe in der Einheit Punkt, wenn die Zeile ausgeblendet ist.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode Cells.GetRowHeight(int,bool,CellsUnitType). Diese Methode wird 12 Monate nach April 2024 entfernt. Aspense entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Der Zeilenindex. |

**Returns:**
double -
### getRows() {#getRows--}
```
public RowCollection getRows()
```


Ermittelt die Sammlung von [Row](../../com.aspose.cells/row)-Objekten, die die einzelnen Zeilen in diesem Arbeitsblatt darstellen.

**Returns:**
[RowCollection](../../com.aspose.cells/rowcollection)
### getStandardHeight() {#getStandardHeight--}
```
public double getStandardHeight()
```


Ermittelt die Standardzeilenhöhe in diesem Arbeitsblatt in der Einheit Punkte.

**Returns:**
double
### getStandardHeightInch() {#getStandardHeightInch--}
```
public double getStandardHeightInch()
```


Ermittelt die Standardzeilenhöhe in diesem Arbeitsblatt in der Einheit Zoll.

**Returns:**
double
### getStandardHeightPixels() {#getStandardHeightPixels--}
```
public int getStandardHeightPixels()
```


Ermittelt die Standardzeilenhöhe in diesem Arbeitsblatt in der Einheit Pixel.

**Returns:**
int
### getStandardWidth() {#getStandardWidth--}
```
public double getStandardWidth()
```


Ermittelt die Standardspaltenbreite im Arbeitsblatt in der Einheit Zeichen.

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
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Ermittelt den Standardstil des Arbeitsblatts.

**Returns:**
[Style](../../com.aspose.cells/style)
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
### getViewRowHeight(int row) {#getViewRowHeight-int-}
```
public double getViewRowHeight(int row)
```


Ermittelt die Höhe einer angegebenen Zeile.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex. |

**Returns:**
double – Höhe der Zeile.
### getViewRowHeightInch(int row) {#getViewRowHeightInch-int-}
```
public double getViewRowHeightInch(int row)
```


Ermittelt die Höhe einer angegebenen Zeile in der Einheit Zoll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex |

**Returns:**
double – Höhe der Zeile
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

### groupRows(int firstIndex, int lastIndex, boolean isHidden) {#groupRows-int-int-boolean-}
```
public void groupRows(int firstIndex, int lastIndex, boolean isHidden)
```


Gruppiert Zeilen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstIndex | int | Der erste Zeilenindex, der gruppiert werden soll. |
| lastIndex | int | Der letzte Zeilenindex, der gruppiert werden soll. |
| isHidden | boolean | Gibt an, ob die gruppierten Zeilen ausgeblendet sind. |

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

### hideColumns(int column, int totalColumns) {#hideColumns-int-int-}
```
public void hideColumns(int column, int totalColumns)
```


Mehrere Spalten ausblenden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Spalte | int | Spaltenindex. |
| totalColumns | int | Spaltennummer. |

### hideGroupDetail(boolean isVertical, int index) {#hideGroupDetail-boolean-int-}
```
public void hideGroupDetail(boolean isVertical, int index)
```


Klappt die gruppierten Zeilen/Spalten zusammen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isVertical | boolean | True, gruppierte Zeilen zusammenfalten. |
| Index | int | Der Zeilen-/Spaltenindex |

### hideRow(int row) {#hideRow-int-}
```
public void hideRow(int row)
```


Blendet eine Zeile aus.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex. |

### hideRows(int row, int totalRows) {#hideRows-int-int-}
```
public void hideRows(int row, int totalRows)
```


Mehrere Zeilen ausblenden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Der Zeilenindex. |
| totalRows | int | Die Zeilennummer. |

### importArray(double[] doubleArray, int firstRow, int firstColumn, boolean isVertical) {#importArray-double---int-int-boolean-}
```
public void importArray(double[] doubleArray, int firstRow, int firstColumn, boolean isVertical)
```


Importiert ein Array von Double in ein Arbeitsblatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| doubleArray | double[] | Double-Array. |
| firstRow | int | Die Zeilennummer der ersten Zelle, die importiert werden soll. |
| firstColumn | int | Die Spaltennummer der ersten Zelle, die importiert werden soll. |
| isVertical | boolean | Gibt an, ob Daten vertikal oder horizontal importiert werden. |

### importArray(double[][] doubleArray, int firstRow, int firstColumn) {#importArray-double-----int-int-}
```
public void importArray(double[][] doubleArray, int firstRow, int firstColumn)
```


Importiert ein zweidimensionales Array von Double in ein Arbeitsblatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| doubleArray | double[][] | Zweidimensionales Double-Array. |
| firstRow | int | Die Zeilennummer der ersten Zelle, die importiert werden soll. |
| firstColumn | int | Die Spaltennummer der ersten Zelle, die importiert werden soll. |

### importArray(int[] intArray, int firstRow, int firstColumn, boolean isVertical) {#importArray-int---int-int-boolean-}
```
public void importArray(int[] intArray, int firstRow, int firstColumn, boolean isVertical)
```


Importiert ein Array von Integer in ein Arbeitsblatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| intArray | int[] | Integer-Array. |
| firstRow | int | Die Zeilennummer der ersten Zelle, die importiert werden soll. |
| firstColumn | int | Die Spaltennummer der ersten Zelle, die importiert werden soll. |
| isVertical | boolean | Gibt an, ob Daten vertikal oder horizontal importiert werden. |

### importArray(int[][] intArray, int firstRow, int firstColumn) {#importArray-int-----int-int-}
```
public void importArray(int[][] intArray, int firstRow, int firstColumn)
```


Importiert ein zweidimensionales Array von Integer in ein Arbeitsblatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| intArray | int[][] | Zweidimensionales Integer-Array. |
| firstRow | int | Die Zeilennummer der ersten Zelle, die importiert werden soll. |
| firstColumn | int | Die Spaltennummer der ersten Zelle, die importiert werden soll. |

### importArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical) {#importArray-java.lang.String---int-int-boolean-}
```
public void importArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical)
```


Importiert ein Array von String in ein Arbeitsblatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stringArray | java.lang.String[] | String-Array. |
| firstRow | int | Die Zeilennummer der ersten Zelle, die importiert werden soll. |
| firstColumn | int | Die Spaltennummer der ersten Zelle, die importiert werden soll. |
| isVertical | boolean | Gibt an, ob Daten vertikal oder horizontal importiert werden. |

### importArray(String[][] stringArray, int firstRow, int firstColumn) {#importArray-java.lang.String-----int-int-}
```
public void importArray(String[][] stringArray, int firstRow, int firstColumn)
```


Importiert ein zweidimensionales Array von String in ein Arbeitsblatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stringArray | java.lang.String[][] | Zweidimensionales String-Array. |
| firstRow | int | Die Zeilennummer der ersten Zelle, die importiert werden soll. |
| firstColumn | int | Die Spaltennummer der ersten Zelle, die importiert werden soll. |

### importArrayList(ArrayList arrayList, int firstRow, int firstColumn, boolean isVertical) {#importArrayList-java.util.ArrayList-int-int-boolean-}
```
public void importArrayList(ArrayList arrayList, int firstRow, int firstColumn, boolean isVertical)
```


Importiert eine ArrayList von Daten in ein Arbeitsblatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arrayList | java.util.ArrayList | Daten-Arraylist. |
| firstRow | int | Die Zeilennummer der ersten Zelle, die importiert werden soll. |
| firstColumn | int | Die Spaltennummer der ersten Zelle, die importiert werden soll. |
| isVertical | boolean | Gibt an, ob Daten vertikal oder horizontal importiert werden. |

### importCSV(InputStream stream, TxtLoadOptions options, int firstRow, int firstColumn) {#importCSV-java.io.InputStream-com.aspose.cells.TxtLoadOptions-int-int-}
```
public void importCSV(InputStream stream, TxtLoadOptions options, int firstRow, int firstColumn)
```


Importiere eine CSV-Datei in die Zellen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.InputStream | Der CSV-Dateistream. |
| options | [TxtLoadOptions](../../com.aspose.cells/txtloadoptions) | Die Ladeoptionen zum Lesen der Textdatei |
| firstRow | int | Die Zeilennummer der ersten Zelle, die importiert werden soll. |
| firstColumn | int | Die Spaltennummer der ersten Zelle, die importiert werden soll. |

### importCSV(InputStream stream, String splitter, boolean convertNumericData, int firstRow, int firstColumn) {#importCSV-java.io.InputStream-java.lang.String-boolean-int-int-}
```
public void importCSV(InputStream stream, String splitter, boolean convertNumericData, int firstRow, int firstColumn)
```


Importiere eine CSV-Datei in die Zellen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.InputStream | Der CSV-Dateistream. |
| splitter | java.lang.String | Der Splitter |
| convertNumericData | boolean | Ob die Zeichenkette in der Textdatei in numerische Daten konvertiert wird. |
| firstRow | int | Die Zeilennummer der ersten Zelle, die importiert werden soll. |
| firstColumn | int | Die Spaltennummer der ersten Zelle, die importiert werden soll. |

### importCSV(String fileName, TxtLoadOptions options, int firstRow, int firstColumn) {#importCSV-java.lang.String-com.aspose.cells.TxtLoadOptions-int-int-}
```
public void importCSV(String fileName, TxtLoadOptions options, int firstRow, int firstColumn)
```


Importiere eine CSV-Datei in die Zellen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | java.lang.String | Der CSV-Dateiname. |
| options | [TxtLoadOptions](../../com.aspose.cells/txtloadoptions) | Die Ladeoptionen zum Lesen der Textdatei |
| firstRow | int | Die Zeilennummer der ersten Zelle, die importiert werden soll. |
| firstColumn | int | Die Spaltennummer der ersten Zelle, die importiert werden soll. |

### importCSV(String fileName, String splitter, boolean convertNumericData, int firstRow, int firstColumn) {#importCSV-java.lang.String-java.lang.String-boolean-int-int-}
```
public void importCSV(String fileName, String splitter, boolean convertNumericData, int firstRow, int firstColumn)
```


Importiere eine CSV-Datei in die Zellen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | java.lang.String | Der CSV-Dateiname. |
| splitter | java.lang.String | Der Splitter |
| convertNumericData | boolean | Ob die Zeichenkette in der Textdatei in numerische Daten konvertiert wird. |
| firstRow | int | Die Zeilennummer der ersten Zelle, die importiert werden soll. |
| firstColumn | int | Die Spaltennummer der ersten Zelle, die importiert werden soll. |

### importCustomObjects(Collection list, int firstRow, int firstColumn, ImportTableOptions options) {#importCustomObjects-java.util.Collection-int-int-com.aspose.cells.ImportTableOptions-}
```
public int importCustomObjects(Collection list, int firstRow, int firstColumn, ImportTableOptions options)
```


Importiert benutzerdefinierte Objekte.

**Remarks**

Die benutzerdefinierten Objekte sollten vom selben Typ sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Liste | java.util.Collection | Das benutzerdefinierte Objekt |
| firstRow | int | Die Zeilennummer der ersten Zelle, die importiert werden soll. |
| firstColumn | int | Die Spaltennummer der ersten Zelle, die importiert werden soll. |
| options | [ImportTableOptions](../../com.aspose.cells/importtableoptions) | Die Importoptionen. |

**Returns:**
int – Gesamtzahl der importierten Zeilen.
### importCustomObjects(Collection list, String[] propertyNames, boolean isPropertyNameShown, int firstRow, int firstColumn, int rowNumber, boolean insertRows, String dateFormatString, boolean convertStringToNumber) {#importCustomObjects-java.util.Collection-java.lang.String---boolean-int-int-int-boolean-java.lang.String-boolean-}
```
public int importCustomObjects(Collection list, String[] propertyNames, boolean isPropertyNameShown, int firstRow, int firstColumn, int rowNumber, boolean insertRows, String dateFormatString, boolean convertStringToNumber)
```


Importiert benutzerdefinierte Objekte.

**Remarks**

Die benutzerdefinierten Objekte sollten vom selben Typ sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Liste | java.util.Collection | Das benutzerdefinierte Objekt |
| propertyNames | java.lang.String[] | Die Eigenschaftsnamen. Wenn sie null ist, importieren wir alle Eigenschaften des Objekts. |
| isPropertyNameShown | boolean | Gibt an, ob der Eigenschaftsname in die erste Zeile importiert wird. |
| firstRow | int | Die Zeilennummer der ersten Zelle, die importiert werden soll. |
| firstColumn | int | Die Spaltennummer der ersten Zelle, die importiert werden soll. |
| rowNumber | int | Anzahl der zu importierenden Zeilen. |
| insertRows | boolean | Gibt an, ob zusätzliche Zeilen hinzugefügt werden, um die Daten anzupassen. |
| dateFormatString | java.lang.String | Datumsformatzeichenfolge für Zellen. |
| convertStringToNumber | boolean | Gibt an, ob diese Methode versucht, Zeichenketten in Zahlen zu konvertieren. |

**Returns:**
int – Gesamtzahl der importierten Zeilen.
### importData(ICellsDataTable table, int firstRow, int firstColumn, ImportTableOptions options) {#importData-com.aspose.cells.ICellsDataTable-int-int-com.aspose.cells.ImportTableOptions-}
```
public int importData(ICellsDataTable table, int firstRow, int firstColumn, ImportTableOptions options)
```


Importiere Daten aus einer benutzerdefinierten Datentabelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| table | [ICellsDataTable](../../com.aspose.cells/icellsdatatable) | Die benutzerdefinierte Datentabelle. |
| firstRow | int | Erster Zeilenindex. |
| firstColumn | int | Erster Spaltenindex. |
| options | [ImportTableOptions](../../com.aspose.cells/importtableoptions) | Die Importoptionen |

**Returns:**
int -
### importFormulaArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical) {#importFormulaArray-java.lang.String---int-int-boolean-}
```
public void importFormulaArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical)
```


Importiert ein Array von Formeln in ein Arbeitsblatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stringArray | java.lang.String[] | Formel-Array. |
| firstRow | int | Die Zeilennummer der ersten Zelle, die importiert werden soll. |
| firstColumn | int | Die Spaltennummer der ersten Zelle, die importiert werden soll. |
| isVertical | boolean | Gibt an, ob Daten vertikal oder horizontal importiert werden. |

### importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical) {#importObjectArray-java.lang.Object---int-int-boolean-}
```
public void importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical)
```


Importiert ein Array von Daten in ein Arbeitsblatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| objArray | java.lang.Object[] | Daten-Array. |
| firstRow | int | Die Zeilennummer der ersten Zelle, die importiert werden soll. |
| firstColumn | int | Die Spaltennummer der ersten Zelle, die importiert werden soll. |
| isVertical | boolean | Gibt an, ob Daten vertikal oder horizontal importiert werden. |

### importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical, int skip) {#importObjectArray-java.lang.Object---int-int-boolean-int-}
```
public void importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical, int skip)
```


Importiert ein Array von Daten in ein Arbeitsblatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| objArray | java.lang.Object[] | Daten-Array. |
| firstRow | int | Die Zeilennummer der ersten Zelle, die importiert werden soll. |
| firstColumn | int | Die Spaltennummer der ersten Zelle, die importiert werden soll. |
| isVertical | boolean | Gibt an, ob Daten vertikal oder horizontal importiert werden. |
| überspringen | int | Übersprungene Anzahl von Zeilen oder Spalten. |

### importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown) {#importResultSet-java.sql.ResultSet-int-int-boolean-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown)
```


Importiert Daten aus einem ResultSet-Objekt in das Arbeitsblatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rs | java.sql.ResultSet | das ResultSet-Objekt, aus dem importiert werden soll. |
| rowIndex | int | Startzeilenindex im Arbeitsblatt. |
| columnIndex | int | Startspaltenindex im Arbeitsblatt. |
| isFieldNameShown | boolean | Gibt an, ob der Feldname des Resultsets in die erste Zeile importiert wird. |

**Returns:**
int – wie viele Zeilen tatsächlich importiert wurden.
### importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber) {#importResultSet-java.sql.ResultSet-int-int-boolean-java.lang.String-boolean-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber)
```


Importiert Daten aus einem ResultSet-Objekt in das Arbeitsblatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rs | java.sql.ResultSet | das ResultSet-Objekt, aus dem importiert werden soll. |
| rowIndex | int | Startzeilenindex im Arbeitsblatt. |
| columnIndex | int | Startspaltenindex im Arbeitsblatt. |
| isFieldNameShown | boolean | Gibt an, ob der Feldname des Resultsets in die erste Zeile importiert wird. |
| customDateFormatString | java.lang.String | Datumsformatzeichenfolge für Zellen, die einen Datumswert enthalten. |
| convertStringToNumber | boolean | Gibt an, ob diese Methode versucht, Zeichenketten in Zahlen zu konvertieren. |

**Returns:**
int – wie viele Zeilen tatsächlich importiert wurden.
### importResultSet(ResultSet rs, int rowIndex, int columnIndex, ImportTableOptions options) {#importResultSet-java.sql.ResultSet-int-int-com.aspose.cells.ImportTableOptions-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, ImportTableOptions options)
```


Importiert Daten aus einem ResultSet-Objekt in das Arbeitsblatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rs | java.sql.ResultSet | das ResultSet-Objekt, aus dem importiert werden soll. |
| rowIndex | int | Startzeilenindex im Arbeitsblatt. |
| columnIndex | int | Startspaltenindex im Arbeitsblatt. |
| options | [ImportTableOptions](../../com.aspose.cells/importtableoptions) | Die Importoptionen |

**Returns:**
int – wie viele Zeilen tatsächlich importiert wurden.
### importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown) {#importResultSet-java.sql.ResultSet-int-int-int-int-boolean-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown)
```


Importiert Daten aus einem ResultSet-Objekt in das Arbeitsblatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rs | java.sql.ResultSet | das ResultSet-Objekt, aus dem importiert werden soll. |
| rowIndex | int | Startzeilenindex im Arbeitsblatt. |
| columnIndex | int | Startspaltenindex im Arbeitsblatt. |
| rowNum | int | Anzahl der zu importierenden Zeilen. -1, um alle Datensätze im angegebenen Resultset zu importieren. |
| columnNum | int | Anzahl der zu importierenden Spalten. -1, um alle Spalten im angegebenen Resultset zu importieren. |
| isFieldNameShown | boolean | Gibt an, ob der Feldname des Resultsets in die erste Zeile importiert wird. |

**Returns:**
int – wie viele Zeilen tatsächlich importiert wurden.
### importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber) {#importResultSet-java.sql.ResultSet-int-int-int-int-boolean-java.lang.String-boolean-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber)
```


Importiert Daten aus einem ResultSet-Objekt in das Arbeitsblatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rs | java.sql.ResultSet | das ResultSet-Objekt, aus dem importiert werden soll. |
| rowIndex | int | Startzeilenindex im Arbeitsblatt. |
| columnIndex | int | Startspaltenindex im Arbeitsblatt. |
| rowNum | int | Anzahl der zu importierenden Zeilen. -1, um alle Datensätze im angegebenen Resultset zu importieren. |
| columnNum | int | Anzahl der zu importierenden Spalten. -1, um alle Spalten im angegebenen Resultset zu importieren. |
| isFieldNameShown | boolean | Gibt an, ob der Feldname des Resultsets in die erste Zeile importiert wird. |
| customDateFormatString | java.lang.String | Datumsformatzeichenfolge für Zellen, die einen Datumswert enthalten. |
| convertStringToNumber | boolean | Gibt an, ob diese Methode versucht, Zeichenketten in Zahlen zu konvertieren. |

**Returns:**
int – wie viele Zeilen tatsächlich importiert wurden.
### importResultSet(ResultSet rs, String startCell, boolean isFieldNameShown) {#importResultSet-java.sql.ResultSet-java.lang.String-boolean-}
```
public int importResultSet(ResultSet rs, String startCell, boolean isFieldNameShown)
```


Importiert Daten aus einem ResultSet-Objekt in das Arbeitsblatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rs | java.sql.ResultSet | das ResultSet-Objekt, aus dem importiert werden soll. |
| startCell | java.lang.String | Name der Startzelle, in die das Resultset eingefügt wird, z. B. "A1". |
| isFieldNameShown | boolean | Gibt an, ob der Feldname des Resultsets in die erste Zeile importiert wird. |

**Returns:**
int – wie viele Zeilen tatsächlich importiert wurden.
### importResultSet(ResultSet rs, String startCell, ImportTableOptions options) {#importResultSet-java.sql.ResultSet-java.lang.String-com.aspose.cells.ImportTableOptions-}
```
public int importResultSet(ResultSet rs, String startCell, ImportTableOptions options)
```


Importiert Daten aus einem ResultSet-Objekt in das Arbeitsblatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rs | java.sql.ResultSet | das ResultSet-Objekt, aus dem importiert werden soll. |
| startCell | java.lang.String | Name der Startzelle, in die das Resultset eingefügt wird, z. B. "A1". |
| options | [ImportTableOptions](../../com.aspose.cells/importtableoptions) | Die Importoptionen |

**Returns:**
int – wie viele Zeilen tatsächlich importiert wurden.
### importResultSet(ResultSet rs, String startCell, int rowNum, int columnNum, boolean isFieldNameShown) {#importResultSet-java.sql.ResultSet-java.lang.String-int-int-boolean-}
```
public int importResultSet(ResultSet rs, String startCell, int rowNum, int columnNum, boolean isFieldNameShown)
```


Importiert Daten aus einem ResultSet-Objekt in das Arbeitsblatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rs | java.sql.ResultSet | das ResultSet-Objekt, aus dem importiert werden soll. |
| startCell | java.lang.String | Name der Startzelle, in die das Resultset eingefügt wird, z. B. "A1". |
| rowNum | int | Anzahl der zu importierenden Zeilen. -1, um alle Datensätze im angegebenen Resultset zu importieren. |
| columnNum | int | Anzahl der zu importierenden Spalten. -1, um alle Spalten im angegebenen Resultset zu importieren. |
| isFieldNameShown | boolean | Gibt an, ob der Feldname des Resultsets in die erste Zeile importiert wird. |

**Returns:**
int – wie viele Zeilen tatsächlich importiert wurden.
### importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn) {#importTwoDimensionArray-java.lang.Object-----int-int-}
```
public void importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn)
```


Importiert ein zweidimensionales Array von Daten in ein Arbeitsblatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| objArray | java.lang.Object[][] | Zweidimensionales Datenarray. |
| firstRow | int | Die Zeilennummer der ersten Zelle, die importiert werden soll. |
| firstColumn | int | Die Spaltennummer der ersten Zelle, die importiert werden soll. |

### importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn, boolean convertStringToNumber) {#importTwoDimensionArray-java.lang.Object-----int-int-boolean-}
```
public void importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn, boolean convertStringToNumber)
```


Importiert ein zweidimensionales Array von Daten in ein Arbeitsblatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| objArray | java.lang.Object[][] | Zweidimensionales Datenarray. |
| firstRow | int | Die Zeilennummer der ersten Zelle, die importiert werden soll. |
| firstColumn | int | Die Spaltennummer der ersten Zelle, die importiert werden soll. |
| convertStringToNumber | boolean | Gibt an, ob diese Methode versucht, Zeichenketten in Zahlen zu konvertieren. |

### importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, boolean convertStringToNumber) {#importTwoDimensionArray-java.lang.Object-----java.lang.Object-----int-int-boolean-}
```
public void importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, boolean convertStringToNumber)
```


Importiert ein zweidimensionales Array von Daten in ein Arbeitsblatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| objArray | java.lang.Object[][] | Zweidimensionales Datenarray. |
| Stile | java.lang.Object[][] | Zweidimensionaler Datenstil. |
| firstRow | int | Die Zeilennummer der ersten Zelle, die importiert werden soll. |
| firstColumn | int | Die Spaltennummer der ersten Zelle, die importiert werden soll. |
| convertStringToNumber | boolean | Gibt an, ob diese Methode versucht, Zeichenketten in Zahlen zu konvertieren. |

### importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, TxtLoadOptions opts) {#importTwoDimensionArray-java.lang.Object-----java.lang.Object-----int-int-com.aspose.cells.TxtLoadOptions-}
```
public void importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, TxtLoadOptions opts)
```


Importiert ein zweidimensionales Array von Daten in ein Arbeitsblatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| objArray | java.lang.Object[][] | Zweidimensionales Datenarray. |
| Stile | java.lang.Object[][] | Zweidimensionaler Datenstil. |
| firstRow | int | Die Zeilennummer der ersten Zelle, die importiert werden soll. |
| firstColumn | int | Die Spaltennummer der ersten Zelle, die importiert werden soll. |
| opts | [TxtLoadOptions](../../com.aspose.cells/txtloadoptions) | Optionen zum Konvertieren von Zeichenkettenwerten |

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

### insertColumns(int columnIndex, int totalColumns, InsertOptions options) {#insertColumns-int-int-com.aspose.cells.InsertOptions-}
```
public void insertColumns(int columnIndex, int totalColumns, InsertOptions options)
```


Fügt mehrere Spalten in das Arbeitsblatt ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnIndex | int | Spaltenindex. |
| totalColumns | int | Die Anzahl der Spalten. |
| options | [InsertOptions](../../com.aspose.cells/insertoptions) | Die Optionen für den Einfügevorgang. |

### insertCutCells(Range cutRange, int row, int column, int shiftType) {#insertCutCells-com.aspose.cells.Range-int-int-int-}
```
public void insertCutCells(Range cutRange, int row, int column, int shiftType)
```


Einfügen des ausgeschnittenen Bereichs.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cutRange | [Range](../../com.aspose.cells/range) | Der Ausschneidebereich. |
| Zeile | int | Die Zeile. |
| Spalte | int | Die Spalte. |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). Gibt an, wie andere Objekte des Zielbereichs verschoben werden sollen, wenn ein ausgeschnittener Bereich eingefügt wird. |

### insertRange(CellArea area, int shiftType) {#insertRange-com.aspose.cells.CellArea-int-}
```
public void insertRange(CellArea area, int shiftType)
```


Fügt einen Zellbereich ein und verschiebt Zellen gemäß der Verschiebungsoption.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| area | [CellArea](../../com.aspose.cells/cellarea) | Verschiebebereich. |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). Option zum Verschieben von Zellen. |

### insertRange(CellArea area, int shiftNumber, int shiftType) {#insertRange-com.aspose.cells.CellArea-int-int-}
```
public void insertRange(CellArea area, int shiftNumber, int shiftType)
```


Fügt einen Zellbereich ein und verschiebt Zellen gemäß der Verschiebungsoption.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| area | [CellArea](../../com.aspose.cells/cellarea) | Verschiebebereich. |
| shiftNumber | int | Anzahl der einzufügenden Zeilen oder Spalten. |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). Option zum Verschieben von Zellen. |

### insertRange(CellArea area, int shiftNumber, int shiftType, boolean updateReference) {#insertRange-com.aspose.cells.CellArea-int-int-boolean-}
```
public void insertRange(CellArea area, int shiftNumber, int shiftType, boolean updateReference)
```


Fügt einen Zellbereich ein und verschiebt Zellen gemäß der Verschiebungsoption.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| area | [CellArea](../../com.aspose.cells/cellarea) | Verschiebebereich. |
| shiftNumber | int | Anzahl der einzufügenden Zeilen oder Spalten. |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). Option zum Verschieben von Zellen. |
| updateReference | boolean | Gibt an, ob Referenzen in anderen Arbeitsblättern aktualisiert werden. |

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

### insertRows(int rowIndex, int totalRows, InsertOptions options) {#insertRows-int-int-com.aspose.cells.InsertOptions-}
```
public void insertRows(int rowIndex, int totalRows, InsertOptions options)
```


Fügt mehrere Zeilen in das Arbeitsblatt ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowIndex | int | Zeilenindex. |
| totalRows | int | Anzahl der einzufügenden Zeilen. |
| options | [InsertOptions](../../com.aspose.cells/insertoptions) | Optionen für den Einfügevorgang. |

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
### isDefaultColumnHidden() {#isDefaultColumnHidden--}
```
public boolean isDefaultColumnHidden()
```




**Returns:**
boolean
### isDefaultRowHeightMatched() {#isDefaultRowHeightMatched--}
```
public boolean isDefaultRowHeightMatched()
```


Zeigt an, dass Zeilenhöhe und Standard‑Schriftgröße übereinstimmen.

**Returns:**
boolean
### isDefaultRowHidden() {#isDefaultRowHidden--}
```
public boolean isDefaultRowHidden()
```


Zeigt an, ob die Zeile standardmäßig ausgeblendet ist.

**Returns:**
boolean
### isDeletingRangeEnabled(int startRow, int startColumn, int totalRows, int totalColumns) {#isDeletingRangeEnabled-int-int-int-int-}
```
public boolean isDeletingRangeEnabled(int startRow, int startColumn, int totalRows, int totalColumns)
```


Überprüft, ob der Bereich gelöscht werden kann.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | int | Der Startzeilenindex des Bereichs. |
| startColumn | int | Der Startspaltenindex des Bereichs. |
| totalRows | int | Die Anzahl der Zeilen im Bereich. |
| totalColumns | int | Die Anzahl der Spalten im Bereich. |

**Returns:**
boolean -
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


Gibt den Zellen‑Enumerator zurück.

**Remarks**

Beim Durchlaufen von Elementen mit dem zurückgegebenen Enumerator sollte die Zellen‑Sammlung nicht verändert werden (z. B. Operationen, die dazu führen, dass neue Cell/Row erzeugt oder vorhandene Cell/Row gelöscht werden). Andernfalls kann der Enumerator möglicherweise nicht alle Zellen korrekt durchlaufen (einige Elemente können mehrfach durchlaufen oder übersprungen werden).

**Example**

```
         Workbook workbook = new Workbook("template.xlsx");
         	Cells cells = workbook.getWorksheets().get(0).getCells();
 
         	Iterator en = cells.iterator();
         	while (en.hasNext())
         	{
         	    Cell cell = (Cell)en.next();
         	    System.out.println(cell.getName() + ": " + cell.getValue());
         	}
```

**Returns:**
java.util.Iterator - Der Zellen‑Enumerator
### linkToXmlMap(String mapName, int row, int column, String path) {#linkToXmlMap-java.lang.String-int-int-java.lang.String-}
```
public void linkToXmlMap(String mapName, int row, int column, String path)
```


Link zu einer XML‑Zuordnung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| mapName | java.lang.String | Name der XML‑Karte |
| Zeile | int | Zeile der Zielzelle |
| Spalte | int | Spalte der Zielzelle |
| Pfad | java.lang.String | Pfad des XML‑Elements in der XML‑Karte |

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

### merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean mergeConflict) {#merge-int-int-int-int-boolean-}
```
public void merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean mergeConflict)
```


Führt einen angegebenen Zellbereich zu einer einzelnen Zelle zusammen.

**Remarks**

Referenzieren Sie die zusammengeführte Zelle über die Adresse der oberen linken Zelle im Bereich. Wenn mergeConflict true ist und der zusammengeführte Bereich mit anderen zusammengeführten Zellen kollidiert, werden andere zusammengeführte Zellen automatisch entfernt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstRow | int | Erste Zeile dieses Bereichs (nullbasiert) |
| firstColumn | int | Erste Spalte dieses Bereichs (nullbasiert) |
| totalRows | int | Anzahl der Zeilen (einsbasiert) |
| totalColumns | int | Anzahl der Spalten (beginnend bei 1) |
| mergeConflict | boolean | Zusammenführungs-Konflikt bei zusammengeführten Bereichen. |

### merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean checkConflict, boolean mergeConflict) {#merge-int-int-int-int-boolean-boolean-}
```
public void merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean checkConflict, boolean mergeConflict)
```


Führt einen angegebenen Zellbereich zu einer einzelnen Zelle zusammen.

**Remarks**

Referenzieren Sie die zusammengeführte Zelle über die Adresse der oberen linken Zelle im Bereich. Wenn mergeConflict true ist und der zusammengeführte Bereich mit anderen zusammengeführten Zellen kollidiert, werden andere zusammengeführte Zellen automatisch entfernt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstRow | int | Erste Zeile dieses Bereichs (nullbasiert) |
| firstColumn | int | Erste Spalte dieses Bereichs (nullbasiert) |
| totalRows | int | Anzahl der Zeilen (einsbasiert) |
| totalColumns | int | Anzahl der Spalten (beginnend bei 1) |
| checkConflict | boolean | Gibt an, ob überprüft wird, ob die zusammengeführten Zellen andere zusammengeführte Zellen überschneiden. |
| mergeConflict | boolean | Zusammenführungs-Konflikt bei zusammengeführten Bereichen. |

### moveRange(CellArea sourceArea, int destRow, int destColumn) {#moveRange-com.aspose.cells.CellArea-int-int-}
```
public void moveRange(CellArea sourceArea, int destRow, int destColumn)
```


Verschiebt den Bereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceArea | [CellArea](../../com.aspose.cells/cellarea) | Der Bereich, der verschoben werden soll. |
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




### removeDuplicates() {#removeDuplicates--}
```
public void removeDuplicates()
```


Entfernt doppelte Zeilen im Blatt.

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

### removeDuplicates(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders, int[] columnOffsets) {#removeDuplicates-int-int-int-int-boolean-int---}
```
public void removeDuplicates(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders, int[] columnOffsets)
```


Entfernt doppelte Daten des Bereichs.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | int | Die Startzeile. |
| startColumn | int | Die Startspalte |
| endRow | int | Der Endzeilenindex. |
| endColumn | int | Der Endspaltenindex. |
| hasHeaders | boolean | Gibt an, ob der Bereich Header enthält. |
| columnOffsets | int[] | Die Spaltenversätze. |

### removeFormulas() {#removeFormulas--}
```
public void removeFormulas()
```


Entfernt alle Formeln und ersetzt sie durch den Ergebniswert.

### retrieveSubtotalSetting(CellArea ca) {#retrieveSubtotalSetting-com.aspose.cells.CellArea-}
```
public SubtotalSetting retrieveSubtotalSetting(CellArea ca)
```


Ruft die Zwischensummen‑Einstellung des Bereichs ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Der Bereich |

**Returns:**
[SubtotalSetting](../../com.aspose.cells/subtotalsetting) - 
### setColumnWidth(int column, double width) {#setColumnWidth-int-double-}
```
public void setColumnWidth(int column, double width)
```


Setzt die Breite der angegebenen Spalte in der Normalansicht.

**Remarks**

Für Tabellenkalkulationen wird die Spaltenbreite als die Anzahl der Zeichen der maximalen Ziffernbreite der Zahlen 0~9 gemessen, wie sie in der Schriftart des normalen Stils dargestellt werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Spalte | int | Spaltenindex. |
| Breite | double | Breite der Spalte in Zeichen. Die Spaltenbreite muss zwischen 0 und 255 liegen. |

### setColumnWidthInch(int column, double inches) {#setColumnWidthInch-int-double-}
```
public void setColumnWidthInch(int column, double inches)
```


Setzt die Spaltenbreite in Zoll in der Normalansicht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Spalte | int | Spaltenindex. |
| Zoll | double | Anzahl der Zoll. |

### setColumnWidthPixel(int column, int pixels) {#setColumnWidthPixel-int-int-}
```
public void setColumnWidthPixel(int column, int pixels)
```


Setzt die Spaltenbreite in Pixeln in der Normalansicht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Spalte | int | Spaltenindex. |
| Pixel | int | Anzahl der Pixel. |

### setDefaultColumnHidden(boolean value) {#setDefaultColumnHidden-boolean-}
```
public void setDefaultColumnHidden(boolean value)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setDefaultRowHeightMatched(boolean value) {#setDefaultRowHeightMatched-boolean-}
```
public void setDefaultRowHeightMatched(boolean value)
```


Zeigt an, dass Zeilenhöhe und Standard‑Schriftgröße übereinstimmen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setDefaultRowHidden(boolean value) {#setDefaultRowHidden-boolean-}
```
public void setDefaultRowHidden(boolean value)
```


Zeigt an, ob die Zeile standardmäßig ausgeblendet ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setMemorySetting(int value) {#setMemorySetting-int-}
```
public void setMemorySetting(int value)
```


Setzt die Speicherverbrauchs‑Option für diese Zellen.

Siehe [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

Bemerkenswerte Grenzen und empfohlene Vorgänge für einige Modi:

| Modus | Bemerkungen | Unterstützt |
| ------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------- |
| [MemorySetting.MEMORY\_PREFERENCE](../../com.aspose.cells/memorysetting\#MEMORY-PREFERENCE) | Cells data will be maintained in compact format to decrease the memory cost. On other hand, the compact data also may cause higher time cost, especially when updating the cells data, or accessing cells/rows randomly | v8.0.0 |
|  | [MemorySetting.FILE\_CACHE](../../com.aspose.cells/memorysetting\#FILE-CACHE) | Wenn dieser Modus für ein beliebiges Arbeitsblatt in einer Arbeitsmappe verwendet wird, sollte am Ende der Arbeit [Workbook.dispose()](../../com.aspose.cells/workbook\#dispose--) aufgerufen werden, um alle Ressourcen wie die temporären Dateien freizugeben. |
 
Zufälliger Zugriff auf Zellen führt zu schlechter Leistung, weil Daten zufällig und wiederholt gelesen/aktualisiert werden müssen (so wird der Zeiger in der Datei entsprechend geändert und I/O‑Operationen werden wiederholt benötigt). Wenn möglich, greifen Sie bitte immer sequenziell auf die Daten zu (Zeile für Zeile).
 
Wenn die Daten einer Zeile/einer Zelle geändert werden, können die Daten anderer Zellen/Zeilen ebenfalls beeinflusst werden (z. B. werden die Daten verschoben/umgelagert, um ausreichend Platz für die geänderten Daten zu schaffen). Daher erfordert jede Änderung aller Daten die Synchronisation anderer vorhandener Objekte (wie Zeilen‑ oder Zellenobjekte). Um eine bessere Leistung zu erzielen, sollten Sie nicht mehrere Zeilen/Zellen gleichzeitig beibehalten. Die Verarbeitung nacheinander reduziert die Datensynchronisation und verbessert die Leistung ein wenig. | v25.7     |

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setMultiThreadReading(boolean value) {#setMultiThreadReading-boolean-}
```
public void setMultiThreadReading(boolean value)
```


Legt fest, ob das Zellen-Datenmodell das Lesen in mehreren Threads unterstützen soll. Der Standardwert dieser Eigenschaft ist false.

**Remarks**

Wenn mehrere Threads gleichzeitig Row/Cell‑Objekte in dieser Sammlung lesen, sollte diese Eigenschaft auf true gesetzt werden, sonst können unerwartete Ergebnisse entstehen. Die Unterstützung von Multi‑Thread‑Lesen kann die Leistung beim Zugriff auf Row/Cell‑Objekte aus dieser Sammlung beeinträchtigen. Bitte beachten Sie, dass einige Funktionen Multi‑Thread‑Lesen nicht unterstützen, wie z. B. das Formatieren von Werten (durch [Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--), [Cell.getDisplayStringValue()](../../com.aspose.cells/cell\#getDisplayStringValue--), usw.). Daher können diese APIs selbst bei auf true gesetzter Eigenschaft weiterhin unerwartete Ergebnisse beim Multi‑Thread‑Lesen liefern.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setPreserveString(boolean value) {#setPreserveString-boolean-}
```
public void setPreserveString(boolean value)
```


Legt einen Wert fest, der angibt, ob alle Arbeitsblattwerte als Zeichenfolgen erhalten bleiben. Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setRowHeight(int row, double height) {#setRowHeight-int-double-}
```
public void setRowHeight(int row, double height)
```


Setzt die Höhe der angegebenen Zeile.

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
| Zoll | double | Anzahl der Zoll. Sie sollte zwischen 0 und 409,5/72 liegen. |

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

### setStandardHeight(double value) {#setStandardHeight-double-}
```
public void setStandardHeight(double value)
```


Legt die Standardzeilenhöhe in diesem Arbeitsblatt fest, in der Einheit Punkte.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setStandardHeightInch(double value) {#setStandardHeightInch-double-}
```
public void setStandardHeightInch(double value)
```


Legt die Standardzeilenhöhe in diesem Arbeitsblatt fest, in der Einheit Zoll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setStandardHeightPixels(int value) {#setStandardHeightPixels-int-}
```
public void setStandardHeightPixels(int value)
```


Legt die Standardzeilenhöhe in diesem Arbeitsblatt fest, in der Einheit Pixel.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setStandardWidth(double value) {#setStandardWidth-double-}
```
public void setStandardWidth(double value)
```


Legt die Standardspaltenbreite im Arbeitsblatt fest, in der Einheit Zeichen.

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

### setStyle(Style value) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style value)
```


Legt den Standardstil des Arbeitsblatts fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Style](../../com.aspose.cells/style) |  |

### setViewColumnWidthPixel(int column, int pixels) {#setViewColumnWidthPixel-int-int-}
```
public void setViewColumnWidthPixel(int column, int pixels)
```


Legt die Spaltenbreite in verschiedenen Ansichten fest.

**Remarks**

Wenn der aktuelle Ansichtstyp [ViewType.PAGE\_LAYOUT\_VIEW](../../com.aspose.cells/viewtype\#PAGE-LAYOUT-VIEW) ist, entspricht die Spaltenbreite der gedruckten Breite.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Spalte | int | Der Spaltenindex. |
| Pixel | int | Die Breite in Pixeln. |

### showGroupDetail(boolean isVertical, int index) {#showGroupDetail-boolean-int-}
```
public void showGroupDetail(boolean isVertical, int index)
```


Erweitert die gruppierten Zeilen/Spalten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isVertical | boolean | Wahr, erweitert die gruppierten Zeilen. |
| Index | int | Der Zeilen-/Spaltenindex |

### subtotal(CellArea ca, int groupBy, int function, int[] totalList) {#subtotal-com.aspose.cells.CellArea-int-int-int---}
```
public void subtotal(CellArea ca, int groupBy, int function, int[] totalList)
```


Erstellt Zwischensummen für den Bereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Der Bereich |
| groupBy | int | Das Feld, nach dem gruppiert wird, als nullbasierter ganzzahliger Offset |
| function | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). Die Zwischensummenfunktion. |
| totalList | int[] | Ein Array von nullbasierten Feld-Offsets, das die Felder angibt, zu denen die Zwischensummen hinzugefügt werden. |

### subtotal(CellArea ca, int groupBy, int function, int[] totalList, boolean replace, boolean pageBreaks, boolean summaryBelowData) {#subtotal-com.aspose.cells.CellArea-int-int-int---boolean-boolean-boolean-}
```
public void subtotal(CellArea ca, int groupBy, int function, int[] totalList, boolean replace, boolean pageBreaks, boolean summaryBelowData)
```


Erstellt Zwischensummen für den Bereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Der Bereich |
| groupBy | int | Das Feld, nach dem gruppiert wird, als nullbasierter ganzzahliger Offset |
| function | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). Die Zwischensummenfunktion. |
| totalList | int[] | Ein Array von nullbasierten Feld-Offsets, das die Felder angibt, zu denen die Zwischensummen hinzugefügt werden. |
| replace | boolean | Gibt an, ob die aktuellen Zwischensummen ersetzt werden sollen |
| pageBreaks | boolean | Gibt an, ob ein Seitenumbruch zwischen Gruppen eingefügt werden soll |
| summaryBelowData | boolean | Gibt an, ob eine Zusammenfassung unter den Daten hinzugefügt wird. |

### textToColumns(int row, int column, int totalRows, TxtLoadOptions options) {#textToColumns-int-int-int-com.aspose.cells.TxtLoadOptions-}
```
public int textToColumns(int row, int column, int totalRows, TxtLoadOptions options)
```


Teilt den Inhalt in der angegebenen Spalte in mehrere Spalten auf..

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Der Zeilenindex. |
| Spalte | int | Der Spaltenindex. |
| totalRows | int | Die Anzahl der Zeilen. |
| options | [TxtLoadOptions](../../com.aspose.cells/txtloadoptions) | Die Aufteilungsoptionen. |

**Returns:**
int - Gesamtzahl der Spalten der geteilten Werte.
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

### ungroupRows(int firstIndex, int lastIndex, boolean isAll) {#ungroupRows-int-int-boolean-}
```
public void ungroupRows(int firstIndex, int lastIndex, boolean isAll)
```


Hebt die Gruppierung von Zeilen auf.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstIndex | int | Der Index der ersten Zeile, die aufgelöst werden soll. |
| lastIndex | int | Der Index der letzten Zeile, die aufgelöst werden soll. |
| isAll | boolean | Wahr, entfernt alle gruppierten Informationen. Andernfalls wird die äußere Gruppeninformation entfernt. |

### unhideColumn(int column, double width) {#unhideColumn-int-double-}
```
public void unhideColumn(int column, double width)
```


Blendet eine Spalte ein

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Spalte | int | Spaltenindex. |
| Breite | double | Spaltenbreite. |

### unhideColumns(int column, int totalColumns, double width) {#unhideColumns-int-int-double-}
```
public void unhideColumns(int column, int totalColumns, double width)
```


Blendet mehrere Spalten ein.

**Remarks**

Wendet die Spaltenbreite nur auf versteckte Spalten an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Spalte | int | Spaltenindex. |
| totalColumns | int | Spaltennummer |
| Breite | double | Spaltenbreite. |

### unhideRow(int row, double height) {#unhideRow-int-double-}
```
public void unhideRow(int row, double height)
```


Blendet eine Zeile ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex. |
| Höhe | double | Zeilenhöhe. Die Höhe der Zeile wird nur geändert, wenn die Zeile ausgeblendet ist und der angegebene Höhenwert positiv ist. |

### unhideRows(int row, int totalRows, double height) {#unhideRows-int-int-double-}
```
public void unhideRows(int row, int totalRows, double height)
```


Blendet die ausgeblendeten Zeilen ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Der Zeilenindex. |
| totalRows | int | Die Zeilennummer. |
| Höhe | double | Zeilenhöhe. Die Höhe der Zeile wird nur geändert, wenn die Zeile ausgeblendet ist und der angegebene Höhenwert positiv ist. |

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

