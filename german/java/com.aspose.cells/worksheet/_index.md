---
title: "Arbeitsblatt"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Kapselt das Objekt, das ein einzelnes Arbeitsblatt darstellt."
type: docs
url: /de/java/com.aspose.cells/worksheet/
---

**Inheritance:**
java.lang.Object
```
public class Worksheet
```

Kapselt das Objekt, das ein einzelnes Arbeitsblatt darstellt.

**Example**

Das folgende Beispiel zeigt, wie man Bereiche einfriert und einen Hyperlink zum Arbeitsblatt mit .Net oder VB einfügt.

```
         Workbook workbook = new Workbook();
 
         Worksheet sheet = workbook.getWorksheets().get(0);
 
         //Freeze panes at "AS40" with 10 rows and 10 columns
         sheet.freezePanes("AS40", 10, 10);
 
         //Add a hyperlink in Cell A1
         sheet.getHyperlinks().add("A1", 1, 1, "http://www.aspose.com");
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [addPageBreaks(String cellName)](#addPageBreaks-java.lang.String-) | Fügt einen Seitenumbruch hinzu. |
| [advancedFilter(boolean isFilter, String listRange, String criteriaRange, String copyTo, boolean uniqueRecordOnly)](#advancedFilter-boolean-java.lang.String-java.lang.String-java.lang.String-boolean-) | Filtert Daten mithilfe komplexer Kriterien. |
| [autoFitColumn(int columnIndex)](#autoFitColumn-int-) | Passt die Spaltenbreite automatisch an. |
| [autoFitColumn(int columnIndex, int firstRow, int lastRow)](#autoFitColumn-int-int-int-) | Passt die Spaltenbreite automatisch an. |
| [autoFitColumns()](#autoFitColumns--) | Passt alle Spalten in diesem Arbeitsblatt automatisch an. |
| [autoFitColumns(AutoFitterOptions options)](#autoFitColumns-com.aspose.cells.AutoFitterOptions-) | Passt alle Spalten in diesem Arbeitsblatt automatisch an. |
| [autoFitColumns(int firstColumn, int lastColumn)](#autoFitColumns-int-int-) | Passt die Spaltenbreite automatisch an. |
| [autoFitColumns(int firstColumn, int lastColumn, AutoFitterOptions options)](#autoFitColumns-int-int-com.aspose.cells.AutoFitterOptions-) | Passt die Spaltenbreite automatisch an. |
| [autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn)](#autoFitColumns-int-int-int-int-) | Passt die Spaltenbreite automatisch an. |
| [autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn, AutoFitterOptions options)](#autoFitColumns-int-int-int-int-com.aspose.cells.AutoFitterOptions-) | Passt die Spaltenbreite automatisch an. |
| [autoFitRow(int rowIndex)](#autoFitRow-int-) | Passt die Zeilenhöhe automatisch an. |
| [autoFitRow(int rowIndex, int firstColumn, int lastColumn)](#autoFitRow-int-int-int-) | Passt die Zeilenhöhe automatisch an. |
| [autoFitRow(int rowIndex, int firstColumn, int lastColumn, AutoFitterOptions options)](#autoFitRow-int-int-int-com.aspose.cells.AutoFitterOptions-) | Passt die Zeilenhöhe automatisch an. |
| [autoFitRow(int startRow, int endRow, int startColumn, int endColumn)](#autoFitRow-int-int-int-int-) | Passt die Zeilenhöhe in einem rechteckigen Bereich automatisch an. |
| [autoFitRows()](#autoFitRows--) | Passt alle Zeilen in diesem Arbeitsblatt automatisch an. |
| [autoFitRows(boolean onlyAuto)](#autoFitRows-boolean-) | Passt alle Zeilen in diesem Arbeitsblatt automatisch an. |
| [autoFitRows(AutoFitterOptions options)](#autoFitRows-com.aspose.cells.AutoFitterOptions-) | Passt alle Zeilen in diesem Arbeitsblatt automatisch an. |
| [autoFitRows(int startRow, int endRow)](#autoFitRows-int-int-) | Passt die Zeilenhöhe in einem Bereich automatisch an. |
| [autoFitRows(int startRow, int endRow, AutoFitterOptions options)](#autoFitRows-int-int-com.aspose.cells.AutoFitterOptions-) | Passt die Zeilenhöhe in einem Bereich automatisch an. |
| [calculateArrayFormula(String formula, CalculationOptions opts)](#calculateArrayFormula-java.lang.String-com.aspose.cells.CalculationOptions-) | Berechnet eine Formel als Array-Formel. |
| [calculateArrayFormula(String formula, CalculationOptions opts, int maxRowCount, int maxColumnCount)](#calculateArrayFormula-java.lang.String-com.aspose.cells.CalculationOptions-int-int-) | Berechnet eine Formel als Array-Formel. |
| [calculateArrayFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, int maxRowCount, int maxColumnCount, CalculationData calculationData)](#calculateArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-com.aspose.cells.CalculationOptions-int-int-int-int-com.aspose.cells.CalculationData-) | Berechnet eine Formel als Array-Formel. |
| [calculateFormula(CalculationOptions options, boolean recursive)](#calculateFormula-com.aspose.cells.CalculationOptions-boolean-) | Berechnet alle Formeln in diesem Arbeitsblatt. |
| [calculateFormula(String formula)](#calculateFormula-java.lang.String-) | Berechnet eine Formel. |
| [calculateFormula(String formula, CalculationOptions opts)](#calculateFormula-java.lang.String-com.aspose.cells.CalculationOptions-) | Berechnet einen Formelausdruck direkt. |
| [calculateFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, CalculationData calculationData)](#calculateFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-com.aspose.cells.CalculationOptions-int-int-com.aspose.cells.CalculationData-) | Berechnet einen Formelausdruck direkt. |
| [clearComments()](#clearComments--) | Löscht alle Kommentare im Designer-Tabellenblatt. |
| [closeAccessCache(int opts)](#closeAccessCache-int-) | Schließt die Sitzung, die Caches verwendet, um auf die Daten in diesem Arbeitsblatt zuzugreifen. |
| [convertFormulaReferenceStyle(String formula, boolean toR1C1, int baseCellRow, int baseCellColumn)](#convertFormulaReferenceStyle-java.lang.String-boolean-int-int-) | Konvertiert den Formel-Referenzstil. |
| [copy(Worksheet sourceSheet)](#copy-com.aspose.cells.Worksheet-) | Kopiert Inhalte und Formate von einem anderen Arbeitsblatt. |
| [copy(Worksheet sourceSheet, CopyOptions copyOptions)](#copy-com.aspose.cells.Worksheet-com.aspose.cells.CopyOptions-) | Kopiert Inhalte und Formate von einem anderen Arbeitsblatt. |
| [dispose()](#dispose--) | Führt anwendungsspezifische Aufgaben aus, die mit dem Freigeben, Freisetzen oder Zurücksetzen nicht verwalteter Ressourcen verbunden sind. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filter(CellArea ca)](#filter-com.aspose.cells.CellArea-) | Filtert den Bereich. |
| [freezePanes(int row, int column, int freezedRows, int freezedColumns)](#freezePanes-int-int-int-int-) | Friert Bereiche an der angegebenen Zelle im Arbeitsblatt ein. |
| [freezePanes(String cellName, int freezedRows, int freezedColumns)](#freezePanes-java.lang.String-int-int-) | Friert Bereiche an der angegebenen Zelle im Arbeitsblatt ein. |
| [getActiveCell()](#getActiveCell--) | Ermittelt die aktive Zelle im Arbeitsblatt. |
| [getAdvancedFilter()](#getAdvancedFilter--) | Ermittelt die Einstellungen des erweiterten Filters. |
| [getAllPictures()](#getAllPictures--) | Ermittelt alle Bilder, einschließlich der in der Zelle eingebetteten und über den Zellen liegenden Bilder. |
| [getAllowEditRanges()](#getAllowEditRanges--) | Ermittelt die Sammlung zulässiger Bearbeitungsbereiche im Arbeitsblatt. |
| [getAreasOfXmlMapQuery(String path, XmlMap xmlMap)](#getAreasOfXmlMapQuery-java.lang.String-com.aspose.cells.XmlMap-) | Abfrage von Zellbereichen, die mit dem spezifischen Pfad der XML‑Map verknüpft/verbunden sind. |
| [getAutoFilter()](#getAutoFilter--) | Stellt den AutoFilter für das angegebene Arbeitsblatt dar. |
| [getBackgroundImage()](#getBackgroundImage--) | Liefert das Hintergrundbild des Arbeitsblatts. |
| [getCellWatches()](#getCellWatches--) | Liefert die Sammlung von Zellen dieses Arbeitsblatts, die im „Watch‑Fenster“ überwacht werden. |
| [getCells()](#getCells--) | Liefert die [Cells](../../com.aspose.cells/cells)-Sammlung. |
| [getCharts()](#getCharts--) | Liefert eine [Chart](../../com.aspose.cells/chart)-Sammlung |
| [getCheckBoxes()](#getCheckBoxes--) | Liefert eine [CheckBox](../../com.aspose.cells/checkbox)-Sammlung. |
| [getClass()](#getClass--) |  |
| [getCodeName()](#getCodeName--) | Liefert den Code‑Namen des Arbeitsblatts. |
| [getComments()](#getComments--) | Liefert die [Comment](../../com.aspose.cells/comment)-Sammlung. |
| [getConditionalFormattings()](#getConditionalFormattings--) | Liefert die ConditionalFormattings im Arbeitsblatt. |
| [getCustomProperties()](#getCustomProperties--) | Liefert ein Objekt, das die Kennzeichnungsinformationen eines Arbeitsblatts darstellt. |
| [getDisplayRightToLeft()](#getDisplayRightToLeft--) | Gibt an, ob das angegebene Arbeitsblatt von rechts nach links statt von links nach rechts angezeigt wird. |
| [getDisplayZeros()](#getDisplayZeros--) | Wahr, wenn Nullwerte angezeigt werden. |
| [getErrorCheckOptions()](#getErrorCheckOptions--) | Liefert die Fehlerprüfungs‑Einstellung, die auf bestimmte Bereiche angewendet wird. |
| [getFirstVisibleColumn()](#getFirstVisibleColumn--) | Stellt den Index der ersten sichtbaren Spalte dar. |
| [getFirstVisibleRow()](#getFirstVisibleRow--) | Stellt den Index der ersten sichtbaren Zeile dar. |
| [getFreezedPanes()](#getFreezedPanes--) | Liefert die Freeze‑Panes. |
| [getGridlineColor()](#getGridlineColor--) | Liefert die Farbe der Rasterlinien |
| [getHorizontalPageBreaks()](#getHorizontalPageBreaks--) | Liefert die [HorizontalPageBreakCollection](../../com.aspose.cells/horizontalpagebreakcollection)-Sammlung. |
| [getHyperlinks()](#getHyperlinks--) | Liefert die [HyperlinkCollection](../../com.aspose.cells/hyperlinkcollection)-Sammlung. |
| [getIndex()](#getIndex--) | Liefert den Index des Blatts in der Arbeitsblatt‑Sammlung. |
| [getListObjects()](#getListObjects--) | Liefert alle ListObjects in diesem Arbeitsblatt. |
| [getName()](#getName--) | Liefert den Namen des Arbeitsblatts. |
| [getOleObjects()](#getOleObjects--) | Stellt eine Sammlung von [OleObject](../../com.aspose.cells/oleobject) in einem Arbeitsblatt dar. |
| [getOutline()](#getOutline--) | Liefert die Gliederung dieses Arbeitsblatts. |
| [getPageSetup()](#getPageSetup--) | Stellt die Seitenlayout‑Beschreibung in diesem Blatt dar. |
| [getPaneState()](#getPaneState--) | Gibt an, ob das Fenster horizontale oder vertikale Teilungen hat und ob diese Teilungen eingefroren sind. |
| [getPanes()](#getPanes--) | Ruft die Fensterbereiche ab. |
| [getPictures()](#getPictures--) | Ruft eine [Picture](../../com.aspose.cells/picture)-Sammlung ab. |
| [getPivotTables()](#getPivotTables--) | Ruft alle Pivot‑Tabellen in diesem Arbeitsblatt ab. |
| [getPrintingPageBreaks(ImageOrPrintOptions options)](#getPrintingPageBreaks-com.aspose.cells.ImageOrPrintOptions-) | Ruft automatische Seitenumbrüche ab. |
| [getProtection()](#getProtection--) | Stellt die verschiedenen Arten von Schutzoptionen dar, die für ein Arbeitsblatt verfügbar sind. |
| [getQueryTables()](#getQueryTables--) | Ruft die [QueryTableCollection](../../com.aspose.cells/querytablecollection) im Arbeitsblatt ab. |
| [getScenarios()](#getScenarios--) | Ruft die Sammlung von [Scenario](../../com.aspose.cells/scenario) ab. |
| [getSelectedAreas()](#getSelectedAreas--) | Ruft ausgewählte Zellbereiche im Designer‑Tabellenblatt ab. |
| [getSelectedRanges()](#getSelectedRanges--) | Ruft ausgewählte Zellbereiche im Designer‑Tabellenblatt ab. |
| [getShapes()](#getShapes--) | Gibt alle Zeichenformen in diesem Arbeitsblatt zurück. |
| [getShowDataTypeIcons()](#getShowDataTypeIcons--) | Gibt an, ob Datentyp‑Symbole angezeigt werden sollen. |
| [getShowFormulas()](#getShowFormulas--) | Gibt an, ob Formeln oder deren Ergebnisse angezeigt werden sollen. |
| [getSlicers()](#getSlicers--) | Ruft die Slicer‑Sammlung im Arbeitsblatt ab |
| [getSmartTagSetting()](#getSmartTagSetting--) | Ruft alle [SmartTagCollection](../../com.aspose.cells/smarttagcollection)-Objekte des Arbeitsblatts ab. |
| [getSparklineGroups()](#getSparklineGroups--) | Ruft die Sparkline‑Gruppen im Arbeitsblatt ab. |
| [getTabColor()](#getTabColor--) | Stellt die Registerkartenfarbe des Arbeitsblatts dar. |
| [getTabId()](#getTabId--) | Gibt den internen Bezeichner für das Blatt an. |
| [getTextBoxes()](#getTextBoxes--) | Ruft eine [TextBox](../../com.aspose.cells/textbox)-Sammlung ab. |
| [getTimelines()](#getTimelines--) | Ruft die Timeline‑Sammlung im Arbeitsblatt ab |
| [getTransitionEntry()](#getTransitionEntry--) | Gibt an, ob die Option Transition Formula Entry (Lotus‑Kompatibilität) aktiviert ist. |
| [getTransitionEvaluation()](#getTransitionEvaluation--) | Gibt an, ob die Option Transition Formula Evaluation (Lotus‑Kompatibilität) aktiviert ist. |
| [getType()](#getType--) | Stellt den Arbeitsblatttyp dar. |
| [getUniqueId()](#getUniqueId--) | Ruft die eindeutige ID ab, sie ist dieselbe wie \{15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F\}. |
| [getValidations()](#getValidations--) | Ruft die Datengültigkeits‑Einstellungs‑Sammlung im Arbeitsblatt ab. |
| [getVerticalPageBreaks()](#getVerticalPageBreaks--) | Ruft die [VerticalPageBreakCollection](../../com.aspose.cells/verticalpagebreakcollection)-Sammlung ab. |
| [getViewType()](#getViewType--) | Liefert den Ansichtstyp. |
| [getVisibilityType()](#getVisibilityType--) | Gibt den sichtbaren Zustand dieses Blatts an. |
| [getWorkbook()](#getWorkbook--) | Liefert das Arbeitsmappen-Objekt, das dieses Blatt enthält. |
| [getZoom()](#getZoom--) | Stellt den Skalierungsfaktor in Prozent dar. |
| [hasAutofilter()](#hasAutofilter--) | Gibt an, ob dieses Arbeitsblatt einen Auto-Filter hat. |
| [hashCode()](#hashCode--) |  |
| [isGridlinesVisible()](#isGridlinesVisible--) | Liefert einen Wert, der angibt, ob die Gitternetzlinien sichtbar sind. Standard ist wahr. |
| [isOutlineShown()](#isOutlineShown--) | Gibt an, ob die Gliederung angezeigt werden soll. |
| [isPageBreakPreview()](#isPageBreakPreview--) | Gibt an, ob das angegebene Arbeitsblatt in Normalansicht oder Seitenumbruchvorschau angezeigt wird. |
| [isProtected()](#isProtected--) | Gibt an, ob das Arbeitsblatt geschützt ist. |
| [isRowColumnHeadersVisible()](#isRowColumnHeadersVisible--) | Liefert einen Wert, der angibt, ob das Arbeitsblatt Zeilen- und Spaltenüberschriften anzeigt. |
| [isRulerVisible()](#isRulerVisible--) | Gibt an, ob das Lineal sichtbar ist. |
| [isSelected()](#isSelected--) | Gibt an, ob dieses Arbeitsblatt beim Öffnen der Arbeitsmappe ausgewählt ist. |
| [isVisible()](#isVisible--) | Stellt dar, ob das Arbeitsblatt sichtbar ist. |
| [moveTo(int index)](#moveTo-int-) | Verschiebt das Blatt an eine andere Position in der Tabelle. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [protect(int type)](#protect-int-) | Schützt das Arbeitsblatt. |
| [protect(int type, String password, String oldPassword)](#protect-int-java.lang.String-java.lang.String-) | Schützt das Arbeitsblatt. |
| [refreshPivotTables()](#refreshPivotTables--) | Aktualisiert alle PivotTables in diesem Arbeitsblatt. |
| [refreshPivotTables(PivotTableRefreshOption option)](#refreshPivotTables-com.aspose.cells.PivotTableRefreshOption-) | Aktualisiert alle PivotTables in diesem Arbeitsblatt. |
| [removeAllDrawingObjects()](#removeAllDrawingObjects--) | Entfernt alle Zeichenobjekte in diesem Arbeitsblatt. |
| [removeAutoFilter()](#removeAutoFilter--) | Entfernt den Auto-Filter des Arbeitsblatts. |
| [removeSplit()](#removeSplit--) | Entfernt das geteilte Fenster. |
| [replace(String oldString, String newString)](#replace-java.lang.String-java.lang.String-) | Ersetzt den Text aller Zellen durch eine neue Zeichenfolge. |
| [selectRange(int startRow, int startColumn, int totalRows, int totalColumns, boolean removeOthers)](#selectRange-int-int-int-int-boolean-) | Wählt einen Bereich aus. |
| [setActiveCell(String value)](#setActiveCell-java.lang.String-) | Setzt die aktive Zelle im Arbeitsblatt. |
| [setBackgroundImage(byte[] value)](#setBackgroundImage-byte---) | Setzt das Hintergrundbild des Arbeitsblatts. |
| [setCodeName(String value)](#setCodeName-java.lang.String-) | Liefert den Code‑Namen des Arbeitsblatts. |
| [setDisplayRightToLeft(boolean value)](#setDisplayRightToLeft-boolean-) | Gibt an, ob das angegebene Arbeitsblatt von rechts nach links statt von links nach rechts angezeigt wird. |
| [setDisplayZeros(boolean value)](#setDisplayZeros-boolean-) | Wahr, wenn Nullwerte angezeigt werden. |
| [setFirstVisibleColumn(int value)](#setFirstVisibleColumn-int-) | Stellt den Index der ersten sichtbaren Spalte dar. |
| [setFirstVisibleRow(int value)](#setFirstVisibleRow-int-) | Stellt den Index der ersten sichtbaren Zeile dar. |
| [setGridlineColor(Color value)](#setGridlineColor-com.aspose.cells.Color-) | Setzt die Farbe der Gitternetzlinie |
| [setGridlinesVisible(boolean value)](#setGridlinesVisible-boolean-) | Setzt einen Wert, der angibt, ob die Gitternetzlinien sichtbar sind. Standard ist wahr. |
| [setName(String value)](#setName-java.lang.String-) | Legt den Namen des Arbeitsblatts fest. |
| [setOutlineShown(boolean value)](#setOutlineShown-boolean-) | Gibt an, ob die Gliederung angezeigt werden soll. |
| [setPageBreakPreview(boolean value)](#setPageBreakPreview-boolean-) | Gibt an, ob das angegebene Arbeitsblatt in Normalansicht oder Seitenumbruchvorschau angezeigt wird. |
| [setRowColumnHeadersVisible(boolean value)](#setRowColumnHeadersVisible-boolean-) | Legt einen Wert fest, der angibt, ob das Arbeitsblatt Zeilen- und Spaltenüberschriften anzeigt. |
| [setRulerVisible(boolean value)](#setRulerVisible-boolean-) | Gibt an, ob das Lineal sichtbar ist. |
| [setSelected(boolean value)](#setSelected-boolean-) | Gibt an, ob dieses Arbeitsblatt beim Öffnen der Arbeitsmappe ausgewählt ist. |
| [setShowDataTypeIcons(boolean value)](#setShowDataTypeIcons-boolean-) | Gibt an, ob Datentyp‑Symbole angezeigt werden sollen. |
| [setShowFormulas(boolean value)](#setShowFormulas-boolean-) | Gibt an, ob Formeln oder deren Ergebnisse angezeigt werden sollen. |
| [setTabColor(Color value)](#setTabColor-com.aspose.cells.Color-) | Stellt die Registerkartenfarbe des Arbeitsblatts dar. |
| [setTabId(int value)](#setTabId-int-) | Gibt den internen Bezeichner für das Blatt an. |
| [setTransitionEntry(boolean value)](#setTransitionEntry-boolean-) | Gibt an, ob die Option Transition Formula Entry (Lotus‑Kompatibilität) aktiviert ist. |
| [setTransitionEvaluation(boolean value)](#setTransitionEvaluation-boolean-) | Gibt an, ob die Option Transition Formula Evaluation (Lotus‑Kompatibilität) aktiviert ist. |
| [setType(int value)](#setType-int-) | Stellt den Arbeitsblatttyp dar. |
| [setUniqueId(String value)](#setUniqueId-java.lang.String-) | Legt die eindeutige ID fest, sie ist dieselbe wie \{15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F\}. |
| [setViewType(int value)](#setViewType-int-) | Legt den Ansichtstyp fest. |
| [setVisibilityType(int value)](#setVisibilityType-int-) | Gibt den sichtbaren Zustand dieses Blatts an. |
| [setVisible(boolean value)](#setVisible-boolean-) | Stellt dar, ob das Arbeitsblatt sichtbar ist. |
| [setVisible(boolean isVisible, boolean ignoreError)](#setVisible-boolean-boolean-) | Legt die sichtbaren Optionen fest. |
| [setZoom(int value)](#setZoom-int-) | Stellt den Skalierungsfaktor in Prozent dar. |
| [split()](#split--) | Teilt das Fenster. |
| [startAccessCache(int opts)](#startAccessCache-int-) | Startet die Sitzung, die Caches verwendet, um auf die Daten in diesem Arbeitsblatt zuzugreifen. |
| [toString()](#toString--) | Gibt einen String zurück, der das aktuelle Arbeitsblatt-Objekt darstellt. |
| [unFreezePanes()](#unFreezePanes--) | Löst das Einfrieren von Bereichen im Arbeitsblatt. |
| [unprotect()](#unprotect--) | Entfernt den Schutz des Arbeitsblatts. |
| [unprotect(String password)](#unprotect-java.lang.String-) | Entfernt den Schutz des Arbeitsblatts. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
| [xmlMapQuery(String path, XmlMap xmlMap)](#xmlMapQuery-java.lang.String-com.aspose.cells.XmlMap-) | Abfrage von Zellbereichen, die mit dem spezifischen Pfad der XML‑Map verknüpft/verbunden sind. |
### addPageBreaks(String cellName) {#addPageBreaks-java.lang.String-}
```
public void addPageBreaks(String cellName)
```


Fügt einen Seitenumbruch hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellName | java.lang.String |  |

### advancedFilter(boolean isFilter, String listRange, String criteriaRange, String copyTo, boolean uniqueRecordOnly) {#advancedFilter-boolean-java.lang.String-java.lang.String-java.lang.String-boolean-}
```
public void advancedFilter(boolean isFilter, String listRange, String criteriaRange, String copyTo, boolean uniqueRecordOnly)
```


Filtert Daten mithilfe komplexer Kriterien.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isFilter | boolean | Gibt an, ob die Liste vor Ort gefiltert wird. |
| listRange | java.lang.String | Der Listenbereich. |
| criteriaRange | java.lang.String | Der Kriterienbereich. |
| copyTo | java.lang.String | Der Bereich, in den Daten kopiert werden. |
| uniqueRecordOnly | boolean | Nur eindeutige Zeilen anzeigen oder kopieren. |

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


Passt alle Spalten in diesem Arbeitsblatt automatisch an.

### autoFitColumns(AutoFitterOptions options) {#autoFitColumns-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitColumns(AutoFitterOptions options)
```


