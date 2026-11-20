---
title: "ChartDataTable"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt eine Diagrammdatentabelle dar."
type: docs
url: /de/java/com.aspose.cells/chartdatatable/
---

**Inheritance:**
java.lang.Object
```
public class ChartDataTable
```

Stellt eine Diagrammdatentabelle dar.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the first worksheet
         Worksheet worksheet = workbook.getWorksheets().get(0);
 
         //Adding a sample value to "A1" cell
         worksheet.getCells().get("A1").putValue(50);
 
         //Adding a sample value to "A2" cell
         worksheet.getCells().get("A2").putValue(100);
 
         //Adding a sample value to "A3" cell
         worksheet.getCells().get("A3").putValue(150);
 
         //Adding a sample value to "B1" cell
         worksheet.getCells().get("B1").putValue(60);
 
         //Adding a sample value to "B2" cell
         worksheet.getCells().get("B2").putValue(32);
 
         //Adding a sample value to "B3" cell
         worksheet.getCells().get("B3").putValue(50);
 
         //Adding a chart to the worksheet
         int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 25, 10);
 
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
 
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
         chart.getNSeries().add("A1:B3", true);
 
         chart.setShowDataTable(true);
 
         //Getting Chart Table
         ChartDataTable chartTable = chart.getChartDataTable();
 
         //Setting Chart Table Font Color
         chartTable.getFont().setColor(com.aspose.cells.Color.getRed());
 
         //Setting Legend Key VisibilityOptions
         chartTable.setShowLegendKey(false);
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoScaleFont()](#getAutoScaleFont--) | True, wenn der Text im Objekt die Schriftgröße ändert, wenn die Objektgröße geändert wird. |
| [getBackgroundMode()](#getBackgroundMode--) | Ermittelt den Anzeigemodus des Hintergrunds. |
| [getBorder()](#getBorder--) | Gibt ein Border‑Objekt zurück, das den Rand des Objekts darstellt. |
| [getClass()](#getClass--) |  |
| [getFont()](#getFont--) | Liest ein [getFont()](../../com.aspose.cells/chartdatatable\#getFont--) Objekt, das die Schriftarteinstellung der angegebenen Diagrammdatentabelle darstellt. |
| [getShowLegendKey()](#getShowLegendKey--) | Wahr, wenn der Legenden‑Schlüssel der Datenbeschriftung sichtbar ist. |
| [hasBorderHorizontal()](#hasBorderHorizontal--) | Wahr, wenn die Diagrammdatentabelle horizontale Zellenränder hat |
| [hasBorderOutline()](#hasBorderOutline--) | Wahr, wenn die Diagrammdatentabelle Umrissränder hat |
| [hasBorderVertical()](#hasBorderVertical--) | Wahr, wenn die Diagrammdatentabelle vertikale Zellenränder hat |
| [hasHorizontalBorder()](#hasHorizontalBorder--) | Wahr, wenn die Diagrammdatentabelle horizontale Zellenränder hat |
| [hasOutlineBorder()](#hasOutlineBorder--) | Wahr, wenn die Diagrammdatentabelle Umrissränder hat |
| [hasVerticalBorder()](#hasVerticalBorder--) | Wahr, wenn die Diagrammdatentabelle vertikale Zellenränder hat |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoScaleFont(boolean value)](#setAutoScaleFont-boolean-) | True, wenn der Text im Objekt die Schriftgröße ändert, wenn die Objektgröße geändert wird. |
| [setBackgroundMode(int value)](#setBackgroundMode-int-) | Legt den Anzeigemodus des Hintergrunds fest. |
| [setHasBorderHorizontal(boolean value)](#setHasBorderHorizontal-boolean-) | Wahr, wenn die Diagrammdatentabelle horizontale Zellenränder hat |
| [setHasBorderOutline(boolean value)](#setHasBorderOutline-boolean-) | Wahr, wenn die Diagrammdatentabelle Umrissränder hat |
| [setHasBorderVertical(boolean value)](#setHasBorderVertical-boolean-) | Wahr, wenn die Diagrammdatentabelle vertikale Zellenränder hat |
| [setHasHorizontalBorder(boolean value)](#setHasHorizontalBorder-boolean-) | Wahr, wenn die Diagrammdatentabelle horizontale Zellenränder hat |
| [setHasOutlineBorder(boolean value)](#setHasOutlineBorder-boolean-) | Wahr, wenn die Diagrammdatentabelle Umrissränder hat |
| [setHasVerticalBorder(boolean value)](#setHasVerticalBorder-boolean-) | Wahr, wenn die Diagrammdatentabelle vertikale Zellenränder hat |
| [setShowLegendKey(boolean value)](#setShowLegendKey-boolean-) | Wahr, wenn der Legenden‑Schlüssel der Datenbeschriftung sichtbar ist. |
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
### getAutoScaleFont() {#getAutoScaleFont--}
```
public boolean getAutoScaleFont()
```


True, wenn der Text im Objekt die Schriftgröße ändert, wenn sich die Objektgröße ändert. Der Standardwert ist True.

**Returns:**
boolean
### getBackgroundMode() {#getBackgroundMode--}
```
public int getBackgroundMode()
```


Ermittelt den Anzeigemodus des Hintergrunds.

Siehe [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Returns:**
int
### getBorder() {#getBorder--}
```
public Line getBorder()
```


Gibt ein Border‑Objekt zurück, das den Rand des Objekts darstellt.

**Returns:**
[Line](../../com.aspose.cells/line)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFont() {#getFont--}
```
public Font getFont()
```


Liest ein [getFont()](../../com.aspose.cells/chartdatatable\#getFont--) Objekt, das die Schriftarteinstellung der angegebenen Diagrammdatentabelle darstellt.

**Returns:**
[Font](../../com.aspose.cells/font)
### getShowLegendKey() {#getShowLegendKey--}
```
public boolean getShowLegendKey()
```


Wahr, wenn der Legenden‑Schlüssel der Datenbeschriftung sichtbar ist.

**Returns:**
boolean
### hasBorderHorizontal() {#hasBorderHorizontal--}
```
public boolean hasBorderHorizontal()
```


Wahr, wenn die Diagrammdatentabelle horizontale Zellenränder hat

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft ChartDataTable.HasHorizontalBorder. Diese Eigenschaft wird 12 Monate später, seit Juni 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

**Returns:**
boolean
### hasBorderOutline() {#hasBorderOutline--}
```
public boolean hasBorderOutline()
```


Wahr, wenn die Diagrammdatentabelle Umrissränder hat

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft ChartDataTable.HasOutlineBorder. Diese Eigenschaft wird 12 Monate später, seit Juni 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

**Returns:**
boolean
### hasBorderVertical() {#hasBorderVertical--}
```
public boolean hasBorderVertical()
```


Wahr, wenn die Diagrammdatentabelle vertikale Zellenränder hat

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft ChartDataTable.HasVerticalBorder. Diese Eigenschaft wird 12 Monate später, seit Juni 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

**Returns:**
boolean
### hasHorizontalBorder() {#hasHorizontalBorder--}
```
public boolean hasHorizontalBorder()
```


Wahr, wenn die Diagrammdatentabelle horizontale Zellenränder hat

**Returns:**
boolean
### hasOutlineBorder() {#hasOutlineBorder--}
```
public boolean hasOutlineBorder()
```


Wahr, wenn die Diagrammdatentabelle Umrissränder hat

**Returns:**
boolean
### hasVerticalBorder() {#hasVerticalBorder--}
```
public boolean hasVerticalBorder()
```


Wahr, wenn die Diagrammdatentabelle vertikale Zellenränder hat

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




### setAutoScaleFont(boolean value) {#setAutoScaleFont-boolean-}
```
public void setAutoScaleFont(boolean value)
```


True, wenn der Text im Objekt die Schriftgröße ändert, wenn sich die Objektgröße ändert. Der Standardwert ist True.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setBackgroundMode(int value) {#setBackgroundMode-int-}
```
public void setBackgroundMode(int value)
```


Legt den Anzeigemodus des Hintergrunds fest.

Siehe [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setHasBorderHorizontal(boolean value) {#setHasBorderHorizontal-boolean-}
```
public void setHasBorderHorizontal(boolean value)
```


Wahr, wenn die Diagrammdatentabelle horizontale Zellenränder hat

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft ChartDataTable.HasHorizontalBorder. Diese Eigenschaft wird 12 Monate später, seit Juni 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setHasBorderOutline(boolean value) {#setHasBorderOutline-boolean-}
```
public void setHasBorderOutline(boolean value)
```


Wahr, wenn die Diagrammdatentabelle Umrissränder hat

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft ChartDataTable.HasOutlineBorder. Diese Eigenschaft wird 12 Monate später, seit Juni 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setHasBorderVertical(boolean value) {#setHasBorderVertical-boolean-}
```
public void setHasBorderVertical(boolean value)
```


Wahr, wenn die Diagrammdatentabelle vertikale Zellenränder hat

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft ChartDataTable.HasVerticalBorder. Diese Eigenschaft wird 12 Monate später, seit Juni 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setHasHorizontalBorder(boolean value) {#setHasHorizontalBorder-boolean-}
```
public void setHasHorizontalBorder(boolean value)
```


Wahr, wenn die Diagrammdatentabelle horizontale Zellenränder hat

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setHasOutlineBorder(boolean value) {#setHasOutlineBorder-boolean-}
```
public void setHasOutlineBorder(boolean value)
```


Wahr, wenn die Diagrammdatentabelle Umrissränder hat

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setHasVerticalBorder(boolean value) {#setHasVerticalBorder-boolean-}
```
public void setHasVerticalBorder(boolean value)
```


Wahr, wenn die Diagrammdatentabelle vertikale Zellenränder hat

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowLegendKey(boolean value) {#setShowLegendKey-boolean-}
```
public void setShowLegendKey(boolean value)
```


Wahr, wenn der Legenden‑Schlüssel der Datenbeschriftung sichtbar ist.

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

