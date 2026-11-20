---
title: "PivotFieldTop10AutoShowSettings"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Top‑10‑AutoShow‑Einstellungen für ein Pivotfeld dar."
type: docs
url: /de/java/com.aspose.cells/pivotfieldtop10autoshowsettings/
---

**Inheritance:**
java.lang.Object
```
public class PivotFieldTop10AutoShowSettings
```

Stellt die Top‑10‑AutoShow‑Einstellungen für ein Pivotfeld dar.

**Remarks**

In xls : Implementierung von Top‑10‑Filtern in Xls über Top 10 AutoShow In ooxml‑Dateien: Das zugrunde liegende ooxml‑Dateiformat unterstützt Top10 AutoShow, aber die Benutzeroberfläche von Excel 2007 und neuer bietet nur Zugriff über den Top10‑Filter. Wenn XLS‑Kompatibilität nicht erforderlich ist, wird empfohlen, stattdessen den Top10‑Filter zu verwenden.

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
 
         //Show top 2 items by row field label.
         rowField.top10AutoShow(true, true, 2, -1);
 
         PivotFieldTop10AutoShowSettings sortSetting = rowField.getTop10AutoShowSettings();
         System.out.println(sortSetting.isAutoShow());
 
          pivot.calculateData();
 
         book.save("out.xlsx");
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoShowCount()](#getAutoShowCount--) | Stellt die Anzahl der obersten oder untersten Elemente dar, die im angegebenen PivotTable‑Feld automatisch angezeigt werden. |
| [getClass()](#getClass--) |  |
| [getRankBy()](#getRankBy--) | Gibt den Index des Datenfelds für das AutoShow‑Ranking an. |
| [hashCode()](#hashCode--) |  |
| [isAutoShow()](#isAutoShow--) | Gibt an, ob ein "Top 10 AutoShow"‑Filter auf dieses Feld angewendet wird. |
| [isTop()](#isTop--) | Gibt an, ob das angegebene PivotTable‑Feld aufsteigend automatisch angezeigt wird. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoShow(boolean value)](#setAutoShow-boolean-) | Gibt an, ob ein "Top 10 AutoShow"‑Filter auf dieses Feld angewendet wird. |
| [setAutoShowCount(int value)](#setAutoShowCount-int-) | Stellt die Anzahl der obersten oder untersten Elemente dar, die im angegebenen PivotTable‑Feld automatisch angezeigt werden. |
| [setRankBy(int value)](#setRankBy-int-) | Gibt den Index des Datenfelds für das AutoShow‑Ranking an. |
| [setTop(boolean value)](#setTop-boolean-) | Gibt an, ob das angegebene PivotTable‑Feld aufsteigend automatisch angezeigt wird. |
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
### getAutoShowCount() {#getAutoShowCount--}
```
public int getAutoShowCount()
```


Stellt die Anzahl der obersten oder untersten Elemente dar, die im angegebenen PivotTable‑Feld automatisch angezeigt werden.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getRankBy() {#getRankBy--}
```
public int getRankBy()
```


Gibt den Index des Datenfelds für das AutoShow‑Ranking an. Stellt den Index des AutoShow‑Feldes dar. -1 bedeutet das PivotField selbst. Es sollte der Index der Datenfelder sein.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoShow() {#isAutoShow--}
```
public boolean isAutoShow()
```


Gibt an, ob ein "Top 10 AutoShow"‑Filter auf dieses Feld angewendet wird.

**Returns:**
boolean
### isTop() {#isTop--}
```
public boolean isTop()
```


Gibt an, ob das angegebene PivotTable‑Feld aufsteigend automatisch angezeigt wird.

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




### setAutoShow(boolean value) {#setAutoShow-boolean-}
```
public void setAutoShow(boolean value)
```


Gibt an, ob ein "Top 10 AutoShow"‑Filter auf dieses Feld angewendet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAutoShowCount(int value) {#setAutoShowCount-int-}
```
public void setAutoShowCount(int value)
```


Stellt die Anzahl der obersten oder untersten Elemente dar, die im angegebenen PivotTable‑Feld automatisch angezeigt werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setRankBy(int value) {#setRankBy-int-}
```
public void setRankBy(int value)
```


Gibt den Index des Datenfelds für das AutoShow‑Ranking an. Stellt den Index des AutoShow‑Feldes dar. -1 bedeutet das PivotField selbst. Es sollte der Index der Datenfelder sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setTop(boolean value) {#setTop-boolean-}
```
public void setTop(boolean value)
```


Gibt an, ob das angegebene PivotTable‑Feld aufsteigend automatisch angezeigt wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

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