Passt alle Spalten in diesem Arbeitsblatt automatisch an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | Die Optionen für die automatische Anpassung |

### autoFitColumns(int firstColumn, int lastColumn) {#autoFitColumns-int-int-}
```
public void autoFitColumns(int firstColumn, int lastColumn)
```


Passt die Spaltenbreite automatisch an.

**Remarks**

AutoFitColumn ist eine ungenaue Funktion.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstColumn | int | Erster Spaltenindex. |
| lastColumn | int | Letzter Spaltenindex. |

### autoFitColumns(int firstColumn, int lastColumn, AutoFitterOptions options) {#autoFitColumns-int-int-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitColumns(int firstColumn, int lastColumn, AutoFitterOptions options)
```


Passt die Spaltenbreite automatisch an.

**Remarks**

AutoFitColumn ist eine ungenaue Funktion.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstColumn | int | Erster Spaltenindex. |
| lastColumn | int | Letzter Spaltenindex. |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | Die Optionen für die automatische Anpassung |

### autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn) {#autoFitColumns-int-int-int-int-}
```
public void autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn)
```


Passt die Spaltenbreite automatisch an.

**Remarks**

AutoFitColumn ist eine ungenaue Funktion.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstRow | int | Erster Zeilenindex. |
| firstColumn | int | Erster Spaltenindex. |
| lastRow | int | Letzter Zeilenindex. |
| lastColumn | int | Letzter Spaltenindex. |

### autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn, AutoFitterOptions options) {#autoFitColumns-int-int-int-int-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn, AutoFitterOptions options)
```


