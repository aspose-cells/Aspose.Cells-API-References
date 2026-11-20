---
title: "Timeline"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Zusammenfassende Beschreibung der Timeline‑Ansicht. Aufgrund von MS Excel 2003 wird Timeline nicht unterstützt."
type: docs
url: /de/java/com.aspose.cells/timeline/
---

**Inheritance:**
java.lang.Object
```
public class Timeline
```

Zusammenfassende Beschreibung der Timeline-Ansicht. Aufgrund von MS Excel unterstützt Excel 2003 keine Timeline.

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
 
         //Create date style
         Style dateStyle = new CellsFactory().createStyle();
         dateStyle.setCustom("m/d/yyyy");
         cells.get(0, 1).setValue("date");
         cells.get(1, 1).setValue(new DateTime(2021, 2, 5));
         cells.get(2, 1).setValue(new DateTime(2022, 3, 8));
         cells.get(3, 1).setValue(new DateTime(2023, 4, 10));
         cells.get(4, 1).setValue(new DateTime(2024, 5, 16));
         //Set date style
         cells.get(1, 1).setStyle(dateStyle);
         cells.get(2, 1).setStyle(dateStyle);
         cells.get(3, 1).setStyle(dateStyle);
         cells.get(4, 1).setStyle(dateStyle);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
 
         PivotTableCollection pivots = sheet.getPivotTables();
         //Add a PivotTable
         PivotTable pivot = pivots.add("=Sheet1!A1:C5", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "date");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         pivot.calculateData();
         //Add time line based on date field.
         int index = sheet.getTimelines().add(pivot, "E1","date");
         Timeline timeline = sheet.getTimelines().get(index);
 
         //do your business
         book.save("out.xlsx");
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCaption()](#getCaption--) | Liefert die Beschriftung dieser Timeline. |
| [getClass()](#getClass--) |  |
| [getCurrentLevel()](#getCurrentLevel--) | Die aktuelle Zeitebene der Timeline. |
| [getHeightPixel()](#getHeightPixel--) | Gibt die Höhe der angegebenen Timeline zurück oder legt sie fest, in Pixel. |
| [getLeftPixel()](#getLeftPixel--) | Gibt den horizontalen Versatz der Timeline-Form von ihrer linken Spalte zurück oder legt ihn fest, in Pixel. |
| [getName()](#getName--) | Gibt den Namen der angegebenen Timeline zurück oder legt ihn fest |
| [getSelectedDateTimeRange()](#getSelectedDateTimeRange--) | Ermittelt den ausgewählten Datums‑Zeit‑Bereich. |
| [getSelectionLevel()](#getSelectionLevel--) | Ermittelt die Zeitebene, auf der die aktuelle Auswahl für die Timeline getroffen wurde. |
| [getShape()](#getShape--) | Gibt das [TimelineShape](../../com.aspose.cells/timelineshape)-Objekt zurück, das mit dieser Timeline verknüpft ist. |
| [getShowHeader()](#getShowHeader--) | Gibt an, ob die Kopfzeile dieser Timeline angezeigt werden soll. |
| [getShowHorizontalScrollbar()](#getShowHorizontalScrollbar--) | Gibt an, ob die horizontale Bildlaufleiste angezeigt werden soll. |
| [getShowSelectionLabel()](#getShowSelectionLabel--) | Gibt an, ob das Auswahl‑Label angezeigt werden soll. |
| [getShowTimeLevel()](#getShowTimeLevel--) | Gibt an, ob das Dropdown‑Auswahlfeld der Zeitebene angezeigt werden soll. |
| [getStartDate()](#getStartDate--) | Ermittelt das Startdatum der Zeitspanne‑Scrollposition dieser [Timeline](../../com.aspose.cells/timeline). |
| [getTopPixel()](#getTopPixel--) | Gibt den vertikalen Versatz der Timeline-Form von ihrer oberen Zeile zurück oder legt ihn fest, in Pixel. |
| [getWidthPixel()](#getWidthPixel--) | Gibt die Breite der angegebenen Timeline zurück oder legt sie fest, in Pixel. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [select(DateTime start, DateTime end, boolean calculate)](#select-com.aspose.cells.DateTime-com.aspose.cells.DateTime-boolean-) | Element zwischen den Datum‑Zeit‑Werten auswählen. |
| [setCaption(String value)](#setCaption-java.lang.String-) | Legt die Beschriftung dieser Timeline fest. |
| [setCurrentLevel(int value)](#setCurrentLevel-int-) | Die aktuelle Zeitebene der Timeline. |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Gibt die Höhe der angegebenen Timeline zurück oder legt sie fest, in Pixel. |
| [setLeftPixel(int value)](#setLeftPixel-int-) | Gibt den horizontalen Versatz der Timeline-Form von ihrer linken Spalte zurück oder legt ihn fest, in Pixel. |
| [setName(String value)](#setName-java.lang.String-) | Gibt den Namen der angegebenen Timeline zurück oder legt ihn fest |
| [setSelectionLevel(int value)](#setSelectionLevel-int-) | Legt die Zeitebene fest, auf der die aktuelle Auswahl für die Timeline getroffen wurde. |
| [setShowHeader(boolean value)](#setShowHeader-boolean-) | Gibt an, ob die Kopfzeile dieser Timeline angezeigt werden soll. |
| [setShowHorizontalScrollbar(boolean value)](#setShowHorizontalScrollbar-boolean-) | Gibt an, ob die horizontale Bildlaufleiste angezeigt werden soll. |
| [setShowSelectionLabel(boolean value)](#setShowSelectionLabel-boolean-) | Gibt an, ob das Auswahl‑Label angezeigt werden soll. |
| [setShowTimeLevel(boolean value)](#setShowTimeLevel-boolean-) | Gibt an, ob das Dropdown‑Auswahlfeld der Zeitebene angezeigt werden soll. |
| [setStartDate(DateTime value)](#setStartDate-com.aspose.cells.DateTime-) | Legt das Startdatum der Zeitspanne‑Scrollposition dieser [Timeline](../../com.aspose.cells/timeline) fest. |
| [setTopPixel(int value)](#setTopPixel-int-) | Gibt den vertikalen Versatz der Timeline-Form von ihrer oberen Zeile zurück oder legt ihn fest, in Pixel. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | Gibt die Breite der angegebenen Timeline zurück oder legt sie fest, in Pixel. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getCaption() {#getCaption--}
```
public String getCaption()
```


Liefert die Beschriftung dieser Timeline.

**Example**

```
         //Set the caption of this Timeline.
         timeline.setCaption("timeline caption test");
```

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCurrentLevel() {#getCurrentLevel--}
```
public int getCurrentLevel()
```


Die aktuelle Zeitebene der Timeline.

Siehe [TimelineLevelType](../../com.aspose.cells/timelineleveltype).

**Returns:**
int
### getHeightPixel() {#getHeightPixel--}
```
public int getHeightPixel()
```


Gibt die Höhe der angegebenen Timeline zurück oder legt sie fest, in Pixel.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft Shape.Height. Diese Eigenschaft wird 12 Monate nach Mai 2025 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Returns:**
int
### getLeftPixel() {#getLeftPixel--}
```
public int getLeftPixel()
```


Gibt den horizontalen Versatz der Timeline-Form von ihrer linken Spalte zurück oder legt ihn fest, in Pixel.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft Shape.Left. Diese Eigenschaft wird 12 Monate nach Mai 2025 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Gibt den Namen der angegebenen Timeline zurück oder legt ihn fest

**Example**

```
         //Set the name of the specified Timeline.
         timeline.setName("timeline name test");
```

**Returns:**
java.lang.String
### getSelectedDateTimeRange() {#getSelectedDateTimeRange--}
```
public DateTime[] getSelectedDateTimeRange()
```


Ermittelt den ausgewählten Datums‑Zeit‑Bereich.

**Returns:**
com.aspose.cells.DateTime[] -
### getSelectionLevel() {#getSelectionLevel--}
```
public int getSelectionLevel()
```


Ermittelt die Zeitebene, auf der die aktuelle Auswahl für die Timeline getroffen wurde.

Siehe [TimelineLevelType](../../com.aspose.cells/timelineleveltype).

**Returns:**
int
### getShape() {#getShape--}
```
public TimelineShape getShape()
```


Gibt das [TimelineShape](../../com.aspose.cells/timelineshape)-Objekt zurück, das mit dieser Timeline verknüpft ist.

**Returns:**
[TimelineShape](../../com.aspose.cells/timelineshape)
### getShowHeader() {#getShowHeader--}
```
public boolean getShowHeader()
```


Gibt an, ob die Kopfzeile dieser Timeline angezeigt werden soll.

**Returns:**
boolean
### getShowHorizontalScrollbar() {#getShowHorizontalScrollbar--}
```
public boolean getShowHorizontalScrollbar()
```


Gibt an, ob die horizontale Bildlaufleiste angezeigt werden soll.

**Returns:**
boolean
### getShowSelectionLabel() {#getShowSelectionLabel--}
```
public boolean getShowSelectionLabel()
```


Gibt an, ob das Auswahl‑Label angezeigt werden soll.

**Returns:**
boolean
### getShowTimeLevel() {#getShowTimeLevel--}
```
public boolean getShowTimeLevel()
```


Gibt an, ob das Dropdown‑Auswahlfeld der Zeitebene angezeigt werden soll.

**Returns:**
boolean
### getStartDate() {#getStartDate--}
```
public DateTime getStartDate()
```


Ermittelt das Startdatum der Zeitspanne‑Scrollposition dieser [Timeline](../../com.aspose.cells/timeline).

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getTopPixel() {#getTopPixel--}
```
public int getTopPixel()
```


Gibt den vertikalen Versatz der Timeline-Form von ihrer oberen Zeile zurück oder legt ihn fest, in Pixel.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft Shape.Top. Diese Eigenschaft wird 12 Monate nach Mai 2025 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Returns:**
int
### getWidthPixel() {#getWidthPixel--}
```
public int getWidthPixel()
```


Gibt die Breite der angegebenen Timeline zurück oder legt sie fest, in Pixel.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft Shape.Width. Diese Eigenschaft wird 12 Monate nach Mai 2025 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Returns:**
int
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




### select(DateTime start, DateTime end, boolean calculate) {#select-com.aspose.cells.DateTime-com.aspose.cells.DateTime-boolean-}
```
public void select(DateTime start, DateTime end, boolean calculate)
```


Element zwischen den Datum‑Zeit‑Werten auswählen.

**Remarks**

[getCurrentLevel()](../../com.aspose.cells/timeline\#getCurrentLevel--) must be set before calling this method. If this method is called, [getSelectionLevel()](../../com.aspose.cells/timeline\#getSelectionLevel--) will be [getCurrentLevel()](../../com.aspose.cells/timeline\#getCurrentLevel--).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| start | [DateTime](../../com.aspose.cells/datetime) | Das Startdatum und die Uhrzeit |
| end | [DateTime](../../com.aspose.cells/datetime) | Das Enddatum und die Uhrzeit |
| berechnen | boolean | Gibt an, ob relative Pivot-Tabellen berechnet werden sollen |

### setCaption(String value) {#setCaption-java.lang.String-}
```
public void setCaption(String value)
```


Legt die Beschriftung dieser Timeline fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setCurrentLevel(int value) {#setCurrentLevel-int-}
```
public void setCurrentLevel(int value)
```


Die aktuelle Zeitebene der Timeline.

Siehe [TimelineLevelType](../../com.aspose.cells/timelineleveltype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setHeightPixel(int value) {#setHeightPixel-int-}
```
public void setHeightPixel(int value)
```


Gibt die Höhe der angegebenen Timeline zurück oder legt sie fest, in Pixel.

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


Gibt den horizontalen Versatz der Timeline-Form von ihrer linken Spalte zurück oder legt ihn fest, in Pixel.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft Shape.Left. Diese Eigenschaft wird 12 Monate nach Mai 2025 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Gibt den Namen der angegebenen Timeline zurück oder legt ihn fest

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setSelectionLevel(int value) {#setSelectionLevel-int-}
```
public void setSelectionLevel(int value)
```


Legt die Zeitebene fest, auf der die aktuelle Auswahl für die Timeline getroffen wurde.

Siehe [TimelineLevelType](../../com.aspose.cells/timelineleveltype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setShowHeader(boolean value) {#setShowHeader-boolean-}
```
public void setShowHeader(boolean value)
```


Gibt an, ob die Kopfzeile dieser Timeline angezeigt werden soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowHorizontalScrollbar(boolean value) {#setShowHorizontalScrollbar-boolean-}
```
public void setShowHorizontalScrollbar(boolean value)
```


Gibt an, ob die horizontale Bildlaufleiste angezeigt werden soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowSelectionLabel(boolean value) {#setShowSelectionLabel-boolean-}
```
public void setShowSelectionLabel(boolean value)
```


Gibt an, ob das Auswahl‑Label angezeigt werden soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowTimeLevel(boolean value) {#setShowTimeLevel-boolean-}
```
public void setShowTimeLevel(boolean value)
```


Gibt an, ob das Dropdown‑Auswahlfeld der Zeitebene angezeigt werden soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setStartDate(DateTime value) {#setStartDate-com.aspose.cells.DateTime-}
```
public void setStartDate(DateTime value)
```


Legt das Startdatum der Zeitspanne‑Scrollposition dieser [Timeline](../../com.aspose.cells/timeline) fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setTopPixel(int value) {#setTopPixel-int-}
```
public void setTopPixel(int value)
```


Gibt den vertikalen Versatz der Timeline-Form von ihrer oberen Zeile zurück oder legt ihn fest, in Pixel.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft Shape.Top. Diese Eigenschaft wird 12 Monate nach Mai 2025 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setWidthPixel(int value) {#setWidthPixel-int-}
```
public void setWidthPixel(int value)
```


Gibt die Breite der angegebenen Timeline zurück oder legt sie fest, in Pixel.

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

