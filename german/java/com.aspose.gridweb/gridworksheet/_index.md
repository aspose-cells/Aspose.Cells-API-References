---
title: "GridWorksheet"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Kapselt das Objekt, das ein einzelnes Arbeitsblatt darstellt."
type: docs
url: /de/java/com.aspose.gridweb/gridworksheet/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.Control](../../com.aspose.gridweb/control)
```
public class GridWorksheet extends Control
```

Kapselt das Objekt, das ein einzelnes Arbeitsblatt darstellt.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [addAutoFilter(int row, int startColumn, int endColumn)](#addAutoFilter-int-int-int-) | Legt den Bereich fest, auf den der angegebene AutoFilter angewendet wird. |
| [addCustomFilter(int row, String critira)](#addCustomFilter-int-java.lang.String-) | Füge benutzerdefinierten Filter für die angegebene Zeile hinzu. |
| [autoFitColumn(int columnIndex)](#autoFitColumn-int-) | Passt die Spaltenbreite automatisch an. |
| [autoFitColumn(int columnIndex, int firstRow, int lastRow)](#autoFitColumn-int-int-int-) | Passt die Spaltenbreite automatisch an. |
| [autoFitColumns()](#autoFitColumns--) |  |
| [autoFitRow(int rowIndex)](#autoFitRow-int-) | Passt die Zeilenhöhe automatisch an. |
| [autoFitRow(int rowIndex, int firstColumn, int lastColumn)](#autoFitRow-int-int-int-) | Passt die Zeilenhöhe automatisch an. |
| [autoFitRow(int startRow, int endRow, int startColumn, int endColumn)](#autoFitRow-int-int-int-int-) | Passt die Zeilenhöhe in einem rechteckigen Bereich automatisch an. |
| [autoFitRows()](#autoFitRows--) | Passt alle Zeilen in diesem Arbeitsblatt automatisch an. |
| [autoFitRows(boolean onlyAuto)](#autoFitRows-boolean-) | Passt alle Zeilen in diesem Arbeitsblatt automatisch an. |
| [autoFitRows(int startRow, int endRow)](#autoFitRows-int-int-) | Passt die Zeilenhöhe in einem Bereich automatisch an. |
| [calculateFormula(String formula)](#calculateFormula-java.lang.String-) | Berechnet eine Formel. |
| [clearComments()](#clearComments--) | Löscht alle Kommentare im Designer-Tabellenblatt. |
| [copy(GridWorksheet sourceSheet)](#copy-com.aspose.gridweb.GridWorksheet-) | Kopiert Inhalte und Formate von einem anderen Arbeitsblatt. |
| [createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList)](#createSubtotal-int-int-int-int-int---) | Erstellt Zwischensumme im Blatt. |
| [createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString)](#createSubtotal-int-int-int-int-int---java.lang.String-com.aspose.gridweb.GridTableItemStyle-com.aspose.gridweb.GridTableItemStyle-int-java.lang.String-) | Erstellt Zwischensumme im Blatt. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filterString(int column, String criteria)](#filterString-int-java.lang.String-) | Setzt den Filter für die Spalte. Hinweis: Wir sollten AddAutoFilter aufrufen, bevor filterString verwendet wird. Der Filterkriterien-String. Hinweis: Wir verwenden das Komma -> \",\" als Trennzeichen, daher darf der zu filternde Zellenwert kein Komma enthalten. filterString(10,\"123,456\") bedeutet, Spalte 10 soll 123 oder 456 enthalten, filterString(10,\"123\") bedeutet, Spalte 10 soll 123 enthalten, der Spaltenindexwert wird durch Komma getrennt, z.B. 123,456,789 oder abc |
| [freezePanes(int row, int column, int freezedRows, int freezedColumns)](#freezePanes-int-int-int-int-) | Friert Bereiche an der angegebenen Zelle im Arbeitsblatt ein. |
| [freezePanes(String cellName, int freezedRows, int freezedColumns)](#freezePanes-java.lang.String-int-int-) | Friert Bereiche an der angegebenen Zelle im Arbeitsblatt ein. |
| [getActiveCell()](#getActiveCell--) | Ermittelt die aktive Zelle im Arbeitsblatt. |
| [getBackgroundImage()](#getBackgroundImage--) | Liefert das Hintergrundbild des Arbeitsblatts. |
| [getCells()](#getCells--) | Ruft die [GridCell](../../com.aspose.gridweb/gridcell)-Sammlung ab. |
| [getClass()](#getClass--) |  |
| [getCodeName()](#getCodeName--) | Stellt den Code-Namen des Arbeitsblatts dar. |
| [getColumnCaption(int column)](#getColumnCaption-int-) | Ruft die Spaltenbeschriftung ab. |
| [getColumnHeaderToolTip(int colIndex)](#getColumnHeaderToolTip-int-) | Ruft den Tooltip-Text des Spaltenkopfes ab. |
| [getColumnReadonly(int columnIndex)](#getColumnReadonly-int-) | Ruft ab, ob eine Spalte schreibgeschützt ist. |
| [getComments()](#getComments--) | Ruft die [GridComment](../../com.aspose.gridweb/gridcomment)-Sammlung ab. |
| [getDisplayRightToLeft()](#getDisplayRightToLeft--) | Gibt an, ob das angegebene Arbeitsblatt von rechts nach links statt von links nach rechts angezeigt wird. |
| [getDisplayZeros()](#getDisplayZeros--) | Wahr, wenn Nullwerte angezeigt werden. |
| [getFirstVisibleColumn()](#getFirstVisibleColumn--) | Stellt den Index der ersten sichtbaren Spalte dar. |
| [getFirstVisibleRow()](#getFirstVisibleRow--) | Stellt den Index der ersten sichtbaren Zeile dar. |
| [getFreezedPanes()](#getFreezedPanes--) | Liefert die Freeze‑Panes. |
| [getGridActiveCell()](#getGridActiveCell--) | Ermittelt die aktive Zelle im Arbeitsblatt. |
| [getHyperlinks()](#getHyperlinks--) | Ruft die [GridHyperlinkCollection](../../com.aspose.gridweb/gridhyperlinkcollection)-Sammlung ab. |
| [getIndex()](#getIndex--) | Liefert den Index des Blatts in der Arbeitsblatt‑Sammlung. |
| [getIsReadonly(int row, int col)](#getIsReadonly-int-int-) | Ruft ab, ob die Zelle schreibgeschützt ist. Dies ist ein erweitertes Attribut von GridWeb, das nicht in der tatsächlichen Excel-Datei erhalten bleibt. |
| [getName()](#getName--) | Liefert den Namen des Arbeitsblatts. |
| [getOutlineShown()](#getOutlineShown--) | Gibt an, ob die Gliederung angezeigt wird. |
| [getPictures()](#getPictures--) | Ruft eine [getPictures()](../../com.aspose.gridweb/gridworksheet\#getPictures--)‑Sammlung ab. |
| [getPivotTables()](#getPivotTables--) | Ruft die PivotTables im Arbeitsblatt ab. |
| [getRowCaption(int row)](#getRowCaption-int-) | Ruft die Zeilenbeschriftung ab. |
| [getRowHeaderToolTip(int rowIndex)](#getRowHeaderToolTip-int-) | Ruft den Tooltip-Text des Zeilenkopfes ab. |
| [getRowReadonly(int rowIndex)](#getRowReadonly-int-) | Ruft ab, ob eine Zeile schreibgeschützt ist. |
| [getSelected()](#getSelected--) | Gibt an, ob dieses Arbeitsblatt beim Öffnen der Arbeitsmappe ausgewählt ist. |
| [getShapes()](#getShapes--) | Ruft eine [getPictures()](../../com.aspose.gridweb/gridworksheet\#getPictures--)‑Sammlung ab. |
| [getStandardHeight()](#getStandardHeight--) | Ruft die Standardzeilenhöhe in diesem Arbeitsblatt in Punkten ab. |
| [getStandardHeightPixels()](#getStandardHeightPixels--) | Ruft die Standardzeilenhöhe in diesem Arbeitsblatt in Pixeln ab. |
| [getTabColor()](#getTabColor--) | Stellt die Registerkartenfarbe des Arbeitsblatts dar. |
| [getUniqueID()](#getUniqueID--) | Ruft die UniqueID im Steuerelement ab. |
| [getValidations()](#getValidations--) | Ruft die Datengültigkeits‑Einstellungs‑Sammlung im Arbeitsblatt ab. |
| [getVisible()](#getVisible--) | Gibt an, ob der Name dieses Blatts in den Blattregisterkarten des Steuerelements angezeigt wird. |
| [getWorkbook()](#getWorkbook--) | Ruft das [GridWorkbook](../../com.aspose.gridweb/gridworkbook)-Objekt der Arbeitsblattsammlung ab. |
| [getZoom()](#getZoom--) | Stellt den Skalierungsfaktor in Prozent dar. |
| [groupRows(int firstIndex, int lastIndex, boolean isHidden)](#groupRows-int-int-boolean-) | Gruppiert Zeilen. |
| [hashCode()](#hashCode--) |  |
| [isGridlinesVisible()](#isGridlinesVisible--) | Ruft einen Wert ab, der angibt, ob die Gitternetzlinien sichtbar sind. Standard ist true. |
| [isProtected()](#isProtected--) | Gibt an, ob das Arbeitsblatt geschützt ist. |
| [isSummaryRowBelow()](#isSummaryRowBelow--) | Gibt an, ob die Zusammenfassungszeile unter den Detailzeilen in der Gliederung positioniert wird. |
| [moveTo(int index)](#moveTo-int-) | Verschiebt das Blatt an eine andere Position in der Tabelle. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshFilter()](#refreshFilter--) | Aktualisiert Autofilter, um Zeilen auszublenden oder einzublenden. |
| [removeAutoFilter()](#removeAutoFilter--) | Entfernt den AutoFilter des Arbeitsblatts. |
| [removeSubtotal()](#removeSubtotal--) | Entfernt die durch die Methode CreateSubtotal im Blatt erstellte Zwischensumme. |
| [resetFilter(int fieldIndex)](#resetFilter-int-) | Der ganzzahlige Versatz des Feldes, auf das Sie anwenden möchten, basierend auf der ersten Filterspalte (von links in der Liste; das linkeste Feld ist Feld 0). |
| [setActiveCell(String value)](#setActiveCell-java.lang.String-) | Setzt die aktive Zelle im Arbeitsblatt. |
| [setAllCellsEditable()](#setAllCellsEditable--) | Macht alle Zellen editierbar. Dies ist ein erweitertes Attribut. |
| [setAllCellsReadonly()](#setAllCellsReadonly--) | Macht alle Zellen schreibgeschützt. Dies ist ein erweitertes Attribut; beachten Sie, dass dieses Attribut nicht in der tatsächlichen Zelle erhalten bleibt. Wenn Sie den Schutz beibehalten möchten, verwenden Sie bitte setProtect. |
| [setBackgroundImage(byte[] value)](#setBackgroundImage-byte---) | Setzt das Hintergrundbild des Arbeitsblatts. |
| [setColumnCaption(int column, String caption)](#setColumnCaption-int-java.lang.String-) | Setzt die Beschriftung für die Spalte. Bitte beachten Sie, dass dies ein Erweiterungsattribut ist und nicht in der Excel-Datei erhalten bleibt. |
| [setColumnHeaderToolTip(int colIndex, String toolTip)](#setColumnHeaderToolTip-int-java.lang.String-) | Setzt den Tooltip-Text des Spaltenkopfes. |
| [setColumnReadonly(int columnIndex, boolean isReadonly)](#setColumnReadonly-int-boolean-) | Setzt eine Spalte auf schreibgeschützt, sodass der Benutzer sie nicht von der Clientseite löschen kann. |
| [setDisplayRightToLeft(boolean value)](#setDisplayRightToLeft-boolean-) | Gibt an, ob das angegebene Arbeitsblatt von rechts nach links statt von links nach rechts angezeigt wird. |
| [setDisplayZeros(boolean value)](#setDisplayZeros-boolean-) | Wahr, wenn Nullwerte angezeigt werden. |
| [setEditableRange(int startRow, int startColumn, int rows, int columns)](#setEditableRange-int-int-int-int-) | Macht einen Zellbereich editierbar. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Machen Sie alle Zellen schreibgeschützt, indem Sie die Methode SetAllCellsReadonly aufrufen. |
| [setFirstVisibleColumn(int value)](#setFirstVisibleColumn-int-) | Stellt den Index der ersten sichtbaren Spalte dar. |
| [setFirstVisibleRow(int value)](#setFirstVisibleRow-int-) | Stellt den Index der ersten sichtbaren Zeile dar. |
| [setGridActiveCell(GridCell value)](#setGridActiveCell-com.aspose.gridweb.GridCell-) | Setzt die aktive Zelle im Arbeitsblatt. |
| [setGridlinesVisible(boolean value)](#setGridlinesVisible-boolean-) | Setzt einen Wert, der angibt, ob die Gitternetzlinien sichtbar sind. Standard ist true. |
| [setIsReadonly(int row, int col, boolean value)](#setIsReadonly-int-int-boolean-) | Legt fest, ob die Zelle schreibgeschützt ist. Dies ist ein erweitertes Attribut von GridWeb, das nicht in der tatsächlichen Excel-Datei gespeichert wird. |
| [setName(String value)](#setName-java.lang.String-) | Legt den Namen des Arbeitsblatts fest. |
| [setOutlineShown(boolean value)](#setOutlineShown-boolean-) | Gibt an, ob die Gliederung angezeigt wird. |
| [setProtect()](#setProtect--) | Schützt das Arbeitsblatt. |
| [setReadonlyRange(int startRow, int startColumn, int rows, int columns)](#setReadonlyRange-int-int-int-int-) | Macht einen Zellbereich schreibgeschützt. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Zuerst alle Zellen editierbar machen, indem Sie die Methode SetAllCellsEditable aufrufen. |
| [setRowCaption(int row, String caption)](#setRowCaption-int-java.lang.String-) | Setzt die Beschriftung für die Zeile. |
| [setRowHeaderToolTip(int rowIndex, String toolTip)](#setRowHeaderToolTip-int-java.lang.String-) | Setzt den Tooltip-Text der Zeilenüberschrift. |
| [setRowReadonly(int rowIndex, boolean isReadonly)](#setRowReadonly-int-boolean-) | Setzt eine Zeile auf schreibgeschützt, sodass der Benutzer sie clientseitig nicht löschen kann. |
| [setSelected(boolean value)](#setSelected-boolean-) | Gibt an, ob dieses Arbeitsblatt beim Öffnen der Arbeitsmappe ausgewählt ist. |
| [setStandardHeight(double value)](#setStandardHeight-double-) | Setzt die Standardzeilenhöhe in diesem Arbeitsblatt, in Punkten. |
| [setStandardHeightPixels(int value)](#setStandardHeightPixels-int-) | Setzt die Standardzeilenhöhe in diesem Arbeitsblatt, in Pixeln. |
| [setSummaryRowBelow(boolean value)](#setSummaryRowBelow-boolean-) | Gibt an, ob die Zusammenfassungszeile unter den Detailzeilen in der Gliederung positioniert wird. |
| [setTabColor(Color value)](#setTabColor-com.aspose.gridweb.Color-) | Stellt die Registerkartenfarbe des Arbeitsblatts dar. |
| [setVisible(boolean value)](#setVisible-boolean-) | Gibt an, ob der Name dieses Blatts in den Blattregisterkarten des Steuerelements angezeigt wird. |
| [setZoom(int value)](#setZoom-int-) | Stellt den Skalierungsfaktor in Prozent dar. |
| [toString()](#toString--) |  |
| [unFreezePanes()](#unFreezePanes--) | Löst das Einfrieren von Bereichen im Arbeitsblatt. |
| [unGroupRows(int firstIndex, int lastIndex)](#unGroupRows-int-int-) | Hebt die Gruppierung von Zeilen auf. |
| [unProtect()](#unProtect--) | Entfernt den Schutz des Arbeitsblatts. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addAutoFilter(int row, int startColumn, int endColumn) {#addAutoFilter-int-int-int-}
```
public void addAutoFilter(int row, int startColumn, int endColumn)
```


Legt den Bereich fest, auf den der angegebene AutoFilter angewendet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex. |
| startColumn | int | Startspaltenindex. |
| endColumn | int | Endspaltenindex. |

### addCustomFilter(int row, String critira) {#addCustomFilter-int-java.lang.String-}
```
public void addCustomFilter(int row, String critira)
```


Füge benutzerdefinierten Filter für die angegebene Zeile hinzu.

**Remarks**

Der Filterkriterien-String. Hinweis: Wir verwenden , und ; als Trennzeichen, daher darf der Zellenwert diese Trennzeichen nicht enthalten. Nachfolgend Beispiele für Kriterien-Strings //column 0 with value 12.3 CELL0 = 12.3 //column 1 with value ABC CELL1 = ABC //column 0 with value 123 or 456 or ABC and column 1 with value ABC CELL0 = 123,456,ABC; CELL1 = ABC

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int |  |
| Kriterium | java.lang.String |  |

### autoFitColumn(int columnIndex) {#autoFitColumn-int-}
```
public void autoFitColumn(int columnIndex)
```


Passt die Spaltenbreite automatisch an.

**Remarks**

AutoFitColumn ist eine ungenaue Funktion.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnIndex | int | Spaltenindex. |

### autoFitColumn(int columnIndex, int firstRow, int lastRow) {#autoFitColumn-int-int-int-}
```
public void autoFitColumn(int columnIndex, int firstRow, int lastRow)
```


Passt die Spaltenbreite automatisch an.

**Remarks**

Diese Methode passt die Zeile automatisch an den Inhalt eines Zellbereichs in der Zeile an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnIndex | int | Spaltenindex. |
| firstRow | int | Erster Zeilenindex. |
| lastRow | int | Letzter Zeilenindex. |

### autoFitColumns() {#autoFitColumns--}
```
public void autoFitColumns()
```




### autoFitRow(int rowIndex) {#autoFitRow-int-}
```
public void autoFitRow(int rowIndex)
```


Passt die Zeilenhöhe automatisch an.

**Remarks**

AutoFitRow ist eine ungenaue Funktion.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowIndex | int | Zeilenindex. |

### autoFitRow(int rowIndex, int firstColumn, int lastColumn) {#autoFitRow-int-int-int-}
```
public void autoFitRow(int rowIndex, int firstColumn, int lastColumn)
```


Passt die Zeilenhöhe automatisch an.

**Remarks**

Diese Methode passt die Zeile automatisch an den Inhalt eines Zellbereichs in der Zeile an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowIndex | int | Zeilenindex. |
| firstColumn | int | Erster Spaltenindex. |
| lastColumn | int | Letzter Spaltenindex. |

### autoFitRow(int startRow, int endRow, int startColumn, int endColumn) {#autoFitRow-int-int-int-int-}
```
public void autoFitRow(int startRow, int endRow, int startColumn, int endColumn)
```


Passt die Zeilenhöhe in einem rechteckigen Bereich automatisch an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | int | Startzeilenindex. |
| endRow | int | Endzeilenindex. |
| startColumn | int | Startspaltenindex. |
| endColumn | int | Endspaltenindex. |

### autoFitRows() {#autoFitRows--}
```
public void autoFitRows()
```


Passt alle Zeilen in diesem Arbeitsblatt automatisch an.

### autoFitRows(boolean onlyAuto) {#autoFitRows-boolean-}
```
public void autoFitRows(boolean onlyAuto)
```


Passt alle Zeilen in diesem Arbeitsblatt automatisch an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| onlyAuto | boolean | True, passt die Zeilenhöhe nur automatisch an, wenn die Zeilenhöhe nicht benutzerdefiniert ist. |

### autoFitRows(int startRow, int endRow) {#autoFitRows-int-int-}
```
public void autoFitRows(int startRow, int endRow)
```


Passt die Zeilenhöhe in einem Bereich automatisch an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | int | Startzeilenindex. |
| endRow | int | Endzeilenindex. |

### calculateFormula(String formula) {#calculateFormula-java.lang.String-}
```
public Object calculateFormula(String formula)
```


Berechnet eine Formel.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| formula | java.lang.String |  |

**Returns:**
java.lang.Object -
### clearComments() {#clearComments--}
```
public void clearComments()
```


Löscht alle Kommentare im Designer-Tabellenblatt.

### copy(GridWorksheet sourceSheet) {#copy-com.aspose.gridweb.GridWorksheet-}
```
public void copy(GridWorksheet sourceSheet)
```


Kopiert Inhalte und Formate von einem anderen Arbeitsblatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceSheet | [GridWorksheet](../../com.aspose.gridweb/gridworksheet) | Quellarbeitsblatt. |

### createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList) {#createSubtotal-int-int-int-int-int---}
```
public void createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList)
```


Erstellt Zwischensumme im Blatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnNameRowIndex | int | Der Zeilenindex der Spaltennamenzeile. |
| dataRows | int | Die Anzahl der Datenzeilen. |
| groupByColumnIndex | int | Der Spaltenindex der zu gruppierenden Spalte. |
| subtotalFunction | int | [SubtotalFunction](../../com.aspose.gridweb/subtotalfunction). Der Typ der Zwischensumme-Funktion. |
| subtotalColumnIndexList | int[] | Die Spaltenindizes, die zusammengefasst werden sollen. |

### createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString) {#createSubtotal-int-int-int-int-int---java.lang.String-com.aspose.gridweb.GridTableItemStyle-com.aspose.gridweb.GridTableItemStyle-int-java.lang.String-}
```
public void createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString)
```


Erstellt Zwischensumme im Blatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnNameRowIndex | int | Der Zeilenindex der Spaltennamenzeile. |
| dataRows | int | Die Anzahl der Datenzeilen. |
| groupByColumnIndex | int | Der Spaltenindex der zu gruppierenden Spalte. |
| subtotalFunction | int | [SubtotalFunction](../../com.aspose.gridweb/subtotalfunction). Der Typ der Zwischensumme-Funktion. |
| subtotalColumnIndexList | int[] | Die Spaltenindizes, die zusammengefasst werden sollen. |
| functionLabel | java.lang.String | Die Bezeichnung der Zwischensumme-Funktion. |
| grandCellStyle | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | Der Stil der Gesamtsummenzeile. |
| subtotalCellStyle | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | Der Stil der Zwischensummenzeile. |
| numberType | int | [NumberType](../../com.aspose.gridweb/numbertype). Der Zahlentyp der Zwischensummen-Ergebniszellen. |
| customString | java.lang.String | Der benutzerdefinierte Formatstring der Zwischensummen-Ergebniszellen. Kann null sein. |

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
### filterString(int column, String criteria) {#filterString-int-java.lang.String-}
```
public void filterString(int column, String criteria)
```


Setzt den Filter für die Spalte. Hinweis: Wir sollten AddAutoFilter aufrufen, bevor filterString verwendet wird. Der Filterkriterien-String. Hinweis: Wir verwenden das Komma -> \",\" als Trennzeichen, daher darf der zu filternde Zellenwert kein Komma enthalten. filterString(10,\"123,456\") bedeutet, Spalte 10 soll 123 oder 456 enthalten, filterString(10,\"123\") bedeutet, Spalte 10 soll 123 enthalten, der Spaltenindexwert wird durch Komma getrennt, z.B. 123,456,789 oder abc

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Spalte | int |  |
| criteria | java.lang.String |  |

### freezePanes(int row, int column, int freezedRows, int freezedColumns) {#freezePanes-int-int-int-int-}
```
public void freezePanes(int row, int column, int freezedRows, int freezedColumns)
```


Friert Bereiche an der angegebenen Zelle im Arbeitsblatt ein.

**Remarks**

Zeilenindex und Spaltenindex können nicht beide Null sein. Die Anzahl der Zeilen und die Anzahl der Spalten können ebenfalls nicht beide Null sein.

Die ersten beiden Parameter geben die eingefrorene Position an und die letzten beiden Parameter geben den eingefrorenen Bereich im linken oberen Bereich an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex. |
| Spalte | int | Spaltenindex. |
| freezedRows | int | Anzahl der sichtbaren Zeilen im oberen Bereich, nicht mehr als Zeilenindex. |
| freezedColumns | int | Anzahl der sichtbaren Spalten im linken Bereich, nicht mehr als Spaltenindex. |

### freezePanes(String cellName, int freezedRows, int freezedColumns) {#freezePanes-java.lang.String-int-int-}
```
public void freezePanes(String cellName, int freezedRows, int freezedColumns)
```


Friert Bereiche an der angegebenen Zelle im Arbeitsblatt ein.

**Remarks**

Zeilenindex und Spaltenindex können nicht beide Null sein. Die Anzahl der Zeilen und die Anzahl der Spalten können ebenfalls nicht beide Null sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellName | java.lang.String | Zellenname. |
| freezedRows | int | Anzahl der sichtbaren Zeilen im oberen Bereich, nicht mehr als Zeilenindex. |
| freezedColumns | int | Anzahl der sichtbaren Spalten im linken Bereich, nicht mehr als Spaltenindex. |

### getActiveCell() {#getActiveCell--}
```
public String getActiveCell()
```


Ermittelt die aktive Zelle im Arbeitsblatt.

**Returns:**
java.lang.String
### getBackgroundImage() {#getBackgroundImage--}
```
public byte[] getBackgroundImage()
```


Liefert das Hintergrundbild des Arbeitsblatts.

**Returns:**
byte[]
### getCells() {#getCells--}
```
public GridCells getCells()
```


Ruft die [GridCell](../../com.aspose.gridweb/gridcell)-Sammlung ab.

**Returns:**
[GridCells](../../com.aspose.gridweb/gridcells)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCodeName() {#getCodeName--}
```
public String getCodeName()
```


Stellt den Code-Namen des Arbeitsblatts dar.

**Remarks**

Sie können den Codenamen nicht ändern, solange die Vorlagendatei VBA/Makros enthält.

**Returns:**
java.lang.String
### getColumnCaption(int column) {#getColumnCaption-int-}
```
public String getColumnCaption(int column)
```


Liefert die Spaltenbeschriftung. Wenn die Beschriftung nicht gesetzt ist, wird ein leerer String zurückgegeben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Spalte | int | Spaltenindex. |

**Returns:**
java.lang.String - Die Spaltenbeschriftung. Wenn die Beschriftung nicht gesetzt ist, wird ein leerer String zurückgegeben.
### getColumnHeaderToolTip(int colIndex) {#getColumnHeaderToolTip-int-}
```
public String getColumnHeaderToolTip(int colIndex)
```


Ruft den Tooltip-Text des Spaltenkopfes ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| colIndex | int | Der Index der Spalte. |

**Returns:**
java.lang.String - Der Tooltip-Text.
### getColumnReadonly(int columnIndex) {#getColumnReadonly-int-}
```
public boolean getColumnReadonly(int columnIndex)
```


Ermittelt, ob eine Spalte schreibgeschützt ist. Dies ist eine erweiterte Methode von GridWeb speziell, sie wird nicht im tatsächlichen Excel‑Datei beibehalten oder wirksam.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnIndex | int | Spaltenindex. |

**Returns:**
boolean - Gibt true zurück, wenn schreibgeschützt.
### getComments() {#getComments--}
```
public GridCommentCollection getComments()
```


Ruft die [GridComment](../../com.aspose.gridweb/gridcomment)-Sammlung ab.

**Returns:**
[GridCommentCollection](../../com.aspose.gridweb/gridcommentcollection)
### getDisplayRightToLeft() {#getDisplayRightToLeft--}
```
public boolean getDisplayRightToLeft()
```


Gibt an, ob das angegebene Arbeitsblatt von rechts nach links statt von links nach rechts angezeigt wird. Standard ist false.

**Returns:**
boolean
### getDisplayZeros() {#getDisplayZeros--}
```
public boolean getDisplayZeros()
```


Wahr, wenn Nullwerte angezeigt werden.

**Returns:**
boolean
### getFirstVisibleColumn() {#getFirstVisibleColumn--}
```
public int getFirstVisibleColumn()
```


Stellt den Index der ersten sichtbaren Spalte dar.

**Returns:**
int
### getFirstVisibleRow() {#getFirstVisibleRow--}
```
public int getFirstVisibleRow()
```


Stellt den Index der ersten sichtbaren Zeile dar.

**Returns:**
int
### getFreezedPanes() {#getFreezedPanes--}
```
public int[] getFreezedPanes()
```


Liefert die Freeze‑Panes.

**Returns:**
int[] - Rückgabe null bedeutet, dass das Arbeitsblatt nicht eingefroren ist 0:Zeilenindex;1:Spalte;2:freezedRows;3:freezedRows
### getGridActiveCell() {#getGridActiveCell--}
```
public GridCell getGridActiveCell()
```


Ermittelt die aktive Zelle im Arbeitsblatt.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getHyperlinks() {#getHyperlinks--}
```
public GridHyperlinkCollection getHyperlinks()
```


Ruft die [GridHyperlinkCollection](../../com.aspose.gridweb/gridhyperlinkcollection)-Sammlung ab.

**Returns:**
[GridHyperlinkCollection](../../com.aspose.gridweb/gridhyperlinkcollection)
### getIndex() {#getIndex--}
```
public int getIndex()
```


Liefert den Index des Blatts in der Arbeitsblatt‑Sammlung.

**Returns:**
int
### getIsReadonly(int row, int col) {#getIsReadonly-int-int-}
```
public boolean getIsReadonly(int row, int col)
```


Ruft ab, ob die Zelle schreibgeschützt ist. Dies ist ein erweitertes Attribut von GridWeb, das nicht in der tatsächlichen Excel-Datei erhalten bleibt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int |  |
| Spalte | int |  |

**Returns:**
boolean
### getName() {#getName--}
```
public String getName()
```


Liefert den Namen des Arbeitsblatts.

**Remarks**

Die maximale Länge eines Blattnamens beträgt 31 Zeichen. Und Sie können nicht denselben Namen (Groß-/Kleinschreibung ignorierend) zwei Arbeitsblättern zuweisen. Zum Beispiel können Sie nicht "SheetName1" dem ersten Arbeitsblatt zuweisen und "SHEETNAME1" dem zweiten Arbeitsblatt.

**Returns:**
java.lang.String
### getOutlineShown() {#getOutlineShown--}
```
public boolean getOutlineShown()
```


Gibt an, ob die Gliederung angezeigt wird.

**Returns:**
boolean
### getPictures() {#getPictures--}
```
public GridPictureCollection getPictures()
```


Ruft eine [getPictures()](../../com.aspose.gridweb/gridworksheet\#getPictures--)‑Sammlung ab.

**Returns:**
[GridPictureCollection](../../com.aspose.gridweb/gridpicturecollection)
### getPivotTables() {#getPivotTables--}
```
public GridPivotTableCollection getPivotTables()
```


Ruft die PivotTables im Arbeitsblatt ab.

**Returns:**
[GridPivotTableCollection](../../com.aspose.gridweb/gridpivottablecollection)
### getRowCaption(int row) {#getRowCaption-int-}
```
public String getRowCaption(int row)
```


Liefert die Zeilenbeschriftung. Wenn die Beschriftung nicht gesetzt ist, wird ein leerer String zurückgegeben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex. |

**Returns:**
java.lang.String - Die Zeilenbeschriftung. Wenn die Beschriftung nicht gesetzt ist, wird ein leerer String zurückgegeben.
### getRowHeaderToolTip(int rowIndex) {#getRowHeaderToolTip-int-}
```
public String getRowHeaderToolTip(int rowIndex)
```


Ruft den Tooltip-Text des Zeilenkopfes ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowIndex | int | Der Index der Zeile. |

**Returns:**
java.lang.String - Der Tooltip-Text.
### getRowReadonly(int rowIndex) {#getRowReadonly-int-}
```
public boolean getRowReadonly(int rowIndex)
```


Ermittelt, ob eine Zeile schreibgeschützt ist. Dies ist eine erweiterte Methode von GridWeb speziell, sie wird nicht im tatsächlichen Excel‑Datei beibehalten oder wirksam.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowIndex | int | Zeilenindex. |

**Returns:**
boolean - Gibt true zurück, wenn schreibgeschützt.
### getSelected() {#getSelected--}
```
public boolean getSelected()
```


Gibt an, ob dieses Arbeitsblatt beim Öffnen der Arbeitsmappe ausgewählt ist.

**Returns:**
boolean
### getShapes() {#getShapes--}
```
public GridShapeCollection getShapes()
```


Ruft eine [getPictures()](../../com.aspose.gridweb/gridworksheet\#getPictures--)‑Sammlung ab.

**Returns:**
[GridShapeCollection](../../com.aspose.gridweb/gridshapecollection)
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
### getTabColor() {#getTabColor--}
```
public Color getTabColor()
```


Stellt die Registerkartenfarbe des Arbeitsblatts dar.

**Remarks**

Diese Funktion wird nur in ExcelXP (Excel2002) und neueren Versionen unterstützt. Wenn Sie die Datei im Excel97- oder Excel2000-Format speichern, wird sie weggelassen.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getUniqueID() {#getUniqueID--}
```
public String getUniqueID()
```


Ruft die UniqueID im Steuerelement ab.

**Returns:**
java.lang.String
### getValidations() {#getValidations--}
```
public GridValidationCollection getValidations()
```


Ruft die Datengültigkeits‑Einstellungs‑Sammlung im Arbeitsblatt ab.

**Returns:**
[GridValidationCollection](../../com.aspose.gridweb/gridvalidationcollection)
### getVisible() {#getVisible--}
```
public boolean getVisible()
```


Gibt an, ob der Name dieses Blatts in den Blattregisterkarten des Steuerelements angezeigt wird.

**Returns:**
boolean
### getWorkbook() {#getWorkbook--}
```
public GridWorkbook getWorkbook()
```


Ruft das [GridWorkbook](../../com.aspose.gridweb/gridworkbook)-Objekt der Arbeitsblattsammlung ab.

**Returns:**
[GridWorkbook](../../com.aspose.gridweb/gridworkbook)
### getZoom() {#getZoom--}
```
public int getZoom()
```


Stellt den Skalierungsfaktor in Prozent dar. Er sollte zwischen 10 und 400 liegen.

**Returns:**
int
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
### isGridlinesVisible() {#isGridlinesVisible--}
```
public boolean isGridlinesVisible()
```


Ruft einen Wert ab, der angibt, ob die Gitternetzlinien sichtbar sind. Standard ist true.

**Returns:**
boolean
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


Gibt an, ob das Arbeitsblatt geschützt ist.

**Returns:**
boolean
### isSummaryRowBelow() {#isSummaryRowBelow--}
```
public boolean isSummaryRowBelow()
```


Gibt an, ob die Zusammenfassungszeile unter den Detailzeilen in der Gliederung positioniert wird.

**Returns:**
boolean
### moveTo(int index) {#moveTo-int-}
```
public void moveTo(int index)
```


Verschiebt das Blatt an eine andere Position in der Tabelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Index des Zielblatts. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refreshFilter() {#refreshFilter--}
```
public void refreshFilter()
```


Aktualisiert Autofilter, um Zeilen auszublenden oder einzublenden.

### removeAutoFilter() {#removeAutoFilter--}
```
public void removeAutoFilter()
```


Entfernt den AutoFilter des Arbeitsblatts.

### removeSubtotal() {#removeSubtotal--}
```
public void removeSubtotal()
```


Entfernt die durch die Methode CreateSubtotal im Blatt erstellte Zwischensumme.

### resetFilter(int fieldIndex) {#resetFilter-int-}
```
public void resetFilter(int fieldIndex)
```


Der ganzzahlige Versatz des Feldes, auf das Sie anwenden möchten, basierend auf der ersten Filterspalte (von links in der Liste; das linkeste Feld ist Feld 0).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldIndex | int |  |

### setActiveCell(String value) {#setActiveCell-java.lang.String-}
```
public void setActiveCell(String value)
```


Setzt die aktive Zelle im Arbeitsblatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setAllCellsEditable() {#setAllCellsEditable--}
```
public void setAllCellsEditable()
```


Macht alle Zellen editierbar. Dies ist ein erweitertes Attribut.

### setAllCellsReadonly() {#setAllCellsReadonly--}
```
public void setAllCellsReadonly()
```


Macht alle Zellen schreibgeschützt. Dies ist ein erweitertes Attribut; beachten Sie, dass dieses Attribut nicht in der tatsächlichen Zelle erhalten bleibt. Wenn Sie den Schutz beibehalten möchten, verwenden Sie bitte setProtect.

### setBackgroundImage(byte[] value) {#setBackgroundImage-byte---}
```
public void setBackgroundImage(byte[] value)
```


Setzt das Hintergrundbild des Arbeitsblatts.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | byte[] |  |

### setColumnCaption(int column, String caption) {#setColumnCaption-int-java.lang.String-}
```
public void setColumnCaption(int column, String caption)
```


Setzt die Beschriftung für die Spalte. Bitte beachten Sie, dass dies ein Erweiterungsattribut ist und nicht in der Excel-Datei erhalten bleibt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Spalte | int | Spaltenindex. |
| caption | java.lang.String | Die Spaltenbeschriftung. Übergeben Sie null oder einen leeren String, wenn Sie die Beschriftung entfernen möchten. |

### setColumnHeaderToolTip(int colIndex, String toolTip) {#setColumnHeaderToolTip-int-java.lang.String-}
```
public void setColumnHeaderToolTip(int colIndex, String toolTip)
```


Setzt den Tooltip-Text des Spaltenkopfes.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| colIndex | int | Der Index der Spalte. |
| toolTip | java.lang.String | Der Tooltip-Text. |

### setColumnReadonly(int columnIndex, boolean isReadonly) {#setColumnReadonly-int-boolean-}
```
public void setColumnReadonly(int columnIndex, boolean isReadonly)
```


Setzt eine Spalte auf schreibgeschützt, sodass der Benutzer sie clientseitig nicht löschen kann. Dies ist eine erweiterte Methode von GridWeb speziell, sie wird nicht im tatsächlichen Excel‑Datei beibehalten oder wirksam.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnIndex | int | Spaltenindex. |
| isReadonly | boolean | true oder false. |

### setDisplayRightToLeft(boolean value) {#setDisplayRightToLeft-boolean-}
```
public void setDisplayRightToLeft(boolean value)
```


Gibt an, ob das angegebene Arbeitsblatt von rechts nach links statt von links nach rechts angezeigt wird. Standard ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setDisplayZeros(boolean value) {#setDisplayZeros-boolean-}
```
public void setDisplayZeros(boolean value)
```


Wahr, wenn Nullwerte angezeigt werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setEditableRange(int startRow, int startColumn, int rows, int columns) {#setEditableRange-int-int-int-int-}
```
public void setEditableRange(int startRow, int startColumn, int rows, int columns)
```


Macht einen Zellbereich editierbar. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Macht alle Zellen schreibgeschützt, indem die Methode SetAllCellsReadonly aufgerufen wird. Rufen Sie dann diese Methode auf, um den Bereich der Zellen anzugeben, die editierbar sein sollen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | int | Die Startzeile des Bereichs. |
| startColumn | int | Die Startspalte des Bereichs. |
| rows | int | Die Anzahl der Zeilen. |
| Spalten | int | Die Anzahl der Spalten. |

### setFirstVisibleColumn(int value) {#setFirstVisibleColumn-int-}
```
public void setFirstVisibleColumn(int value)
```


Stellt den Index der ersten sichtbaren Spalte dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setFirstVisibleRow(int value) {#setFirstVisibleRow-int-}
```
public void setFirstVisibleRow(int value)
```


Stellt den Index der ersten sichtbaren Zeile dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setGridActiveCell(GridCell value) {#setGridActiveCell-com.aspose.gridweb.GridCell-}
```
public void setGridActiveCell(GridCell value)
```


Setzt die aktive Zelle im Arbeitsblatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [GridCell](../../com.aspose.gridweb/gridcell) |  |

### setGridlinesVisible(boolean value) {#setGridlinesVisible-boolean-}
```
public void setGridlinesVisible(boolean value)
```


Setzt einen Wert, der angibt, ob die Gitternetzlinien sichtbar sind. Standard ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setIsReadonly(int row, int col, boolean value) {#setIsReadonly-int-int-boolean-}
```
public void setIsReadonly(int row, int col, boolean value)
```


Legt fest, ob die Zelle schreibgeschützt ist. Dies ist ein erweitertes Attribut von GridWeb, das nicht in der tatsächlichen Excel-Datei gespeichert wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int |  |
| Spalte | int |  |
| Wert | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Legt den Namen des Arbeitsblatts fest.

**Remarks**

Die maximale Länge eines Blattnamens beträgt 31 Zeichen. Und Sie können nicht denselben Namen (Groß-/Kleinschreibung ignorierend) zwei Arbeitsblättern zuweisen. Zum Beispiel können Sie nicht "SheetName1" dem ersten Arbeitsblatt zuweisen und "SHEETNAME1" dem zweiten Arbeitsblatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setOutlineShown(boolean value) {#setOutlineShown-boolean-}
```
public void setOutlineShown(boolean value)
```


Gibt an, ob die Gliederung angezeigt wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setProtect() {#setProtect--}
```
public void setProtect()
```


Schützt das Arbeitsblatt.

**Remarks**

Diese Methode schützt das Arbeitsblatt ohne Passwort. Sie kann das Arbeitsblatt in allen Excel-Dateiversionen schützen.

### setReadonlyRange(int startRow, int startColumn, int rows, int columns) {#setReadonlyRange-int-int-int-int-}
```
public void setReadonlyRange(int startRow, int startColumn, int rows, int columns)
```


Macht einen Zellbereich schreibgeschützt. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Zuerst alle Zellen editierbar machen, indem die Methode SetAllCellsEditable aufgerufen wird. Dann diese Methode aufrufen, um den Bereich von Zellen anzugeben, der schreibgeschützt sein soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | int | Die Startzeile des Bereichs. |
| startColumn | int | Die Startspalte des Bereichs. |
| rows | int | Die Anzahl der Zeilen. |
| Spalten | int | Die Anzahl der Spalten. |

### setRowCaption(int row, String caption) {#setRowCaption-int-java.lang.String-}
```
public void setRowCaption(int row, String caption)
```


Setzt die Beschriftung für die Zeile.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex. |
| caption | java.lang.String | Die Zeilenbeschriftung. Übergeben Sie null oder einen leeren String, wenn Sie die Beschriftung abbrechen möchten. |

### setRowHeaderToolTip(int rowIndex, String toolTip) {#setRowHeaderToolTip-int-java.lang.String-}
```
public void setRowHeaderToolTip(int rowIndex, String toolTip)
```


Setzt den Tooltip-Text der Zeilenüberschrift.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowIndex | int | Der Index der Zeile. |
| toolTip | java.lang.String | Der Tooltip-Text. |

### setRowReadonly(int rowIndex, boolean isReadonly) {#setRowReadonly-int-boolean-}
```
public void setRowReadonly(int rowIndex, boolean isReadonly)
```


Setzt eine Zeile auf schreibgeschützt, sodass der Benutzer sie nicht von der Clientseite löschen kann. Dies ist eine erweiterte Methode von GridWeb speziell; sie wird nicht beibehalten und wirkt sich nicht auf die tatsächliche Excel-Datei aus.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowIndex | int | Zeilenindex. |
| isReadonly | boolean | true oder false. |

### setSelected(boolean value) {#setSelected-boolean-}
```
public void setSelected(boolean value)
```


Gibt an, ob dieses Arbeitsblatt beim Öffnen der Arbeitsmappe ausgewählt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

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

### setSummaryRowBelow(boolean value) {#setSummaryRowBelow-boolean-}
```
public void setSummaryRowBelow(boolean value)
```


Gibt an, ob die Zusammenfassungszeile unter den Detailzeilen in der Gliederung positioniert wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setTabColor(Color value) {#setTabColor-com.aspose.gridweb.Color-}
```
public void setTabColor(Color value)
```


Stellt die Registerkartenfarbe des Arbeitsblatts dar.

**Remarks**

Diese Funktion wird nur in ExcelXP (Excel2002) und neueren Versionen unterstützt. Wenn Sie die Datei im Excel97- oder Excel2000-Format speichern, wird sie weggelassen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Gibt an, ob der Name dieses Blatts in den Blattregisterkarten des Steuerelements angezeigt wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setZoom(int value) {#setZoom-int-}
```
public void setZoom(int value)
```


Stellt den Skalierungsfaktor in Prozent dar. Er sollte zwischen 10 und 400 liegen.

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
### unFreezePanes() {#unFreezePanes--}
```
public void unFreezePanes()
```


Löst das Einfrieren von Bereichen im Arbeitsblatt.

### unGroupRows(int firstIndex, int lastIndex) {#unGroupRows-int-int-}
```
public void unGroupRows(int firstIndex, int lastIndex)
```


Hebt die Gruppierung von Zeilen auf.

**Remarks**

Entfernt nur äußere Gruppeninformationen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstIndex | int | Der Index der ersten Zeile, die aufgelöst werden soll. |
| lastIndex | int | Der Index der letzten Zeile, die aufgelöst werden soll. |

### unProtect() {#unProtect--}
```
public void unProtect()
```


Entfernt den Schutz des Arbeitsblatts.

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