Passt die Spaltenbreite automatisch an.

**Remarks**

AutoFitColumn ist eine ungenaue Funktion.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstRow | int | Erster Zeilenindex. |
| firstColumn | int | Erster Spaltenindex. |
| lastRow | int | Letzter Zeilenindex. |
| lastColumn | int | Letzter Spaltenindex. |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | Die Optionen für die automatische Anpassung |

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

### autoFitRow(int rowIndex, int firstColumn, int lastColumn, AutoFitterOptions options) {#autoFitRow-int-int-int-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitRow(int rowIndex, int firstColumn, int lastColumn, AutoFitterOptions options)
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
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | Die Auto-Fitter-Optionen |

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

### autoFitRows(AutoFitterOptions options) {#autoFitRows-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitRows(AutoFitterOptions options)
```


Passt alle Zeilen in diesem Arbeitsblatt automatisch an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | Die Auto-Fitter-Optionen |

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

### autoFitRows(int startRow, int endRow, AutoFitterOptions options) {#autoFitRows-int-int-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitRows(int startRow, int endRow, AutoFitterOptions options)
```


Passt die Zeilenhöhe in einem Bereich automatisch an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | int | Startzeilenindex. |
| endRow | int | Endzeilenindex. |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | Die Optionen des Auto-Fitters. |

