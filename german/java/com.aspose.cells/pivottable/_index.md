---
title: "PivotTable"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Zusammenfassende Beschreibung für PivotTable."
type: docs
url: /de/java/com.aspose.cells/pivottable/
---

**Inheritance:**
java.lang.Object
```
public class PivotTable
```

Zusammenfassende Beschreibung für PivotTable.

**Example**

```
         Workbook book = new Workbook();
         Worksheet sheet = book.getWorksheets().get(0);
         Cells cells = sheet.getCells();
         cells.get(0, 0).setValue("fruit");
         cells.get(1, 0).setValue("grape");
         cells.get(2, 0).setValue("blueberry");
         cells.get(3, 0).setValue("kiwi");
         cells.get(4, 0).setValue("cherry");
         cells.get(5, 0).setValue("grape");
         cells.get(6, 0).setValue("blueberry");
         cells.get(7, 0).setValue("kiwi");
         cells.get(8, 0).setValue("cherry");
 
         cells.get(0, 1).setValue("year");
         cells.get(1, 1).setValue(2020);
         cells.get(2, 1).setValue(2020);
         cells.get(3, 1).setValue(2020);
         cells.get(4, 1).setValue(2020);
         cells.get(5, 1).setValue(2021);
         cells.get(6, 1).setValue(2021);
         cells.get(7, 1).setValue(2021);
         cells.get(8, 1).setValue(2021);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
         cells.get(5, 2).setValue(90);
         cells.get(6, 2).setValue(100);
         cells.get(7, 2).setValue(110);
         cells.get(8, 2).setValue(120);
 
         PivotTableCollection pivots = sheet.getPivotTables();
 
         PivotTable pivot = pivots.add("=Sheet1!A1:C9", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
 
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         //Change PivotField's attributes
         PivotField rowField = pivot.getRowFields().get(0);
         rowField.setDisplayName("custom display name");
 
         //Add PivotFilter
         PivotFilter filter = pivot.getRowFields().get(0).filterTop10(0, PivotFilterType.PERCENT, false, 2);
 
 
         //Add PivotFormatCondition
         int formatIndex = pivot.getConditionalFormats().add();
         PivotConditionalFormat pfc = pivot.getConditionalFormats().get(formatIndex);
         pfc.addCellArea(pivot.getDataBodyRange());
         FormatConditionCollection fcc = pfc.getFormatConditions();
         int ii = fcc.addCondition(FormatConditionType.CELL_VALUE, OperatorType.GREATER_OR_EQUAL, "100", null);
 
         FormatCondition fc = fcc.get(ii);
 
         fc.getStyle().setBackgroundColor(Color.getRed());
 
          PivotTableCalculateOption calculateOption = new PivotTableCalculateOption();
          calculateOption.setRefreshData(true);
          calculateOption.setRefreshCharts(true);
          pivot.calculateData(calculateOption); 
 
         //do your business
 
         book.save("out.xlsx");
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [addCalculatedField(String name, String formula)](#addCalculatedField-java.lang.String-java.lang.String-) | Fügt ein berechnetes Feld zum Pivot-Feld hinzu und zieht es in den Datenbereich. |
| [addCalculatedField(String name, String formula, boolean dragToDataArea)](#addCalculatedField-java.lang.String-java.lang.String-boolean-) | Fügt ein berechnetes Feld zum Pivot-Feld hinzu. |
| [addFieldToArea(int fieldType, PivotField pivotField)](#addFieldToArea-int-com.aspose.cells.PivotField-) | Fügt das Feld zum spezifischen Bereich hinzu. |
| [addFieldToArea(int fieldType, int baseFieldIndex)](#addFieldToArea-int-int-) | Fügt das Feld zum spezifischen Bereich hinzu. |
| [addFieldToArea(int fieldType, String fieldName)](#addFieldToArea-int-java.lang.String-) | Fügt das Feld zum spezifischen Bereich hinzu. |
| [calculateData()](#calculateData--) | Berechnet Daten der PivotTable in Zellen. |
| [calculateData(PivotTableCalculateOption option)](#calculateData-com.aspose.cells.PivotTableCalculateOption-) | Berechnet die PivotTable mit Optionen. |
| [calculateRange()](#calculateRange--) | Berechnet den Bereich der PivotTable. |
| [changeDataSource(String[] source)](#changeDataSource-java.lang.String---) | Ändere die Datenquelle der PivotTable. |
| [clearAll()](#clearAll--) | Entferne alle Felder aus Regionen. |
| [clearData()](#clearData--) | Lösche Daten und Formatierung der PivotTable-Ansicht. |
| [clearFilters()](#clearFilters--) | Löscht alle Filter dieser PivotTable. |
| [copyStyle(PivotTable pivotTable)](#copyStyle-com.aspose.cells.PivotTable-) | Kopiert benannten Stil von einer anderen Pivot-Tabelle. |
| [dispose()](#dispose--) | Führt anwendungsspezifische Aufgaben aus, die mit dem Freigeben, Freisetzen oder Zurücksetzen nicht verwalteter Ressourcen verbunden sind. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportViewToJson(PivotViewToJsonOptions options)](#exportViewToJson-com.aspose.cells.PivotViewToJsonOptions-) | Exportiert die Pivot-Ansicht als JSON. |
| [fields(int fieldType)](#fields-int-) | Ruft die spezifischen Felder nach dem Feldtyp ab. |
| [format(CellArea ca, Style style)](#format-com.aspose.cells.CellArea-com.aspose.cells.Style-) | Formatiert den ausgewählten Bereich der Pivot-Tabelle. |
| [format(PivotArea pivotArea, Style style)](#format-com.aspose.cells.PivotArea-com.aspose.cells.Style-) | Formatiert den ausgewählten Bereich der Pivot-Tabelle. |
| [format(int row, int column, Style style)](#format-int-int-com.aspose.cells.Style-) | Formatiert die Zelle im Pivot-Tabellenbereich |
| [formatAll(Style style)](#formatAll-com.aspose.cells.Style-) | Formatiert alle Zellen im Pivot-Tabellenbereich |
| [formatRow(int row, Style style)](#formatRow-int-com.aspose.cells.Style-) | Formatiert die Zeilendaten im Pivot-Tabellenbereich |
| [getAllowMultipleFiltersPerField()](#getAllowMultipleFiltersPerField--) | Gibt einen booleschen Wert an, der angibt, ob die Felder einer Pivot-Tabelle mehrere Filter haben können. |
| [getAltTextDescription()](#getAltTextDescription--) | Ruft die Beschreibung des Alternativtexts ab. |
| [getAltTextTitle()](#getAltTextTitle--) | Ruft den Titel des Alternativtexts ab. |
| [getAutoFormatType()](#getAutoFormatType--) | Ruft den Autoformattyp der Pivot-Tabelle ab. |
| [getAutofitColumnWidthOnUpdate()](#getAutofitColumnWidthOnUpdate--) | Gibt an, ob die Spaltenbreite bei Aktualisierung automatisch angepasst werden soll |
| [getBaseFields()](#getBaseFields--) | Gibt alle Basis-Pivot-Felder in der Pivot-Tabelle zurück. |
| [getButtonArea(int axisType)](#getButtonArea-int-) | Ruft den Bereich ab, der die Feldschaltfläche enthält. |
| [getCellByDisplayName(String displayName)](#getCellByDisplayName-java.lang.String-) | Ruft das [Cell](../../com.aspose.cells/cell)-Objekt anhand des Anzeigenamens des PivotField ab. |
| [getChildren()](#getChildren--) | Ruft die untergeordneten Pivot-Tabellen ab, die diese Pivot-Tabellendaten als Datenquelle verwenden. |
| [getClass()](#getClass--) |  |
| [getColumnFields()](#getColumnFields--) | Gibt ein PivotFields-Objekt zurück, das derzeit als Spaltenfelder angezeigt wird. |
| [getColumnGrand()](#getColumnGrand--) | Gibt an, ob der Pivot-Tabellenbericht Gesamtsummen für Spalten anzeigt. |
| [getColumnHeaderCaption()](#getColumnHeaderCaption--) | Ruft die benutzerdefinierte Beschriftung der Spaltenüberschrift der Pivot-Tabelle ab. |
| [getColumnRange()](#getColumnRange--) | Gibt ein CellArea-Objekt zurück, das den Bereich darstellt, der den Spaltenbereich im Pivot-Tabellenbericht enthält. |
| [getConditionalFormats()](#getConditionalFormats--) | Ruft die bedingten Formate der Pivot-Tabelle ab. |
| [getCustomListSort()](#getCustomListSort--) | Gibt an, ob beim Sortieren von Daten die integrierte benutzerdefinierte Liste berücksichtigt wird. |
| [getDataBodyRange()](#getDataBodyRange--) | Gibt ein [CellArea](../../com.aspose.cells/cellarea)-Objekt zurück, das den Bereich darstellt, der den Datenbereich in der Liste zwischen der Kopfzeile und der Einfügezeile enthält. |
| [getDataField()](#getDataField--) | Ruft ein [PivotField](../../com.aspose.cells/pivotfield)-Objekt ab, das alle Datenfelder in einer Pivot-Tabelle darstellt. |
| [getDataFieldHeaderName()](#getDataFieldHeaderName--) | Ermittelt den Namen der Feldkopfzeile des Wertebereichs in der PivotTable. |
| [getDataFields()](#getDataFields--) | Ermittelt eine [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection), die alle Datenfelder in einer PivotTable darstellt. |
| [getDataSource()](#getDataSource--) | Ermittelt die Datenquelle der PivotTable. |
| [getDependentPivotTables()](#getDependentPivotTables--) | Ermittelt alle [PivotTable](../../com.aspose.cells/pivottable)s, die diese PivotTable als Datenquelle verwenden. |
| [getDisplayErrorString()](#getDisplayErrorString--) | Gibt an, ob der PivotTable-Bericht in Zellen, die Fehler enthalten, einen benutzerdefinierten Text anzeigt. |
| [getDisplayImmediateItems()](#getDisplayImmediateItems--) | Gibt an, ob Elemente in den Zeilen- und Spaltenbereichen sichtbar sind, wenn der Datenbereich der PivotTable leer ist. |
| [getDisplayNullString()](#getDisplayNullString--) | Gibt an, ob der PivotTable-Bericht einen benutzerdefinierten Text anzeigt, wenn der Wert null ist. |
| [getEnableDataValueEditing()](#getEnableDataValueEditing--) | Gibt einen booleschen Wert an, der festlegt, ob der Benutzer die Zellen im Datenbereich der PivotTable bearbeiten darf. |
| [getEnableDrilldown()](#getEnableDrilldown--) | Gibt an, ob Drilldown aktiviert ist. |
| [getEnableFieldDialog()](#getEnableFieldDialog--) | Gibt an, ob das Dialogfeld PivotTable-Feld verfügbar ist, wenn der Benutzer das PivotTable-Feld doppelklickt. |
| [getEnableFieldList()](#getEnableFieldList--) | Gibt an, ob die Feldliste für die PivotTable in der Excel-Ansicht verfügbar ist. |
| [getEnableWizard()](#getEnableWizard--) | Gibt an, ob der PivotTable-Assistent verfügbar ist. |
| [getErrorString()](#getErrorString--) | Ermittelt den Text, der in Zellen angezeigt wird, die Fehler enthalten, wenn die Eigenschaft DisplayErrorString true ist. Der Standardwert ist ein leerer String. |
| [getExternalConnectionDataSource()](#getExternalConnectionDataSource--) | Ermittelt die externe Verbindungsdatenquelle. |
| [getFieldListSortAscending()](#getFieldListSortAscending--) | Gibt an, ob Felder in der PivotTable in der Feldliste in einer nicht standardmäßigen Reihenfolge sortiert sind. |
| [getFields(int fieldType)](#getFields-int-) | Ermittelt die spezifische Pivot-Feldliste nach Region. |
| [getFilterArea()](#getFilterArea--) | Ermittelt den Bereich der Filterregion. |
| [getGrandTotalName()](#getGrandTotalName--) | Gibt die Beschriftung zurück, die in der Spalten- oder Zeilenüberschrift der Gesamtsumme angezeigt wird. |
| [getHorizontalBreaks()](#getHorizontalBreaks--) | Ermittelt die Zeilenindexliste der PivotTable für horizontale Seitenumbrüche |
| [getHorizontalPageBreaks()](#getHorizontalPageBreaks--) | Ermittelt die horizontalen Seitenumbrüche dieser PivotTable. |
| [getIndent()](#getIndent--) | Gibt die Einrückungssteigerung für die kompakte Achse an und kann verwendet werden, um das Berichtslayout auf kompakte Form einzustellen. |
| [getItemPrintTitles()](#getItemPrintTitles--) | Gibt an, ob PivotItem-Namen oben auf jeder gedruckten Seite wiederholt werden sollen. |
| [getManualUpdate()](#getManualUpdate--) | Gibt an, ob der PivotTable-Bericht nur auf Anforderung des Benutzers neu berechnet wird. |
| [getMergeLabels()](#getMergeLabels--) | Ermittelt, ob Zeilen-/Spaltenfeldbeschriftungen, die mehrere Zellen umfassen, zusammengeführt werden sollen. |
| [getMissingItemsLimit()](#getMissingItemsLimit--) | Gibt einen booleschen Wert an, der angibt, ob die Felder einer Pivot-Tabelle mehrere Filter haben können. |
| [getName()](#getName--) | Ermittelt den Namen der PivotTable |
| [getNamesOfSourceDataConnections()](#getNamesOfSourceDataConnections--) | Ruft die Namen von externen Quell-Datenverbindungen ab. |
| [getNullString()](#getNullString--) | Ruft die Zeichenkette ab, die in Zellen angezeigt wird, die Nullwerte enthalten, wenn die Eigenschaft DisplayNullString true ist. Der Standardwert ist eine leere Zeichenkette. |
| [getPageFieldOrder()](#getPageFieldOrder--) | Ruft die Reihenfolge ab, in der Seitenfelder zum Layout des PivotTable-Berichts hinzugefügt werden. |
| [getPageFieldWrapCount()](#getPageFieldWrapCount--) | Ruft die Anzahl der Seitenfelder in jeder Spalte oder Zeile im PivotTable-Bericht ab. |
| [getPageFields()](#getPageFields--) | Gibt eine [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) zurück, die derzeit als Seitenfelder angezeigt werden. |
| [getPivotCache()](#getPivotCache--) | Ruft die Datenquelle ab. |
| [getPivotFilters()](#getPivotFilters--) | Gibt alle Filter in der Pivot-Tabelle zurück. |
| [getPivotFormatConditions()](#getPivotFormatConditions--) | Ruft die Formatbedingungen der Pivot-Tabelle ab. |
| [getPivotFormats()](#getPivotFormats--) | Ruft alle Zellformate ab, die auf diese Pivot-Tabelle angewendet wurden. |
| [getPivotTableStyle()](#getPivotTableStyle--) | Ruft die [TableStyle](../../com.aspose.cells/tablestyle)-Einstellungen dieser Pivot-Tabelle ab. |
| [getPivotTableStyleName()](#getPivotTableStyleName--) | Ruft den Stilnamen der Pivot-Tabelle ab. |
| [getPivotTableStyleType()](#getPivotTableStyleType--) | Ruft den integrierten Pivot-Tabellenstil ab. |
| [getPivotTablesWithSamePivotCache()](#getPivotTablesWithSamePivotCache--) | Ruft alle Pivot-Tabellen mit demselben Pivot-Cache ab. |
| [getPreserveCellFormattingOnUpdate()](#getPreserveCellFormattingOnUpdate--) | Gibt an, ob die Zellformatierung ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) beibehalten werden soll, wenn die Pivot-Tabelle aktualisiert oder neu berechnet wird. |
| [getPreserveFormatting()](#getPreserveFormatting--) | Gibt an, ob die Zellformatierung ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) beibehalten wird, wenn die PivotTable aktualisiert oder neu berechnet wird. |
| [getPrintDrill()](#getPrintDrill--) | Gibt einen booleschen Wert an, der angibt, ob Drill-Indikatoren gedruckt werden sollen. |
| [getPrintTitles()](#getPrintTitles--) | Gibt an, ob die Drucktitel für das Arbeitsblatt basierend auf dem PivotTable-Bericht festgelegt sind. |
| [getRefreshDataOnOpeningFile()](#getRefreshDataOnOpeningFile--) | Gibt an, ob Daten beim Öffnen der Datei aktualisiert werden. |
| [getRefreshDate()](#getRefreshDate--) | Ruft das letzte Datum und die Uhrzeit ab, zu der die PivotTable aktualisiert wurde. |
| [getRefreshedByWho()](#getRefreshedByWho--) | Ruft den Namen des letzten Benutzers ab, der diese PivotTable aktualisiert hat. |
| [getRepeatItemsOnEachPrintedPage()](#getRepeatItemsOnEachPrintedPage--) | Gibt an, ob Beschriftungen von Pivot-Elementen im Zeilenbereich auf jeder gedruckten Seite für Pivot-Felder in Tabellenform wiederholt werden. |
| [getRowFields()](#getRowFields--) | Gibt eine [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) zurück, die derzeit als Zeilenfelder angezeigt werden. |
| [getRowGrand()](#getRowGrand--) | Gibt an, ob Gesamtsummen für Zeilen dieser Pivot-Tabelle angezeigt werden sollen. |
| [getRowHeaderCaption()](#getRowHeaderCaption--) | Ruft die benutzerdefinierte Beschriftung der Zeilenüberschrift in dieser PivotTable ab. |
| [getRowRange()](#getRowRange--) | Gibt ein CellArea-Objekt zurück, das den Bereich darstellt, der den Zeilenbereich im PivotTable-Bericht enthält. |
| [getSaveData()](#getSaveData--) | Gibt an, ob Daten für den PivotTable-Bericht mit der Arbeitsmappe gespeichert werden. |
| [getShowColumnGrandTotals()](#getShowColumnGrandTotals--) | Gibt an, ob Gesamtsummen für die Spalten dieser PivotTable angezeigt werden. |
| [getShowDataTips()](#getShowDataTips--) | Gibt an, ob Tooltips für PivotTable-Datenzellen angezeigt werden sollen. |
| [getShowDrill()](#getShowDrill--) | Ermittelt, ob Expand/Collapse-Schaltflächen angezeigt werden. |
| [getShowEmptyCol()](#getShowEmptyCol--) | Gibt an, ob leere Spalten in die Tabelle aufgenommen werden sollen. |
| [getShowEmptyRow()](#getShowEmptyRow--) | Gibt an, ob leere Zeilen in die Tabelle aufgenommen werden sollen. |
| [getShowHeaders()](#getShowHeaders--) | Ob Datenfeldbeschriftungen und Pivotfeldbeschriftungen auf der Zeilen‑ und Spaltenachse in der PivotTable‑Ansicht angezeigt werden. |
| [getShowMemberPropertyTips()](#getShowMemberPropertyTips--) | Gibt einen booleschen Wert an, der festlegt, ob Mitgliedseigenschaftsinformationen aus PivotTable-Tooltips weggelassen werden sollen. |
| [getShowPivotStyleColumnHeader()](#getShowPivotStyleColumnHeader--) | Gibt an, ob die Spaltenüberschrift in der PivotTable den Stil erhalten soll. |
| [getShowPivotStyleColumnStripes()](#getShowPivotStyleColumnStripes--) | Gibt an, ob für die Spalte Streifenformatierung angewendet wird. |
| [getShowPivotStyleLastColumn()](#getShowPivotStyleLastColumn--) | Gibt an, ob die Spaltenformatierung angewendet wird. |
| [getShowPivotStyleRowHeader()](#getShowPivotStyleRowHeader--) | Gibt an, ob die Zeilenüberschrift in der PivotTable den Stil erhalten soll. |
| [getShowPivotStyleRowStripes()](#getShowPivotStyleRowStripes--) | Gibt an, ob Zeilenstreifenformatierung angewendet wird. |
| [getShowRowGrandTotals()](#getShowRowGrandTotals--) | Gibt an, ob Gesamtsummen für die Zeilen der PivotTable angezeigt werden sollen. |
| [getShowRowHeaderCaption()](#getShowRowHeaderCaption--) | Gibt an, ob die Zeilenüberschriftsbeschriftung im PivotTable-Bericht angezeigt wird. Gibt an, ob Feldbeschriftungen und Filter‑Dropdowns angezeigt werden. |
| [getShowValuesRow()](#getShowValuesRow--) | Gibt an, ob die Wertezeile angezeigt wird. |
| [getSource()](#getSource--) | Ruft die Datenquelle dieser PivotTable ab. |
| [getSource(boolean isOriginal)](#getSource-boolean-) | Ruft die Datenquelle dieser PivotTable ab. |
| [getSourceDataConnections()](#getSourceDataConnections--) | Ermittelt die externen Verbindungsdatenquellen. |
| [getSourceType()](#getSourceType--) | Ermittelt den Datentyp der Datenquelle der PivotTable. |
| [getSubtotalHiddenPageItems()](#getSubtotalHiddenPageItems--) | Gibt an, ob versteckte Seitenfeld‑Elemente im PivotTable-Bericht in Zeilen‑ und Spaltensummen, Blocksummen und Gesamtsummen einbezogen werden. |
| [getTableRange1()](#getTableRange1--) | Gibt ein CellArea‑Objekt zurück, das den Bereich darstellt, der den gesamten PivotTable-Bericht enthält, jedoch keine Seitenfelder einschließt. |
| [getTableRange2()](#getTableRange2--) | Gibt ein CellArea‑Objekt zurück, das den Bereich darstellt, der den gesamten PivotTable-Bericht einschließlich Seitenfelder enthält. |
| [getTag()](#getTag--) | Ermittelt einen benutzerdefinierten String, der mit dieser PivotTable‑Ansicht verknüpft ist. |
| [getTopRightArea()](#getTopRightArea--) | Stellt den leeren Bereich oben rechts der PivotTable dar (oben links für RTL‑Blätter). |
| [getValuesField()](#getValuesField--) | Ruft ein [PivotField](../../com.aspose.cells/pivotfield)-Objekt ab, das alle Datenfelder in einer Pivot-Tabelle darstellt. |
| [hasBlankRows()](#hasBlankRows--) | Gibt an, ob leere Zeilen hinzugefügt werden sollen. |
| [hashCode()](#hashCode--) |  |
| [isAutoFormat()](#isAutoFormat--) | Gibt an, ob der PivotTable-Bericht automatisch formatiert wird. |
| [isExcel2003Compatible()](#isExcel2003Compatible--) | Gibt an, ob die PivotTable bei der Aktualisierung mit Excel2003 kompatibel ist; wenn true, muss ein String höchstens 255 Zeichen lang sein, sodass ein längerer String abgeschnitten wird. Wenn false, gilt die oben genannte Einschränkung nicht. |
| [isGridDropZones()](#isGridDropZones--) | Gibt an, ob der PivotTable-Bericht das klassische PivotTable-Layout anzeigt. |
| [isMultipleFieldFilters()](#isMultipleFieldFilters--) | Gibt einen booleschen Wert an, der angibt, ob die Felder einer Pivot-Tabelle mehrere Filter haben können. |
| [isSelected()](#isSelected--) | Gibt an, ob diese PivotTable ausgewählt ist. |
| [move(int row, int column)](#move-int-int-) | Verschiebt die PivotTable an eine andere Position im Arbeitsblatt. |
| [move(String destCellName)](#move-java.lang.String-) | Verschiebt die PivotTable an eine andere Position im Arbeitsblatt. |
| [moveItem(int region, String[] nodes, boolean absolute, int offset)](#moveItem-int-java.lang.String---boolean-int-) | Verschiebt ein Element nach oben oder unten. |
| [moveTo(int row, int column)](#moveTo-int-int-) | Verschiebt die PivotTable an eine andere Position im Arbeitsblatt. |
| [moveTo(int sheetIndex, int row, int column)](#moveTo-int-int-int-) | Verschiebt die PivotTable an eine andere Position im Arbeitsblatt. |
| [moveTo(String destCellName)](#moveTo-java.lang.String-) | Verschiebt die PivotTable an eine andere Position im Arbeitsblatt. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refresh()](#refresh--) | Aktualisiert [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) aus der Datenquelle und berechnet Daten und Stil für die Pivot-Ansicht. |
| [refresh(PivotTableRefreshOption option)](#refresh-com.aspose.cells.PivotTableRefreshOption-) | Aktualisiert [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) aus der Datenquelle und berechnet Daten und Stil für die Pivot-Ansicht. |
| [refreshData()](#refreshData--) | Aktualisiert Daten aus seiner Datenquelle in den Pivot-Cache. |
| [refreshData(PivotTableRefreshOption option)](#refreshData-com.aspose.cells.PivotTableRefreshOption-) | Aktualisiert die Daten und Einstellungen der PivotTable aus seiner Datenquelle mit Optionen. |
| [removeField(int fieldType, PivotField pivotField)](#removeField-int-com.aspose.cells.PivotField-) | Feld aus einem bestimmten Feldbereich entfernen |
| [removeField(int fieldType, int baseFieldIndex)](#removeField-int-int-) | Entfernt ein Feld aus einem bestimmten Pivot-Bereich. |
| [removeField(int fieldType, String fieldName)](#removeField-int-java.lang.String-) | Entfernt ein Feld aus einem bestimmten Feldbereich. |
| [selectArea(CellArea ca)](#selectArea-com.aspose.cells.CellArea-) | Wählt einen Bereich der PivotTable-Ansicht aus. |
| [setAllowMultipleFiltersPerField(boolean value)](#setAllowMultipleFiltersPerField-boolean-) | Gibt einen booleschen Wert an, der angibt, ob die Felder einer Pivot-Tabelle mehrere Filter haben können. |
| [setAltTextDescription(String value)](#setAltTextDescription-java.lang.String-) | Ruft die Beschreibung des Alternativtexts ab. |
| [setAltTextTitle(String value)](#setAltTextTitle-java.lang.String-) | Legt den Titel des alternativen Textes fest. |
| [setAutoFormat(boolean value)](#setAutoFormat-boolean-) | Gibt an, ob der PivotTable-Bericht automatisch formatiert wird. |
| [setAutoFormatType(int value)](#setAutoFormatType-int-) | Legt den automatischen Formattyp der PivotTable fest. |
| [setAutofitColumnWidthOnUpdate(boolean value)](#setAutofitColumnWidthOnUpdate-boolean-) | Gibt an, ob die Spaltenbreite bei Aktualisierung automatisch angepasst werden soll |
| [setColumnGrand(boolean value)](#setColumnGrand-boolean-) | Gibt an, ob der Pivot-Tabellenbericht Gesamtsummen für Spalten anzeigt. |
| [setColumnHeaderCaption(String value)](#setColumnHeaderCaption-java.lang.String-) | Legt die benutzerdefinierte Beschriftung der Spaltenüberschrift der PivotTable fest. |
| [setCustomListSort(boolean value)](#setCustomListSort-boolean-) | Gibt an, ob beim Sortieren von Daten die integrierte benutzerdefinierte Liste berücksichtigt wird. |
| [setDataFieldHeaderName(String value)](#setDataFieldHeaderName-java.lang.String-) | Legt den Namen der Feldüberschrift des Wertebereichs in der PivotTable fest. |
| [setDataSource(String[] value)](#setDataSource-java.lang.String---) | Legt die Datenquelle der PivotTable fest. |
| [setDisplayErrorString(boolean value)](#setDisplayErrorString-boolean-) | Gibt an, ob der PivotTable-Bericht in Zellen, die Fehler enthalten, einen benutzerdefinierten Text anzeigt. |
| [setDisplayImmediateItems(boolean value)](#setDisplayImmediateItems-boolean-) | Gibt an, ob Elemente in den Zeilen- und Spaltenbereichen sichtbar sind, wenn der Datenbereich der PivotTable leer ist. |
| [setDisplayNullString(boolean value)](#setDisplayNullString-boolean-) | Gibt an, ob der PivotTable-Bericht einen benutzerdefinierten Text anzeigt, wenn der Wert null ist. |
| [setEnableDataValueEditing(boolean value)](#setEnableDataValueEditing-boolean-) | Gibt einen booleschen Wert an, der festlegt, ob der Benutzer die Zellen im Datenbereich der PivotTable bearbeiten darf. |
| [setEnableDrilldown(boolean value)](#setEnableDrilldown-boolean-) | Gibt an, ob Drilldown aktiviert ist. |
| [setEnableFieldDialog(boolean value)](#setEnableFieldDialog-boolean-) | Gibt an, ob das Dialogfeld PivotTable-Feld verfügbar ist, wenn der Benutzer das PivotTable-Feld doppelklickt. |
| [setEnableFieldList(boolean value)](#setEnableFieldList-boolean-) | Gibt an, ob die Feldliste für die PivotTable in der Excel-Ansicht verfügbar ist. |
| [setEnableWizard(boolean value)](#setEnableWizard-boolean-) | Gibt an, ob der PivotTable-Assistent verfügbar ist. |
| [setErrorString(String value)](#setErrorString-java.lang.String-) | Ermittelt den Text, der in Zellen angezeigt wird, die Fehler enthalten, wenn die Eigenschaft DisplayErrorString true ist. Der Standardwert ist ein leerer String. |
| [setExcel2003Compatible(boolean value)](#setExcel2003Compatible-boolean-) | Gibt an, ob die PivotTable bei der Aktualisierung mit Excel2003 kompatibel ist; wenn true, muss ein String höchstens 255 Zeichen lang sein, sodass ein längerer String abgeschnitten wird. Wenn false, gilt die oben genannte Einschränkung nicht. |
| [setFieldListSortAscending(boolean value)](#setFieldListSortAscending-boolean-) | Gibt an, ob Felder in der PivotTable in der Feldliste in einer nicht standardmäßigen Reihenfolge sortiert sind. |
| [setGrandTotalName(String value)](#setGrandTotalName-java.lang.String-) | Gibt die Beschriftung zurück, die in der Spalten- oder Zeilenüberschrift der Gesamtsumme angezeigt wird. |
| [setGridDropZones(boolean value)](#setGridDropZones-boolean-) | Gibt an, ob der PivotTable-Bericht das klassische PivotTable-Layout anzeigt. |
| [setHasBlankRows(boolean value)](#setHasBlankRows-boolean-) | Gibt an, ob leere Zeilen hinzugefügt werden sollen. |
| [setIndent(int value)](#setIndent-int-) | Gibt die Einrückungssteigerung für die kompakte Achse an und kann verwendet werden, um das Berichtslayout auf kompakte Form einzustellen. |
| [setItemPrintTitles(boolean value)](#setItemPrintTitles-boolean-) | Gibt an, ob PivotItem-Namen oben auf jeder gedruckten Seite wiederholt werden sollen. |
| [setManualUpdate(boolean value)](#setManualUpdate-boolean-) | Gibt an, ob der PivotTable-Bericht nur auf Anforderung des Benutzers neu berechnet wird. |
| [setMergeLabels(boolean value)](#setMergeLabels-boolean-) | Legt fest, ob Zeilen-/Spaltenfeldbeschriftungen, die sich über mehrere Zellen erstrecken, zusammengeführt werden. |
| [setMissingItemsLimit(int value)](#setMissingItemsLimit-int-) | Gibt einen booleschen Wert an, der angibt, ob die Felder einer Pivot-Tabelle mehrere Filter haben können. |
| [setMultipleFieldFilters(boolean value)](#setMultipleFieldFilters-boolean-) | Gibt einen booleschen Wert an, der angibt, ob die Felder einer Pivot-Tabelle mehrere Filter haben können. |
| [setName(String value)](#setName-java.lang.String-) | Ermittelt den Namen der PivotTable |
| [setNullString(String value)](#setNullString-java.lang.String-) | Ruft die Zeichenkette ab, die in Zellen angezeigt wird, die Nullwerte enthalten, wenn die Eigenschaft DisplayNullString true ist. Der Standardwert ist eine leere Zeichenkette. |
| [setPageFieldOrder(int value)](#setPageFieldOrder-int-) | Legt die Reihenfolge fest, in der Seitenfelder zum Layout des PivotTable-Berichts hinzugefügt werden. |
| [setPageFieldWrapCount(int value)](#setPageFieldWrapCount-int-) | Ruft die Anzahl der Seitenfelder in jeder Spalte oder Zeile im PivotTable-Bericht ab. |
| [setPivotTableStyle(TableStyle value)](#setPivotTableStyle-com.aspose.cells.TableStyle-) | Ruft die [TableStyle](../../com.aspose.cells/tablestyle)-Einstellungen dieser Pivot-Tabelle ab. |
| [setPivotTableStyleName(String value)](#setPivotTableStyleName-java.lang.String-) | Legt den Stilnamen der PivotTable fest. |
| [setPivotTableStyleType(int value)](#setPivotTableStyleType-int-) | Legt den integrierten PivotTable-Stil fest. |
| [setPreserveCellFormattingOnUpdate(boolean value)](#setPreserveCellFormattingOnUpdate-boolean-) | Gibt an, ob die Zellformatierung ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) beibehalten werden soll, wenn die Pivot-Tabelle aktualisiert oder neu berechnet wird. |
| [setPreserveFormatting(boolean value)](#setPreserveFormatting-boolean-) | Gibt an, ob die Zellformatierung ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) beibehalten wird, wenn die PivotTable aktualisiert oder neu berechnet wird. |
| [setPrintDrill(boolean value)](#setPrintDrill-boolean-) | Gibt einen booleschen Wert an, der angibt, ob Drill-Indikatoren gedruckt werden sollen. |
| [setPrintTitles(boolean value)](#setPrintTitles-boolean-) | Gibt an, ob die Drucktitel für das Arbeitsblatt basierend auf dem PivotTable-Bericht festgelegt sind. |
| [setRefreshDataOnOpeningFile(boolean value)](#setRefreshDataOnOpeningFile-boolean-) | Gibt an, ob Daten beim Öffnen der Datei aktualisiert werden. |
| [setRepeatItemsOnEachPrintedPage(boolean value)](#setRepeatItemsOnEachPrintedPage-boolean-) | Gibt an, ob Beschriftungen von Pivot-Elementen im Zeilenbereich auf jeder gedruckten Seite für Pivot-Felder in Tabellenform wiederholt werden. |
| [setRowGrand(boolean value)](#setRowGrand-boolean-) | Gibt an, ob Gesamtsummen für Zeilen dieser Pivot-Tabelle angezeigt werden sollen. |
| [setRowHeaderCaption(String value)](#setRowHeaderCaption-java.lang.String-) | Legt die benutzerdefinierte Beschriftung der Zeilenüberschrift in dieser PivotTable fest. |
| [setSaveData(boolean value)](#setSaveData-boolean-) | Gibt an, ob Daten für den PivotTable-Bericht mit der Arbeitsmappe gespeichert werden. |
| [setSelected(boolean value)](#setSelected-boolean-) | Gibt an, ob diese PivotTable ausgewählt ist. |
| [setShowColumnGrandTotals(boolean value)](#setShowColumnGrandTotals-boolean-) | Gibt an, ob Gesamtsummen für die Spalten dieser PivotTable angezeigt werden. |
| [setShowDataTips(boolean value)](#setShowDataTips-boolean-) | Gibt an, ob Tooltips für PivotTable-Datenzellen angezeigt werden sollen. |
| [setShowDrill(boolean value)](#setShowDrill-boolean-) | Legt fest, ob Expand/Collapse-Schaltflächen angezeigt werden. |
| [setShowEmptyCol(boolean value)](#setShowEmptyCol-boolean-) | Gibt an, ob leere Spalten in die Tabelle aufgenommen werden sollen. |
| [setShowEmptyRow(boolean value)](#setShowEmptyRow-boolean-) | Gibt an, ob leere Zeilen in die Tabelle aufgenommen werden sollen. |
| [setShowHeaders(boolean value)](#setShowHeaders-boolean-) | Ob Datenfeldbeschriftungen und Pivotfeldbeschriftungen auf der Zeilen‑ und Spaltenachse in der PivotTable‑Ansicht angezeigt werden. |
| [setShowMemberPropertyTips(boolean value)](#setShowMemberPropertyTips-boolean-) | Gibt einen booleschen Wert an, der festlegt, ob Mitgliedseigenschaftsinformationen aus PivotTable-Tooltips weggelassen werden sollen. |
| [setShowPivotStyleColumnHeader(boolean value)](#setShowPivotStyleColumnHeader-boolean-) | Gibt an, ob die Spaltenüberschrift in der PivotTable den Stil erhalten soll. |
| [setShowPivotStyleColumnStripes(boolean value)](#setShowPivotStyleColumnStripes-boolean-) | Gibt an, ob für die Spalte Streifenformatierung angewendet wird. |
| [setShowPivotStyleLastColumn(boolean value)](#setShowPivotStyleLastColumn-boolean-) | Gibt an, ob die Spaltenformatierung angewendet wird. |
| [setShowPivotStyleRowHeader(boolean value)](#setShowPivotStyleRowHeader-boolean-) | Gibt an, ob die Zeilenüberschrift in der PivotTable den Stil erhalten soll. |
| [setShowPivotStyleRowStripes(boolean value)](#setShowPivotStyleRowStripes-boolean-) | Gibt an, ob Zeilenstreifenformatierung angewendet wird. |
| [setShowRowGrandTotals(boolean value)](#setShowRowGrandTotals-boolean-) | Gibt an, ob Gesamtsummen für die Zeilen der PivotTable angezeigt werden sollen. |
| [setShowRowHeaderCaption(boolean value)](#setShowRowHeaderCaption-boolean-) | Gibt an, ob die Zeilenüberschriftsbeschriftung im PivotTable-Bericht angezeigt wird. Gibt an, ob Feldbeschriftungen und Filter‑Dropdowns angezeigt werden. |
| [setShowValuesRow(boolean value)](#setShowValuesRow-boolean-) | Gibt an, ob die Wertezeile angezeigt wird. |
| [setSubtotalHiddenPageItems(boolean value)](#setSubtotalHiddenPageItems-boolean-) | Gibt an, ob versteckte Seitenfeld‑Elemente im PivotTable-Bericht in Zeilen‑ und Spaltensummen, Blocksummen und Gesamtsummen einbezogen werden. |
| [setTag(String value)](#setTag-java.lang.String-) | Legt eine benutzerdefinierte Zeichenkette fest, die mit dieser PivotTable-Ansicht verknüpft ist. |
| [showDetail(int rowOffset, int columnOffset, boolean newSheet, int destRow, int destColumn)](#showDetail-int-int-boolean-int-int-) | Zeige die Details eines Elements im Datenbereich in einer neuen Tabelle an. |
| [showInCompactForm()](#showInCompactForm--) | Gestaltet die PivotTable-Ansicht in kompakter Form. |
| [showInOutlineForm()](#showInOutlineForm--) | Gestaltet die PivotTable in Gliederungsform. |
| [showInTabularForm()](#showInTabularForm--) | Gestaltet die PivotTable in Tabellenform. |
| [showReportFilterPage(PivotField pageField)](#showReportFilterPage-com.aspose.cells.PivotField-) | Zeige alle Berichtfilterseiten basierend auf dem PivotField an, das PivotField muss sich in den PageFields befinden. |
| [showReportFilterPageByIndex(int posIndex)](#showReportFilterPageByIndex-int-) | Zeige alle Berichtfilterseiten basierend auf dem Positionsindex in den PageFields an. |
| [showReportFilterPageByName(String fieldName)](#showReportFilterPageByName-java.lang.String-) | Zeige alle Berichtfilterseiten basierend auf dem Namen des PivotField an, das PivotField muss sich in den PageFields befinden. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addCalculatedField(String name, String formula) {#addCalculatedField-java.lang.String-java.lang.String-}
```
public void addCalculatedField(String name, String formula)
```


Fügt ein berechnetes Feld zum Pivot-Feld hinzu und zieht es in den Datenbereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | Der Name des berechneten Feldes |
| formula | java.lang.String | Die Formel des berechneten Feldes. |

### addCalculatedField(String name, String formula, boolean dragToDataArea) {#addCalculatedField-java.lang.String-java.lang.String-boolean-}
```
public void addCalculatedField(String name, String formula, boolean dragToDataArea)
```


Fügt ein berechnetes Feld zum Pivot-Feld hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | Der Name des berechneten Feldes |
| formula | java.lang.String | Die Formel des berechneten Feldes. |
| dragToDataArea | boolean | True, ziehe dieses Feld sofort in den Datenbereich. |

### addFieldToArea(int fieldType, PivotField pivotField) {#addFieldToArea-int-com.aspose.cells.PivotField-}
```
public int addFieldToArea(int fieldType, PivotField pivotField)
```


Fügt das Feld zum spezifischen Bereich hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). der Feldbereichstyp. |
| pivotField | [PivotField](../../com.aspose.cells/pivotfield) | das Feld in den Basisfeldern. |

**Returns:**
int - die Feldposition in den spezifischen Feldern.
### addFieldToArea(int fieldType, int baseFieldIndex) {#addFieldToArea-int-int-}
```
public int addFieldToArea(int fieldType, int baseFieldIndex)
```


Fügt das Feld zum spezifischen Bereich hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Der Feldbereichstyp. |
| baseFieldIndex | int | Der Index in den Basisfeldern. |

**Returns:**
int - die Feldposition in den spezifischen Feldern.
### addFieldToArea(int fieldType, String fieldName) {#addFieldToArea-int-java.lang.String-}
```
public int addFieldToArea(int fieldType, String fieldName)
```


Fügt das Feld zum spezifischen Bereich hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Der Feldbereichstyp. |
| fieldName | java.lang.String | Der Name in den Basisfeldern. |

**Returns:**
int - die Feldposition in den spezifischen Feldern. Wenn es kein Feld mit diesem Namen gibt, wird -1 zurückgegeben.
### calculateData() {#calculateData--}
```
public void calculateData()
```


Berechnet Daten der PivotTable in Zellen.

**Remarks**

Diese Methode berechnet Daten nur mit den im Cache gespeicherten Daten in [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--). Wenn Sie mit der neuesten Datenquelle berechnen möchten, verwenden Sie bitte die Methode [PivotCache.refresh()](../../com.aspose.cells/pivotcache\#refresh--). Wenn nur die Einstellung der PivotTable geändert wurde, reicht [calculateData()](../../com.aspose.cells/pivottable\#calculateData--) aus.

### calculateData(PivotTableCalculateOption option) {#calculateData-com.aspose.cells.PivotTableCalculateOption-}
```
public PivotTable[] calculateData(PivotTableCalculateOption option)
```


Berechnet die PivotTable mit Optionen.

**Remarks**

Wenn [PivotTableCalculateOption.getRefreshData()](../../com.aspose.cells/pivottablecalculateoption\#getRefreshData--) wahr ist, wird diese Methode den Pivot-Cache aus der Datenquelle aktualisieren und anschließend alle Pivot-Tabellen basierend auf demselben Pivot-Cache berechnen. Andernfalls wird nur mit den im Pivot-Cache gespeicherten Daten gerechnet.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| option | [PivotTableCalculateOption](../../com.aspose.cells/pivottablecalculateoption) | Die Optionen für die Berechnung der Pivot-Tabelle |

**Returns:**
com.aspose.cells.PivotTable[] – Gibt alle Pivot-Tabellen zurück, die berechnet wurden. Wenn [PivotTableCalculateOption.getRefreshData()](../../com.aspose.cells/pivottablecalculateoption\#getRefreshData--) wahr ist, werden alle Pivot-Tabellen, die auf demselben Pivot-Cache basieren, zusammen berechnet.
### calculateRange() {#calculateRange--}
```
public void calculateRange()
```


Berechnet den Bereich der PivotTable.

**Remarks**

Wenn diese Methode nicht aufgerufen wurde, ist möglicherweise der PivotTable‑Bereich nicht korrekt.

### changeDataSource(String[] source) {#changeDataSource-java.lang.String---}
```
public void changeDataSource(String[] source)
```


Ändere die Datenquelle der PivotTable.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Quelle | java.lang.String[] |  |

### clearAll() {#clearAll--}
```
public void clearAll()
```


Entferne alle Felder aus Regionen.

### clearData() {#clearData--}
```
public void clearData()
```


Lösche Daten und Formatierung der PivotTable-Ansicht.

**Remarks**

Wenn diese Methode nicht aufgerufen wird, bevor Sie ein PivotField hinzufügen oder löschen, sind die PivotTable-Daten möglicherweise nicht korrekt.

### clearFilters() {#clearFilters--}
```
public void clearFilters()
```


Löscht alle Filter dieser PivotTable.

### copyStyle(PivotTable pivotTable) {#copyStyle-com.aspose.cells.PivotTable-}
```
public void copyStyle(PivotTable pivotTable)
```


Kopiert benannten Stil von einer anderen Pivot-Tabelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | Quell-Pivot-Tabelle. |

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
### exportViewToJson(PivotViewToJsonOptions options) {#exportViewToJson-com.aspose.cells.PivotViewToJsonOptions-}
```
public String exportViewToJson(PivotViewToJsonOptions options)
```


Exportiert die Pivot-Ansicht als JSON.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| options | [PivotViewToJsonOptions](../../com.aspose.cells/pivotviewtojsonoptions) |  |

**Returns:**
java.lang.String -
### fields(int fieldType) {#fields-int-}
```
public PivotFieldCollection fields(int fieldType)
```


Ruft die spezifischen Felder nach dem Feldtyp ab.

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotField.GetFields(PivotFieldType). Diese Methode wird 12 Monate später, seit Mai 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). der Feldtyp. |

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) - the specific field collection
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

### formatAll(Style style) {#formatAll-com.aspose.cells.Style-}
```
public void formatAll(Style style)
```


Formatiert alle Zellen im Pivot-Tabellenbereich

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Stil, der formatieren soll |

### formatRow(int row, Style style) {#formatRow-int-com.aspose.cells.Style-}
```
public void formatRow(int row, Style style)
```


Formatiert die Zeilendaten im Pivot-Tabellenbereich

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex des Zeilenobjekts |
| style | [Style](../../com.aspose.cells/style) | Stil, der formatieren soll |

### getAllowMultipleFiltersPerField() {#getAllowMultipleFiltersPerField--}
```
public boolean getAllowMultipleFiltersPerField()
```


Gibt einen booleschen Wert an, der angibt, ob die Felder einer Pivot-Tabelle mehrere Filter haben können.

**Returns:**
boolean
### getAltTextDescription() {#getAltTextDescription--}
```
public String getAltTextDescription()
```


Ruft die Beschreibung des Alternativtexts ab.

**Returns:**
java.lang.String
### getAltTextTitle() {#getAltTextTitle--}
```
public String getAltTextTitle()
```


Ruft den Titel des Alternativtexts ab.

**Returns:**
java.lang.String
### getAutoFormatType() {#getAutoFormatType--}
```
public int getAutoFormatType()
```


Ruft den Autoformattyp der Pivot-Tabelle ab.

Siehe [PivotTableAutoFormatType](../../com.aspose.cells/pivottableautoformattype).

**Returns:**
int
### getAutofitColumnWidthOnUpdate() {#getAutofitColumnWidthOnUpdate--}
```
public boolean getAutofitColumnWidthOnUpdate()
```


Gibt an, ob die Spaltenbreite bei Aktualisierung automatisch angepasst werden soll

**Returns:**
boolean
### getBaseFields() {#getBaseFields--}
```
public PivotFieldCollection getBaseFields()
```


Gibt alle Basis-Pivot-Felder in der Pivot-Tabelle zurück.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getButtonArea(int axisType) {#getButtonArea-int-}
```
public CellArea getButtonArea(int axisType)
```


Ruft den Bereich ab, der die Feldschaltfläche enthält.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Der Regionstyp. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - 
### getCellByDisplayName(String displayName) {#getCellByDisplayName-java.lang.String-}
```
public Cell getCellByDisplayName(String displayName)
```


Ruft das [Cell](../../com.aspose.cells/cell)-Objekt anhand des Anzeigenamens des PivotField ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| displayName | java.lang.String | der DisplayName von PivotField |

**Returns:**
[Cell](../../com.aspose.cells/cell) - the Cell object
### getChildren() {#getChildren--}
```
public PivotTable[] getChildren()
```


Ruft die untergeordneten Pivot-Tabellen ab, die diese Pivot-Tabellendaten als Datenquelle verwenden.

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotTable.GetDependentPivotTables(). Diese Methode wird 12 Monate später, seit April 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
com.aspose.cells.PivotTable[] - das PivotTable-Array-Objekt
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnFields() {#getColumnFields--}
```
public PivotFieldCollection getColumnFields()
```


Gibt ein PivotFields-Objekt zurück, das derzeit als Spaltenfelder angezeigt wird.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getColumnGrand() {#getColumnGrand--}
```
public boolean getColumnGrand()
```


Gibt an, ob der Pivot-Tabellenbericht Gesamtsummen für Spalten anzeigt.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotTable.ShowColumnGrandTotals. Diese Methode wird 12 Monate später, seit Dezember 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
boolean
### getColumnHeaderCaption() {#getColumnHeaderCaption--}
```
public String getColumnHeaderCaption()
```


Ruft die benutzerdefinierte Beschriftung der Spaltenüberschrift der Pivot-Tabelle ab.

**Returns:**
java.lang.String
### getColumnRange() {#getColumnRange--}
```
public CellArea getColumnRange()
```


Gibt ein CellArea-Objekt zurück, das den Bereich darstellt, der den Spaltenbereich im PivotTable-Bericht enthält. Nur lesbar.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getConditionalFormats() {#getConditionalFormats--}
```
public PivotConditionalFormatCollection getConditionalFormats()
```


Ruft die bedingten Formate der Pivot-Tabelle ab.

**Returns:**
[PivotConditionalFormatCollection](../../com.aspose.cells/pivotconditionalformatcollection)
### getCustomListSort() {#getCustomListSort--}
```
public boolean getCustomListSort()
```


Gibt an, ob beim Sortieren von Daten die integrierte benutzerdefinierte Liste berücksichtigt wird.

**Returns:**
boolean
### getDataBodyRange() {#getDataBodyRange--}
```
public CellArea getDataBodyRange()
```


Gibt ein [CellArea](../../com.aspose.cells/cellarea)-Objekt zurück, das den Bereich darstellt, der den Datenbereich in der Liste zwischen der Kopfzeile und der Einfügezeile enthält. Nur lesbar.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getDataField() {#getDataField--}
```
public PivotField getDataField()
```


Liefert ein [PivotField](../../com.aspose.cells/pivotfield)-Objekt, das alle Datenfelder in einer PivotTable darstellt. Nur lesbar. Es wird nur erstellt, wenn im Datenbereich zwei oder mehr Datenfelder vorhanden sind. Standardmäßig befindet es sich im Zeilenbereich. Sie können es mit der Methode PivotTable.AddFieldToArea() in den Zeilen‑/Spaltenbereich ziehen.

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotTable.ValuesField. Diese Methode wird 12 Monate später, seit Oktober 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
[PivotField](../../com.aspose.cells/pivotfield)
### getDataFieldHeaderName() {#getDataFieldHeaderName--}
```
public String getDataFieldHeaderName()
```


Ermittelt den Namen der Feldkopfzeile des Wertebereichs in der PivotTable.

**Returns:**
java.lang.String
### getDataFields() {#getDataFields--}
```
public PivotFieldCollection getDataFields()
```


Ermittelt eine [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection), die alle Datenfelder in einer PivotTable darstellt.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getDataSource() {#getDataSource--}
```
public String[] getDataSource()
```


Ermittelt die Datenquelle der PivotTable.

**Returns:**
java.lang.String[]
### getDependentPivotTables() {#getDependentPivotTables--}
```
public PivotTable[] getDependentPivotTables()
```


Ermittelt alle [PivotTable](../../com.aspose.cells/pivottable)s, die diese PivotTable als Datenquelle verwenden.

**Remarks**

Da Pivot-Tabellen von den Daten anderer abhängen können, müssen sie in der richtigen Reihenfolge aktualisiert werden, um Datenkonsistenz zu gewährleisten.

**Returns:**
com.aspose.cells.PivotTable[] -
### getDisplayErrorString() {#getDisplayErrorString--}
```
public boolean getDisplayErrorString()
```


Gibt an, ob der PivotTable-Bericht in Zellen, die Fehler enthalten, einen benutzerdefinierten Text anzeigt.

**Returns:**
boolean
### getDisplayImmediateItems() {#getDisplayImmediateItems--}
```
public boolean getDisplayImmediateItems()
```


Gibt an, ob Elemente in den Zeilen- und Spaltenbereichen sichtbar sind, wenn der Datenbereich der PivotTable leer ist. Der Standardwert ist true.

**Returns:**
boolean
### getDisplayNullString() {#getDisplayNullString--}
```
public boolean getDisplayNullString()
```


Gibt an, ob der PivotTable-Bericht einen benutzerdefinierten Text anzeigt, wenn der Wert null ist.

**Returns:**
boolean
### getEnableDataValueEditing() {#getEnableDataValueEditing--}
```
public boolean getEnableDataValueEditing()
```


Gibt einen booleschen Wert an, der angibt, ob der Benutzer die Zellen im Datenbereich der PivotTable bearbeiten darf. Der Standardwert ist false.

**Returns:**
boolean
### getEnableDrilldown() {#getEnableDrilldown--}
```
public boolean getEnableDrilldown()
```


Gibt an, ob Drilldown aktiviert ist.

**Returns:**
boolean
### getEnableFieldDialog() {#getEnableFieldDialog--}
```
public boolean getEnableFieldDialog()
```


Gibt an, ob das Dialogfeld PivotTable-Feld verfügbar ist, wenn der Benutzer das PivotTable-Feld doppelklickt.

**Returns:**
boolean
### getEnableFieldList() {#getEnableFieldList--}
```
public boolean getEnableFieldList()
```


Gibt an, ob die Feldliste für die PivotTable in der Excel-Ansicht verfügbar ist.

**Returns:**
boolean
### getEnableWizard() {#getEnableWizard--}
```
public boolean getEnableWizard()
```


Gibt an, ob der PivotTable-Assistent verfügbar ist.

**Returns:**
boolean
### getErrorString() {#getErrorString--}
```
public String getErrorString()
```


Ermittelt den Text, der in Zellen angezeigt wird, die Fehler enthalten, wenn die Eigenschaft DisplayErrorString true ist. Der Standardwert ist ein leerer String.

**Returns:**
java.lang.String
### getExternalConnectionDataSource() {#getExternalConnectionDataSource--}
```
public ExternalConnection getExternalConnectionDataSource()
```


Ermittelt die externe Verbindungsdatenquelle.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotTable.GetSourceDataConnections(). Diese Methode wird 12 Monate später, ab Oktober 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Returns:**
[ExternalConnection](../../com.aspose.cells/externalconnection)
### getFieldListSortAscending() {#getFieldListSortAscending--}
```
public boolean getFieldListSortAscending()
```


Gibt an, ob Felder in der PivotTable in der Feldliste in einer nicht standardmäßigen Reihenfolge sortiert sind.

**Returns:**
boolean
### getFields(int fieldType) {#getFields-int-}
```
public PivotFieldCollection getFields(int fieldType)
```


Ermittelt die spezifische Pivot-Feldliste nach Region.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). der Regionstyp. |

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) - the specific pivot field collection
### getFilterArea() {#getFilterArea--}
```
public CellArea getFilterArea()
```


Ermittelt den Bereich der Filterregion.

**Remarks**

Nur gültig, wenn Filter-Pivotfelder vorhanden sind. Ein leerer Bereich wird zurückgegeben, wenn diese PivotTable keine Filter-Pivotfelder enthält.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getGrandTotalName() {#getGrandTotalName--}
```
public String getGrandTotalName()
```


Gibt die Bezeichnung zurück, die in der Gesamtsumme‑Spalte oder -Zeilenüberschrift angezeigt wird. Der Standardwert ist die Zeichenkette "Grand Total".

**Returns:**
java.lang.String
### getHorizontalBreaks() {#getHorizontalBreaks--}
```
public ArrayList getHorizontalBreaks()
```


Ermittelt die Zeilenindexliste der PivotTable für horizontale Seitenumbrüche

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotTable.GetHorizontalPageBreaks(). Diese Methode wird 12 Monate später, ab Dezember 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Returns:**
java.util.ArrayList -
### getHorizontalPageBreaks() {#getHorizontalPageBreaks--}
```
public int[] getHorizontalPageBreaks()
```


Ermittelt die horizontalen Seitenumbrüche dieser PivotTable.

**Returns:**
int[] -
### getIndent() {#getIndent--}
```
public int getIndent()
```


Gibt die Einrückungssteigerung für die kompakte Achse an und kann verwendet werden, um das Berichtslayout auf kompakte Form einzustellen.

**Returns:**
int
### getItemPrintTitles() {#getItemPrintTitles--}
```
public boolean getItemPrintTitles()
```


Gibt an, ob PivotItem-Namen oben auf jeder gedruckten Seite wiederholt werden sollen.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotTable.RepeatItemsOnEachPrintedPage. Diese Methode wird 12 Monate später, ab Oktober 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Returns:**
boolean
### getManualUpdate() {#getManualUpdate--}
```
public boolean getManualUpdate()
```


Gibt an, ob der PivotTable-Bericht nur auf Anforderung des Benutzers neu berechnet wird.

**Returns:**
boolean
### getMergeLabels() {#getMergeLabels--}
```
public boolean getMergeLabels()
```


Ermittelt, ob Zeilen-/Spaltenfeldbeschriftungen, die mehrere Zellen umfassen, zusammengeführt werden sollen.

**Returns:**
boolean
### getMissingItemsLimit() {#getMissingItemsLimit--}
```
public int getMissingItemsLimit()
```


Gibt einen booleschen Wert an, der angibt, ob die Felder einer Pivot-Tabelle mehrere Filter haben können.

Siehe [PivotMissingItemLimitType](../../com.aspose.cells/pivotmissingitemlimittype).

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotCache.MissingItemsLimit. Diese Methode wird 12 Monate später, ab September 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Ermittelt den Namen der PivotTable

**Returns:**
java.lang.String
### getNamesOfSourceDataConnections() {#getNamesOfSourceDataConnections--}
```
public String[] getNamesOfSourceDataConnections()
```


Ruft die Namen von externen Quell-Datenverbindungen ab.

**Returns:**
java.lang.String[]
### getNullString() {#getNullString--}
```
public String getNullString()
```


Ruft die Zeichenkette ab, die in Zellen angezeigt wird, die Nullwerte enthalten, wenn die Eigenschaft DisplayNullString true ist. Der Standardwert ist eine leere Zeichenkette.

**Returns:**
java.lang.String
### getPageFieldOrder() {#getPageFieldOrder--}
```
public int getPageFieldOrder()
```


Ruft die Reihenfolge ab, in der Seitenfelder zum Layout des PivotTable-Berichts hinzugefügt werden.

Siehe [PrintOrderType](../../com.aspose.cells/printordertype).

**Returns:**
int
### getPageFieldWrapCount() {#getPageFieldWrapCount--}
```
public int getPageFieldWrapCount()
```


Ruft die Anzahl der Seitenfelder in jeder Spalte oder Zeile im PivotTable-Bericht ab.

**Returns:**
int
### getPageFields() {#getPageFields--}
```
public PivotFieldCollection getPageFields()
```


Gibt eine [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) zurück, die derzeit als Seitenfelder angezeigt werden.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getPivotCache() {#getPivotCache--}
```
public PivotCache getPivotCache()
```


Ruft die Datenquelle ab.

**Returns:**
[PivotCache](../../com.aspose.cells/pivotcache)
### getPivotFilters() {#getPivotFilters--}
```
public PivotFilterCollection getPivotFilters()
```


Gibt alle Filter in der Pivot-Tabelle zurück.

**Returns:**
[PivotFilterCollection](../../com.aspose.cells/pivotfiltercollection)
### getPivotFormatConditions() {#getPivotFormatConditions--}
```
public PivotFormatConditionCollection getPivotFormatConditions()
```


Ruft die Formatbedingungen der Pivot-Tabelle ab.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotTable.ConditionalFormats. Diese Methode wird 12 Monate später, ab Dezember 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Returns:**
[PivotFormatConditionCollection](../../com.aspose.cells/pivotformatconditioncollection)
### getPivotFormats() {#getPivotFormats--}
```
public PivotTableFormatCollection getPivotFormats()
```


Ruft alle Zellformate ab, die auf diese Pivot-Tabelle angewendet wurden.

**Returns:**
[PivotTableFormatCollection](../../com.aspose.cells/pivottableformatcollection)
### getPivotTableStyle() {#getPivotTableStyle--}
```
public TableStyle getPivotTableStyle()
```


Ruft die [TableStyle](../../com.aspose.cells/tablestyle)-Einstellungen dieser Pivot-Tabelle ab.

**Returns:**
[TableStyle](../../com.aspose.cells/tablestyle)
### getPivotTableStyleName() {#getPivotTableStyleName--}
```
public String getPivotTableStyleName()
```


Ruft den Stilnamen der Pivot-Tabelle ab.

**Returns:**
java.lang.String
### getPivotTableStyleType() {#getPivotTableStyleType--}
```
public int getPivotTableStyleType()
```


Ruft den integrierten Pivot-Tabellenstil ab.

Siehe [PivotTableStyleType](../../com.aspose.cells/pivottablestyletype).

**Returns:**
int
### getPivotTablesWithSamePivotCache() {#getPivotTablesWithSamePivotCache--}
```
public PivotTable[] getPivotTablesWithSamePivotCache()
```


Ruft alle Pivot-Tabellen mit demselben Pivot-Cache ab.

**Returns:**
com.aspose.cells.PivotTable[] -
### getPreserveCellFormattingOnUpdate() {#getPreserveCellFormattingOnUpdate--}
```
public boolean getPreserveCellFormattingOnUpdate()
```


Gibt an, ob die Zellformatierung ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) beibehalten werden soll, wenn die Pivot-Tabelle aktualisiert oder neu berechnet wird.

**Returns:**
boolean
### getPreserveFormatting() {#getPreserveFormatting--}
```
public boolean getPreserveFormatting()
```


Gibt an, ob die Zellformatierung ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) beibehalten wird, wenn die PivotTable aktualisiert oder neu berechnet wird.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotTable.PreserveCellFormattingOnUpdate. Diese Methode wird 12 Monate später, ab Juli 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Returns:**
boolean
### getPrintDrill() {#getPrintDrill--}
```
public boolean getPrintDrill()
```


Gibt einen booleschen Wert an, der angibt, ob Drill‑Indikatoren gedruckt werden sollen. Druckt Expand/Collapse‑Schaltflächen, wenn sie in der PivotTable angezeigt werden.

**Returns:**
boolean
### getPrintTitles() {#getPrintTitles--}
```
public boolean getPrintTitles()
```


Gibt an, ob die Drucktitel für das Arbeitsblatt basierend auf dem PivotTable‑Bericht festgelegt werden. Der Standardwert ist false.

**Returns:**
boolean
### getRefreshDataOnOpeningFile() {#getRefreshDataOnOpeningFile--}
```
public boolean getRefreshDataOnOpeningFile()
```


Gibt an, ob Daten beim Öffnen der Datei aktualisiert werden.

**Returns:**
boolean
### getRefreshDate() {#getRefreshDate--}
```
public DateTime getRefreshDate()
```


Ruft das letzte Datum und die Uhrzeit ab, zu der die PivotTable aktualisiert wurde.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getRefreshedByWho() {#getRefreshedByWho--}
```
public String getRefreshedByWho()
```


Ruft den Namen des letzten Benutzers ab, der diese PivotTable aktualisiert hat.

**Returns:**
java.lang.String
### getRepeatItemsOnEachPrintedPage() {#getRepeatItemsOnEachPrintedPage--}
```
public boolean getRepeatItemsOnEachPrintedPage()
```


Gibt an, ob Beschriftungen von Pivot-Elementen im Zeilenbereich auf jeder gedruckten Seite für Pivot-Felder in Tabellenform wiederholt werden.

**Returns:**
boolean
### getRowFields() {#getRowFields--}
```
public PivotFieldCollection getRowFields()
```


Gibt eine [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) zurück, die derzeit als Zeilenfelder angezeigt werden.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getRowGrand() {#getRowGrand--}
```
public boolean getRowGrand()
```


Gibt an, ob Gesamtsummen für Zeilen dieser Pivot-Tabelle angezeigt werden sollen.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotTable.ShowRowGrandTotals. Diese Methode wird 12 Monate später, ab Dezember 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Returns:**
boolean
### getRowHeaderCaption() {#getRowHeaderCaption--}
```
public String getRowHeaderCaption()
```


Ruft die benutzerdefinierte Beschriftung der Zeilenüberschrift in dieser PivotTable ab.

**Returns:**
java.lang.String
### getRowRange() {#getRowRange--}
```
public CellArea getRowRange()
```


Gibt ein CellArea-Objekt zurück, das den Bereich darstellt, der den Zeilenbereich im PivotTable-Bericht enthält. Nur lesbar.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getSaveData() {#getSaveData--}
```
public boolean getSaveData()
```


Gibt an, ob Daten für den PivotTable-Bericht mit der Arbeitsmappe gespeichert werden.

**Returns:**
boolean
### getShowColumnGrandTotals() {#getShowColumnGrandTotals--}
```
public boolean getShowColumnGrandTotals()
```


Gibt an, ob Gesamtsummen für die Spalten dieser PivotTable angezeigt werden.

**Returns:**
boolean
### getShowDataTips() {#getShowDataTips--}
```
public boolean getShowDataTips()
```


Gibt an, ob Tooltips für PivotTable-Datenzellen angezeigt werden sollen.

**Returns:**
boolean
### getShowDrill() {#getShowDrill--}
```
public boolean getShowDrill()
```


Ermittelt, ob Expand/Collapse-Schaltflächen angezeigt werden.

**Returns:**
boolean
### getShowEmptyCol() {#getShowEmptyCol--}
```
public boolean getShowEmptyCol()
```


Gibt an, ob leere Spalten in die Tabelle aufgenommen werden sollen.

**Returns:**
boolean
### getShowEmptyRow() {#getShowEmptyRow--}
```
public boolean getShowEmptyRow()
```


Gibt an, ob leere Zeilen in die Tabelle aufgenommen werden sollen.

**Returns:**
boolean
### getShowHeaders() {#getShowHeaders--}
```
public boolean getShowHeaders()
```


Ob Datenfeldbeschriftungen und Pivotfeldbeschriftungen auf der Zeilen‑ und Spaltenachse in der PivotTable‑Ansicht angezeigt werden.

**Returns:**
boolean
### getShowMemberPropertyTips() {#getShowMemberPropertyTips--}
```
public boolean getShowMemberPropertyTips()
```


Gibt einen booleschen Wert an, der festlegt, ob Mitgliedseigenschaftsinformationen aus PivotTable-Tooltips weggelassen werden sollen.

**Returns:**
boolean
### getShowPivotStyleColumnHeader() {#getShowPivotStyleColumnHeader--}
```
public boolean getShowPivotStyleColumnHeader()
```


Gibt an, ob die Spaltenüberschrift in der PivotTable den Stil erhalten soll.

**Returns:**
boolean
### getShowPivotStyleColumnStripes() {#getShowPivotStyleColumnStripes--}
```
public boolean getShowPivotStyleColumnStripes()
```


Gibt an, ob für die Spalte Streifenformatierung angewendet wird.

**Returns:**
boolean
### getShowPivotStyleLastColumn() {#getShowPivotStyleLastColumn--}
```
public boolean getShowPivotStyleLastColumn()
```


Gibt an, ob die Spaltenformatierung angewendet wird.

**Returns:**
boolean
### getShowPivotStyleRowHeader() {#getShowPivotStyleRowHeader--}
```
public boolean getShowPivotStyleRowHeader()
```


Gibt an, ob die Zeilenüberschrift in der PivotTable den Stil erhalten soll.

**Returns:**
boolean
### getShowPivotStyleRowStripes() {#getShowPivotStyleRowStripes--}
```
public boolean getShowPivotStyleRowStripes()
```


Gibt an, ob Zeilenstreifenformatierung angewendet wird.

**Returns:**
boolean
### getShowRowGrandTotals() {#getShowRowGrandTotals--}
```
public boolean getShowRowGrandTotals()
```


Gibt an, ob Gesamtsummen für die Zeilen der PivotTable angezeigt werden sollen.

**Remarks**

**Returns:**
boolean
### getShowRowHeaderCaption() {#getShowRowHeaderCaption--}
```
public boolean getShowRowHeaderCaption()
```


Gibt an, ob die Zeilenüberschriftsbeschriftung im PivotTable-Bericht angezeigt wird. Gibt an, ob Feldbeschriftungen und Filter‑Dropdowns angezeigt werden.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotTable.ShowHeaders. Diese Methode wird 12 Monate später, seit April 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
boolean
### getShowValuesRow() {#getShowValuesRow--}
```
public boolean getShowValuesRow()
```


Gibt an, ob die Wertezeile angezeigt wird.

**Returns:**
boolean
### getSource() {#getSource--}
```
public String[] getSource()
```


Ruft die Datenquelle dieser PivotTable ab.

**Returns:**
java.lang.String[]
### getSource(boolean isOriginal) {#getSource-boolean-}
```
public String[] getSource(boolean isOriginal)
```


Ruft die Datenquelle dieser PivotTable ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isOriginal | boolean | Gibt an, ob das Original zurückgegeben oder die Datenquelle angezeigt werden soll. |

**Returns:**
java.lang.String[] -
### getSourceDataConnections() {#getSourceDataConnections--}
```
public ExternalConnection[] getSourceDataConnections()
```


Ermittelt die externen Verbindungsdatenquellen.

**Returns:**
com.aspose.cells.ExternalConnection[]
### getSourceType() {#getSourceType--}
```
public byte getSourceType()
```


Ermittelt den Datentyp der Datenquelle der PivotTable.

Siehe [PivotTableSourceType](../../com.aspose.cells/pivottablesourcetype).

**Returns:**
byte
### getSubtotalHiddenPageItems() {#getSubtotalHiddenPageItems--}
```
public boolean getSubtotalHiddenPageItems()
```


Gibt an, ob versteckte Seitenfeld-Elemente im PivotTable-Bericht in Zeilen- und Spalten-Teilsummen, Blocksummen und Gesamtsummen einbezogen werden. Der Standardwert ist False.

**Returns:**
boolean
### getTableRange1() {#getTableRange1--}
```
public CellArea getTableRange1()
```


Gibt ein CellArea-Objekt zurück, das den Bereich darstellt, der den gesamten PivotTable-Bericht enthält, jedoch keine Seitenfelder. Nur lesbar.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getTableRange2() {#getTableRange2--}
```
public CellArea getTableRange2()
```


Gibt ein CellArea-Objekt zurück, das den Bereich darstellt, der den gesamten PivotTable-Bericht einschließlich Seitenfelder enthält. Nur lesbar.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getTag() {#getTag--}
```
public String getTag()
```


Ermittelt einen benutzerdefinierten String, der mit dieser PivotTable‑Ansicht verknüpft ist.

**Returns:**
java.lang.String
### getTopRightArea() {#getTopRightArea--}
```
public CellArea getTopRightArea()
```


Stellt den leeren Bereich oben rechts der PivotTable dar (oben links für RTL‑Blätter).

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getValuesField() {#getValuesField--}
```
public PivotField getValuesField()
```


Liefert ein [PivotField](../../com.aspose.cells/pivotfield)-Objekt, das alle Datenfelder in einer PivotTable darstellt. Nur lesbar. Es wird nur erstellt, wenn im Datenbereich zwei oder mehr Datenfelder vorhanden sind. Standardmäßig befindet es sich im Zeilenbereich. Sie können es mit der Methode PivotTable.AddFieldToArea() in den Zeilen‑/Spaltenbereich ziehen.

**Returns:**
[PivotField](../../com.aspose.cells/pivotfield)
### hasBlankRows() {#hasBlankRows--}
```
public boolean hasBlankRows()
```


Gibt an, ob leere Zeilen hinzugefügt werden sollen. Diese Eigenschaft gilt nur für PivotTable-Autoformat-Typen, die leere Zeilen benötigen.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotField.InsertBlankRow. Diese Methode wird 12 Monate später, seit April 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoFormat() {#isAutoFormat--}
```
public boolean isAutoFormat()
```


Gibt an, ob der PivotTable-Bericht automatisch formatiert wird. Kontrollkästchen \"autoformat table\", das in den PivotTable-Optionen für Excel 2003 vorhanden ist.

**Returns:**
boolean
### isExcel2003Compatible() {#isExcel2003Compatible--}
```
public boolean isExcel2003Compatible()
```


Gibt an, ob die PivotTable bei der Aktualisierung mit Excel2003 kompatibel ist; wenn true, muss ein String höchstens 255 Zeichen lang sein, andernfalls wird er abgeschnitten. Wenn false, gilt diese Beschränkung nicht. Der Standardwert ist true.

**Returns:**
boolean
### isGridDropZones() {#isGridDropZones--}
```
public boolean isGridDropZones()
```


Gibt an, ob der PivotTable-Bericht das klassische PivotTable-Layout anzeigt (ermöglicht das Ziehen von Feldern im Raster).

**Returns:**
boolean
### isMultipleFieldFilters() {#isMultipleFieldFilters--}
```
public boolean isMultipleFieldFilters()
```


Gibt einen booleschen Wert an, der angibt, ob die Felder einer Pivot-Tabelle mehrere Filter haben können.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotTable.AllowMultipleFiltersPerField. Diese Methode wird 12 Monate später, seit Dezember 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
boolean
### isSelected() {#isSelected--}
```
public boolean isSelected()
```


Gibt an, ob diese PivotTable ausgewählt ist.

**Returns:**
boolean
### move(int row, int column) {#move-int-int-}
```
public void move(int row, int column)
```


Verschiebt die PivotTable an eine andere Position im Arbeitsblatt.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotTable.MoveTo(). Diese Methode wird 12 Monate später, seit Dezember 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex. |
| Spalte | int | Spaltenindex. |

### move(String destCellName) {#move-java.lang.String-}
```
public void move(String destCellName)
```


Verschiebt die PivotTable an eine andere Position im Arbeitsblatt.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotTable.MoveTo(). Diese Methode wird 12 Monate später, seit Dezember 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| destCellName | java.lang.String | Der Zielzellenname. |

### moveItem(int region, String[] nodes, boolean absolute, int offset) {#moveItem-int-java.lang.String---boolean-int-}
```
public void moveItem(int region, String[] nodes, boolean absolute, int offset)
```


Verschiebt ein Element nach oben oder unten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| region | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Die Region. Nur für Zeile oder Spalte. |
| nodes | java.lang.String[] | Das Element. |
| absolute | boolean | Gibt an, ob der Versatz eine absolute Position ist. |
| offset | int | Wenn absolute true ist: 0 bewegt zum Anfang, -1 bewegt zum Ende, andere Werte bedeuten absolute Position; sonst ist offset eine relative Position. |

### moveTo(int row, int column) {#moveTo-int-int-}
```
public void moveTo(int row, int column)
```


Verschiebt die PivotTable an eine andere Position im Arbeitsblatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex. |
| Spalte | int | Spaltenindex. |

### moveTo(int sheetIndex, int row, int column) {#moveTo-int-int-int-}
```
public void moveTo(int sheetIndex, int row, int column)
```


Verschiebt die PivotTable an eine andere Position im Arbeitsblatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheetIndex | int | der Index des Zielarbeitsblatts |
| Zeile | int | Zeilenindex. |
| Spalte | int | Spaltenindex. |

### moveTo(String destCellName) {#moveTo-java.lang.String-}
```
public void moveTo(String destCellName)
```


Verschiebt die PivotTable an eine andere Position im Arbeitsblatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| destCellName | java.lang.String | Der Zielzellenname. |

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
public int refresh()
```


