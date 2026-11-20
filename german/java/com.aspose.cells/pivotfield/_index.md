---
title: "PivotField"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt ein Feld in einem PivotTable-Bericht dar."
type: docs
url: /de/java/com.aspose.cells/pivotfield/
---

**Inheritance:**
java.lang.Object
```
public class PivotField
```

Stellt ein Feld in einem PivotTable-Bericht dar.

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
 
          pivot.calculateData(new PivotTableCalculateOption());
 
         //do your business
 
         book.save("out.xlsx");
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [addCalculatedItem(String name, String formula)](#addCalculatedItem-java.lang.String-java.lang.String-) | Füge ein berechnetes Formelelement zum PivotField hinzu. |
| [clearFilter()](#clearFilter--) | Löscht die Filtereinstellung dieses PivotField. |
| [dispose()](#dispose--) | Führt anwendungsspezifische Aufgaben aus, die mit dem Freigeben, Freisetzen oder Zurücksetzen nicht verwalteter Ressourcen verbunden sind. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filterByDate(int type, DateTime dateTime1, DateTime dateTime2)](#filterByDate-int-com.aspose.cells.DateTime-com.aspose.cells.DateTime-) | Filtert nach Datumswerten des Zeilen- oder Spalten‑PivotField. |
| [filterByLabel(int type, String label1, String label2)](#filterByLabel-int-java.lang.String-java.lang.String-) | Filtert nach Beschriftungen des Zeilen- oder Spalten-Pivotfeldes. |
| [filterByValue(int valueFieldIndex, int type, double value1, double value2)](#filterByValue-int-int-double-double-) | Filtert nach Werten des Daten-Pivotfeldes. |
| [filterTop10(int valueFieldIndex, int type, boolean isTop, int itemCount)](#filterTop10-int-int-boolean-int-) | Filtert nach Werten des Daten-Pivotfeldes. |
| [getAllowDraggingToColumn()](#getAllowDraggingToColumn--) | Gibt an, ob das angegebene Feld in den Spaltenbereich gezogen werden kann. |
| [getAllowDraggingToData()](#getAllowDraggingToData--) | Gibt an, ob das angegebene Feld in den Wertebereich gezogen werden kann. |
| [getAllowDraggingToPage()](#getAllowDraggingToPage--) | Gibt an, ob das angegebene Feld in den Seitenbereich gezogen werden kann. |
| [getAllowDraggingToRow()](#getAllowDraggingToRow--) | Gibt an, ob das angegebene Feld in den Zeilenbereich gezogen werden kann. |
| [getAllowRemovingFromView()](#getAllowRemovingFromView--) | Gibt an, ob dieses PivotField aus der PivotTable‑Ansicht entfernt werden kann. |
| [getAutoShowCount()](#getAutoShowCount--) | Stellt die Anzahl der obersten oder untersten Elemente dar, die im angegebenen PivotTable‑Feld automatisch angezeigt werden. |
| [getAutoShowField()](#getAutoShowField--) | Stellt den Index des automatisch angezeigten Feldes dar. -1 bedeutet das PivotField selbst. |
| [getAutoSortField()](#getAutoSortField--) | Stellt den Index des automatisch sortierten Feldes dar. |
| [getBaseIndex()](#getBaseIndex--) | Stellt den Index in den Quell‑PivotFields dar. |
| [getCalculatedFieldFormula()](#getCalculatedFieldFormula--) | Hole die Formelkette des angegebenen berechneten Feldes. |
| [getClass()](#getClass--) |  |
| [getCurrentPageItem()](#getCurrentPageItem--) | Ruft das aktuell angezeigte Seitenelement für dieses PivotField ab (nur Seitenfeld). |
| [getCurrentPageItemText()](#getCurrentPageItemText--) | Ruft den Anzeigetext des aktuellen Seitenelements für dieses PivotField ab (nur Seitenfeld). |
| [getDisplayName()](#getDisplayName--) | Stellt den Anzeigenamen des PivotField in der PivotTable‑Ansicht dar. |
| [getDragToColumn()](#getDragToColumn--) | Gibt an, ob das angegebene Feld in den Spaltenbereich gezogen werden kann. |
| [getDragToData()](#getDragToData--) | Gibt an, ob das angegebene Feld in den Wertebereich gezogen werden kann. |
| [getDragToHide()](#getDragToHide--) | Gibt an, ob dieses PivotField aus der PivotTable‑Ansicht entfernt werden kann. |
| [getDragToPage()](#getDragToPage--) | Gibt an, ob das angegebene Feld in den Seitenbereich gezogen werden kann. |
| [getDragToRow()](#getDragToRow--) | Gibt an, ob das angegebene Feld in den Zeilenbereich gezogen werden kann. |
| [getFilters()](#getFilters--) | Ruft alle für dieses PivotField angewendeten Pivot-Filter ab. |
| [getFormula()](#getFormula--) | Ruft die Formel des berechneten Feldes ab. |
| [getFunction()](#getFunction--) | Stellt die Funktion dar, die verwendet wird, um dieses PivotTable-Datenfeld zusammenzufassen. |
| [getGroupSettings()](#getGroupSettings--) | Ruft die Gruppeneinstellungen des Pivot-Felds ab. |
| [getInsertBlankRow()](#getInsertBlankRow--) | Gibt an, ob nach jedem Element eine leere Zeile eingefügt werden soll. |
| [getItemCount()](#getItemCount--) | Ruft die Anzahl der Basiselemente in diesem Pivot-Feld ab. |
| [getItems()](#getItems--) | Alle Bezeichnungen der Pivot-Elemente in diesem Feld abrufen. |
| [getMaxValue()](#getMaxValue--) | Ruft den Maximalwert dieses Feldes ab. |
| [getMinValue()](#getMinValue--) | Ruft den Maximalwert dieses Feldes ab. |
| [getName()](#getName--) | Stellt den Namen von PivotField dar. |
| [getNonAutoSortDefault()](#getNonAutoSortDefault--) | Gibt an, ob ein Sortiervorgang, der auf dieses Pivot-Feld angewendet wird, ein Autosort-Vorgang oder ein einfacher Datensort ist. |
| [getNumber()](#getNumber--) | Stellt das integrierte Anzeigeformat von Zahlen und Datumsangaben dar. |
| [getNumberFormat()](#getNumberFormat--) | Stellt das benutzerdefinierte Anzeigeformat von Zahlen und Datumsangaben dar. |
| [getOriginalItems()](#getOriginalItems--) | Die ursprünglichen Basiselemente abrufen; |
| [getPivotFilterByType(int type)](#getPivotFilterByType-int-) | Ruft den Pivot-Filter des Pivot-Felds nach Typ ab |
| [getPivotFilters()](#getPivotFilters--) | Ruft die Pivot-Filter des Pivot-Felds ab |
| [getPivotItems()](#getPivotItems--) | Ruft die Pivot-Elemente des Pivot-Felds ab |
| [getPosition()](#getPosition--) | Stellt den Index von [PivotField](../../com.aspose.cells/pivotfield) in der Region dar. |
| [getRegionType()](#getRegionType--) | Gibt die Region der Pivot-Tabelle an, in der dieses Feld angezeigt wird. |
| [getShowAllItems()](#getShowAllItems--) | Gibt an, ob alle Elemente in der PivotTable-Ansicht angezeigt werden sollen, selbst wenn sie keine Zusammenfassungsdaten enthalten. |
| [getShowCompact()](#getShowCompact--) | Gibt an, ob die Bezeichnungen des nächsten Feldes in derselben Spalte in der Pivot-Tabellen-Ansicht angezeigt werden sollen. |
| [getShowInCompactForm()](#getShowInCompactForm--) | Ruft einen Wert ab, der angibt, ob dieses Zeilenfeld das kompakte Layout verwendet. |
| [getShowInOutlineForm()](#getShowInOutlineForm--) | Ruft einen Wert ab, der angibt, ob dieses Zeilenfeld das Gliederungslayout verwendet. |
| [getShowSubtotalAtTop()](#getShowSubtotalAtTop--) | Gibt an, ob Zwischensummen oben oder unten bei den Elementen angezeigt werden sollen. |
| [getShowValuesSetting()](#getShowValuesSetting--) | Ruft die Einstellungen zum Anzeigen von Werten ab, wenn die ShowDataAs-Berechnung verwendet wird. |
| [getSortSetting()](#getSortSetting--) | Ruft alle Einstellungen des automatischen Sortierens ab |
| [getSubtotals()](#getSubtotals--) | Ruft die Zwischensummen des Feldes ab. |
| [getSubtotals(int subtotalType)](#getSubtotals-int-) | Gibt an, ob die angegebene Zwischensumme für dieses Pivot-Feld angezeigt werden soll. |
| [getTop10AutoShowSettings()](#getTop10AutoShowSettings--) | Ruft die Top‑10‑AutoShow‑Einstellungen für ein Pivot‑Feld ab. |
| [group()](#group--) | Feld automatisch gruppieren. |
| [group(PivotFieldGroupOptions options)](#group-com.aspose.cells.PivotFieldGroupOptions-) | Gruppiert das Pivot‑Feld mit Optionen. |
| [groupBy(boolean isAutoStart, DateTime start, boolean isAutoEnd, DateTime end, int[] groups, double interval, boolean firstAsNewField)](#groupBy-boolean-com.aspose.cells.DateTime-boolean-com.aspose.cells.DateTime-int---double-boolean-) | Datei nach den Datumsgruppentypen gruppieren. |
| [groupBy(boolean isAutoStart, double start, boolean isAutoEnd, double end, double interval, boolean newField)](#groupBy-boolean-double-boolean-double-double-boolean-) | Datei nach Nummer gruppieren. |
| [groupBy(CustomPiovtFieldGroupItem[] customGroupItems, boolean newField)](#groupBy-com.aspose.cells.CustomPiovtFieldGroupItem---boolean-) | Feld benutzerdefiniert gruppieren. |
| [groupBy(DateTime start, DateTime end, int[] groups, double interval, boolean firstAsNewField)](#groupBy-com.aspose.cells.DateTime-com.aspose.cells.DateTime-int---double-boolean-) | Datei nach den Datumsgruppentypen gruppieren. |
| [groupBy(DiscreteGroupItem[] customGroupItems, boolean newField)](#groupBy-com.aspose.cells.DiscreteGroupItem---boolean-) | Feld benutzerdefiniert gruppieren. |
| [groupBy(double interval, boolean newField)](#groupBy-double-boolean-) | Feld automatisch mit Intervall gruppieren |
| [groupBy(double start, double end, double interval, boolean newField)](#groupBy-double-double-double-boolean-) | Datei nach Nummer gruppieren. |
| [groupBy(int[] groups, double interval, boolean newField)](#groupBy-int---double-boolean-) | Feld automatisch mit internal gruppieren |
| [hashCode()](#hashCode--) |  |
| [hideAllDetails()](#hideAllDetails--) | Blendet alle Details jedes Pivot‑Elements aus. |
| [hideDetail(boolean isHiddenDetail)](#hideDetail-boolean-) | Legt fest, ob die Details aller PivotItems in einem Pivot‑Feld ausgeblendet werden. |
| [hideItem(int index, boolean isHidden)](#hideItem-int-boolean-) | Legt fest, ob das bestimmte PivotItem in einem Datenfeld ausgeblendet ist. |
| [hideItem(String itemValue, boolean isHidden)](#hideItem-java.lang.String-boolean-) | Legt fest, ob das bestimmte PivotItem in einem Datenfeld ausgeblendet ist. |
| [hideItemDetail(int index, boolean isHiddenDetail)](#hideItemDetail-int-boolean-) | Legt fest, ob das bestimmte PivotItem in einem Pivot‑Feld Details ausblendet. |
| [initPivotItems()](#initPivotItems--) | Initialisiert die Pivot‑Items des Pivot‑Felds |
| [isAscendShow()](#isAscendShow--) | Gibt an, ob das angegebene PivotTable‑Feld aufsteigend automatisch angezeigt wird. |
| [isAscendSort()](#isAscendSort--) | Gibt an, ob die Elemente dieses Pivot‑Felds aufsteigend automatisch sortiert werden. |
| [isAutoShow()](#isAutoShow--) | Gibt an, ob das angegebene PivotTable‑Feld automatisch angezeigt wird. |
| [isAutoSort()](#isAutoSort--) | Gibt an, ob die Elemente dieses PivotTable‑Felds automatisch sortiert werden. |
| [isAutoSubtotals()](#isAutoSubtotals--) | Gibt an, ob das angegebene Feld automatische Zwischensummen anzeigt. |
| [isCalculatedField()](#isCalculatedField--) | Gibt an, ob dieses Pivot‑Feld ein berechnetes Feld ist. |
| [isHiddenItem(int index)](#isHiddenItem-int-) | Gibt an, ob das bestimmte PivotItem ausgeblendet ist. |
| [isHiddenItemDetail(int index)](#isHiddenItemDetail-int-) | Gibt an, ob die Details des bestimmten PivotItems ausgeblendet werden sollen. |
| [isIncludeNewItemsInFilter()](#isIncludeNewItemsInFilter--) | Gibt an, ob neue Elemente dem Feld im manuellen Filter hinzugefügt werden sollen. |
| [isInsertPageBreaksBetweenItems()](#isInsertPageBreaksBetweenItems--) | Gibt an, ob nach jedem Element Seitenumbrüche eingefügt werden sollen. |
| [isMultipleItemSelectionAllowed()](#isMultipleItemSelectionAllowed--) | Gibt an, ob im Seitenfeld mehrere Elemente ausgewählt werden können. |
| [isRepeatItemLabels()](#isRepeatItemLabels--) | Gibt an, ob die Beschriftungen des Feldes in der Zeilen‑ oder Spaltenregion wiederholt werden. |
| [isValueFields()](#isValueFields--) | Gibt an, ob dieses Feld Wertefelder darstellt. |
| [isValuesField()](#isValuesField--) | Gibt an, ob dieses Feld ein Wertefeld darstellt. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllowDraggingToColumn(boolean value)](#setAllowDraggingToColumn-boolean-) | Gibt an, ob das angegebene Feld in den Spaltenbereich gezogen werden kann. |
| [setAllowDraggingToData(boolean value)](#setAllowDraggingToData-boolean-) | Gibt an, ob das angegebene Feld in den Wertebereich gezogen werden kann. |
| [setAllowDraggingToPage(boolean value)](#setAllowDraggingToPage-boolean-) | Gibt an, ob das angegebene Feld in den Seitenbereich gezogen werden kann. |
| [setAllowDraggingToRow(boolean value)](#setAllowDraggingToRow-boolean-) | Gibt an, ob das angegebene Feld in den Zeilenbereich gezogen werden kann. |
| [setAllowRemovingFromView(boolean value)](#setAllowRemovingFromView-boolean-) | Gibt an, ob dieses PivotField aus der PivotTable‑Ansicht entfernt werden kann. |
| [setAscendShow(boolean value)](#setAscendShow-boolean-) | Gibt an, ob das angegebene PivotTable‑Feld aufsteigend automatisch angezeigt wird. |
| [setAscendSort(boolean value)](#setAscendSort-boolean-) | Gibt an, ob die Elemente dieses Pivot‑Felds aufsteigend automatisch sortiert werden. |
| [setAutoShow(boolean value)](#setAutoShow-boolean-) | Gibt an, ob das angegebene PivotTable‑Feld automatisch angezeigt wird. |
| [setAutoShowCount(int value)](#setAutoShowCount-int-) | Stellt die Anzahl der obersten oder untersten Elemente dar, die im angegebenen PivotTable‑Feld automatisch angezeigt werden. |
| [setAutoShowField(int value)](#setAutoShowField-int-) | Stellt den Index des automatisch angezeigten Feldes dar. -1 bedeutet das PivotField selbst. |
| [setAutoSort(boolean value)](#setAutoSort-boolean-) | Gibt an, ob die Elemente dieses PivotTable‑Felds automatisch sortiert werden. |
| [setAutoSortField(int value)](#setAutoSortField-int-) | Stellt den Index des automatisch sortierten Feldes dar. |
| [setAutoSubtotals(boolean value)](#setAutoSubtotals-boolean-) | Gibt an, ob das angegebene Feld automatische Zwischensummen anzeigt. |
| [setBaseIndex(int value)](#setBaseIndex-int-) | Stellt den Index in den Quell‑PivotFields dar. |
| [setCurrentPageItem(short value)](#setCurrentPageItem-short-) | Legt das aktuell angezeigte Seitenobjekt für dieses Pivotfeld fest (nur Seitenfeld). |
| [setCurrentPageItemText(String value)](#setCurrentPageItemText-java.lang.String-) | Ruft den Anzeigetext des aktuellen Seitenelements für dieses PivotField ab (nur Seitenfeld). |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | Stellt den Anzeigenamen des PivotField in der PivotTable‑Ansicht dar. |
| [setDragToColumn(boolean value)](#setDragToColumn-boolean-) | Gibt an, ob das angegebene Feld in den Spaltenbereich gezogen werden kann. |
| [setDragToData(boolean value)](#setDragToData-boolean-) | Gibt an, ob das angegebene Feld in den Wertebereich gezogen werden kann. |
| [setDragToHide(boolean value)](#setDragToHide-boolean-) | Gibt an, ob dieses PivotField aus der PivotTable‑Ansicht entfernt werden kann. |
| [setDragToPage(boolean value)](#setDragToPage-boolean-) | Gibt an, ob das angegebene Feld in den Seitenbereich gezogen werden kann. |
| [setDragToRow(boolean value)](#setDragToRow-boolean-) | Gibt an, ob das angegebene Feld in den Zeilenbereich gezogen werden kann. |
| [setFunction(int value)](#setFunction-int-) | Stellt die Funktion dar, die verwendet wird, um dieses PivotTable-Datenfeld zusammenzufassen. |
| [setIncludeNewItemsInFilter(boolean value)](#setIncludeNewItemsInFilter-boolean-) | Gibt an, ob neue Elemente dem Feld im manuellen Filter hinzugefügt werden sollen. |
| [setInsertBlankRow(boolean value)](#setInsertBlankRow-boolean-) | Gibt an, ob nach jedem Element eine leere Zeile eingefügt werden soll. |
| [setInsertPageBreaksBetweenItems(boolean value)](#setInsertPageBreaksBetweenItems-boolean-) | Gibt an, ob nach jedem Element Seitenumbrüche eingefügt werden sollen. |
| [setMultipleItemSelectionAllowed(boolean value)](#setMultipleItemSelectionAllowed-boolean-) | Gibt an, ob im Seitenfeld mehrere Elemente ausgewählt werden können. |
| [setName(String value)](#setName-java.lang.String-) | Stellt den Namen von PivotField dar. |
| [setNonAutoSortDefault(boolean value)](#setNonAutoSortDefault-boolean-) | Gibt an, ob ein Sortiervorgang, der auf dieses Pivot-Feld angewendet wird, ein Autosort-Vorgang oder ein einfacher Datensort ist. |
| [setNumber(int value)](#setNumber-int-) | Stellt das integrierte Anzeigeformat von Zahlen und Datumsangaben dar. |
| [setNumberFormat(String value)](#setNumberFormat-java.lang.String-) | Stellt das benutzerdefinierte Anzeigeformat von Zahlen und Datumsangaben dar. |
| [setRepeatItemLabels(boolean value)](#setRepeatItemLabels-boolean-) | Gibt an, ob die Beschriftungen des Feldes in der Zeilen‑ oder Spaltenregion wiederholt werden. |
| [setShowAllItems(boolean value)](#setShowAllItems-boolean-) | Gibt an, ob alle Elemente in der PivotTable-Ansicht angezeigt werden sollen, selbst wenn sie keine Zusammenfassungsdaten enthalten. |
| [setShowCompact(boolean value)](#setShowCompact-boolean-) | Gibt an, ob die Bezeichnungen des nächsten Feldes in derselben Spalte in der Pivot-Tabellen-Ansicht angezeigt werden sollen. |
| [setShowInCompactForm(boolean value)](#setShowInCompactForm-boolean-) | Legt einen Wert fest, der angibt, ob dieses Zeilenfeld das kompakte Layout verwendet. |
| [setShowInOutlineForm(boolean value)](#setShowInOutlineForm-boolean-) | Legt einen Wert fest, der angibt, ob dieses Zeilenfeld das Gliederungslayout verwendet. |
| [setShowSubtotalAtTop(boolean value)](#setShowSubtotalAtTop-boolean-) | Gibt an, ob Zwischensummen oben oder unten bei den Elementen angezeigt werden sollen. |
| [setSubtotals(int value)](#setSubtotals-int-) | Legt die Zwischensummen des Feldes fest. |
| [setSubtotals(int subtotalType, boolean shown)](#setSubtotals-int-boolean-) | Legt fest, wie das angegebene Feld zwischengesummiert wird. |
| [showAllDetails()](#showAllDetails--) | Alle Details jedes Pivot-Elements anzeigen. |
| [showValuesAs(int showValuesAsType, int baseField, int baseItem)](#showValuesAs-int-int-int-) | Legt die Berechnung „Werte anzeigen als“ für dieses Pivotfeld fest. |
| [showValuesAs(int displayFormat, int baseField, int baseItemPositionType, int baseItem)](#showValuesAs-int-int-int-int-) | Zeigt Werte des Datenfelds in einem anderen Anzeigeformat an, wenn die Berechnung ShowDataAs verwendet wird. |
| [showValuesAs(int showValuesAsType, String baseField, String baseItem)](#showValuesAs-int-java.lang.String-java.lang.String-) | Konfiguriert die Berechnung „Werte anzeigen als“ für dieses Datenfeld. |
| [sortBy(int sortType)](#sortBy-int-) | Sortiert dieses Pivotfeld. |
| [sortBy(int sortType, int fieldSortedBy)](#sortBy-int-int-) | Sortiert dieses Pivotfeld. |
| [sortBy(int sortType, int fieldSortedBy, int dataType, String cellName)](#sortBy-int-int-int-java.lang.String-) | Sortiert dieses Pivotfeld. |
| [sortBy(int sortType, int fieldSortedBy, String cellName)](#sortBy-int-int-java.lang.String-) | Sortiert dieses Pivotfeld. |
| [toString()](#toString--) |  |
| [top10AutoShow(boolean isAutoShow, boolean isTop, int count, int rankBy)](#top10AutoShow-boolean-boolean-int-int-) | Konfiguriert die Top10‑AutoShow‑Einstellungen für dieses Pivotfeld. |
| [ungroup()](#ungroup--) | Gruppierung des Pivotfelds aufheben. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addCalculatedItem(String name, String formula) {#addCalculatedItem-java.lang.String-java.lang.String-}
```
public void addCalculatedItem(String name, String formula)
```


Füge ein berechnetes Formelelement zum PivotField hinzu.

**Remarks**

Unterstützt nur das Hinzufügen berechneter Elemente zu Zeilen‑/Spaltenfeldern.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | Der Name des Elements. |
| formula | java.lang.String | Die Formel des Pivot‑Elements. |

### clearFilter() {#clearFilter--}
```
public void clearFilter()
```


Löscht die Filtereinstellung dieses PivotField.

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
### filterByDate(int type, DateTime dateTime1, DateTime dateTime2) {#filterByDate-int-com.aspose.cells.DateTime-com.aspose.cells.DateTime-}
```
public PivotFilter filterByDate(int type, DateTime dateTime1, DateTime dateTime2)
```


Filtert nach Datumswerten des Zeilen- oder Spalten‑PivotField.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Der Typ der zu filternden Daten. |
| dateTime1 | [DateTime](../../com.aspose.cells/datetime) | Das Datumslabel der Filterbedingung |
| dateTime2 | [DateTime](../../com.aspose.cells/datetime) | Das obere Datumslabel der Zwischenfilterbedingung |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### filterByLabel(int type, String label1, String label2) {#filterByLabel-int-java.lang.String-java.lang.String-}
```
public PivotFilter filterByLabel(int type, String label1, String label2)
```


Filtert nach Beschriftungen des Zeilen- oder Spalten-Pivotfeldes.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Der Typ der zu filternden Daten. |
| label1 | java.lang.String | Das Label der Filterbedingung |
| label2 | java.lang.String | Das obere Label der Zwischenfilterbedingung |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### filterByValue(int valueFieldIndex, int type, double value1, double value2) {#filterByValue-int-int-double-double-}
```
public PivotFilter filterByValue(int valueFieldIndex, int type, double value1, double value2)
```


Filtert nach Werten des Daten-Pivotfeldes.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| valueFieldIndex | int | Der Index des Wertefelds im Wertebereich. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Der Typ der zu filternden Daten. |
| value1 | double | Der Wert der Filterbedingung |
| value2 | double | Der obere Grenzwert der Zwischenfilterbedingung |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### filterTop10(int valueFieldIndex, int type, boolean isTop, int itemCount) {#filterTop10-int-int-boolean-int-}
```
public PivotFilter filterTop10(int valueFieldIndex, int type, boolean isTop, int itemCount)
```


Filtert nach Werten des Daten-Pivotfeldes.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| valueFieldIndex | int | Der Index des Datenfelds im Datenbereich. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Der Typ der Datenfilterung. Es können nur Count, Sum und Percent sein. |
| isTop | boolean | Gibt an, ob der Filter von oben oder unten ist. |
| itemCount | int | Die Elementanzahl |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### getAllowDraggingToColumn() {#getAllowDraggingToColumn--}
```
public boolean getAllowDraggingToColumn()
```


Gibt an, ob das angegebene Feld in den Spaltenbereich gezogen werden kann. Der Standardwert ist true.

**Returns:**
boolean
### getAllowDraggingToData() {#getAllowDraggingToData--}
```
public boolean getAllowDraggingToData()
```


Gibt an, ob das angegebene Feld in den Wertebereich gezogen werden kann. Der Standardwert ist true.

**Returns:**
boolean
### getAllowDraggingToPage() {#getAllowDraggingToPage--}
```
public boolean getAllowDraggingToPage()
```


Gibt an, ob das angegebene Feld in den Seitenbereich gezogen werden kann. Der Standardwert ist true.

**Returns:**
boolean
### getAllowDraggingToRow() {#getAllowDraggingToRow--}
```
public boolean getAllowDraggingToRow()
```


Gibt an, ob das angegebene Feld in den Zeilenbereich gezogen werden kann. Der Standardwert ist true.

**Returns:**
boolean
### getAllowRemovingFromView() {#getAllowRemovingFromView--}
```
public boolean getAllowRemovingFromView()
```


Gibt an, ob dieses Pivotfeld aus der PivotTable‑Ansicht entfernt werden kann. Der Standardwert ist true.

**Returns:**
boolean
### getAutoShowCount() {#getAutoShowCount--}
```
public int getAutoShowCount()
```


Stellt die Anzahl der obersten oder untersten Elemente dar, die im angegebenen PivotTable‑Feld automatisch angezeigt werden.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft **PivotField.Top10AutoShowSettings.AutoShowCount** oder die Methode **PivotField.Top10AutoShow()**. Diese Methode wird 12 Monate nach September 2026 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Returns:**
int
### getAutoShowField() {#getAutoShowField--}
```
public int getAutoShowField()
```


Stellt den Index des automatischen Anzeige‑feldes dar. -1 bedeutet das PivotField selbst. Es sollte der Index der Datenfelder sein.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft **PivotField.Top10AutoShowSettings.RankBy** oder die Methode **PivotField.Top10AutoShow()**. Diese Methode wird 12 Monate nach September 2026 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Returns:**
int
### getAutoSortField() {#getAutoSortField--}
```
public int getAutoSortField()
```


Stellt den Index des Feldes dar, das automatisch sortiert wird. -1 bedeutet das PivotField selbst, andere bedeuten die Position der Datenfelder.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotField.SortSetting.SortBy oder die Methode PivotField.SortBy(). Diese Methode wird 12 Monate später, seit September 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
int
### getBaseIndex() {#getBaseIndex--}
```
public int getBaseIndex()
```


Stellt den Index in den Quell‑PivotFields dar.

**Remarks**

HINWEIS: Dieser Setter dieser Eigenschaft ist jetzt veraltet. Dieser Setter dieser Eigenschaft wird 12 Monate später, seit September 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
int
### getCalculatedFieldFormula() {#getCalculatedFieldFormula--}
```
public String getCalculatedFieldFormula()
```


Hole die Formelkette des angegebenen berechneten Feldes.

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotField.GetFormula(). Diese Methode wird 12 Monate später, seit August 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCurrentPageItem() {#getCurrentPageItem--}
```
public short getCurrentPageItem()
```


Ruft das aktuell angezeigte Seitenelement für dieses PivotField ab (nur Seitenfeld).

**Remarks**

Verwenden Sie [PivotItem.ALL\_PAGE\_ITEMS\_INDEX](../../com.aspose.cells/pivotitem\#ALL-PAGE-ITEMS-INDEX) (0x7FFD) als Sentinelwert, um "Alle auswählen" anzuzeigen. Dies ist ein vordefinierter Marker und kein gültiger Elementindex.

**Returns:**
short
### getCurrentPageItemText() {#getCurrentPageItemText--}
```
public String getCurrentPageItemText()
```


Ruft den Anzeigetext des aktuellen Seitenelements für dieses PivotField ab (nur Seitenfeld).

**Remarks**

Gibt "(All)" zurück, wenn [getCurrentPageItem()](../../com.aspose.cells/pivotfield\#getCurrentPageItem--) gleich [PivotItem.ALL\_PAGE\_ITEMS\_INDEX](../../com.aspose.cells/pivotitem\#ALL-PAGE-ITEMS-INDEX) ist. Für andere Werte wird die Zeichenkettenrepräsentation des Elementindexes zurückgegeben.

**Returns:**
java.lang.String
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Stellt den Anzeigenamen des PivotField in der PivotTable‑Ansicht dar.

**Returns:**
java.lang.String
### getDragToColumn() {#getDragToColumn--}
```
public boolean getDragToColumn()
```


Gibt an, ob das angegebene Feld in den Spaltenbereich gezogen werden kann. Der Standardwert ist true.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotField.AllowDraggingToColumn. Diese Methode wird 12 Monate später, seit Juli 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
boolean
### getDragToData() {#getDragToData--}
```
public boolean getDragToData()
```


Gibt an, ob das angegebene Feld in den Wertebereich gezogen werden kann. Der Standardwert ist true.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotField.AllowDraggingToData. Diese Methode wird 12 Monate später, seit Juli 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
boolean
### getDragToHide() {#getDragToHide--}
```
public boolean getDragToHide()
```


Gibt an, ob dieses Pivotfeld aus der PivotTable‑Ansicht entfernt werden kann. Der Standardwert ist true.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotField.AllowRemovingFromView. Diese Methode wird 12 Monate später, seit Juli 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
boolean
### getDragToPage() {#getDragToPage--}
```
public boolean getDragToPage()
```


Gibt an, ob das angegebene Feld in den Seitenbereich gezogen werden kann. Der Standardwert ist true.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotField.AllowDraggingToPage. Diese Methode wird 12 Monate später, seit Juli 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
boolean
### getDragToRow() {#getDragToRow--}
```
public boolean getDragToRow()
```


Gibt an, ob das angegebene Feld in den Zeilenbereich gezogen werden kann. Der Standardwert ist true.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotField.AllowDraggingToRow. Diese Methode wird 12 Monate später, seit Juli 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
boolean
### getFilters() {#getFilters--}
```
public PivotFilter[] getFilters()
```


Ruft alle für dieses PivotField angewendeten Pivot-Filter ab.

**Returns:**
com.aspose.cells.PivotFilter[]
### getFormula() {#getFormula--}
```
public String getFormula()
```


Gibt die Formel des berechneten Feldes zurück. Funktioniert nur für das berechnete Feld.

**Returns:**
java.lang.String
### getFunction() {#getFunction--}
```
public int getFunction()
```


Stellt die Funktion dar, die verwendet wird, um dieses PivotTable-Datenfeld zusammenzufassen.

Siehe [ConsolidationFunction](../../com.aspose.cells/consolidationfunction).

**Returns:**
int
### getGroupSettings() {#getGroupSettings--}
```
public PivotFieldGroupSettings getGroupSettings()
```


Ruft die Gruppeneinstellungen des Pivot-Felds ab.

**Remarks**

Wenn dieses Feld nicht gruppiert ist, wird Null zurückgegeben.

**Returns:**
[PivotFieldGroupSettings](../../com.aspose.cells/pivotfieldgroupsettings)
### getInsertBlankRow() {#getInsertBlankRow--}
```
public boolean getInsertBlankRow()
```


Gibt an, ob nach jedem Element eine leere Zeile eingefügt werden soll. Nur für Zeilenfelder.

**Returns:**
boolean
### getItemCount() {#getItemCount--}
```
public int getItemCount()
```


Ruft die Anzahl der Basiselemente in diesem Pivot-Feld ab.

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotField.PivotItems.Count. Diese Methode wird 12 Monate später, seit August 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
int
### getItems() {#getItems--}
```
public String[] getItems()
```


Alle Bezeichnungen der Pivot-Elemente in diesem Feld abrufen.

**Returns:**
java.lang.String[]
### getMaxValue() {#getMaxValue--}
```
public CellValue getMaxValue()
```


Ruft den Maximalwert dieses Feldes ab.

**Remarks**

Funktioniert nur für Zeilen- oder Spaltenfelder, deren Wert Datum/Zeit, Zahl oder leer sein muss.

**Returns:**
[CellValue](../../com.aspose.cells/cellvalue) - 
### getMinValue() {#getMinValue--}
```
public CellValue getMinValue()
```


Ruft den Maximalwert dieses Feldes ab.

**Remarks**

Funktioniert nur für Zeilen- oder Spaltenfelder, deren Wert Datum/Zeit, Zahl oder leer sein muss.

**Returns:**
[CellValue](../../com.aspose.cells/cellvalue) - 
### getName() {#getName--}
```
public String getName()
```


Stellt den Namen von PivotField dar.

**Returns:**
java.lang.String
### getNonAutoSortDefault() {#getNonAutoSortDefault--}
```
public boolean getNonAutoSortDefault()
```


Gibt an, ob ein Sortiervorgang, der auf dieses Pivot-Feld angewendet wird, ein Autosort-Vorgang oder ein einfacher Datensort ist.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die !PivotField.SortSetting.IsSimpleSort‑Eigenschaft. Diese Methode wird 12 Monate später, seit September 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
boolean
### getNumber() {#getNumber--}
```
public int getNumber()
```


Stellt das integrierte Anzeigeformat von Zahlen und Datumsangaben dar.

**Returns:**
int
### getNumberFormat() {#getNumberFormat--}
```
public String getNumberFormat()
```


Stellt das benutzerdefinierte Anzeigeformat von Zahlen und Datumsangaben dar.

**Returns:**
java.lang.String
### getOriginalItems() {#getOriginalItems--}
```
public String[] getOriginalItems()
```


Die ursprünglichen Basiselemente abrufen;

**Returns:**
java.lang.String[]
### getPivotFilterByType(int type) {#getPivotFilterByType-int-}
```
public PivotFilter getPivotFilterByType(int type)
```


Ruft den Pivot-Filter des Pivot-Felds nach Typ ab

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | int |  |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### getPivotFilters() {#getPivotFilters--}
```
public ArrayList getPivotFilters()
```


Ruft die Pivot-Filter des Pivot-Felds ab

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die PivotField.GetFilters()‑Methode. Diese Methode wird 12 Monate später, seit November 2023, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
java.util.ArrayList
### getPivotItems() {#getPivotItems--}
```
public PivotItemCollection getPivotItems()
```


Ruft die Pivot-Elemente des Pivot-Felds ab

**Returns:**
[PivotItemCollection](../../com.aspose.cells/pivotitemcollection)
### getPosition() {#getPosition--}
```
public int getPosition()
```


Stellt den Index von [PivotField](../../com.aspose.cells/pivotfield) in der Region dar.

**Returns:**
int
### getRegionType() {#getRegionType--}
```
public int getRegionType()
```


Gibt die Region der Pivot-Tabelle an, in der dieses Feld angezeigt wird.

Siehe [PivotFieldType](../../com.aspose.cells/pivotfieldtype).

**Returns:**
int
### getShowAllItems() {#getShowAllItems--}
```
public boolean getShowAllItems()
```


Gibt an, ob alle Elemente in der PivotTable‑Ansicht angezeigt werden sollen, selbst wenn sie keine Zusammenfassungsdaten enthalten. Der Standardwert ist false.

**Returns:**
boolean
### getShowCompact() {#getShowCompact--}
```
public boolean getShowCompact()
```


Gibt an, ob die Bezeichnungen des nächsten Feldes in derselben Spalte in der Pivot‑Tabellen‑Ansicht angezeigt werden sollen. Nur für Zeilenfelder.

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die PivotField.ShowInCompactForm‑Eigenschaft. Diese Methode wird 12 Monate später, seit November 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
boolean
### getShowInCompactForm() {#getShowInCompactForm--}
```
public boolean getShowInCompactForm()
```


Gibt einen Wert zurück, der angibt, ob dieses Zeilenfeld das kompakte Layout verwendet. Gilt nur für Zeilenfelder.

**Remarks**

Kompaktes Layout ist ein Untermodus des Gliederungs‑Layouts. Diese Einstellung wirkt nur, wenn [getShowInOutlineForm()](../../com.aspose.cells/pivotfield\#getShowInOutlineForm--) true ist.

**Returns:**
boolean
### getShowInOutlineForm() {#getShowInOutlineForm--}
```
public boolean getShowInOutlineForm()
```


Gibt einen Wert zurück, der angibt, ob dieses Zeilenfeld das Gliederungs‑Layout verwendet. Gilt nur für Zeilenfelder.

**Returns:**
boolean
### getShowSubtotalAtTop() {#getShowSubtotalAtTop--}
```
public boolean getShowSubtotalAtTop()
```


Gibt an, ob Zwischensummen oben oder unten bei den Elementen angezeigt werden sollen.

**Remarks**

Funktioniert nur für die Pivot‑Felder im Zeilenbereich, wenn ShowInOutlineForm true ist.

**Returns:**
boolean
### getShowValuesSetting() {#getShowValuesSetting--}
```
public PivotShowValuesSetting getShowValuesSetting()
```


Ruft die Einstellungen zum Anzeigen von Werten ab, wenn die ShowDataAs-Berechnung verwendet wird.

**Returns:**
[PivotShowValuesSetting](../../com.aspose.cells/pivotshowvaluessetting)
### getSortSetting() {#getSortSetting--}
```
public PivotFieldSortSetting getSortSetting()
```


Ruft alle Einstellungen des automatischen Sortierens ab

**Returns:**
[PivotFieldSortSetting](../../com.aspose.cells/pivotfieldsortsetting)
### getSubtotals() {#getSubtotals--}
```
public int getSubtotals()
```


Gibt die Zwischensummen des Feldes zurück. Nur für Zeilen‑ oder Spalten‑Pivot‑Felder.

Siehe [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype).

**Example**

```
         //No subtotals
         rowField.setSubtotals(PivotFieldSubtotalType.NONE);
         //Automatic subtotals
         //rowField.Subtotals = PivotFieldSubtotalType.Automatic;
         //Single subtotals: Sum
         //rowField.Subtotals = PivotFieldSubtotalType.Sum;
         //Multipl subtotals: Sum and count numbers 
         //rowField.Subtotals = PivotFieldSubtotalType.Sum | PivotFieldSubtotalType.Count;
```

**Returns:**
int
### getSubtotals(int subtotalType) {#getSubtotals-int-}
```
public boolean getSubtotals(int subtotalType)
```


Gibt an, ob die angegebene Zwischensumme für dieses Pivot-Feld angezeigt werden soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| subtotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). Zwischensummentyp. |

**Returns:**
boolean – Gibt zurück, ob die angegebene Zwischensumme angezeigt wird.
### getTop10AutoShowSettings() {#getTop10AutoShowSettings--}
```
public PivotFieldTop10AutoShowSettings getTop10AutoShowSettings()
```


Ruft die Top‑10‑AutoShow‑Einstellungen für ein Pivot‑Feld ab.

**Returns:**
[PivotFieldTop10AutoShowSettings](../../com.aspose.cells/pivotfieldtop10autoshowsettings)
### group() {#group--}
```
public boolean group()
```


Feld automatisch gruppieren.

**Remarks**

Wenn das Feld nur leere Werte und Datum/Zeit enthält, wird das Feld nach Monaten gruppiert. Wenn das Feld nur leere Werte und Zahlen enthält, wird das Feld nach Zahlen gruppiert. Andernfalls wird nur false zurückgegeben, ohne irgendeine Gruppierung.

**Returns:**
boolean
### group(PivotFieldGroupOptions options) {#group-com.aspose.cells.PivotFieldGroupOptions-}
```
public boolean group(PivotFieldGroupOptions options)
```


Gruppiert das Pivot‑Feld mit Optionen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| options | [PivotFieldGroupOptions](../../com.aspose.cells/pivotfieldgroupoptions) | Optionen für die Gruppierungseinstellungen des Pivot-Feldes. |

**Returns:**
boolean -
### groupBy(boolean isAutoStart, DateTime start, boolean isAutoEnd, DateTime end, int[] groups, double interval, boolean firstAsNewField) {#groupBy-boolean-com.aspose.cells.DateTime-boolean-com.aspose.cells.DateTime-int---double-boolean-}
```
public boolean groupBy(boolean isAutoStart, DateTime start, boolean isAutoEnd, DateTime end, int[] groups, double interval, boolean firstAsNewField)
```


Datei nach den Datumsgruppentypen gruppieren.

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die PivotField.Group(PivotFieldGroupOptions)‑Methode. Diese Methode wird 6 Monate später, seit September 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isAutoStart | boolean | Gibt an, ob das Start‑Datum/Zeit‑Wert automatisch erkannt werden soll. |
| start | [DateTime](../../com.aspose.cells/datetime) | Das Start‑Datum/Zeit |
| isAutoEnd | boolean | Gibt an, ob das End‑Datum/Zeit‑Wert automatisch erkannt werden soll. |
| end | [DateTime](../../com.aspose.cells/datetime) | Das Ende des Datums/Zeit |
| groups | int[] | [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype). Gruppierungstypen |
| Intervall | double | Das Intervall |
| firstAsNewField | boolean | Gibt an, ob ein neues Feld zur Pivot‑Tabelle hinzugefügt wird. Nur für das erste Gruppenelement. |

**Returns:**
boolesch - False bedeutet, dass dieses Feld nicht nach Datum/Zeit gruppiert werden kann.
### groupBy(boolean isAutoStart, double start, boolean isAutoEnd, double end, double interval, boolean newField) {#groupBy-boolean-double-boolean-double-double-boolean-}
```
public boolean groupBy(boolean isAutoStart, double start, boolean isAutoEnd, double end, double interval, boolean newField)
```


Datei nach Nummer gruppieren.

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die PivotField.Group(PivotFieldGroupOptions)‑Methode. Diese Methode wird 6 Monate später, seit September 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isAutoStart | boolean | Gibt an, ob der Startwert automatisch erkannt werden soll. |
| Start | double | Der Startwert |
| isAutoEnd | boolean | Gibt an, ob der Endwert automatisch erkannt werden soll. |
| Ende | double | Der Endwert |
| Intervall | double | Das Intervall |
| newField | boolean | Gibt an, ob ein neues Feld zur Pivot‑Tabelle hinzugefügt wird |

**Returns:**
boolesch - False bedeutet, dass dieses Feld nicht nach Datum/Zeit gruppiert werden kann.
### groupBy(CustomPiovtFieldGroupItem[] customGroupItems, boolean newField) {#groupBy-com.aspose.cells.CustomPiovtFieldGroupItem---boolean-}
```
public boolean groupBy(CustomPiovtFieldGroupItem[] customGroupItems, boolean newField)
```


Feld benutzerdefiniert gruppieren.

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotField.Group(PivotFieldGroupOptions options) mit der Eigenschaft PivotFieldGroupOptions.DiscreteGroupItems. Diese Methode wird 6 Monate später, ab Juli 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| customGroupItems | [CustomPiovtFieldGroupItem\[\]](../../com.aspose.cells/custompiovtfieldgroupitem) | Die benutzerdefinierten Gruppenelemente. |
| newField | boolean | Gibt an, ob ein neues Feld zur Pivot‑Tabelle hinzugefügt wird |

**Returns:**
boolesch - False bedeutet, dass dieses Feld nicht nach Datum/Zeit gruppiert werden kann.
### groupBy(DateTime start, DateTime end, int[] groups, double interval, boolean firstAsNewField) {#groupBy-com.aspose.cells.DateTime-com.aspose.cells.DateTime-int---double-boolean-}
```
public boolean groupBy(DateTime start, DateTime end, int[] groups, double interval, boolean firstAsNewField)
```


Datei nach den Datumsgruppentypen gruppieren.

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die PivotField.Group(PivotFieldGroupOptions)‑Methode. Diese Methode wird 6 Monate später, seit September 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| start | [DateTime](../../com.aspose.cells/datetime) | Das Start‑Datum/Zeit |
| end | [DateTime](../../com.aspose.cells/datetime) | Das Ende des Datums/Zeit |
| groups | int[] | [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype). Gruppierungstypen |
| Intervall | double | Das Intervall |
| firstAsNewField | boolean | Gibt an, ob ein neues Feld zur Pivot‑Tabelle hinzugefügt wird. Nur für das erste Gruppenelement. |

**Returns:**
boolesch - False bedeutet, dass dieses Feld nicht nach Datum/Zeit gruppiert werden kann.
### groupBy(DiscreteGroupItem[] customGroupItems, boolean newField) {#groupBy-com.aspose.cells.DiscreteGroupItem---boolean-}
```
public boolean groupBy(DiscreteGroupItem[] customGroupItems, boolean newField)
```


Feld benutzerdefiniert gruppieren.

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotField.Group(PivotFieldGroupOptions options) mit der Eigenschaft PivotFieldGroupOptions.DiscreteGroupItems. Diese Methode wird 6 Monate später, ab Juli 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| customGroupItems | [DiscreteGroupItem\[\]](../../com.aspose.cells/discretegroupitem) | Die benutzerdefinierten Gruppenelemente. |
| newField | boolean | Gibt an, ob ein neues Feld zur Pivot‑Tabelle hinzugefügt wird |

**Returns:**
boolean -
### groupBy(double interval, boolean newField) {#groupBy-double-boolean-}
```
public void groupBy(double interval, boolean newField)
```


Feld automatisch mit Intervall gruppieren

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die PivotField.Group(PivotFieldGroupOptions)‑Methode. Diese Methode wird 6 Monate später, seit September 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Intervall | double | Der interne Wert der Gruppe. Ein automatischer Wert wird zugewiesen, wenn er Null ist, |
| newField | boolean | Gibt an, ob ein neues Feld zur Pivot‑Tabelle hinzugefügt wird. Nur für DateTime‑Gruppen. |

### groupBy(double start, double end, double interval, boolean newField) {#groupBy-double-double-double-boolean-}
```
public boolean groupBy(double start, double end, double interval, boolean newField)
```


Datei nach Nummer gruppieren.

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die PivotField.Group(PivotFieldGroupOptions)‑Methode. Diese Methode wird 6 Monate später, seit September 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Start | double | Der Startwert |
| Ende | double | Der Endwert |
| Intervall | double | Das Intervall |
| newField | boolean | Gibt an, ob ein neues Feld zur Pivot‑Tabelle hinzugefügt wird |

**Returns:**
boolesch - False bedeutet, dass dieses Feld nicht nach Datum/Zeit gruppiert werden kann.
### groupBy(int[] groups, double interval, boolean newField) {#groupBy-int---double-boolean-}
```
public void groupBy(int[] groups, double interval, boolean newField)
```


Feld automatisch mit internal gruppieren

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die PivotField.Group(PivotFieldGroupOptions)‑Methode. Diese Methode wird 6 Monate später, seit September 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| groups | int[] | [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype). Gruppierungstypen |
| Intervall | double | Der interne Wert der Gruppe. Ein automatischer Wert wird zugewiesen, wenn er Null ist, funktioniert nur für die Gruppierung nach Zahlen oder Tagen. |
| newField | boolean | Gibt an, ob ein neues Feld zur Pivot‑Tabelle hinzugefügt wird. |

### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### hideAllDetails() {#hideAllDetails--}
```
public void hideAllDetails()
```


Blendet alle Details jedes Pivot‑Elements aus.

### hideDetail(boolean isHiddenDetail) {#hideDetail-boolean-}
```
public void hideDetail(boolean isHiddenDetail)
```


Legt fest, ob die Details aller PivotItems in einem Pivot‑Feld ausgeblendet sind. Das heißt, dieses Feld zusammen- bzw. ausklappen.

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Methoden PivotItemsCollection.HideAllDetails() und UnhideAllDetails(). Diese Methode wird 12 Monate später, ab November 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isHiddenDetail | boolean | Gibt an, ob die Details des Pivot-Feldes ausgeblendet werden. |

### hideItem(int index, boolean isHidden) {#hideItem-int-boolean-}
```
public void hideItem(int index, boolean isHidden)
```


Legt fest, ob das bestimmte PivotItem in einem Datenfeld ausgeblendet ist.

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotField.PivotItems[int].IsHidden. Diese Methode wird 12 Monate später, ab August 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der Index des PivotItems im PivotField. |
| isHidden | boolean | Ob das spezifische PivotItem ausgeblendet ist |

### hideItem(String itemValue, boolean isHidden) {#hideItem-java.lang.String-boolean-}
```
public void hideItem(String itemValue, boolean isHidden)
```


Legt fest, ob das bestimmte PivotItem in einem Datenfeld ausgeblendet ist.

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotField.PivotItems[string].IsHidden. Diese Methode wird 12 Monate später, ab August 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| itemValue | java.lang.String | Der Name des PivotItems im PivotField. |
| isHidden | boolean | Ob das spezifische PivotItem ausgeblendet ist |

### hideItemDetail(int index, boolean isHiddenDetail) {#hideItemDetail-int-boolean-}
```
public void hideItemDetail(int index, boolean isHiddenDetail)
```


Legt fest, ob das bestimmte PivotItem in einem Pivot‑Feld Details ausblendet.

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotField.PivotItems[int].IsDetailHidden. Diese Methode wird 12 Monate später, ab August 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der Index des PivotItems im PivotField. |
| isHiddenDetail | boolean | Ob das spezifische PivotItem ausgeblendet ist |

### initPivotItems() {#initPivotItems--}
```
public void initPivotItems()
```


Initialisiert die Pivot‑Items des Pivot‑Felds

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Bitte entfernen Sie einfach den Aufruf dieser Methode. Diese Methode wird 6 Monate später, seit Oktober 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

### isAscendShow() {#isAscendShow--}
```
public boolean isAscendShow()
```


Gibt an, ob das angegebene PivotTable‑Feld aufsteigend automatisch angezeigt wird.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Stattdessen verwenden Sie bitte die Eigenschaft PivotField.Top10AutoShowSettings.IsTop oder die Methode PivotField.Top10AutoShow(). Diese Methode wird 12 Monate später, seit September 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

**Returns:**
boolean
### isAscendSort() {#isAscendSort--}
```
public boolean isAscendSort()
```


Gibt an, ob die Elemente dieses Pivot‑Felds aufsteigend automatisch sortiert werden.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Stattdessen verwenden Sie bitte die Eigenschaft PivotField.SortSetting.SortType oder die Methode PivotField.SortBy(). Diese Methode wird 12 Monate später, seit September 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

**Returns:**
boolean
### isAutoShow() {#isAutoShow--}
```
public boolean isAutoShow()
```


Gibt an, ob das angegebene PivotTable‑Feld automatisch angezeigt wird.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Stattdessen verwenden Sie bitte die Eigenschaft PivotField.Top10AutoShowSettings.IsAutoShow oder die Methode PivotField.Top10AutoShow(). Diese Methode wird 12 Monate später, seit September 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

**Returns:**
boolean
### isAutoSort() {#isAutoSort--}
```
public boolean isAutoSort()
```


Gibt an, ob die Elemente dieses PivotTable‑Felds automatisch sortiert werden.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Stattdessen verwenden Sie bitte die Eigenschaft PivotField.SortSetting.SortType oder die Methode PivotField.SortBy(). Diese Methode wird 12 Monate später, seit September 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

**Returns:**
boolean
### isAutoSubtotals() {#isAutoSubtotals--}
```
public boolean isAutoSubtotals()
```


Gibt an, ob das angegebene Feld automatische Zwischensummen anzeigt. Standard ist true.

**Returns:**
boolean
### isCalculatedField() {#isCalculatedField--}
```
public boolean isCalculatedField()
```


Gibt an, ob dieses Pivot‑Feld ein berechnetes Feld ist.

**Returns:**
boolean
### isHiddenItem(int index) {#isHiddenItem-int-}
```
public boolean isHiddenItem(int index)
```


Gibt an, ob das bestimmte PivotItem ausgeblendet ist.

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotField.PivotItems[int].IsHidden. Diese Methode wird 12 Monate später, ab August 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der Index des PivotItem im PivotField. |

**Returns:**
boolean – ob das spezifische PivotItem ausgeblendet ist
### isHiddenItemDetail(int index) {#isHiddenItemDetail-int-}
```
public boolean isHiddenItemDetail(int index)
```


Gibt an, ob die Details des bestimmten PivotItems ausgeblendet werden sollen.

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotField.PivotItems[int].IsDetailHidden. Diese Methode wird 12 Monate später, ab August 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der Index des PivotItem im PivotField. |

**Returns:**
boolean – ob das spezifische PivotItem ausgeblendete Details hat
### isIncludeNewItemsInFilter() {#isIncludeNewItemsInFilter--}
```
public boolean isIncludeNewItemsInFilter()
```


Gibt an, ob neue Elemente im Feld in manuellen Filtern einbezogen werden sollen. Der Standardwert ist false.

**Returns:**
boolean
### isInsertPageBreaksBetweenItems() {#isInsertPageBreaksBetweenItems--}
```
public boolean isInsertPageBreaksBetweenItems()
```


Gibt an, ob nach jedem Element Seitenumbrüche eingefügt werden sollen. Der Standardwert ist false.

**Returns:**
boolean
### isMultipleItemSelectionAllowed() {#isMultipleItemSelectionAllowed--}
```
public boolean isMultipleItemSelectionAllowed()
```


Gibt an, ob im Seitenfeld mehrere Elemente ausgewählt werden können. Der Standardwert ist false.

**Remarks**

Nur für Seiten‑(Filter‑)Felder.

**Returns:**
boolean
### isRepeatItemLabels() {#isRepeatItemLabels--}
```
public boolean isRepeatItemLabels()
```


Gibt an, ob die Beschriftungen des Feldes in der Zeilen‑ oder Spaltenregion wiederholt werden sollen. Der Standardwert ist false.

**Returns:**
boolean
### isValueFields() {#isValueFields--}
```
public boolean isValueFields()
```


Gibt an, ob dieses Feld Wertefelder darstellt.

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen bitte die Eigenschaft PivotField.IsValuesField. Diese Methode wird 12 Monate später, seit November 2023, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

**Returns:**
boolean
### isValuesField() {#isValuesField--}
```
public boolean isValuesField()
```


Gibt an, ob dieses Feld ein Wertefeld darstellt.

**Remarks**

Funktioniert nur, wenn im Pivot‑Tabellen‑Ansicht mindestens zwei Datenfelder vorhanden sind.

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




### setAllowDraggingToColumn(boolean value) {#setAllowDraggingToColumn-boolean-}
```
public void setAllowDraggingToColumn(boolean value)
```


Gibt an, ob das angegebene Feld in den Spaltenbereich gezogen werden kann. Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAllowDraggingToData(boolean value) {#setAllowDraggingToData-boolean-}
```
public void setAllowDraggingToData(boolean value)
```


Gibt an, ob das angegebene Feld in den Wertebereich gezogen werden kann. Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAllowDraggingToPage(boolean value) {#setAllowDraggingToPage-boolean-}
```
public void setAllowDraggingToPage(boolean value)
```


Gibt an, ob das angegebene Feld in den Seitenbereich gezogen werden kann. Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAllowDraggingToRow(boolean value) {#setAllowDraggingToRow-boolean-}
```
public void setAllowDraggingToRow(boolean value)
```


Gibt an, ob das angegebene Feld in den Zeilenbereich gezogen werden kann. Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAllowRemovingFromView(boolean value) {#setAllowRemovingFromView-boolean-}
```
public void setAllowRemovingFromView(boolean value)
```


Gibt an, ob dieses Pivotfeld aus der PivotTable‑Ansicht entfernt werden kann. Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAscendShow(boolean value) {#setAscendShow-boolean-}
```
public void setAscendShow(boolean value)
```


Gibt an, ob das angegebene PivotTable‑Feld aufsteigend automatisch angezeigt wird.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Stattdessen verwenden Sie bitte die Eigenschaft PivotField.Top10AutoShowSettings.IsTop oder die Methode PivotField.Top10AutoShow(). Diese Methode wird 12 Monate später, seit September 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAscendSort(boolean value) {#setAscendSort-boolean-}
```
public void setAscendSort(boolean value)
```


Gibt an, ob die Elemente dieses Pivot‑Felds aufsteigend automatisch sortiert werden.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Stattdessen verwenden Sie bitte die Eigenschaft PivotField.SortSetting.SortType oder die Methode PivotField.SortBy(). Diese Methode wird 12 Monate später, seit September 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAutoShow(boolean value) {#setAutoShow-boolean-}
```
public void setAutoShow(boolean value)
```


Gibt an, ob das angegebene PivotTable‑Feld automatisch angezeigt wird.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Stattdessen verwenden Sie bitte die Eigenschaft PivotField.Top10AutoShowSettings.IsAutoShow oder die Methode PivotField.Top10AutoShow(). Diese Methode wird 12 Monate später, seit September 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAutoShowCount(int value) {#setAutoShowCount-int-}
```
public void setAutoShowCount(int value)
```


Stellt die Anzahl der obersten oder untersten Elemente dar, die im angegebenen PivotTable‑Feld automatisch angezeigt werden.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft **PivotField.Top10AutoShowSettings.AutoShowCount** oder die Methode **PivotField.Top10AutoShow()**. Diese Methode wird 12 Monate nach September 2026 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setAutoShowField(int value) {#setAutoShowField-int-}
```
public void setAutoShowField(int value)
```


Stellt den Index des automatischen Anzeige‑feldes dar. -1 bedeutet das PivotField selbst. Es sollte der Index der Datenfelder sein.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft **PivotField.Top10AutoShowSettings.RankBy** oder die Methode **PivotField.Top10AutoShow()**. Diese Methode wird 12 Monate nach September 2026 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setAutoSort(boolean value) {#setAutoSort-boolean-}
```
public void setAutoSort(boolean value)
```


Gibt an, ob die Elemente dieses PivotTable‑Felds automatisch sortiert werden.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Stattdessen verwenden Sie bitte die Eigenschaft PivotField.SortSetting.SortType oder die Methode PivotField.SortBy(). Diese Methode wird 12 Monate später, seit September 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAutoSortField(int value) {#setAutoSortField-int-}
```
public void setAutoSortField(int value)
```


Stellt den Index des Feldes dar, das automatisch sortiert wird. -1 bedeutet das PivotField selbst, andere bedeuten die Position der Datenfelder.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotField.SortSetting.SortBy oder die Methode PivotField.SortBy(). Diese Methode wird 12 Monate später, seit September 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setAutoSubtotals(boolean value) {#setAutoSubtotals-boolean-}
```
public void setAutoSubtotals(boolean value)
```


Gibt an, ob das angegebene Feld automatische Zwischensummen anzeigt. Standard ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setBaseIndex(int value) {#setBaseIndex-int-}
```
public void setBaseIndex(int value)
```


Stellt den Index in den Quell‑PivotFields dar.

**Remarks**

HINWEIS: Dieser Setter dieser Eigenschaft ist jetzt veraltet. Dieser Setter dieser Eigenschaft wird 12 Monate später, seit September 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setCurrentPageItem(short value) {#setCurrentPageItem-short-}
```
public void setCurrentPageItem(short value)
```


Legt das aktuell angezeigte Seitenobjekt für dieses Pivotfeld fest (nur Seitenfeld).

**Remarks**

Verwenden Sie [PivotItem.ALL\_PAGE\_ITEMS\_INDEX](../../com.aspose.cells/pivotitem\#ALL-PAGE-ITEMS-INDEX) (0x7FFD) als Sentinelwert, um "Alle auswählen" anzuzeigen. Dies ist ein vordefinierter Marker und kein gültiger Elementindex.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | short |  |

### setCurrentPageItemText(String value) {#setCurrentPageItemText-java.lang.String-}
```
public void setCurrentPageItemText(String value)
```


Ruft den Anzeigetext des aktuellen Seitenelements für dieses PivotField ab (nur Seitenfeld).

**Remarks**

Gibt "(All)" zurück, wenn [getCurrentPageItem()](../../com.aspose.cells/pivotfield\#getCurrentPageItem--) gleich [PivotItem.ALL\_PAGE\_ITEMS\_INDEX](../../com.aspose.cells/pivotitem\#ALL-PAGE-ITEMS-INDEX) ist. Für andere Werte wird die Zeichenkettenrepräsentation des Elementindexes zurückgegeben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


Stellt den Anzeigenamen des PivotField in der PivotTable‑Ansicht dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setDragToColumn(boolean value) {#setDragToColumn-boolean-}
```
public void setDragToColumn(boolean value)
```


Gibt an, ob das angegebene Feld in den Spaltenbereich gezogen werden kann. Der Standardwert ist true.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotField.AllowDraggingToColumn. Diese Methode wird 12 Monate später, seit Juli 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setDragToData(boolean value) {#setDragToData-boolean-}
```
public void setDragToData(boolean value)
```


Gibt an, ob das angegebene Feld in den Wertebereich gezogen werden kann. Der Standardwert ist true.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotField.AllowDraggingToData. Diese Methode wird 12 Monate später, seit Juli 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setDragToHide(boolean value) {#setDragToHide-boolean-}
```
public void setDragToHide(boolean value)
```


Gibt an, ob dieses Pivotfeld aus der PivotTable‑Ansicht entfernt werden kann. Der Standardwert ist true.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotField.AllowRemovingFromView. Diese Methode wird 12 Monate später, seit Juli 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setDragToPage(boolean value) {#setDragToPage-boolean-}
```
public void setDragToPage(boolean value)
```


Gibt an, ob das angegebene Feld in den Seitenbereich gezogen werden kann. Der Standardwert ist true.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotField.AllowDraggingToPage. Diese Methode wird 12 Monate später, seit Juli 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setDragToRow(boolean value) {#setDragToRow-boolean-}
```
public void setDragToRow(boolean value)
```


Gibt an, ob das angegebene Feld in den Zeilenbereich gezogen werden kann. Der Standardwert ist true.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotField.AllowDraggingToRow. Diese Methode wird 12 Monate später, seit Juli 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setFunction(int value) {#setFunction-int-}
```
public void setFunction(int value)
```


Stellt die Funktion dar, die verwendet wird, um dieses PivotTable-Datenfeld zusammenzufassen.

Siehe [ConsolidationFunction](../../com.aspose.cells/consolidationfunction).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setIncludeNewItemsInFilter(boolean value) {#setIncludeNewItemsInFilter-boolean-}
```
public void setIncludeNewItemsInFilter(boolean value)
```


Gibt an, ob neue Elemente im Feld in manuellen Filtern einbezogen werden sollen. Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setInsertBlankRow(boolean value) {#setInsertBlankRow-boolean-}
```
public void setInsertBlankRow(boolean value)
```


Gibt an, ob nach jedem Element eine leere Zeile eingefügt werden soll. Nur für Zeilenfelder.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setInsertPageBreaksBetweenItems(boolean value) {#setInsertPageBreaksBetweenItems-boolean-}
```
public void setInsertPageBreaksBetweenItems(boolean value)
```


Gibt an, ob nach jedem Element Seitenumbrüche eingefügt werden sollen. Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setMultipleItemSelectionAllowed(boolean value) {#setMultipleItemSelectionAllowed-boolean-}
```
public void setMultipleItemSelectionAllowed(boolean value)
```


Gibt an, ob im Seitenfeld mehrere Elemente ausgewählt werden können. Der Standardwert ist false.

**Remarks**

Nur für Seiten‑(Filter‑)Felder.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Stellt den Namen von PivotField dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setNonAutoSortDefault(boolean value) {#setNonAutoSortDefault-boolean-}
```
public void setNonAutoSortDefault(boolean value)
```


Gibt an, ob ein Sortiervorgang, der auf dieses Pivot-Feld angewendet wird, ein Autosort-Vorgang oder ein einfacher Datensort ist.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die !PivotField.SortSetting.IsSimpleSort‑Eigenschaft. Diese Methode wird 12 Monate später, seit September 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setNumber(int value) {#setNumber-int-}
```
public void setNumber(int value)
```


Stellt das integrierte Anzeigeformat von Zahlen und Datumsangaben dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setNumberFormat(String value) {#setNumberFormat-java.lang.String-}
```
public void setNumberFormat(String value)
```


Stellt das benutzerdefinierte Anzeigeformat von Zahlen und Datumsangaben dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setRepeatItemLabels(boolean value) {#setRepeatItemLabels-boolean-}
```
public void setRepeatItemLabels(boolean value)
```


Gibt an, ob die Beschriftungen des Feldes in der Zeilen‑ oder Spaltenregion wiederholt werden sollen. Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowAllItems(boolean value) {#setShowAllItems-boolean-}
```
public void setShowAllItems(boolean value)
```


Gibt an, ob alle Elemente in der PivotTable‑Ansicht angezeigt werden sollen, selbst wenn sie keine Zusammenfassungsdaten enthalten. Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowCompact(boolean value) {#setShowCompact-boolean-}
```
public void setShowCompact(boolean value)
```


Gibt an, ob die Bezeichnungen des nächsten Feldes in derselben Spalte in der Pivot‑Tabellen‑Ansicht angezeigt werden sollen. Nur für Zeilenfelder.

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die PivotField.ShowInCompactForm‑Eigenschaft. Diese Methode wird 12 Monate später, seit November 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowInCompactForm(boolean value) {#setShowInCompactForm-boolean-}
```
public void setShowInCompactForm(boolean value)
```


Legt einen Wert fest, der angibt, ob dieses Zeilenfeld das kompakte Layout verwendet. Gilt nur für Zeilenfelder.

**Remarks**

Kompaktes Layout ist ein Untermodus des Gliederungs‑Layouts. Diese Einstellung wirkt nur, wenn [getShowInOutlineForm()](../../com.aspose.cells/pivotfield\#getShowInOutlineForm--) true ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowInOutlineForm(boolean value) {#setShowInOutlineForm-boolean-}
```
public void setShowInOutlineForm(boolean value)
```


Legt einen Wert fest, der angibt, ob dieses Zeilenfeld das Gliederungs‑Layout verwendet. Gilt nur für Zeilenfelder.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowSubtotalAtTop(boolean value) {#setShowSubtotalAtTop-boolean-}
```
public void setShowSubtotalAtTop(boolean value)
```


Gibt an, ob Zwischensummen oben oder unten bei den Elementen angezeigt werden sollen.

**Remarks**

Funktioniert nur für die Pivot‑Felder im Zeilenbereich, wenn ShowInOutlineForm true ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSubtotals(int value) {#setSubtotals-int-}
```
public void setSubtotals(int value)
```


Legt die Zwischensummen des Feldes fest. Nur für Zeilen‑ oder Spalten‑Pivot‑Felder.

Siehe [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setSubtotals(int subtotalType, boolean shown) {#setSubtotals-int-boolean-}
```
public void setSubtotals(int subtotalType, boolean shown)
```


Legt fest, wie das angegebene Feld zwischengesummiert wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| subtotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) |
| angezeigt | boolean | Ob das angegebene Feld diese Zwischensummen anzeigt. |

### showAllDetails() {#showAllDetails--}
```
public void showAllDetails()
```


Alle Details jedes Pivot-Elements anzeigen.

### showValuesAs(int showValuesAsType, int baseField, int baseItem) {#showValuesAs-int-int-int-}
```
public void showValuesAs(int showValuesAsType, int baseField, int baseItem)
```


Legt die Berechnung „Werte anzeigen als“ für dieses Pivotfeld fest.

**Remarks**

Nur für Datenfeld.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| showValuesAsType | int | [PivotShowValuesAsType](../../com.aspose.cells/pivotshowvaluesastype). Typ der "Show Values As"‑Berechnung. |
| baseField | int | Index des Basisfelds, das für die Berechnung verwendet wird. |
| baseItem | int | Index des Basiselements für die Berechnung. Verwenden Sie [PivotShowValuesSetting.PREVIOUS\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#PREVIOUS-PIVOT-ITEM) (-1) für das vorherige Element, [PivotShowValuesSetting.NEXT\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#NEXT-PIVOT-ITEM) (-2) für das nachfolgende Element; non\\u9225\\u6182egative Werte bezeichnen den ordinalen Index eines bestimmten Pivot-Elements. |

### showValuesAs(int displayFormat, int baseField, int baseItemPositionType, int baseItem) {#showValuesAs-int-int-int-int-}
```
public void showValuesAs(int displayFormat, int baseField, int baseItemPositionType, int baseItem)
```


Zeigt Werte des Datenfelds in einem anderen Anzeigeformat an, wenn die Berechnung ShowDataAs verwendet wird.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotField.ShowValuesAs(PivotShowValuesAsType,int,int). Diese Methode wird 12 Monate später, seit November 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| displayFormat | int | [PivotFieldDataDisplayFormat](../../com.aspose.cells/pivotfielddatadisplayformat). Der Datendarstellungsformattyp. |
| baseField | int | Der Index des Feldes, auf dem die ShowDataAs‑Berechnung basiert. |
| baseItemPositionType | int | [PivotItemPositionType](../../com.aspose.cells/pivotitempositiontype). Der Positionstyp des Basiselements. |
| baseItem | int | Der Index des Basiselements, auf dem die ShowDataAs‑Berechnung basiert. Funktioniert nur, wenn baseItemPositionType benutzerdefiniert ist. |

### showValuesAs(int showValuesAsType, String baseField, String baseItem) {#showValuesAs-int-java.lang.String-java.lang.String-}
```
public void showValuesAs(int showValuesAsType, String baseField, String baseItem)
```


Konfiguriert die Berechnung „Werte anzeigen als“ für dieses Datenfeld.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| showValuesAsType | int | [PivotShowValuesAsType](../../com.aspose.cells/pivotshowvaluesastype). Der Berechnungstyp für „Show Values As“. |
| baseField | java.lang.String | Der Name des im Berechnungsvorgang verwendeten Basisfeldes. |
| baseItem | java.lang.String | Beschriftung eines regulären Pivot-Elements. Akzeptiert außerdem reservierte Schlüsselwörter: `(previous)` für das vorherige Element, `(next)` für das nächste Element. Übergeben Sie `null`, wenn der ausgewählte Berechnungstyp kein Basiselement benötigt. |

### sortBy(int sortType) {#sortBy-int-}
```
public void sortBy(int sortType)
```


Sortiert dieses Pivotfeld.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sortType | int | [SortOrder](../../com.aspose.cells/sortorder). Der Sortierungstyp dieses Feldes. |

### sortBy(int sortType, int fieldSortedBy) {#sortBy-int-int-}
```
public void sortBy(int sortType, int fieldSortedBy)
```


Sortiert dieses Pivotfeld.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotField.SortBy(SortOrder, int,string) oder die Eigenschaft PivotField.IsAutoSort. Diese Methode wird 12 Monate später, seit September 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sortType | int | [SortOrder](../../com.aspose.cells/sortorder). Der Sortierungstyp dieses Feldes. |
| fieldSortedBy | int | Der Index des Pivot-Feldes, nach dem sortiert wird. -1 bedeutet Sortierung nach Datenbeschriftungen dieses Feldes, andere Werte bedeuten den Index des Datenfeldes, nach dem sortiert wird. |

### sortBy(int sortType, int fieldSortedBy, int dataType, String cellName) {#sortBy-int-int-int-java.lang.String-}
```
public void sortBy(int sortType, int fieldSortedBy, int dataType, String cellName)
```


Sortiert dieses Pivotfeld.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotField.SortBy(SortOrder, int,string). Diese Methode wird 12 Monate später, seit September 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sortType | int | [SortOrder](../../com.aspose.cells/sortorder). Der Sortierungstyp dieses Feldes. |
| fieldSortedBy | int | Der Index des Pivot-Feldes, nach dem sortiert wird. -1 bedeutet Sortierung nach Datenbeschriftungen dieses Feldes, andere Werte bedeuten den Index des Datenfeldes, nach dem sortiert wird. |
| dataType | int | [PivotLineType](../../com.aspose.cells/pivotlinetype). Der Typ der Daten, nach denen sortiert wird. |
| cellName | java.lang.String | Nach Werten in Zeile oder Spalte sortieren |

### sortBy(int sortType, int fieldSortedBy, String cellName) {#sortBy-int-int-java.lang.String-}
```
public void sortBy(int sortType, int fieldSortedBy, String cellName)
```


Sortiert dieses Pivotfeld.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sortType | int | [SortOrder](../../com.aspose.cells/sortorder). Der Sortierungstyp dieses Feldes. |
| fieldSortedBy | int | Der Index des Pivot-Feldes, nach dem sortiert wird. -1 bedeutet Sortierung nach Datenbeschriftungen dieses Feldes, andere Werte bedeuten den Index des Datenfeldes, nach dem sortiert wird. |
| cellName | java.lang.String | Nach Werten in Zeile oder Spalte sortieren. Wenn Null, nach Gesamtsumme des Feldes gruppieren, sonst nach Werten in der ausgewählten Spalte oder Zeile gruppieren. |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### top10AutoShow(boolean isAutoShow, boolean isTop, int count, int rankBy) {#top10AutoShow-boolean-boolean-int-int-}
```
public void top10AutoShow(boolean isAutoShow, boolean isTop, int count, int rankBy)
```


Konfiguriert die Top10‑AutoShow‑Einstellungen für dieses Pivotfeld.

**Remarks**

Diese Methode konfiguriert das .XLS‑Binärformat: AutoShow (Top10) ist die native und einzige unterstützte Option. XLSX (OpenXML): Das zugrunde liegende Dateiformat unterstützt Top10 AutoShow, aber die Benutzeroberfläche von Excel 2007 und neuer stellt dies nur über den Top10‑Filter bereit. Wenn XLS‑Kompatibilität nicht erforderlich ist, wird empfohlen, stattdessen den Top10‑Filter zu verwenden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isAutoShow | boolean | true, um AutoShow zu aktivieren; false, um es zu deaktivieren. |
| isTop | boolean | Wenn true, werden die obersten Elemente angezeigt; false zeigt die untersten Elemente. |
| Anzahl | int | Anzahl der anzuzeigenden obersten/untersten Elemente. |
| rankBy | int | Index des Datenfeldes, das für das Ranking verwendet wird. Verwenden Sie -1, um nach den eigenen Werten des Pivot-Elements zu ranken. |

### ungroup() {#ungroup--}
```
public void ungroup()
```


Gruppierung des Pivotfelds aufheben.

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