### calculateArrayFormula(String formula, CalculationOptions opts) {#calculateArrayFormula-java.lang.String-com.aspose.cells.CalculationOptions-}
```
public Object[][] calculateArrayFormula(String formula, CalculationOptions opts)
```


Berechnet eine Formel als Array-Formel.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| formula | java.lang.String | Formel, die berechnet werden soll. |
| opts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Optionen zur Berechnung der Formel |

**Returns:**
java.lang.Object[][]
### calculateArrayFormula(String formula, CalculationOptions opts, int maxRowCount, int maxColumnCount) {#calculateArrayFormula-java.lang.String-com.aspose.cells.CalculationOptions-int-int-}
```
public Object[][] calculateArrayFormula(String formula, CalculationOptions opts, int maxRowCount, int maxColumnCount)
```


Berechnet eine Formel als Array-Formel.

**Remarks**

Die Formel wird als dynamische Array-Formel verwendet, um die Dimension und das Ergebnis zu berechnen. Die vom Benutzer angegebene maximale Dimension wird in Fällen verwendet, in denen das berechnete Ergebnis ein großer Datensatz ist (zum Beispiel kann das berechnete Ergebnis einer gesamten Zeilen- oder Spaltendaten entsprechen), der Benutzer jedoch nach geschäftlichen Anforderungen oder aus Leistungsgründen nicht so ein großes Array benötigt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| formula | java.lang.String | Formel, die berechnet werden soll. |
| opts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Optionen zur Berechnung der Formel |
| maxRowCount | int | die maximale Zeilenanzahl der Ergebnisdaten. Wenn sie nicht positiv ist oder größer als die tatsächliche Zeilenanzahl, wird die tatsächliche Zeilenanzahl verwendet. |
| maxColumnCount | int | die maximale Spaltenanzahl der Ergebnisdaten. Wenn sie nicht positiv ist oder größer als die tatsächliche Zeilenanzahl, wird die tatsächliche Spaltenanzahl verwendet. |

**Returns:**
java.lang.Object[][] - Berechnetes Formelresultat.
### calculateArrayFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, int maxRowCount, int maxColumnCount, CalculationData calculationData) {#calculateArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-com.aspose.cells.CalculationOptions-int-int-int-int-com.aspose.cells.CalculationData-}
```
public Object[][] calculateArrayFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, int maxRowCount, int maxColumnCount, CalculationData calculationData)
```


Berechnet eine Formel als Array-Formel.

**Remarks**

Die Formel wird als dynamische Array-Formel verwendet, um die Dimension und das Ergebnis zu berechnen. Die vom Benutzer angegebene maximale Dimension wird in Fällen verwendet, in denen das berechnete Ergebnis ein großer Datensatz ist (zum Beispiel kann das berechnete Ergebnis einer gesamten Zeilen- oder Spaltendaten entsprechen), der Benutzer jedoch nach geschäftlichen Anforderungen oder aus Leistungsgründen nicht so ein großes Array benötigt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| formula | java.lang.String | Formel, die berechnet werden soll. |
| pOpts | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Optionen zum Parsen der Formel |
| cOpts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Optionen zur Berechnung der Formel |
| baseCellRow | int | Der Zeilenindex der Basiszelle. |
| baseCellColumn | int | Der Spaltenindex der Basisezelle. |
| maxRowCount | int | Die maximale Zeilenanzahl der Ergebnisdaten. Wenn sie nicht positiv ist oder größer als die tatsächliche Zeilenanzahl, wird die tatsächliche Zeilenanzahl verwendet. |
| maxColumnCount | int | Die maximale Spaltenanzahl der Ergebnisdaten. Wenn sie nicht positiv ist oder größer als die tatsächliche Zeilenanzahl, wird die tatsächliche Spaltenanzahl verwendet. |
| calculationData | [CalculationData](../../com.aspose.cells/calculationdata) | Die Berechnungsdaten. Sie werden für den Fall verwendet, dass der Benutzer einige statische Formeln berechnen muss, wenn er eine benutzerdefinierte Berechnungs-Engine implementiert. Für solche Situationen muss der Benutzer sie mit den Berechnungsdaten angeben, die für [AbstractCalculationEngine.calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-) bereitgestellt werden. |

**Returns:**
java.lang.Object[][] - Berechnetes Formelresultat.
### calculateFormula(CalculationOptions options, boolean recursive) {#calculateFormula-com.aspose.cells.CalculationOptions-boolean-}
```
public void calculateFormula(CalculationOptions options, boolean recursive)
```


Berechnet alle Formeln in diesem Arbeitsblatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| options | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Optionen für die Berechnung |
| rekursiv | boolean | True bedeutet, dass wenn die Zellen des Arbeitsblatts von Zellen anderer Arbeitsblätter abhängen, die abhängigen Zellen in anderen Arbeitsblättern ebenfalls berechnet werden. False bedeutet, dass alle Formeln im Arbeitsblatt berechnet wurden und die Werte korrekt sind. |

### calculateFormula(String formula) {#calculateFormula-java.lang.String-}
```
public Object calculateFormula(String formula)
```


Berechnet eine Formel.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| formula | java.lang.String | Formel, die berechnet werden soll. |

**Returns:**
java.lang.Object - Berechnetes Formelergebnis.
### calculateFormula(String formula, CalculationOptions opts) {#calculateFormula-java.lang.String-com.aspose.cells.CalculationOptions-}
```
public Object calculateFormula(String formula, CalculationOptions opts)
```


Berechnet einen Formelausdruck direkt.

**Remarks**