Aktualisiert [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) aus der Datenquelle und berechnet Daten und Stil für die Pivot-Ansicht.

**Remarks**

Alle Pivot-Tabellen, die vom selben PivotCache abhängen, werden neu berechnet.

**Returns:**
int - [PivotRefreshState](../../com.aspose.cells/pivotrefreshstate).
### refresh(PivotTableRefreshOption option) {#refresh-com.aspose.cells.PivotTableRefreshOption-}
```
public int refresh(PivotTableRefreshOption option)
```


Aktualisiert [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) aus der Datenquelle und berechnet Daten und Stil für die Pivot-Ansicht.

**Remarks**

Alle Pivot-Tabellen, die vom selben PivotCache abhängen, werden neu berechnet.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) |  |

**Returns:**
int - [PivotRefreshState](../../com.aspose.cells/pivotrefreshstate).
### refreshData() {#refreshData--}
```
public int refreshData()
```


Aktualisiert Daten aus seiner Datenquelle in den Pivot-Cache.

**Remarks**

Wir werden Daten aus der Datenquelle in einen Pivot-Cache sammeln und dann die Daten im Cache in die Zellen berechnen. Und es ist besser, wenn Sie einfach [Workbook.refreshAll()](../../com.aspose.cells/workbook\#refreshAll--) aufrufen, um alle Pivot-Tabellen in der Datei zu aktualisieren und zu berechnen, anstatt sie einzeln zu aktualisieren. HINWEIS: Diese Methode ist jetzt veraltet. Stattdessen verwenden Sie bitte die Methode [PivotCache.refresh()](../../com.aspose.cells/pivotcache\#refresh--) und entfernen die folgende [calculateData()](../../com.aspose.cells/pivottable\#calculateData--), da diese Pivot-Tabelle beim Aktualisieren von [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) berechnet wird. Diese Methode wird 12 Monate später, seit Juni 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erfahren haben.

**Returns:**
int
### refreshData(PivotTableRefreshOption option) {#refreshData-com.aspose.cells.PivotTableRefreshOption-}
```
public int refreshData(PivotTableRefreshOption option)
```


Aktualisiert die Daten und Einstellungen der PivotTable aus seiner Datenquelle mit Optionen.

**Remarks**

Wir werden Daten aus der Datenquelle in einen Pivot-Cache sammeln und dann die Daten im Cache in die Zellen berechnen. Und es ist besser, wenn Sie einfach [Workbook.refreshAll()](../../com.aspose.cells/workbook\#refreshAll--) aufrufen, um alle Pivot-Tabellen in der Datei zu aktualisieren und zu berechnen, anstatt sie einzeln zu aktualisieren. HINWEIS: Diese Methode ist jetzt veraltet. Stattdessen verwenden Sie bitte die Methode [PivotCache.refresh()](../../com.aspose.cells/pivotcache\#refresh--) und entfernen die folgende [calculateData()](../../com.aspose.cells/pivottable\#calculateData--), da diese Pivot-Tabelle beim Aktualisieren von [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) berechnet wird. Diese Methode wird 12 Monate später, seit Juni 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) | Die Optionen zum Aktualisieren der Datenquelle der Pivot‑Tabelle. |

**Returns:**
int
### removeField(int fieldType, PivotField pivotField) {#removeField-int-com.aspose.cells.PivotField-}
```
public void removeField(int fieldType, PivotField pivotField)
```


Feld aus einem bestimmten Feldbereich entfernen

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). der Feldbereichstyp. |
| pivotField | [PivotField](../../com.aspose.cells/pivotfield) | das Feld in den Basisfeldern. |

### removeField(int fieldType, int baseFieldIndex) {#removeField-int-int-}
```
public void removeField(int fieldType, int baseFieldIndex)
```


Entfernt ein Feld aus einem bestimmten Pivot-Bereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Der Feldbereichstyp. |
| baseFieldIndex | int | Der Feldindex in den Basisfeldern. |

### removeField(int fieldType, String fieldName) {#removeField-int-java.lang.String-}
```
public void removeField(int fieldType, String fieldName)
```


Entfernt ein Feld aus einem bestimmten Feldbereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Der Feldbereichstyp. |
| fieldName | java.lang.String | Der Name in den Basisfeldern. |

### selectArea(CellArea ca) {#selectArea-com.aspose.cells.CellArea-}
```
public PivotAreaCollection selectArea(CellArea ca)
```


Wählt einen Bereich der PivotTable-Ansicht aus.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Der Zellbereich. |

**Returns:**
[PivotAreaCollection](../../com.aspose.cells/pivotareacollection) - 
### setAllowMultipleFiltersPerField(boolean value) {#setAllowMultipleFiltersPerField-boolean-}
```
public void setAllowMultipleFiltersPerField(boolean value)
```


Gibt einen booleschen Wert an, der angibt, ob die Felder einer Pivot-Tabelle mehrere Filter haben können.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAltTextDescription(String value) {#setAltTextDescription-java.lang.String-}
```
public void setAltTextDescription(String value)
```


Ruft die Beschreibung des Alternativtexts ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setAltTextTitle(String value) {#setAltTextTitle-java.lang.String-}
```
public void setAltTextTitle(String value)
```


Legt den Titel des alternativen Textes fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setAutoFormat(boolean value) {#setAutoFormat-boolean-}
```
public void setAutoFormat(boolean value)
```


Gibt an, ob der PivotTable-Bericht automatisch formatiert wird. Kontrollkästchen \"autoformat table\", das in den PivotTable-Optionen für Excel 2003 vorhanden ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAutoFormatType(int value) {#setAutoFormatType-int-}
```
public void setAutoFormatType(int value)
```


Legt den automatischen Formattyp der PivotTable fest.

Siehe [PivotTableAutoFormatType](../../com.aspose.cells/pivottableautoformattype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setAutofitColumnWidthOnUpdate(boolean value) {#setAutofitColumnWidthOnUpdate-boolean-}
```
public void setAutofitColumnWidthOnUpdate(boolean value)
```


Gibt an, ob die Spaltenbreite bei Aktualisierung automatisch angepasst werden soll

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setColumnGrand(boolean value) {#setColumnGrand-boolean-}
```
public void setColumnGrand(boolean value)
```


Gibt an, ob der Pivot-Tabellenbericht Gesamtsummen für Spalten anzeigt.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotTable.ShowColumnGrandTotals. Diese Methode wird 12 Monate später, seit Dezember 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setColumnHeaderCaption(String value) {#setColumnHeaderCaption-java.lang.String-}
```
public void setColumnHeaderCaption(String value)
```


Legt die benutzerdefinierte Beschriftung der Spaltenüberschrift der PivotTable fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setCustomListSort(boolean value) {#setCustomListSort-boolean-}
```
public void setCustomListSort(boolean value)
```


Gibt an, ob beim Sortieren von Daten die integrierte benutzerdefinierte Liste berücksichtigt wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setDataFieldHeaderName(String value) {#setDataFieldHeaderName-java.lang.String-}
```
public void setDataFieldHeaderName(String value)
```


Legt den Namen der Feldüberschrift des Wertebereichs in der PivotTable fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setDataSource(String[] value) {#setDataSource-java.lang.String---}
```
public void setDataSource(String[] value)
```


Legt die Datenquelle der PivotTable fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String[] |  |

### setDisplayErrorString(boolean value) {#setDisplayErrorString-boolean-}
```
public void setDisplayErrorString(boolean value)
```


Gibt an, ob der PivotTable-Bericht in Zellen, die Fehler enthalten, einen benutzerdefinierten Text anzeigt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setDisplayImmediateItems(boolean value) {#setDisplayImmediateItems-boolean-}
```
public void setDisplayImmediateItems(boolean value)
```


Gibt an, ob Elemente in den Zeilen- und Spaltenbereichen sichtbar sind, wenn der Datenbereich der PivotTable leer ist. Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setDisplayNullString(boolean value) {#setDisplayNullString-boolean-}
```
public void setDisplayNullString(boolean value)
```


Gibt an, ob der PivotTable-Bericht einen benutzerdefinierten Text anzeigt, wenn der Wert null ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setEnableDataValueEditing(boolean value) {#setEnableDataValueEditing-boolean-}
```
public void setEnableDataValueEditing(boolean value)
```


Gibt einen booleschen Wert an, der angibt, ob der Benutzer die Zellen im Datenbereich der PivotTable bearbeiten darf. Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setEnableDrilldown(boolean value) {#setEnableDrilldown-boolean-}
```
public void setEnableDrilldown(boolean value)
```


Gibt an, ob Drilldown aktiviert ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setEnableFieldDialog(boolean value) {#setEnableFieldDialog-boolean-}
```
public void setEnableFieldDialog(boolean value)
```


Gibt an, ob das Dialogfeld PivotTable-Feld verfügbar ist, wenn der Benutzer das PivotTable-Feld doppelklickt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setEnableFieldList(boolean value) {#setEnableFieldList-boolean-}
```
public void setEnableFieldList(boolean value)
```


Gibt an, ob die Feldliste für die PivotTable in der Excel-Ansicht verfügbar ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setEnableWizard(boolean value) {#setEnableWizard-boolean-}
```
public void setEnableWizard(boolean value)
```


Gibt an, ob der PivotTable-Assistent verfügbar ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setErrorString(String value) {#setErrorString-java.lang.String-}
```
public void setErrorString(String value)
```


Ermittelt den Text, der in Zellen angezeigt wird, die Fehler enthalten, wenn die Eigenschaft DisplayErrorString true ist. Der Standardwert ist ein leerer String.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setExcel2003Compatible(boolean value) {#setExcel2003Compatible-boolean-}
```
public void setExcel2003Compatible(boolean value)
```


Gibt an, ob die PivotTable bei der Aktualisierung mit Excel2003 kompatibel ist; wenn true, muss ein String höchstens 255 Zeichen lang sein, andernfalls wird er abgeschnitten. Wenn false, gilt diese Beschränkung nicht. Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setFieldListSortAscending(boolean value) {#setFieldListSortAscending-boolean-}
```
public void setFieldListSortAscending(boolean value)
```


Gibt an, ob Felder in der PivotTable in der Feldliste in einer nicht standardmäßigen Reihenfolge sortiert sind.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setGrandTotalName(String value) {#setGrandTotalName-java.lang.String-}
```
public void setGrandTotalName(String value)
```


Gibt die Bezeichnung zurück, die in der Gesamtsumme‑Spalte oder -Zeilenüberschrift angezeigt wird. Der Standardwert ist die Zeichenkette "Grand Total".

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setGridDropZones(boolean value) {#setGridDropZones-boolean-}
```
public void setGridDropZones(boolean value)
```


Gibt an, ob der PivotTable-Bericht das klassische PivotTable-Layout anzeigt (ermöglicht das Ziehen von Feldern im Raster).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setHasBlankRows(boolean value) {#setHasBlankRows-boolean-}
```
public void setHasBlankRows(boolean value)
```


Gibt an, ob leere Zeilen hinzugefügt werden sollen. Diese Eigenschaft gilt nur für PivotTable-Autoformat-Typen, die leere Zeilen benötigen.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotField.InsertBlankRow. Diese Methode wird 12 Monate später, seit April 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setIndent(int value) {#setIndent-int-}
```
public void setIndent(int value)
```


Gibt die Einrückungssteigerung für die kompakte Achse an und kann verwendet werden, um das Berichtslayout auf kompakte Form einzustellen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setItemPrintTitles(boolean value) {#setItemPrintTitles-boolean-}
```
public void setItemPrintTitles(boolean value)
```


Gibt an, ob PivotItem-Namen oben auf jeder gedruckten Seite wiederholt werden sollen.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotTable.RepeatItemsOnEachPrintedPage. Diese Methode wird 12 Monate später, ab Oktober 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setManualUpdate(boolean value) {#setManualUpdate-boolean-}
```
public void setManualUpdate(boolean value)
```


Gibt an, ob der PivotTable-Bericht nur auf Anforderung des Benutzers neu berechnet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setMergeLabels(boolean value) {#setMergeLabels-boolean-}
```
public void setMergeLabels(boolean value)
```


Legt fest, ob Zeilen-/Spaltenfeldbeschriftungen, die sich über mehrere Zellen erstrecken, zusammengeführt werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setMissingItemsLimit(int value) {#setMissingItemsLimit-int-}
```
public void setMissingItemsLimit(int value)
```


Gibt einen booleschen Wert an, der angibt, ob die Felder einer Pivot-Tabelle mehrere Filter haben können.

Siehe [PivotMissingItemLimitType](../../com.aspose.cells/pivotmissingitemlimittype).

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotCache.MissingItemsLimit. Diese Methode wird 12 Monate später, ab September 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setMultipleFieldFilters(boolean value) {#setMultipleFieldFilters-boolean-}
```
public void setMultipleFieldFilters(boolean value)
```


Gibt einen booleschen Wert an, der angibt, ob die Felder einer Pivot-Tabelle mehrere Filter haben können.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotTable.AllowMultipleFiltersPerField. Diese Methode wird 12 Monate später, seit Dezember 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Ermittelt den Namen der PivotTable

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setNullString(String value) {#setNullString-java.lang.String-}
```
public void setNullString(String value)
```


Ruft die Zeichenkette ab, die in Zellen angezeigt wird, die Nullwerte enthalten, wenn die Eigenschaft DisplayNullString true ist. Der Standardwert ist eine leere Zeichenkette.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setPageFieldOrder(int value) {#setPageFieldOrder-int-}
```
public void setPageFieldOrder(int value)
```


Legt die Reihenfolge fest, in der Seitenfelder zum Layout des PivotTable-Berichts hinzugefügt werden.

Siehe [PrintOrderType](../../com.aspose.cells/printordertype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setPageFieldWrapCount(int value) {#setPageFieldWrapCount-int-}
```
public void setPageFieldWrapCount(int value)
```


Ruft die Anzahl der Seitenfelder in jeder Spalte oder Zeile im PivotTable-Bericht ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setPivotTableStyle(TableStyle value) {#setPivotTableStyle-com.aspose.cells.TableStyle-}
```
public void setPivotTableStyle(TableStyle value)
```


Ruft die [TableStyle](../../com.aspose.cells/tablestyle)-Einstellungen dieser Pivot-Tabelle ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [TableStyle](../../com.aspose.cells/tablestyle) |  |

### setPivotTableStyleName(String value) {#setPivotTableStyleName-java.lang.String-}
```
public void setPivotTableStyleName(String value)
```


Legt den Stilnamen der PivotTable fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setPivotTableStyleType(int value) {#setPivotTableStyleType-int-}
```
public void setPivotTableStyleType(int value)
```


Legt den integrierten PivotTable-Stil fest.

Siehe [PivotTableStyleType](../../com.aspose.cells/pivottablestyletype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setPreserveCellFormattingOnUpdate(boolean value) {#setPreserveCellFormattingOnUpdate-boolean-}
```
public void setPreserveCellFormattingOnUpdate(boolean value)
```


Gibt an, ob die Zellformatierung ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) beibehalten werden soll, wenn die Pivot-Tabelle aktualisiert oder neu berechnet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setPreserveFormatting(boolean value) {#setPreserveFormatting-boolean-}
```
public void setPreserveFormatting(boolean value)
```


Gibt an, ob die Zellformatierung ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) beibehalten wird, wenn die PivotTable aktualisiert oder neu berechnet wird.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotTable.PreserveCellFormattingOnUpdate. Diese Methode wird 12 Monate später, ab Juli 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setPrintDrill(boolean value) {#setPrintDrill-boolean-}
```
public void setPrintDrill(boolean value)
```


Gibt einen booleschen Wert an, der angibt, ob Drill‑Indikatoren gedruckt werden sollen. Druckt Expand/Collapse‑Schaltflächen, wenn sie in der PivotTable angezeigt werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setPrintTitles(boolean value) {#setPrintTitles-boolean-}
```
public void setPrintTitles(boolean value)
```


Gibt an, ob die Drucktitel für das Arbeitsblatt basierend auf dem PivotTable‑Bericht festgelegt werden. Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setRefreshDataOnOpeningFile(boolean value) {#setRefreshDataOnOpeningFile-boolean-}
```
public void setRefreshDataOnOpeningFile(boolean value)
```


Gibt an, ob Daten beim Öffnen der Datei aktualisiert werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setRepeatItemsOnEachPrintedPage(boolean value) {#setRepeatItemsOnEachPrintedPage-boolean-}
```
public void setRepeatItemsOnEachPrintedPage(boolean value)
```


Gibt an, ob Beschriftungen von Pivot-Elementen im Zeilenbereich auf jeder gedruckten Seite für Pivot-Felder in Tabellenform wiederholt werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setRowGrand(boolean value) {#setRowGrand-boolean-}
```
public void setRowGrand(boolean value)
```


Gibt an, ob Gesamtsummen für Zeilen dieser Pivot-Tabelle angezeigt werden sollen.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotTable.ShowRowGrandTotals. Diese Methode wird 12 Monate später, ab Dezember 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setRowHeaderCaption(String value) {#setRowHeaderCaption-java.lang.String-}
```
public void setRowHeaderCaption(String value)
```


Legt die benutzerdefinierte Beschriftung der Zeilenüberschrift in dieser PivotTable fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setSaveData(boolean value) {#setSaveData-boolean-}
```
public void setSaveData(boolean value)
```


Gibt an, ob Daten für den PivotTable-Bericht mit der Arbeitsmappe gespeichert werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSelected(boolean value) {#setSelected-boolean-}
```
public void setSelected(boolean value)
```


Gibt an, ob diese PivotTable ausgewählt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowColumnGrandTotals(boolean value) {#setShowColumnGrandTotals-boolean-}
```
public void setShowColumnGrandTotals(boolean value)
```


Gibt an, ob Gesamtsummen für die Spalten dieser PivotTable angezeigt werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowDataTips(boolean value) {#setShowDataTips-boolean-}
```
public void setShowDataTips(boolean value)
```


Gibt an, ob Tooltips für PivotTable-Datenzellen angezeigt werden sollen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowDrill(boolean value) {#setShowDrill-boolean-}
```
public void setShowDrill(boolean value)
```


Legt fest, ob Expand/Collapse-Schaltflächen angezeigt werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowEmptyCol(boolean value) {#setShowEmptyCol-boolean-}
```
public void setShowEmptyCol(boolean value)
```


Gibt an, ob leere Spalten in die Tabelle aufgenommen werden sollen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowEmptyRow(boolean value) {#setShowEmptyRow-boolean-}
```
public void setShowEmptyRow(boolean value)
```


Gibt an, ob leere Zeilen in die Tabelle aufgenommen werden sollen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowHeaders(boolean value) {#setShowHeaders-boolean-}
```
public void setShowHeaders(boolean value)
```


Ob Datenfeldbeschriftungen und Pivotfeldbeschriftungen auf der Zeilen‑ und Spaltenachse in der PivotTable‑Ansicht angezeigt werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowMemberPropertyTips(boolean value) {#setShowMemberPropertyTips-boolean-}
```
public void setShowMemberPropertyTips(boolean value)
```


Gibt einen booleschen Wert an, der festlegt, ob Mitgliedseigenschaftsinformationen aus PivotTable-Tooltips weggelassen werden sollen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowPivotStyleColumnHeader(boolean value) {#setShowPivotStyleColumnHeader-boolean-}
```
public void setShowPivotStyleColumnHeader(boolean value)
```


Gibt an, ob die Spaltenüberschrift in der PivotTable den Stil erhalten soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowPivotStyleColumnStripes(boolean value) {#setShowPivotStyleColumnStripes-boolean-}
```
public void setShowPivotStyleColumnStripes(boolean value)
```


Gibt an, ob für die Spalte Streifenformatierung angewendet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowPivotStyleLastColumn(boolean value) {#setShowPivotStyleLastColumn-boolean-}
```
public void setShowPivotStyleLastColumn(boolean value)
```


Gibt an, ob die Spaltenformatierung angewendet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowPivotStyleRowHeader(boolean value) {#setShowPivotStyleRowHeader-boolean-}
```
public void setShowPivotStyleRowHeader(boolean value)
```


Gibt an, ob die Zeilenüberschrift in der PivotTable den Stil erhalten soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowPivotStyleRowStripes(boolean value) {#setShowPivotStyleRowStripes-boolean-}
```
public void setShowPivotStyleRowStripes(boolean value)
```


Gibt an, ob Zeilenstreifenformatierung angewendet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowRowGrandTotals(boolean value) {#setShowRowGrandTotals-boolean-}
```
public void setShowRowGrandTotals(boolean value)
```


Gibt an, ob Gesamtsummen für die Zeilen der PivotTable angezeigt werden sollen.

**Remarks**

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowRowHeaderCaption(boolean value) {#setShowRowHeaderCaption-boolean-}
```
public void setShowRowHeaderCaption(boolean value)
```


Gibt an, ob die Zeilenüberschriftsbeschriftung im PivotTable-Bericht angezeigt wird. Gibt an, ob Feldbeschriftungen und Filter‑Dropdowns angezeigt werden.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotTable.ShowHeaders. Diese Methode wird 12 Monate später, seit April 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowValuesRow(boolean value) {#setShowValuesRow-boolean-}
```
public void setShowValuesRow(boolean value)
```


Gibt an, ob die Wertezeile angezeigt wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSubtotalHiddenPageItems(boolean value) {#setSubtotalHiddenPageItems-boolean-}
```
public void setSubtotalHiddenPageItems(boolean value)
```


Gibt an, ob versteckte Seitenfeld-Elemente im PivotTable-Bericht in Zeilen- und Spalten-Teilsummen, Blocksummen und Gesamtsummen einbezogen werden. Der Standardwert ist False.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setTag(String value) {#setTag-java.lang.String-}
```
public void setTag(String value)
```


Legt eine benutzerdefinierte Zeichenkette fest, die mit dieser PivotTable-Ansicht verknüpft ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### showDetail(int rowOffset, int columnOffset, boolean newSheet, int destRow, int destColumn) {#showDetail-int-int-boolean-int-int-}
```
public void showDetail(int rowOffset, int columnOffset, boolean newSheet, int destRow, int destColumn)
```


Zeige die Details eines Elements im Datenbereich in einer neuen Tabelle an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowOffset | int | Versatz zur ersten Datenzeile im Datenbereich. |
| columnOffset | int | Versatz zur ersten Datenspalte im Datenbereich. |
| newSheet | boolean | Zeige die Details in einem neuen Arbeitsblatt. |
| destRow | int | Die Zielzeile. |
| destColumn | int | Die Zielspalte. |

### showInCompactForm() {#showInCompactForm--}
```
public void showInCompactForm()
```


Gestaltet die PivotTable-Ansicht in kompakter Form.

### showInOutlineForm() {#showInOutlineForm--}
```
public void showInOutlineForm()
```


Gestaltet die PivotTable in Gliederungsform.

### showInTabularForm() {#showInTabularForm--}
```
public void showInTabularForm()
```


Gestaltet die PivotTable in Tabellenform.

### showReportFilterPage(PivotField pageField) {#showReportFilterPage-com.aspose.cells.PivotField-}
```
public void showReportFilterPage(PivotField pageField)
```


Zeige alle Berichtfilterseiten basierend auf dem PivotField an, das PivotField muss sich in den PageFields befinden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pageField | [PivotField](../../com.aspose.cells/pivotfield) | Das PivotField-Objekt |

### showReportFilterPageByIndex(int posIndex) {#showReportFilterPageByIndex-int-}
```
public void showReportFilterPageByIndex(int posIndex)
```


Zeige alle Berichtfilterseiten basierend auf dem Positionsindex in den PageFields an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| posIndex | int | Der Positionsindex in den PageFields |

### showReportFilterPageByName(String fieldName) {#showReportFilterPageByName-java.lang.String-}
```
public void showReportFilterPageByName(String fieldName)
```


Zeige alle Berichtfilterseiten basierend auf dem Namen des PivotField an, das PivotField muss sich in den PageFields befinden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldName | java.lang.String | Der Name von PivotField |

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

