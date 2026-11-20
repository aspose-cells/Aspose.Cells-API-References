---
title: "Slicer"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Zusammenfassende Beschreibung der Slicer-Ansicht"
type: docs
url: /de/java/com.aspose.cells/slicer/
---

**Inheritance:**
java.lang.Object
```
public class Slicer
```

Zusammenfassende Beschreibung der Slicer-Ansicht

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
 
         pivot.calculateData();
 
         SlicerCollection slicers = sheet.getSlicers();
         int slicerIndex = slicers.add(pivot, "E12", "fruit");
         Slicer slicer = slicers.get(slicerIndex);
         slicer.setStyleType(SlicerStyleType.SLICER_STYLE_LIGHT_2);
 
         slicer.unselectItems(new String[] { "grape" });
         //do your business
         book.save("out.xlsx");
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [addPivotConnection(PivotTable pivot)](#addPivotConnection-com.aspose.cells.PivotTable-) | Fügt eine PivotTable‑Verbindung hinzu. |
| [clearFilter()](#clearFilter--) | Filter entfernen |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlternativeText()](#getAlternativeText--) | Liefert oder setzt die beschreibende (alternative) Textzeichenkette des Slicer‑Objekts. |
| [getCaption()](#getCaption--) | Gibt die Beschriftung des angegebenen Slicers zurück oder legt sie fest. |
| [getCaptionVisible()](#getCaptionVisible--) | Gibt zurück oder legt fest, ob die Kopfzeile, die die Slicer-Beschriftung anzeigt, sichtbar ist. |
| [getClass()](#getClass--) |  |
| [getColumnWidth()](#getColumnWidth--) | Gibt die Breite jeder Spalte im Slicer in Punkten zurück oder legt sie fest. |
| [getColumnWidthPixel()](#getColumnWidthPixel--) | Ermittelt die Breite von\u807deach column in\u807dthe slicer, in Einheit von\u807dpixels.\u807d |
| [getFirstItemIndex()](#getFirstItemIndex--) | Gibt den nullbasierten Index des ersten Slicer-Elements an. |
| [getHeight()](#getHeight--) | Gibt die Höhe des angegebenen Slicers in Punkten zurück oder legt sie fest. |
| [getHeightPixel()](#getHeightPixel--) | Gibt die Höhe des angegebenen Slicers in Pixeln zurück oder legt sie fest. |
| [getLeftPixel()](#getLeftPixel--) | Gibt den horizontalen Versatz der Slicer-Form von ihrer linken Spalte in Pixeln zurück oder legt ihn fest. |
| [getLockedAspectRatio()](#getLockedAspectRatio--) | Gibt an, ob das Seitenverhältnis gesperrt ist. |
| [getLockedPosition()](#getLockedPosition--) | Gibt an, ob der angegebene Slicer über die Benutzeroberfläche verschoben oder in der Größe geändert werden kann. |
| [getName()](#getName--) | Gibt den Namen des angegebenen Slicers zurück oder legt ihn fest |
| [getNumberOfColumns()](#getNumberOfColumns--) | Gibt die Anzahl der Spalten im Slicer zurück oder legt sie fest. |
| [getParent()](#getParent--) | Gibt das [getWorksheet()](../../com.aspose.cells/slicer\#getWorksheet--) Objekt zurück, das diesen Slicer enthält. |
| [getPlacement()](#getPlacement--) | Stellt die Art dar, wie das Zeichenobjekt an den darunterliegenden Zellen befestigt ist. |
| [getRowHeight()](#getRowHeight--) | Gibt die Höhe jeder Zeile im angegebenen Slicer in Punkten zurück oder legt sie fest. |
| [getRowHeightPixel()](#getRowHeightPixel--) | Gibt die Höhe jeder Zeile im angegebenen Slicer in Pixeln zurück oder legt sie fest. |
| [getShape()](#getShape--) | Gibt das Shape-Objekt zurück, das dem angegebenen Slicer zugeordnet ist. |
| [getShowAllItems()](#getShowAllItems--) | Gibt an, ob alle Elemente angezeigt werden sollen, selbst wenn keine Daten vorhanden sind oder sie gelöscht wurden. |
| [getShowCaption()](#getShowCaption--) | Gibt an, ob die Kopfzeile des Slicers sichtbar ist. |
| [getShowMissing()](#getShowMissing--) | Gibt an, ob Elemente, die aus der Datenquelle gelöscht wurden, angezeigt werden sollen. |
| [getShowTypeOfItemsWithNoData()](#getShowTypeOfItemsWithNoData--) | Gibt an, ob Elemente, die aus der Datenquelle gelöscht wurden, angezeigt werden sollen. |
| [getSlicerCache()](#getSlicerCache--) | Gibt das SlicerCache-Objekt zurück, das dem Slicer zugeordnet ist. |
| [getSortOrderType()](#getSortOrderType--) | Gibt den Typ der Sortierungselemente an. |
| [getStyleType()](#getStyleType--) | Gibt den Typ des integrierten Slicer-Stils an. |
| [getTitle()](#getTitle--) | Gibt den Titel des aktuellen Slicer-Objekts an. |
| [getTopPixel()](#getTopPixel--) | Gibt den vertikalen Versatz der Slicer-Form von ihrer oberen Zeile in Pixeln zurück oder legt ihn fest. |
| [getWidth()](#getWidth--) | Gibt die Breite des angegebenen Slicers in Punkten zurück oder legt sie fest. |
| [getWidthPixel()](#getWidthPixel--) | Gibt die Breite des angegebenen Slicers zurück oder legt sie fest, in Pixeln. |
| [getWorksheet()](#getWorksheet--) | Gibt das [getWorksheet()](../../com.aspose.cells/slicer\#getWorksheet--) Objekt zurück, das diesen Slicer enthält. |
| [hashCode()](#hashCode--) |  |
| [isLocked()](#isLocked--) | Gibt an, ob die Slicer-Form gesperrt ist. |
| [isPrintable()](#isPrintable--) | Gibt an, ob das Slicer-Objekt druckbar ist. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refresh()](#refresh--) | Aktualisiert die Elemente des Slicers aus den zugehörigen Pivot-Tabellen. |
| [removePivotConnection(PivotTable pivot)](#removePivotConnection-com.aspose.cells.PivotTable-) | Entfernt die PivotTable-Verbindung. |
| [selectItems(String[] labels, boolean append)](#selectItems-java.lang.String---boolean-) | **Hinweise** |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | Liefert oder setzt die beschreibende (alternative) Textzeichenkette des Slicer‑Objekts. |
| [setCaption(String value)](#setCaption-java.lang.String-) | Gibt die Beschriftung des angegebenen Slicers zurück oder legt sie fest. |
| [setCaptionVisible(boolean value)](#setCaptionVisible-boolean-) | Gibt zurück oder legt fest, ob die Kopfzeile, die die Slicer-Beschriftung anzeigt, sichtbar ist. |
| [setColumnWidth(double value)](#setColumnWidth-double-) | Gibt die Breite jeder Spalte im Slicer in Punkten zurück oder legt sie fest. |
| [setColumnWidthPixel(int value)](#setColumnWidthPixel-int-) | Setzt die Breite jeder Spalte im Slicer, in Einheit von Pixeln. |
| [setFirstItemIndex(int value)](#setFirstItemIndex-int-) | Gibt den nullbasierten Index des ersten Slicer-Elements an. |
| [setHeight(double value)](#setHeight-double-) | Gibt die Höhe des angegebenen Slicers in Punkten zurück oder legt sie fest. |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Gibt die Höhe des angegebenen Slicers in Pixeln zurück oder legt sie fest. |
| [setLeftPixel(int value)](#setLeftPixel-int-) | Gibt den horizontalen Versatz der Slicer-Form von ihrer linken Spalte in Pixeln zurück oder legt ihn fest. |
| [setLocked(boolean value)](#setLocked-boolean-) | Gibt an, ob die Slicer-Form gesperrt ist. |
| [setLockedAspectRatio(boolean value)](#setLockedAspectRatio-boolean-) | Gibt an, ob das Seitenverhältnis gesperrt ist. |
| [setLockedPosition(boolean value)](#setLockedPosition-boolean-) | Gibt an, ob der angegebene Slicer über die Benutzeroberfläche verschoben oder in der Größe geändert werden kann. |
| [setName(String value)](#setName-java.lang.String-) | Gibt den Namen des angegebenen Slicers zurück oder legt ihn fest |
| [setNumberOfColumns(int value)](#setNumberOfColumns-int-) | Gibt die Anzahl der Spalten im Slicer zurück oder legt sie fest. |
| [setPlacement(int value)](#setPlacement-int-) | Stellt die Art dar, wie das Zeichenobjekt an den darunterliegenden Zellen befestigt ist. |
| [setPrintable(boolean value)](#setPrintable-boolean-) | Gibt an, ob das Slicer-Objekt druckbar ist. |
| [setRowHeight(double value)](#setRowHeight-double-) | Gibt die Höhe jeder Zeile im angegebenen Slicer in Punkten zurück oder legt sie fest. |
| [setRowHeightPixel(int value)](#setRowHeightPixel-int-) | Gibt die Höhe jeder Zeile im angegebenen Slicer in Pixeln zurück oder legt sie fest. |
| [setShowAllItems(boolean value)](#setShowAllItems-boolean-) | Gibt an, ob alle Elemente angezeigt werden sollen, selbst wenn keine Daten vorhanden sind oder sie gelöscht wurden. |
| [setShowCaption(boolean value)](#setShowCaption-boolean-) | Gibt an, ob die Kopfzeile des Slicers sichtbar ist. |
| [setShowMissing(boolean value)](#setShowMissing-boolean-) | Gibt an, ob Elemente, die aus der Datenquelle gelöscht wurden, angezeigt werden sollen. |
| [setShowTypeOfItemsWithNoData(int value)](#setShowTypeOfItemsWithNoData-int-) | Gibt an, ob Elemente, die aus der Datenquelle gelöscht wurden, angezeigt werden sollen. |
| [setSortOrderType(int value)](#setSortOrderType-int-) | Gibt den Typ der Sortierungselemente an. |
| [setStyleType(int value)](#setStyleType-int-) | Gibt den Typ des integrierten Slicer-Stils an. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Gibt den Titel des aktuellen Slicer-Objekts an. |
| [setTopPixel(int value)](#setTopPixel-int-) | Gibt den vertikalen Versatz der Slicer-Form von ihrer oberen Zeile in Pixeln zurück oder legt ihn fest. |
| [setWidth(double value)](#setWidth-double-) | Gibt die Breite des angegebenen Slicers in Punkten zurück oder legt sie fest. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | Gibt die Breite des angegebenen Slicers zurück oder legt sie fest, in Pixeln. |
| [toString()](#toString--) |  |
| [unselectItems(String[] labels)](#unselectItems-java.lang.String---) | Entfernt ausgewählte Filterbeschriftungen. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addPivotConnection(PivotTable pivot) {#addPivotConnection-com.aspose.cells.PivotTable-}
```
public void addPivotConnection(PivotTable pivot)
```


Fügt eine PivotTable‑Verbindung hinzu.

**Example**

```
         slicer.addPivotConnection(pivot);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | Das PivotTable-Objekt |

### clearFilter() {#clearFilter--}
```
public void clearFilter()
```


Filter entfernen

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
### getAlternativeText() {#getAlternativeText--}
```
public String getAlternativeText()
```


Liefert oder setzt die beschreibende (alternative) Textzeichenkette des Slicer‑Objekts.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die [Shape.getAlternativeText()](../../com.aspose.cells/shape\#getAlternativeText--) Eigenschaft. Diese Eigenschaft wird 12 Monate später, seit Januar 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
java.lang.String
### getCaption() {#getCaption--}
```
public String getCaption()
```


Gibt die Beschriftung des angegebenen Slicers zurück oder legt sie fest.

**Example**

```
         slicer.setCaption("slicer caption");
```

**Returns:**
java.lang.String
### getCaptionVisible() {#getCaptionVisible--}
```
public boolean getCaptionVisible()
```


Gibt zurück oder legt fest, ob die Kopfzeile, die die Slicer‑Beschriftung anzeigt, sichtbar ist. Der Standardwert ist true.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die [getShowCaption()](../../com.aspose.cells/slicer\#getShowCaption--) Eigenschaft. Diese Eigenschaft wird 12 Monate später, seit Januar 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Example**

```
         slicer.setCaption("slicer caption");
```

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnWidth() {#getColumnWidth--}
```
public double getColumnWidth()
```


Gibt die Breite jeder Spalte im Slicer in Punkten zurück oder legt sie fest.

**Example**

```
         slicer.setColumnWidth(80);
```

**Returns:**
double
### getColumnWidthPixel() {#getColumnWidthPixel--}
```
public int getColumnWidthPixel()
```


Ermittelt die Breite von\u807deach column in\u807dthe slicer, in Einheit von\u807dpixels.\u807d

**Example**

```
         slicer.setColumnWidthPixel(120);
```

**Returns:**
int
### getFirstItemIndex() {#getFirstItemIndex--}
```
public int getFirstItemIndex()
```


Gibt den nullbasierten Index des ersten Slicer-Elements an.

**Returns:**
int
### getHeight() {#getHeight--}
```
public double getHeight()
```


Gibt die Höhe des angegebenen Slicers in Punkten zurück oder legt sie fest.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Shape.HeightPt‑Eigenschaft. Diese Eigenschaft wird 12 Monate später, seit Mai 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
double
### getHeightPixel() {#getHeightPixel--}
```
public int getHeightPixel()
```


Gibt die Höhe des angegebenen Slicers in Pixeln zurück oder legt sie fest.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft Shape.Height. Diese Eigenschaft wird 12 Monate nach Mai 2025 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getLeftPixel() {#getLeftPixel--}
```
public int getLeftPixel()
```


Gibt den horizontalen Versatz der Slicer-Form von ihrer linken Spalte in Pixeln zurück oder legt ihn fest.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft Shape.Left. Diese Eigenschaft wird 12 Monate nach Mai 2025 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getLockedAspectRatio() {#getLockedAspectRatio--}
```
public boolean getLockedAspectRatio()
```


Gibt an, ob das Seitenverhältnis gesperrt ist.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die [Shape.isAspectRatioLocked()](../../com.aspose.cells/shape\#isAspectRatioLocked--) Methode. Diese Eigenschaft wird 12 Monate später, seit Januar 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
boolean
### getLockedPosition() {#getLockedPosition--}
```
public boolean getLockedPosition()
```


Gibt an, ob der angegebene Slicer über die Benutzeroberfläche verschoben oder in der Größe geändert werden kann.

**Example**

```
         slicer.setLockedPosition(false);
```

**Returns:**
boolean
### getName() {#getName--}
```
public String getName()
```


Gibt den Namen des angegebenen Slicers zurück oder legt ihn fest

**Example**

```
         slicer.setName("slicer name");
```

**Returns:**
java.lang.String
### getNumberOfColumns() {#getNumberOfColumns--}
```
public int getNumberOfColumns()
```


Gibt die Anzahl der Spalten im Slicer zurück oder legt sie fest. Der Standardwert ist 1.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getParent() {#getParent--}
```
public Worksheet getParent()
```


Gibt das [getWorksheet()](../../com.aspose.cells/slicer\#getWorksheet--) Objekt zurück, das diesen Slicer enthält. Nur lesbar.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die [getWorksheet()](../../com.aspose.cells/slicer\#getWorksheet--) Eigenschaft. Diese Eigenschaft wird 12 Monate später, seit Januar 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Example**

```
         SlicerCache slicerCache = slicer.getSlicerCache();
```

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### getPlacement() {#getPlacement--}
```
public int getPlacement()
```


Stellt dar, wie das Zeichenobjekt an den darunter liegenden Zellen befestigt ist. Die property steuert die Platzierung eines Objekts auf einem Arbeitsblatt.

Siehe [PlacementType](../../com.aspose.cells/placementtype).

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die [Shape.getPlacement()](../../com.aspose.cells/shape\#getPlacement--) Eigenschaft. Diese Eigenschaft wird 12 Monate später, seit Januar 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
int
### getRowHeight() {#getRowHeight--}
```
public double getRowHeight()
```


Gibt die Höhe jeder Zeile im angegebenen Slicer in Punkten zurück oder legt sie fest.

**Example**

```
         slicer.setRowHeight(20);
```

**Returns:**
double
### getRowHeightPixel() {#getRowHeightPixel--}
```
public int getRowHeightPixel()
```


Gibt die Höhe jeder Zeile im angegebenen Slicer in Pixeln zurück oder legt sie fest.

**Example**

```
         slicer.setRowHeightPixel(30);
```

**Returns:**
int
### getShape() {#getShape--}
```
public SlicerShape getShape()
```


Gibt das Shape‑Objekt zurück, das dem angegebenen Slicer zugeordnet ist. Nur lesbar.

**Returns:**
[SlicerShape](../../com.aspose.cells/slicershape)
### getShowAllItems() {#getShowAllItems--}
```
public boolean getShowAllItems()
```


Gibt an, ob alle Elemente angezeigt werden sollen, selbst wenn keine Daten vorhanden sind oder sie gelöscht wurden. Standardwert ist true;

**Returns:**
boolean
### getShowCaption() {#getShowCaption--}
```
public boolean getShowCaption()
```


Gibt an, ob die Kopfzeile des Slicers sichtbar ist. Der Standardwert ist true.

**Example**

```
         slicer.setShowCaption(false);
```

**Returns:**
boolean
### getShowMissing() {#getShowMissing--}
```
public boolean getShowMissing()
```


Gibt an, ob Elemente, die aus der Datenquelle gelöscht wurden, angezeigt werden sollen.

**Remarks**

Funktioniert nur, wenn [getShowAllItems()](../../com.aspose.cells/slicer\#getShowAllItems--) true ist.

**Returns:**
boolean
### getShowTypeOfItemsWithNoData() {#getShowTypeOfItemsWithNoData--}
```
public int getShowTypeOfItemsWithNoData()
```


Gibt an, ob Elemente, die aus der Datenquelle gelöscht wurden, angezeigt werden sollen.

Siehe [ItemsWithNoDataShowMode](../../com.aspose.cells/itemswithnodatashowmode).

**Remarks**

Funktioniert nur, wenn [getShowAllItems()](../../com.aspose.cells/slicer\#getShowAllItems--) true ist.

**Returns:**
int
### getSlicerCache() {#getSlicerCache--}
```
public SlicerCache getSlicerCache()
```


Gibt das SlicerCache‑Objekt zurück, das dem Slicer zugeordnet ist. Nur lesbar.

**Example**

```
         SlicerCache slicerCache = slicer.getSlicerCache();
```

**Returns:**
[SlicerCache](../../com.aspose.cells/slicercache)
### getSortOrderType() {#getSortOrderType--}
```
public int getSortOrderType()
```


Gibt den Typ der Sortierungselemente an.

Siehe [SortOrder](../../com.aspose.cells/sortorder).

**Returns:**
int
### getStyleType() {#getStyleType--}
```
public int getStyleType()
```


Gibt den Typ des integrierten Slicer‑Stils an. Der Standardtyp ist SlicerStyleLight1.

Siehe [SlicerStyleType](../../com.aspose.cells/slicerstyletype).

**Example**

```
         slicer.setStyleType(SlicerStyleType.SLICER_STYLE_LIGHT_2);
```

**Returns:**
int
### getTitle() {#getTitle--}
```
public String getTitle()
```


Gibt den Titel des aktuellen Slicer-Objekts an.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die [Shape.getTitle()](../../com.aspose.cells/shape\\#getTitle--) Eigenschaft. Diese Eigenschaft wird 12 Monate später, seit Januar 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
java.lang.String
### getTopPixel() {#getTopPixel--}
```
public int getTopPixel()
```


Gibt den vertikalen Versatz der Slicer-Form von ihrer oberen Zeile in Pixeln zurück oder legt ihn fest.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft Shape.Top. Diese Eigenschaft wird 12 Monate nach Mai 2025 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getWidth() {#getWidth--}
```
public double getWidth()
```


Gibt die Breite des angegebenen Slicers in Punkten zurück oder legt sie fest.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Shape.WidthPt Eigenschaft. Diese Eigenschaft wird 12 Monate später, seit Mai 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
double
### getWidthPixel() {#getWidthPixel--}
```
public int getWidthPixel()
```


Gibt die Breite des angegebenen Slicers zurück oder legt sie fest, in Pixeln.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft Shape.Width. Diese Eigenschaft wird 12 Monate nach Mai 2025 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Gibt das [getWorksheet()](../../com.aspose.cells/slicer\#getWorksheet--) Objekt zurück, das diesen Slicer enthält. Nur lesbar.

**Example**

```
         Worksheet currSheet = slicer.getParent();
```

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


Gibt an, ob die Slicer-Form gesperrt ist.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die [Shape.isLocked()](../../com.aspose.cells/shape\\#isLocked--) Eigenschaft. Diese Eigenschaft wird 12 Monate später, seit Januar 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
boolean
### isPrintable() {#isPrintable--}
```
public boolean isPrintable()
```


Gibt an, ob das Slicer-Objekt druckbar ist.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die [Shape.isPrintable()](../../com.aspose.cells/shape\\#isPrintable--) Eigenschaft. Diese Eigenschaft wird 12 Monate später, seit Januar 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Example**

```
         slicer.removePivotConnection(pivot);
```

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




### refresh() {#refresh--}
```
public void refresh()
```


Aktualisiert die Elemente des Slicers aus den zugehörigen Pivot-Tabellen.

**Example**

```
         slicer.refresh();
```

### removePivotConnection(PivotTable pivot) {#removePivotConnection-com.aspose.cells.PivotTable-}
```
public void removePivotConnection(PivotTable pivot)
```


Entfernt die PivotTable-Verbindung.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | Das PivotTable-Objekt |

### selectItems(String[] labels, boolean append) {#selectItems-java.lang.String---boolean-}
```
public void selectItems(String[] labels, boolean append)
```


**Remarks**

Wenn Sie alle Elemente auswählen möchten, verwenden Sie bitte die [clearFilter()](../../com.aspose.cells/slicer\\#clearFilter--) Methode.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Beschriftungen | java.lang.String[] | Ausgewählte Beschriftungen. |
| anhängen | boolean | False bedeutet, dass nur diese Beschriftungen ausgewählt und andere abgewählt werden. True bedeutet, dass bereits ausgewählte Elemente beibehalten und diese Beschriftungen ausgewählt werden. |

### setAlternativeText(String value) {#setAlternativeText-java.lang.String-}
```
public void setAlternativeText(String value)
```


Liefert oder setzt die beschreibende (alternative) Textzeichenkette des Slicer‑Objekts.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die [Shape.getAlternativeText()](../../com.aspose.cells/shape\#getAlternativeText--) Eigenschaft. Diese Eigenschaft wird 12 Monate später, seit Januar 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setCaption(String value) {#setCaption-java.lang.String-}
```
public void setCaption(String value)
```


Gibt die Beschriftung des angegebenen Slicers zurück oder legt sie fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setCaptionVisible(boolean value) {#setCaptionVisible-boolean-}
```
public void setCaptionVisible(boolean value)
```


Gibt zurück oder legt fest, ob die Kopfzeile, die die Slicer‑Beschriftung anzeigt, sichtbar ist. Der Standardwert ist true.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die [getShowCaption()](../../com.aspose.cells/slicer\#getShowCaption--) Eigenschaft. Diese Eigenschaft wird 12 Monate später, seit Januar 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setColumnWidth(double value) {#setColumnWidth-double-}
```
public void setColumnWidth(double value)
```


Gibt die Breite jeder Spalte im Slicer in Punkten zurück oder legt sie fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setColumnWidthPixel(int value) {#setColumnWidthPixel-int-}
```
public void setColumnWidthPixel(int value)
```


Setzt die Breite jeder Spalte im Slicer, in Einheit von Pixeln.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setFirstItemIndex(int value) {#setFirstItemIndex-int-}
```
public void setFirstItemIndex(int value)
```


Gibt den nullbasierten Index des ersten Slicer-Elements an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


Gibt die Höhe des angegebenen Slicers in Punkten zurück oder legt sie fest.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Shape.HeightPt‑Eigenschaft. Diese Eigenschaft wird 12 Monate später, seit Mai 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setHeightPixel(int value) {#setHeightPixel-int-}
```
public void setHeightPixel(int value)
```


Gibt die Höhe des angegebenen Slicers in Pixeln zurück oder legt sie fest.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft Shape.Height. Diese Eigenschaft wird 12 Monate nach Mai 2025 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setLeftPixel(int value) {#setLeftPixel-int-}
```
public void setLeftPixel(int value)
```


Gibt den horizontalen Versatz der Slicer-Form von ihrer linken Spalte in Pixeln zurück oder legt ihn fest.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft Shape.Left. Diese Eigenschaft wird 12 Monate nach Mai 2025 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Gibt an, ob die Slicer-Form gesperrt ist.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die [Shape.isLocked()](../../com.aspose.cells/shape\\#isLocked--) Eigenschaft. Diese Eigenschaft wird 12 Monate später, seit Januar 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setLockedAspectRatio(boolean value) {#setLockedAspectRatio-boolean-}
```
public void setLockedAspectRatio(boolean value)
```


Gibt an, ob das Seitenverhältnis gesperrt ist.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die [Shape.isAspectRatioLocked()](../../com.aspose.cells/shape\#isAspectRatioLocked--) Methode. Diese Eigenschaft wird 12 Monate später, seit Januar 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setLockedPosition(boolean value) {#setLockedPosition-boolean-}
```
public void setLockedPosition(boolean value)
```


Gibt an, ob der angegebene Slicer über die Benutzeroberfläche verschoben oder in der Größe geändert werden kann.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Gibt den Namen des angegebenen Slicers zurück oder legt ihn fest

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setNumberOfColumns(int value) {#setNumberOfColumns-int-}
```
public void setNumberOfColumns(int value)
```


Gibt die Anzahl der Spalten im Slicer zurück oder legt sie fest. Der Standardwert ist 1.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setPlacement(int value) {#setPlacement-int-}
```
public void setPlacement(int value)
```


Stellt dar, wie das Zeichenobjekt an den darunter liegenden Zellen befestigt ist. Die property steuert die Platzierung eines Objekts auf einem Arbeitsblatt.

Siehe [PlacementType](../../com.aspose.cells/placementtype).

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die [Shape.getPlacement()](../../com.aspose.cells/shape\#getPlacement--) Eigenschaft. Diese Eigenschaft wird 12 Monate später, seit Januar 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setPrintable(boolean value) {#setPrintable-boolean-}
```
public void setPrintable(boolean value)
```


Gibt an, ob das Slicer-Objekt druckbar ist.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die [Shape.isPrintable()](../../com.aspose.cells/shape\\#isPrintable--) Eigenschaft. Diese Eigenschaft wird 12 Monate später, seit Januar 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setRowHeight(double value) {#setRowHeight-double-}
```
public void setRowHeight(double value)
```


Gibt die Höhe jeder Zeile im angegebenen Slicer in Punkten zurück oder legt sie fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setRowHeightPixel(int value) {#setRowHeightPixel-int-}
```
public void setRowHeightPixel(int value)
```


Gibt die Höhe jeder Zeile im angegebenen Slicer in Pixeln zurück oder legt sie fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setShowAllItems(boolean value) {#setShowAllItems-boolean-}
```
public void setShowAllItems(boolean value)
```


Gibt an, ob alle Elemente angezeigt werden sollen, selbst wenn keine Daten vorhanden sind oder sie gelöscht wurden. Standardwert ist true;

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowCaption(boolean value) {#setShowCaption-boolean-}
```
public void setShowCaption(boolean value)
```


Gibt an, ob die Kopfzeile des Slicers sichtbar ist. Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowMissing(boolean value) {#setShowMissing-boolean-}
```
public void setShowMissing(boolean value)
```


Gibt an, ob Elemente, die aus der Datenquelle gelöscht wurden, angezeigt werden sollen.

**Remarks**

Funktioniert nur, wenn [getShowAllItems()](../../com.aspose.cells/slicer\#getShowAllItems--) true ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowTypeOfItemsWithNoData(int value) {#setShowTypeOfItemsWithNoData-int-}
```
public void setShowTypeOfItemsWithNoData(int value)
```


Gibt an, ob Elemente, die aus der Datenquelle gelöscht wurden, angezeigt werden sollen.

Siehe [ItemsWithNoDataShowMode](../../com.aspose.cells/itemswithnodatashowmode).

**Remarks**

Funktioniert nur, wenn [getShowAllItems()](../../com.aspose.cells/slicer\#getShowAllItems--) true ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setSortOrderType(int value) {#setSortOrderType-int-}
```
public void setSortOrderType(int value)
```


Gibt den Typ der Sortierungselemente an.

Siehe [SortOrder](../../com.aspose.cells/sortorder).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setStyleType(int value) {#setStyleType-int-}
```
public void setStyleType(int value)
```


Gibt den Typ des integrierten Slicer‑Stils an. Der Standardtyp ist SlicerStyleLight1.

Siehe [SlicerStyleType](../../com.aspose.cells/slicerstyletype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public void setTitle(String value)
```


Gibt den Titel des aktuellen Slicer-Objekts an.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die [Shape.getTitle()](../../com.aspose.cells/shape\\#getTitle--) Eigenschaft. Diese Eigenschaft wird 12 Monate später, seit Januar 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setTopPixel(int value) {#setTopPixel-int-}
```
public void setTopPixel(int value)
```


Gibt den vertikalen Versatz der Slicer-Form von ihrer oberen Zeile in Pixeln zurück oder legt ihn fest.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft Shape.Top. Diese Eigenschaft wird 12 Monate nach Mai 2025 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setWidth(double value) {#setWidth-double-}
```
public void setWidth(double value)
```


Gibt die Breite des angegebenen Slicers in Punkten zurück oder legt sie fest.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Shape.WidthPt Eigenschaft. Diese Eigenschaft wird 12 Monate später, seit Mai 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setWidthPixel(int value) {#setWidthPixel-int-}
```
public void setWidthPixel(int value)
```


Gibt die Breite des angegebenen Slicers zurück oder legt sie fest, in Pixeln.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft Shape.Width. Diese Eigenschaft wird 12 Monate nach Mai 2025 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

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
### unselectItems(String[] labels) {#unselectItems-java.lang.String---}
```
public void unselectItems(String[] labels)
```


Entfernt ausgewählte Filterbeschriftungen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Beschriftungen | java.lang.String[] | Die Beschriftungen. |

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