Die Formel wird berechnet, als wäre sie in Zelle A1 gesetzt worden. Und die Formel wird als normale Formel behandelt. Wenn Sie die Formel als Array‑Formel berechnen und ein Array für das berechnete Ergebnis erhalten möchten, verwenden Sie stattdessen [calculateArrayFormula(String,CalculationOptions)](../../com.aspose.cells/worksheet\#calculateArrayFormula-String-CalculationOptions-).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| formula | java.lang.String | Formel, die berechnet werden soll. |
| opts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Optionen zur Berechnung der Formel |

**Returns:**
java.lang.Object - Berechnetes Ergebnis der angegebenen Formel. Das zurückgegebene Objekt kann mögliche Typen von [Cell.getValue()](../../com.aspose.cells/cell\#getValue--), oder ReferredArea haben.
### calculateFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, CalculationData calculationData) {#calculateFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-com.aspose.cells.CalculationOptions-int-int-com.aspose.cells.CalculationData-}
```
public Object calculateFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, CalculationData calculationData)
```


Berechnet einen Formelausdruck direkt.

**Remarks**

Die Formel wird berechnet, als wäre sie in die angegebene Basisezelle gesetzt worden. Und die Formel wird als normale Formel behandelt. Wenn Sie die Formel als Array‑Formel berechnen und ein Array für das berechnete Ergebnis erhalten möchten, verwenden Sie stattdessen [calculateArrayFormula(String,FormulaParseOptions,CalculationOptions,int,int,int,int,CalculationData)](../../com.aspose.cells/worksheet\#calculateArrayFormula-String-FormulaParseOptions-CalculationOptions-int-int-int-int-CalculationData-).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| formula | java.lang.String | Formel, die berechnet werden soll. |
| pOpts | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Optionen zum Parsen der Formel. |
| cOpts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Optionen zum Berechnen der Formel. |
| baseCellRow | int | Der Zeilenindex der Basiszelle. |
| baseCellColumn | int | Der Spaltenindex der Basisezelle. |
| calculationData | [CalculationData](../../com.aspose.cells/calculationdata) | Die Berechnungsdaten. Sie werden für den Fall verwendet, dass der Benutzer einige statische Formeln berechnen muss, wenn er eine benutzerdefinierte Berechnungs-Engine implementiert. Für solche Situationen muss der Benutzer sie mit den Berechnungsdaten angeben, die für [AbstractCalculationEngine.calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-) bereitgestellt werden. |

**Returns:**
java.lang.Object - Berechnetes Ergebnis der angegebenen Formel. Das zurückgegebene Objekt kann mögliche Typen von [Cell.getValue()](../../com.aspose.cells/cell\#getValue--), oder ReferredArea haben.
### clearComments() {#clearComments--}
```
public void clearComments()
```


Löscht alle Kommentare im Designer-Tabellenblatt.

### closeAccessCache(int opts) {#closeAccessCache-int-}
```
public void closeAccessCache(int opts)
```


Schließt die Sitzung, die Caches verwendet, um auf die Daten in diesem Arbeitsblatt zuzugreifen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| opts | int | [AccessCacheOptions](../../com.aspose.cells/accesscacheoptions). Optionen für den Datenzugriff |

### convertFormulaReferenceStyle(String formula, boolean toR1C1, int baseCellRow, int baseCellColumn) {#convertFormulaReferenceStyle-java.lang.String-boolean-int-int-}
```
public String convertFormulaReferenceStyle(String formula, boolean toR1C1, int baseCellRow, int baseCellColumn)
```


Konvertiert den Formel-Referenzstil.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| formula | java.lang.String | Die zu konvertierende Formel. |
| toR1C1 | boolean | Welcher Referenzstil für die Konvertierung der Formel verwendet werden soll. Wenn die ursprüngliche Formel im A1‑Referenzstil vorliegt, sollte dieser Wert true sein, damit die Formel von A1 nach R1C1 konvertiert wird; wenn die ursprüngliche Formel im R1C1‑Referenzstil vorliegt, sollte dieser Wert false sein, damit die Formel von R1C1 nach A1 konvertiert wird; |
| baseCellRow | int | Der Zeilenindex der Basiszelle. |
| baseCellColumn | int | Der Spaltenindex der Basisezelle. |

**Returns:**
java.lang.String - Die konvertierte Formel.
### copy(Worksheet sourceSheet) {#copy-com.aspose.cells.Worksheet-}
```
public void copy(Worksheet sourceSheet)
```


Kopiert Inhalte und Formate von einem anderen Arbeitsblatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceSheet | [Worksheet](../../com.aspose.cells/worksheet) | Quellarbeitsblatt. |

### copy(Worksheet sourceSheet, CopyOptions copyOptions) {#copy-com.aspose.cells.Worksheet-com.aspose.cells.CopyOptions-}
```
public void copy(Worksheet sourceSheet, CopyOptions copyOptions)
```


Kopiert Inhalte und Formate von einem anderen Arbeitsblatt.

**Remarks**

Sie können Daten aus einem anderen Arbeitsblatt in derselben Datei oder einer anderen Datei kopieren. Diese Methode unterstützt jedoch nicht das Kopieren von Zeichenobjekten, wie Kommentaren, Bildern und Diagrammen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceSheet | [Worksheet](../../com.aspose.cells/worksheet) | Quellarbeitsblatt. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) |  |

### dispose() {#dispose--}
```
public void dispose()
```


Führt anwendungsspezifische Aufgaben aus, die mit dem Freigeben, Freisetzen oder Zurücksetzen nicht verwalteter Ressourcen verbunden sind.

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
### filter(CellArea ca) {#filter-com.aspose.cells.CellArea-}
```
public void filter(CellArea ca)
```


Filtert den Bereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Der Bereich |

### freezePanes(int row, int column, int freezedRows, int freezedColumns) {#freezePanes-int-int-int-int-}
```
public void freezePanes(int row, int column, int freezedRows, int freezedColumns)
```


Friert Bereiche an der angegebenen Zelle im Arbeitsblatt ein.

**Remarks**

Zeilenindex und Spaltenindex können nicht beide Null sein. Die Anzahl der Zeilen und die Anzahl der Spalten können ebenfalls nicht beide Null sein.

Die ersten beiden Parameter geben die eingefrorene Position an und die letzten beiden Parameter geben den im linken oberen Bereich eingefrorenen Bereich an.

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
### getAdvancedFilter() {#getAdvancedFilter--}
```
public AdvancedFilter getAdvancedFilter()
```


Ermittelt die Einstellungen des erweiterten Filters.

**Returns:**
[AdvancedFilter](../../com.aspose.cells/advancedfilter) - 
### getAllPictures() {#getAllPictures--}
```
public Picture[] getAllPictures()
```


Ermittelt alle Bilder, einschließlich der in der Zelle eingebetteten und über den Zellen liegenden Bilder.

**Returns:**
com.aspose.cells.Picture[] -
### getAllowEditRanges() {#getAllowEditRanges--}
```
public ProtectedRangeCollection getAllowEditRanges()
```


Ermittelt die Sammlung zulässiger Bearbeitungsbereiche im Arbeitsblatt.

**Returns:**
[ProtectedRangeCollection](../../com.aspose.cells/protectedrangecollection)
### getAreasOfXmlMapQuery(String path, XmlMap xmlMap) {#getAreasOfXmlMapQuery-java.lang.String-com.aspose.cells.XmlMap-}
```
public CellArea[] getAreasOfXmlMapQuery(String path, XmlMap xmlMap)
```


Abfrage von Zellbereichen, die mit dem spezifischen Pfad der XML‑Map verknüpft/verbunden sind.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Pfad | java.lang.String | XML-Elementpfad |
| xmlMap | [XmlMap](../../com.aspose.cells/xmlmap) | Geben Sie eine XML-Karte an, wenn Sie den spezifischen Pfad innerhalb einer bestimmten Karte abfragen möchten. |

**Returns:**
com.aspose.cells.CellArea[] - [CellArea](../../com.aspose.cells/cellarea) Liste, die dem spezifischen Pfad der XML-Karte zugeordnet/verknüpft ist; eine leere Liste wird zurückgegeben, wenn nichts zugeordnet/verknüpft ist.
### getAutoFilter() {#getAutoFilter--}
```
public AutoFilter getAutoFilter()
```


Stellt den AutoFilter für das angegebene Arbeitsblatt dar.

**Returns:**
[AutoFilter](../../com.aspose.cells/autofilter)
### getBackgroundImage() {#getBackgroundImage--}
```
public byte[] getBackgroundImage()
```


Liefert das Hintergrundbild des Arbeitsblatts.

**Returns:**
byte[]
### getCellWatches() {#getCellWatches--}
```
public CellWatchCollection getCellWatches()
```


Liefert die Sammlung von Zellen dieses Arbeitsblatts, die im „Watch‑Fenster“ überwacht werden.

**Returns:**
[CellWatchCollection](../../com.aspose.cells/cellwatchcollection)
### getCells() {#getCells--}
```
public Cells getCells()
```


Liefert die [Cells](../../com.aspose.cells/cells)-Sammlung.

**Returns:**
[Cells](../../com.aspose.cells/cells)
### getCharts() {#getCharts--}
```
public ChartCollection getCharts()
```


Liefert eine [Chart](../../com.aspose.cells/chart)-Sammlung

**Returns:**
[ChartCollection](../../com.aspose.cells/chartcollection)
### getCheckBoxes() {#getCheckBoxes--}
```
public CheckBoxCollection getCheckBoxes()
```


Liefert eine [CheckBox](../../com.aspose.cells/checkbox)-Sammlung.

**Returns:**
[CheckBoxCollection](../../com.aspose.cells/checkboxcollection)
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


Liefert den Code‑Namen des Arbeitsblatts.

**Returns:**
java.lang.String
### getComments() {#getComments--}
```
public CommentCollection getComments()
```


Liefert die [Comment](../../com.aspose.cells/comment)-Sammlung.

**Returns:**
[CommentCollection](../../com.aspose.cells/commentcollection)
### getConditionalFormattings() {#getConditionalFormattings--}
```
public ConditionalFormattingCollection getConditionalFormattings()
```


Liefert die ConditionalFormattings im Arbeitsblatt.

**Returns:**
[ConditionalFormattingCollection](../../com.aspose.cells/conditionalformattingcollection)
### getCustomProperties() {#getCustomProperties--}
```
public CustomPropertyCollection getCustomProperties()
```


Liefert ein Objekt, das die Kennzeichnungsinformationen eines Arbeitsblatts darstellt.

**Remarks**

Worksheet.CustomProperties bieten einen bevorzugten Mechanismus zum Speichern beliebiger Daten. Sie unterstützen Legacy-Drittanbieter-Dokumentkomponenten sowie Situationen, die einen strengen Bedarf an Binärteilen haben.

**Returns:**
[CustomPropertyCollection](../../com.aspose.cells/custompropertycollection)
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
### getErrorCheckOptions() {#getErrorCheckOptions--}
```
public ErrorCheckOptionCollection getErrorCheckOptions()
```


Liefert die Fehlerprüfungs‑Einstellung, die auf bestimmte Bereiche angewendet wird.

**Returns:**
[ErrorCheckOptionCollection](../../com.aspose.cells/errorcheckoptioncollection)
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
### getGridlineColor() {#getGridlineColor--}
```
public Color getGridlineColor()
```


Liefert die Farbe der Rasterlinien

**Returns:**
[Color](../../com.aspose.cells/color)
### getHorizontalPageBreaks() {#getHorizontalPageBreaks--}
```
public HorizontalPageBreakCollection getHorizontalPageBreaks()
```


Liefert die [HorizontalPageBreakCollection](../../com.aspose.cells/horizontalpagebreakcollection)-Sammlung.

**Returns:**
[HorizontalPageBreakCollection](../../com.aspose.cells/horizontalpagebreakcollection)
### getHyperlinks() {#getHyperlinks--}
```
public HyperlinkCollection getHyperlinks()
```


Liefert die [HyperlinkCollection](../../com.aspose.cells/hyperlinkcollection)-Sammlung.

**Returns:**
[HyperlinkCollection](../../com.aspose.cells/hyperlinkcollection)
### getIndex() {#getIndex--}
```
public int getIndex()
```


Liefert den Index des Blatts in der Arbeitsblatt‑Sammlung.

**Returns:**
int
### getListObjects() {#getListObjects--}
```
public ListObjectCollection getListObjects()
```


Liefert alle ListObjects in diesem Arbeitsblatt.

**Returns:**
[ListObjectCollection](../../com.aspose.cells/listobjectcollection)
### getName() {#getName--}
```
public String getName()
```


Liefert den Namen des Arbeitsblatts.

**Remarks**

Die maximale Länge eines Blattnamens beträgt 31 Zeichen. Und Sie können nicht denselben Namen (Groß-/Kleinschreibung ignorierend) zwei Arbeitsblättern zuweisen. Zum Beispiel können Sie nicht "SheetName1" dem ersten Arbeitsblatt zuweisen und "SHEETNAME1" dem zweiten Arbeitsblatt.

**Returns:**
java.lang.String
### getOleObjects() {#getOleObjects--}
```
public OleObjectCollection getOleObjects()
```


Stellt eine Sammlung von [OleObject](../../com.aspose.cells/oleobject) in einem Arbeitsblatt dar.

**Returns:**
[OleObjectCollection](../../com.aspose.cells/oleobjectcollection)
### getOutline() {#getOutline--}
```
public Outline getOutline()
```


Liefert die Gliederung dieses Arbeitsblatts.

**Returns:**
[Outline](../../com.aspose.cells/outline)
### getPageSetup() {#getPageSetup--}
```
public PageSetup getPageSetup()
```


Stellt die Seitenlayout‑Beschreibung in diesem Blatt dar.

**Returns:**
[PageSetup](../../com.aspose.cells/pagesetup)
### getPaneState() {#getPaneState--}
```
public int getPaneState()
```


Gibt an, ob das Fenster horizontale oder vertikale Teilungen hat und ob diese Teilungen eingefroren sind.

Siehe [PaneStateType](../../com.aspose.cells/panestatetype).

**Returns:**
int
### getPanes() {#getPanes--}
```
public PaneCollection getPanes()
```


Ruft die Fensterbereiche ab.

**Remarks**

Falls das Fenster nicht geteilt oder eingefroren ist.

**Returns:**
[PaneCollection](../../com.aspose.cells/panecollection)
### getPictures() {#getPictures--}
```
public PictureCollection getPictures()
```


Ruft eine [Picture](../../com.aspose.cells/picture)-Sammlung ab.

**Returns:**
[PictureCollection](../../com.aspose.cells/picturecollection)
### getPivotTables() {#getPivotTables--}
```
public PivotTableCollection getPivotTables()
```


Ruft alle Pivot‑Tabellen in diesem Arbeitsblatt ab.

**Returns:**
[PivotTableCollection](../../com.aspose.cells/pivottablecollection)
### getPrintingPageBreaks(ImageOrPrintOptions options) {#getPrintingPageBreaks-com.aspose.cells.ImageOrPrintOptions-}
```
public CellArea[] getPrintingPageBreaks(ImageOrPrintOptions options)
```


Ruft automatische Seitenumbrüche ab.

**Remarks**

Jeder Zellbereich stellt ein Blatt dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | Die Druckoptionen |

**Returns:**
com.aspose.cells.CellArea[] - Die automatischen Seitenumbruchbereiche.
### getProtection() {#getProtection--}
```
public Protection getProtection()
```


Stellt die verschiedenen Arten von Schutzoptionen dar, die für ein Arbeitsblatt verfügbar sind. Unterstützt erweiterte Schutzoptionen in ExcelXP und höheren Versionen.

**Remarks**

Diese Eigenschaft kann Arbeitsblätter in allen Excel-Dateiversionen schützen und unterstützt erweiterte Schutzoptionen in ExcelXP und höheren Versionen.

**Returns:**
[Protection](../../com.aspose.cells/protection)
### getQueryTables() {#getQueryTables--}
```
public QueryTableCollection getQueryTables()
```


Ruft die [QueryTableCollection](../../com.aspose.cells/querytablecollection) im Arbeitsblatt ab.

**Returns:**
[QueryTableCollection](../../com.aspose.cells/querytablecollection)
### getScenarios() {#getScenarios--}
```
public ScenarioCollection getScenarios()
```


Ruft die Sammlung von [Scenario](../../com.aspose.cells/scenario) ab.

**Returns:**
[ScenarioCollection](../../com.aspose.cells/scenariocollection)
### getSelectedAreas() {#getSelectedAreas--}
```
public Range[] getSelectedAreas()
```


Ruft ausgewählte Zellbereiche im Designer‑Tabellenblatt ab.

**Returns:**
com.aspose.cells.Range[] - Gibt alle ausgewählten Bereiche zurück.
### getSelectedRanges() {#getSelectedRanges--}
```
public ArrayList getSelectedRanges()
```


Ruft ausgewählte Zellbereiche im Designer‑Tabellenblatt ab.

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Methode Worksheet.GetSelectedAreas(). Diese Eigenschaft wird 12 Monate nach März 2025 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
java.util.ArrayList - Eine ArrayList, die ausgewählte Bereiche enthält.
### getShapes() {#getShapes--}
```
public ShapeCollection getShapes()
```


Gibt alle Zeichenformen in diesem Arbeitsblatt zurück.

**Returns:**
[ShapeCollection](../../com.aspose.cells/shapecollection)
### getShowDataTypeIcons() {#getShowDataTypeIcons--}
```
public boolean getShowDataTypeIcons()
```


Gibt an, ob Datentyp‑Symbole angezeigt werden sollen.

**Returns:**
boolean
### getShowFormulas() {#getShowFormulas--}
```
public boolean getShowFormulas()
```


Gibt an, ob Formeln oder deren Ergebnisse angezeigt werden sollen.

**Returns:**
boolean
### getSlicers() {#getSlicers--}
```
public SlicerCollection getSlicers()
```


Ruft die Slicer‑Sammlung im Arbeitsblatt ab

**Returns:**
[SlicerCollection](../../com.aspose.cells/slicercollection)
### getSmartTagSetting() {#getSmartTagSetting--}
```
public SmartTagSetting getSmartTagSetting()
```


Ruft alle [SmartTagCollection](../../com.aspose.cells/smarttagcollection)-Objekte des Arbeitsblatts ab.

**Returns:**
[SmartTagSetting](../../com.aspose.cells/smarttagsetting)
### getSparklineGroups() {#getSparklineGroups--}
```
public SparklineGroupCollection getSparklineGroups()
```


Ruft die Sparkline‑Gruppen im Arbeitsblatt ab.

**Returns:**
[SparklineGroupCollection](../../com.aspose.cells/sparklinegroupcollection)
### getTabColor() {#getTabColor--}
```
public Color getTabColor()
```


Stellt die Registerkartenfarbe des Arbeitsblatts dar.

**Remarks**

Dieses Feature wird nur in ExcelXP (Excel2002) und späteren Versionen unterstützt. Wenn Sie die Datei im Excel97- oder Excel2000-Format speichern, wird es weggelassen.

**Returns:**
[Color](../../com.aspose.cells/color)
### getTabId() {#getTabId--}
```
public int getTabId()
```


Gibt den internen Bezeichner für das Blatt an.

**Returns:**
int
### getTextBoxes() {#getTextBoxes--}
```
public TextBoxCollection getTextBoxes()
```


Ruft eine [TextBox](../../com.aspose.cells/textbox)-Sammlung ab.

**Returns:**
[TextBoxCollection](../../com.aspose.cells/textboxcollection)
### getTimelines() {#getTimelines--}
```
public TimelineCollection getTimelines()
```


Ruft die Timeline‑Sammlung im Arbeitsblatt ab

**Returns:**
[TimelineCollection](../../com.aspose.cells/timelinecollection)
### getTransitionEntry() {#getTransitionEntry--}
```
public boolean getTransitionEntry()
```


Gibt an, ob die Option Transition Formula Entry (Lotus‑Kompatibilität) aktiviert ist.

**Returns:**
boolean
### getTransitionEvaluation() {#getTransitionEvaluation--}
```
public boolean getTransitionEvaluation()
```


Gibt an, ob die Option Transition Formula Evaluation (Lotus‑Kompatibilität) aktiviert ist.

**Returns:**
boolean
### getType() {#getType--}
```
public int getType()
```


Stellt den Arbeitsblatttyp dar.

Siehe [SheetType](../../com.aspose.cells/sheettype).

**Returns:**
int
### getUniqueId() {#getUniqueId--}
```
public String getUniqueId()
```


Ruft die eindeutige ID ab, sie ist dieselbe wie \{15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F\}.

**Returns:**
java.lang.String
### getValidations() {#getValidations--}
```
public ValidationCollection getValidations()
```


Ruft die Datengültigkeits‑Einstellungs‑Sammlung im Arbeitsblatt ab.

**Returns:**
[ValidationCollection](../../com.aspose.cells/validationcollection)
### getVerticalPageBreaks() {#getVerticalPageBreaks--}
```
public VerticalPageBreakCollection getVerticalPageBreaks()
```


Ruft die [VerticalPageBreakCollection](../../com.aspose.cells/verticalpagebreakcollection)-Sammlung ab.

**Returns:**
[VerticalPageBreakCollection](../../com.aspose.cells/verticalpagebreakcollection)
### getViewType() {#getViewType--}
```
public int getViewType()
```


Liefert den Ansichtstyp.

Siehe [ViewType](../../com.aspose.cells/viewtype).

**Returns:**
int
### getVisibilityType() {#getVisibilityType--}
```
public int getVisibilityType()
```


Gibt den sichtbaren Zustand dieses Blatts an.

Siehe [VisibilityType](../../com.aspose.cells/visibilitytype).

**Returns:**
int
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


Liefert das Arbeitsmappen-Objekt, das dieses Blatt enthält.

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### getZoom() {#getZoom--}
```
public int getZoom()
```


Stellt den Skalierungsfaktor in Prozent dar. Er sollte zwischen 10 und 400 liegen.

**Remarks**

Bitte setzen Sie zuerst den Ansichtstyp.

**Returns:**
int
### hasAutofilter() {#hasAutofilter--}
```
public boolean hasAutofilter()
```


Gibt an, ob dieses Arbeitsblatt einen Auto-Filter hat.

**Returns:**
boolean
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


Liefert einen Wert, der angibt, ob die Gitternetzlinien sichtbar sind. Standard ist wahr.

**Returns:**
boolean
### isOutlineShown() {#isOutlineShown--}
```
public boolean isOutlineShown()
```


Gibt an, ob die Gliederung angezeigt werden soll.

**Returns:**
boolean
### isPageBreakPreview() {#isPageBreakPreview--}
```
public boolean isPageBreakPreview()
```


Gibt an, ob das angegebene Arbeitsblatt in Normalansicht oder Seitenumbruchvorschau angezeigt wird.

**Returns:**
boolean
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


Gibt an, ob das Arbeitsblatt geschützt ist.

**Returns:**
boolean
### isRowColumnHeadersVisible() {#isRowColumnHeadersVisible--}
```
public boolean isRowColumnHeadersVisible()
```


Gibt einen Wert zurück, der angibt, ob das Arbeitsblatt Zeilen- und Spaltenüberschriften anzeigt. Standard ist true.

**Returns:**
boolean
### isRulerVisible() {#isRulerVisible--}
```
public boolean isRulerVisible()
```


Gibt an, ob das Lineal sichtbar ist. Diese Eigenschaft wird nur in der Seitenumbruchvorschau angewendet.

**Returns:**
boolean
### isSelected() {#isSelected--}
```
public boolean isSelected()
```


Gibt an, ob dieses Arbeitsblatt beim Öffnen der Arbeitsmappe ausgewählt ist.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Stellt dar, ob das Arbeitsblatt sichtbar ist.

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




### protect(int type) {#protect-int-}
```
public void protect(int type)
```


Schützt das Arbeitsblatt.

**Remarks**

Diese Methode schützt das Arbeitsblatt ohne Passwort. Sie kann das Arbeitsblatt in allen Excel-Dateiversionen schützen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| type | int | [ProtectionType](../../com.aspose.cells/protectiontype). Schutztyp. |

### protect(int type, String password, String oldPassword) {#protect-int-java.lang.String-java.lang.String-}
```
public void protect(int type, String password, String oldPassword)
```


Schützt das Arbeitsblatt.

**Remarks**

Diese Methode kann das Arbeitsblatt in allen Excel-Dateiversionen schützen.

**Example**

```
         //Instantiating a Workbook object
         Workbook excel = new Workbook("template.xlsx");
         //Accessing the first worksheet in the Excel file
         Worksheet worksheet = excel.getWorksheets().get(0);
         //Protecting the worksheet with a password
         worksheet.protect(ProtectionType.ALL, "aspose", null);
         //Saving the modified Excel file in default (that is Excel 20003) format
         excel.save("output.xls");
         //Closing the file stream to free all resources
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| type | int | [ProtectionType](../../com.aspose.cells/protectiontype). Schutztyp. |
| Passwort | java.lang.String | Passwort. |
| oldPassword | java.lang.String | Wenn das Arbeitsblatt bereits durch ein Passwort geschützt ist, geben Sie bitte das alte Passwort an. Andernfalls können Sie diesem Parameter einen Nullwert oder eine leere Zeichenfolge zuweisen. |

### refreshPivotTables() {#refreshPivotTables--}
```
public void refreshPivotTables()
```


Aktualisiert alle PivotTables in diesem Arbeitsblatt.

### refreshPivotTables(PivotTableRefreshOption option) {#refreshPivotTables-com.aspose.cells.PivotTableRefreshOption-}
```
public boolean refreshPivotTables(PivotTableRefreshOption option)
```


Aktualisiert alle PivotTables in diesem Arbeitsblatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) | Die Option zum Aktualisieren der Datenquelle der Pivot-Tabelle. |

**Returns:**
boolean
### removeAllDrawingObjects() {#removeAllDrawingObjects--}
```
public void removeAllDrawingObjects()
```


Entfernt alle Zeichenobjekte in diesem Arbeitsblatt.

### removeAutoFilter() {#removeAutoFilter--}
```
public void removeAutoFilter()
```


Entfernt den Auto-Filter des Arbeitsblatts.

### removeSplit() {#removeSplit--}
```
public void removeSplit()
```


Entfernt das geteilte Fenster.

### replace(String oldString, String newString) {#replace-java.lang.String-java.lang.String-}
```
public int replace(String oldString, String newString)
```


Ersetzt den Text aller Zellen durch eine neue Zeichenfolge.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| oldString | java.lang.String | Alter Zeichenfolgenwert. |
| newString | java.lang.String | Neuer Zeichenfolgenwert. |

**Returns:**
int
### selectRange(int startRow, int startColumn, int totalRows, int totalColumns, boolean removeOthers) {#selectRange-int-int-int-int-boolean-}
```
public void selectRange(int startRow, int startColumn, int totalRows, int totalColumns, boolean removeOthers)
```


Wählt einen Bereich aus.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | int | Die Startzeile. |
| startColumn | int | Die Startspalte |
| totalRows | int | Die Anzahl der Zeilen. |
| totalColumns | int | Die Anzahl der Spalten |
| removeOthers | boolean | True bedeutet, dass andere ausgewählte Bereiche entfernt werden und nur dieser Bereich ausgewählt wird. |

### setActiveCell(String value) {#setActiveCell-java.lang.String-}
```
public void setActiveCell(String value)
```


Setzt die aktive Zelle im Arbeitsblatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setBackgroundImage(byte[] value) {#setBackgroundImage-byte---}
```
public void setBackgroundImage(byte[] value)
```


Setzt das Hintergrundbild des Arbeitsblatts.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | byte[] |  |

### setCodeName(String value) {#setCodeName-java.lang.String-}
```
public void setCodeName(String value)
```


Liefert den Code‑Namen des Arbeitsblatts.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

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

### setGridlineColor(Color value) {#setGridlineColor-com.aspose.cells.Color-}
```
public void setGridlineColor(Color value)
```


Setzt die Farbe der Gitternetzlinie

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setGridlinesVisible(boolean value) {#setGridlinesVisible-boolean-}
```
public void setGridlinesVisible(boolean value)
```


Setzt einen Wert, der angibt, ob die Gitternetzlinien sichtbar sind. Standard ist wahr.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
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


Gibt an, ob die Gliederung angezeigt werden soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setPageBreakPreview(boolean value) {#setPageBreakPreview-boolean-}
```
public void setPageBreakPreview(boolean value)
```


Gibt an, ob das angegebene Arbeitsblatt in Normalansicht oder Seitenumbruchvorschau angezeigt wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setRowColumnHeadersVisible(boolean value) {#setRowColumnHeadersVisible-boolean-}
```
public void setRowColumnHeadersVisible(boolean value)
```


Legt einen Wert fest, der angibt, ob das Arbeitsblatt Zeilen- und Spaltenüberschriften anzeigt. Standard ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setRulerVisible(boolean value) {#setRulerVisible-boolean-}
```
public void setRulerVisible(boolean value)
```


Gibt an, ob das Lineal sichtbar ist. Diese Eigenschaft wird nur in der Seitenumbruchvorschau angewendet.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSelected(boolean value) {#setSelected-boolean-}
```
public void setSelected(boolean value)
```


Gibt an, ob dieses Arbeitsblatt beim Öffnen der Arbeitsmappe ausgewählt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowDataTypeIcons(boolean value) {#setShowDataTypeIcons-boolean-}
```
public void setShowDataTypeIcons(boolean value)
```


Gibt an, ob Datentyp‑Symbole angezeigt werden sollen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowFormulas(boolean value) {#setShowFormulas-boolean-}
```
public void setShowFormulas(boolean value)
```


Gibt an, ob Formeln oder deren Ergebnisse angezeigt werden sollen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setTabColor(Color value) {#setTabColor-com.aspose.cells.Color-}
```
public void setTabColor(Color value)
```


Stellt die Registerkartenfarbe des Arbeitsblatts dar.

**Remarks**

Dieses Feature wird nur in ExcelXP (Excel2002) und späteren Versionen unterstützt. Wenn Sie die Datei im Excel97- oder Excel2000-Format speichern, wird es weggelassen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setTabId(int value) {#setTabId-int-}
```
public void setTabId(int value)
```


Gibt den internen Bezeichner für das Blatt an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setTransitionEntry(boolean value) {#setTransitionEntry-boolean-}
```
public void setTransitionEntry(boolean value)
```


Gibt an, ob die Option Transition Formula Entry (Lotus‑Kompatibilität) aktiviert ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setTransitionEvaluation(boolean value) {#setTransitionEvaluation-boolean-}
```
public void setTransitionEvaluation(boolean value)
```


Gibt an, ob die Option Transition Formula Evaluation (Lotus‑Kompatibilität) aktiviert ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Stellt den Arbeitsblatttyp dar.

Siehe [SheetType](../../com.aspose.cells/sheettype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setUniqueId(String value) {#setUniqueId-java.lang.String-}
```
public void setUniqueId(String value)
```


Legt die eindeutige ID fest, sie ist dieselbe wie \{15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F\}.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setViewType(int value) {#setViewType-int-}
```
public void setViewType(int value)
```


Legt den Ansichtstyp fest.

Siehe [ViewType](../../com.aspose.cells/viewtype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setVisibilityType(int value) {#setVisibilityType-int-}
```
public void setVisibilityType(int value)
```


Gibt den sichtbaren Zustand dieses Blatts an.

Siehe [VisibilityType](../../com.aspose.cells/visibilitytype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Stellt dar, ob das Arbeitsblatt sichtbar ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setVisible(boolean isVisible, boolean ignoreError) {#setVisible-boolean-boolean-}
```
public void setVisible(boolean isVisible, boolean ignoreError)
```


Legt die sichtbaren Optionen fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isVisible | boolean | Ob das Arbeitsblatt sichtbar ist |
| ignoreError | boolean | Ob ein Fehler ignoriert werden soll, wenn diese Option ungültig ist. |

### setZoom(int value) {#setZoom-int-}
```
public void setZoom(int value)
```


Stellt den Skalierungsfaktor in Prozent dar. Er sollte zwischen 10 und 400 liegen.

**Remarks**

Bitte setzen Sie zuerst den Ansichtstyp.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### split() {#split--}
```
public void split()
```


Teilt das Fenster.

### startAccessCache(int opts) {#startAccessCache-int-}
```
public void startAccessCache(int opts)
```


Startet die Sitzung, die Caches verwendet, um auf die Daten in diesem Arbeitsblatt zuzugreifen.

**Remarks**

Nachdem der Zugriff auf die Daten abgeschlossen ist, sollte [closeAccessCache(int)](../../com.aspose.cells/worksheet\#closeAccessCache-int-) mit denselben Optionen aufgerufen werden, um alle Caches zu leeren und den normalen Zugriffsmodus wiederherzustellen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| opts | int | [AccessCacheOptions](../../com.aspose.cells/accesscacheoptions). Optionen für den Datenzugriff |

### toString() {#toString--}
```
public String toString()
```


Gibt einen String zurück, der das aktuelle Arbeitsblatt-Objekt darstellt.

**Returns:**
java.lang.String -
### unFreezePanes() {#unFreezePanes--}
```
public void unFreezePanes()
```


Löst das Einfrieren von Bereichen im Arbeitsblatt.

### unprotect() {#unprotect--}
```
public void unprotect()
```


Entfernt den Schutz des Arbeitsblatts.

**Remarks**

Diese Methode hebt den Schutz des Arbeitsblatts auf, das ohne Passwort geschützt ist.

### unprotect(String password) {#unprotect-java.lang.String-}
```
public void unprotect(String password)
```


Entfernt den Schutz des Arbeitsblatts.

**Remarks**

Wenn das Arbeitsblatt ohne Passwort geschützt ist, können Sie dem Passwortparameter einen Nullwert oder eine leere Zeichenfolge zuweisen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Passwort | java.lang.String | Passwort |

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

### xmlMapQuery(String path, XmlMap xmlMap) {#xmlMapQuery-java.lang.String-com.aspose.cells.XmlMap-}
```
public ArrayList xmlMapQuery(String path, XmlMap xmlMap)
```


Abfrage von Zellbereichen, die mit dem spezifischen Pfad der XML‑Map verknüpft/verbunden sind.

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Methode Worksheet.GetAreasOfXmlMapQuery(). Diese Eigenschaft wird 12 Monate nach August 2026 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Pfad | java.lang.String | XML-Elementpfad |
| xmlMap | [XmlMap](../../com.aspose.cells/xmlmap) | Geben Sie eine XML-Karte an, wenn Sie den spezifischen Pfad innerhalb einer bestimmten Karte abfragen möchten. |

**Returns:**
java.util.ArrayList - [CellArea](../../com.aspose.cells/cellarea)-Liste, die dem spezifischen Pfad der XML‑Map zugeordnet/verbunden ist; eine leere Liste wird zurückgegeben, wenn nichts zugeordnet/verbunden ist.
