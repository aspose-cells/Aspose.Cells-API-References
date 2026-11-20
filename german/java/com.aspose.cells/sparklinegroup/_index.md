---
title: "SparklineGroup"
second_title: "Aspose.Cells for Java API-Referenz"
description: "ist in einer Sparkline-Gruppe organisiert."
type: docs
url: /de/java/com.aspose.cells/sparklinegroup/
---

**Inheritance:**
java.lang.Object
```
public class SparklineGroup
```

[Sparkline](../../com.aspose.cells/sparkline) is organized into a sparkline group. A SparklineGroup contains a variable number of sparkline items. A sparkline group specifies the type, display settings and axis settings for the sparklines.

**Example**

```
         Workbook book = new Workbook(); 
         Worksheet sheet = book.getWorksheets().get(0);
 
         sheet.getCells().get("A1").putValue(5);
         sheet.getCells().get("B1").putValue(2);
         sheet.getCells().get("C1").putValue(1);
         sheet.getCells().get("D1").putValue(3);
 
         // Define the CellArea
         CellArea ca = new CellArea();
         ca.StartColumn = 4;
         ca.EndColumn = 4;
         ca.StartRow = 0;
         ca.EndRow = 0;
         int idx = sheet.getSparklineGroups().add(com.aspose.cells.SparklineType.LINE, "A1:D1", false, ca);
         SparklineGroup group = sheet.getSparklineGroups().get(idx);
         group.getSparklines().add(sheet.getName() + "!A1:D1", 0, 4);
         // Create CellsColor
         CellsColor clr = book.createCellsColor();
         clr.setColor(Color.getOrange());
         group.setSeriesColor(clr);
 
         // set the high points are colored green and the low points are colored red
         group.setShowHighPoint(true);
         group.setShowLowPoint(true);
         group.getHighPointColor().setColor(Color.getGreen());
         group.getLowPointColor().setColor(Color.getRed());
         // set line weight 
         group.setLineWeight(1.0);
         book.save("output.xlsx", SaveFormat.XLSX);
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDisplayHidden()](#getDisplayHidden--) | Gibt an, ob Daten in ausgeblendeten Zeilen und Spalten angezeigt werden sollen. |
| [getFirstPointColor()](#getFirstPointColor--) | Liest die Farbe des ersten Datenpunkts in der Sparkline-Gruppe. |
| [getHighPointColor()](#getHighPointColor--) | Liest die Farbe der höchsten Datenpunkte in der Sparkline-Gruppe. |
| [getHorizontalAxisColor()](#getHorizontalAxisColor--) | Liest die Farbe der horizontalen Achse in der Sparkline-Gruppe. |
| [getHorizontalAxisDateRange()](#getHorizontalAxisDateRange--) | Stellt den Bereich dar, der die Datumswerte für die Sparkline-Daten enthält. |
| [getLastPointColor()](#getLastPointColor--) | Liest die Farbe des letzten Datenpunkts in der Sparkline-Gruppe. |
| [getLineWeight()](#getLineWeight--) | Liest die Linienstärke jeder Linien-Sparkline in der Sparkline-Gruppe, angegeben in Punkten. |
| [getLowPointColor()](#getLowPointColor--) | Liest die Farbe der niedrigsten Datenpunkte in der Sparkline-Gruppe. |
| [getMarkersColor()](#getMarkersColor--) | Liest die Farbe der Punkte jeder Linien-Sparkline in der Sparkline-Gruppe. |
| [getNegativePointsColor()](#getNegativePointsColor--) | Liest die Farbe der negativen Werte in der Sparkline-Gruppe. |
| [getPlotEmptyCellsType()](#getPlotEmptyCellsType--) | Gibt an, wie leere Zellen dargestellt werden. |
| [getPlotRightToLeft()](#getPlotRightToLeft--) | Gibt an, ob die Plot-Daten von rechts nach links verlaufen. |
| [getPresetStyle()](#getPresetStyle--) | Liest den voreingestellten Stiltyp der Sparkline-Gruppe. |
| [getSeriesColor()](#getSeriesColor--) | Liest die Farbe der Sparklines in der Sparkline-Gruppe. |
| [getShowFirstPoint()](#getShowFirstPoint--) | Gibt an, ob der erste Datenpunkt in der Sparkline-Gruppe hervorgehoben werden soll. |
| [getShowHighPoint()](#getShowHighPoint--) | Gibt an, ob die höchsten Datenpunkte in der Sparkline‑Gruppe hervorgehoben werden sollen. |
| [getShowHorizontalAxis()](#getShowHorizontalAxis--) | Gibt an, ob die horizontale Achse der Sparkline angezeigt werden soll. |
| [getShowLastPoint()](#getShowLastPoint--) | Gibt an, ob der letzte Datenpunkt in der Sparkline‑Gruppe hervorgehoben werden soll. |
| [getShowLowPoint()](#getShowLowPoint--) | Gibt an, ob die niedrigsten Datenpunkte in der Sparkline‑Gruppe hervorgehoben werden sollen. |
| [getShowMarkers()](#getShowMarkers--) | Gibt an, ob jeder Punkt in jeder Linien‑Sparkline der Sparkline‑Gruppe hervorgehoben werden soll. |
| [getShowNegativePoints()](#getShowNegativePoints--) | Gibt an, ob die negativen Werte in der Sparkline‑Gruppe mit einer anderen Farbe oder Markierung hervorgehoben werden sollen. |
| [getSparklineCollection()](#getSparklineCollection--) | Ruft die Sammlung von [Sparkline](../../com.aspose.cells/sparkline)-Objekten ab. |
| [getSparklines()](#getSparklines--) | Ruft die Sammlung von [Sparkline](../../com.aspose.cells/sparkline)-Objekten ab. |
| [getType()](#getType--) | Gibt den Sparkline‑Typ der Sparkline‑Gruppe an. |
| [getVerticalAxisMaxValue()](#getVerticalAxisMaxValue--) | Ruft den benutzerdefinierten Maximalwert für die vertikale Achse ab. |
| [getVerticalAxisMaxValueType()](#getVerticalAxisMaxValueType--) | Stellt den Typ des maximalen Achsenwerts für die vertikale Achse dar. |
| [getVerticalAxisMinValue()](#getVerticalAxisMinValue--) | Ruft den benutzerdefinierten Minimalwert für die vertikale Achse ab. |
| [getVerticalAxisMinValueType()](#getVerticalAxisMinValueType--) | Stellt den Typ des minimalen Achsenwerts für die vertikale Achse dar. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [resetRanges(String dataRange, boolean isVertical, CellArea locationRange)](#resetRanges-java.lang.String-boolean-com.aspose.cells.CellArea-) | Setzt den Datenbereich und den Positionsbereich der Sparkline‑Gruppe zurück. |
| [setDisplayHidden(boolean value)](#setDisplayHidden-boolean-) | Gibt an, ob Daten in ausgeblendeten Zeilen und Spalten angezeigt werden sollen. |
| [setFirstPointColor(CellsColor value)](#setFirstPointColor-com.aspose.cells.CellsColor-) | Legt die Farbe des ersten Datenpunkts in der Sparkline‑Gruppe fest. |
| [setHighPointColor(CellsColor value)](#setHighPointColor-com.aspose.cells.CellsColor-) | Legt die Farbe der höchsten Datenpunkte in der Sparkline‑Gruppe fest. |
| [setHorizontalAxisColor(CellsColor value)](#setHorizontalAxisColor-com.aspose.cells.CellsColor-) | Legt die Farbe der horizontalen Achse in der Sparkline‑Gruppe fest. |
| [setHorizontalAxisDateRange(String value)](#setHorizontalAxisDateRange-java.lang.String-) | Stellt den Bereich dar, der die Datumswerte für die Sparkline-Daten enthält. |
| [setLastPointColor(CellsColor value)](#setLastPointColor-com.aspose.cells.CellsColor-) | Legt die Farbe des letzten Datenpunkts in der Sparkline‑Gruppe fest. |
| [setLineWeight(double value)](#setLineWeight-double-) | Legt die Linienstärke in jeder Linien‑Sparkline der Sparkline‑Gruppe fest, gemessen in Punkten. |
| [setLowPointColor(CellsColor value)](#setLowPointColor-com.aspose.cells.CellsColor-) | Legt die Farbe der niedrigsten Datenpunkte in der Sparkline‑Gruppe fest. |
| [setMarkersColor(CellsColor value)](#setMarkersColor-com.aspose.cells.CellsColor-) | Legt die Farbe der Punkte in jeder Linien‑Sparkline der Sparkline‑Gruppe fest. |
| [setNegativePointsColor(CellsColor value)](#setNegativePointsColor-com.aspose.cells.CellsColor-) | Legt die Farbe der negativen Werte in der Sparkline‑Gruppe fest. |
| [setPlotEmptyCellsType(int value)](#setPlotEmptyCellsType-int-) | Gibt an, wie leere Zellen dargestellt werden. |
| [setPlotRightToLeft(boolean value)](#setPlotRightToLeft-boolean-) | Gibt an, ob die Plot-Daten von rechts nach links verlaufen. |
| [setPresetStyle(int value)](#setPresetStyle-int-) | Legt den voreingestellten Stiltyp der Sparkline‑Gruppe fest. |
| [setSeriesColor(CellsColor value)](#setSeriesColor-com.aspose.cells.CellsColor-) | Legt die Farbe der Sparklines in der Sparkline‑Gruppe fest. |
| [setShowFirstPoint(boolean value)](#setShowFirstPoint-boolean-) | Gibt an, ob der erste Datenpunkt in der Sparkline-Gruppe hervorgehoben werden soll. |
| [setShowHighPoint(boolean value)](#setShowHighPoint-boolean-) | Gibt an, ob die höchsten Datenpunkte in der Sparkline‑Gruppe hervorgehoben werden sollen. |
| [setShowHorizontalAxis(boolean value)](#setShowHorizontalAxis-boolean-) | Gibt an, ob die horizontale Achse der Sparkline angezeigt werden soll. |
| [setShowLastPoint(boolean value)](#setShowLastPoint-boolean-) | Gibt an, ob der letzte Datenpunkt in der Sparkline‑Gruppe hervorgehoben werden soll. |
| [setShowLowPoint(boolean value)](#setShowLowPoint-boolean-) | Gibt an, ob die niedrigsten Datenpunkte in der Sparkline‑Gruppe hervorgehoben werden sollen. |
| [setShowMarkers(boolean value)](#setShowMarkers-boolean-) | Gibt an, ob jeder Punkt in jeder Linien‑Sparkline der Sparkline‑Gruppe hervorgehoben werden soll. |
| [setShowNegativePoints(boolean value)](#setShowNegativePoints-boolean-) | Gibt an, ob die negativen Werte in der Sparkline‑Gruppe mit einer anderen Farbe oder Markierung hervorgehoben werden sollen. |
| [setType(int value)](#setType-int-) | Gibt den Sparkline‑Typ der Sparkline‑Gruppe an. |
| [setVerticalAxisMaxValue(double value)](#setVerticalAxisMaxValue-double-) | Legt den benutzerdefinierten Maximalwert für die vertikale Achse fest. |
| [setVerticalAxisMaxValue(int type, double value)](#setVerticalAxisMaxValue-int-double-) | Legt den benutzerdefinierten Maximalwert für die vertikale Sparkline‑Achse mit dem angegebenen Achsenwerttyp fest. |
| [setVerticalAxisMaxValueType(int value)](#setVerticalAxisMaxValueType-int-) | Stellt den Typ des maximalen Achsenwerts für die vertikale Achse dar. |
| [setVerticalAxisMinValue(double value)](#setVerticalAxisMinValue-double-) | Legt den benutzerdefinierten Minimalwert für die vertikale Achse fest. |
| [setVerticalAxisMinValue(int type, double value)](#setVerticalAxisMinValue-int-double-) | Legt den benutzerdefinierten Minimalwert für die vertikale Achse der Sparkline mit dem angegebenen Achsenwerttyp fest. |
| [setVerticalAxisMinValueType(int value)](#setVerticalAxisMinValueType-int-) | Stellt den Typ des minimalen Achsenwerts für die vertikale Achse dar. |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDisplayHidden() {#getDisplayHidden--}
```
public boolean getDisplayHidden()
```


Gibt an, ob Daten in ausgeblendeten Zeilen und Spalten angezeigt werden sollen.

**Returns:**
boolean
### getFirstPointColor() {#getFirstPointColor--}
```
public CellsColor getFirstPointColor()
```


Liest die Farbe des ersten Datenpunkts in der Sparkline-Gruppe.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getHighPointColor() {#getHighPointColor--}
```
public CellsColor getHighPointColor()
```


Liest die Farbe der höchsten Datenpunkte in der Sparkline-Gruppe.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getHorizontalAxisColor() {#getHorizontalAxisColor--}
```
public CellsColor getHorizontalAxisColor()
```


Liest die Farbe der horizontalen Achse in der Sparkline-Gruppe.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getHorizontalAxisDateRange() {#getHorizontalAxisDateRange--}
```
public String getHorizontalAxisDateRange()
```


Stellt den Bereich dar, der die Datumswerte für die Sparkline-Daten enthält.

**Returns:**
java.lang.String
### getLastPointColor() {#getLastPointColor--}
```
public CellsColor getLastPointColor()
```


Liest die Farbe des letzten Datenpunkts in der Sparkline-Gruppe.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getLineWeight() {#getLineWeight--}
```
public double getLineWeight()
```


Liest die Linienstärke jeder Linien-Sparkline in der Sparkline-Gruppe, angegeben in Punkten.

**Returns:**
double
### getLowPointColor() {#getLowPointColor--}
```
public CellsColor getLowPointColor()
```


Liest die Farbe der niedrigsten Datenpunkte in der Sparkline-Gruppe.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getMarkersColor() {#getMarkersColor--}
```
public CellsColor getMarkersColor()
```


Liest die Farbe der Punkte jeder Linien-Sparkline in der Sparkline-Gruppe.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getNegativePointsColor() {#getNegativePointsColor--}
```
public CellsColor getNegativePointsColor()
```


Liest die Farbe der negativen Werte in der Sparkline-Gruppe.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getPlotEmptyCellsType() {#getPlotEmptyCellsType--}
```
public int getPlotEmptyCellsType()
```


Gibt an, wie leere Zellen dargestellt werden.

Siehe [PlotEmptyCellsType](../../com.aspose.cells/plotemptycellstype).

**Returns:**
int
### getPlotRightToLeft() {#getPlotRightToLeft--}
```
public boolean getPlotRightToLeft()
```


Gibt an, ob die Plot-Daten von rechts nach links verlaufen.

**Returns:**
boolean
### getPresetStyle() {#getPresetStyle--}
```
public int getPresetStyle()
```


Liest den voreingestellten Stiltyp der Sparkline-Gruppe.

Siehe [SparklinePresetStyleType](../../com.aspose.cells/sparklinepresetstyletype).

**Remarks**

Wenn diese Eigenschaft gesetzt ist, werden diese Eigenschaften: SeriesColor,NegativePointsColor,HorizontalAxisColor,MarkersColor,FirstPointColor,LastPointColor,HighPointColor,LowPointColor überschrieben. Bitte setzen Sie zuerst die Eigenschaft und dann die anderen.

**Returns:**
int
### getSeriesColor() {#getSeriesColor--}
```
public CellsColor getSeriesColor()
```


Liest die Farbe der Sparklines in der Sparkline-Gruppe.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getShowFirstPoint() {#getShowFirstPoint--}
```
public boolean getShowFirstPoint()
```


Gibt an, ob der erste Datenpunkt in der Sparkline-Gruppe hervorgehoben werden soll.

**Returns:**
boolean
### getShowHighPoint() {#getShowHighPoint--}
```
public boolean getShowHighPoint()
```


Gibt an, ob die höchsten Datenpunkte in der Sparkline‑Gruppe hervorgehoben werden sollen.

**Returns:**
boolean
### getShowHorizontalAxis() {#getShowHorizontalAxis--}
```
public boolean getShowHorizontalAxis()
```


Gibt an, ob die horizontale Achse der Sparkline angezeigt werden soll. Die horizontale Achse erscheint, wenn die Sparkline Daten enthält, die die Nullachse überschreiten.

**Returns:**
boolean
### getShowLastPoint() {#getShowLastPoint--}
```
public boolean getShowLastPoint()
```


Gibt an, ob der letzte Datenpunkt in der Sparkline‑Gruppe hervorgehoben werden soll.

**Returns:**
boolean
### getShowLowPoint() {#getShowLowPoint--}
```
public boolean getShowLowPoint()
```


Gibt an, ob die niedrigsten Datenpunkte in der Sparkline‑Gruppe hervorgehoben werden sollen.

**Returns:**
boolean
### getShowMarkers() {#getShowMarkers--}
```
public boolean getShowMarkers()
```


Gibt an, ob jeder Punkt in jeder Linien‑Sparkline der Sparkline‑Gruppe hervorgehoben werden soll.

**Returns:**
boolean
### getShowNegativePoints() {#getShowNegativePoints--}
```
public boolean getShowNegativePoints()
```


Gibt an, ob die negativen Werte in der Sparkline‑Gruppe mit einer anderen Farbe oder Markierung hervorgehoben werden sollen.

**Returns:**
boolean
### getSparklineCollection() {#getSparklineCollection--}
```
public SparklineCollection getSparklineCollection()
```


Ruft die Sammlung von [Sparkline](../../com.aspose.cells/sparkline)-Objekten ab.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft SparklineGroup.Sparklines. Diese Eigenschaft wird 12 Monate später, seit November 2022, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Returns:**
[SparklineCollection](../../com.aspose.cells/sparklinecollection)
### getSparklines() {#getSparklines--}
```
public SparklineCollection getSparklines()
```


Ruft die Sammlung von [Sparkline](../../com.aspose.cells/sparkline)-Objekten ab.

**Returns:**
[SparklineCollection](../../com.aspose.cells/sparklinecollection)
### getType() {#getType--}
```
public int getType()
```


Gibt den Sparkline‑Typ der Sparkline‑Gruppe an.

Siehe [SparklineType](../../com.aspose.cells/sparklinetype).

**Returns:**
int
### getVerticalAxisMaxValue() {#getVerticalAxisMaxValue--}
```
public double getVerticalAxisMaxValue()
```


Ruft den benutzerdefinierten Maximalwert für die vertikale Achse ab.

**Remarks**

Wenn diese Eigenschaft gesetzt ist, wird [getVerticalAxisMaxValueType()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMaxValueType--) [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM) sein.

**Returns:**
double
### getVerticalAxisMaxValueType() {#getVerticalAxisMaxValueType--}
```
public int getVerticalAxisMaxValueType()
```


Stellt den Typ des maximalen Achsenwerts für die vertikale Achse dar.

Siehe [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype).

**Returns:**
int
### getVerticalAxisMinValue() {#getVerticalAxisMinValue--}
```
public double getVerticalAxisMinValue()
```


Ruft den benutzerdefinierten Minimalwert für die vertikale Achse ab.

**Remarks**

Wenn diese Eigenschaft gesetzt ist, wird [getVerticalAxisMinValueType()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMinValueType--) [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM) sein.

**Returns:**
double
### getVerticalAxisMinValueType() {#getVerticalAxisMinValueType--}
```
public int getVerticalAxisMinValueType()
```


Stellt den Typ des minimalen Achsenwerts für die vertikale Achse dar.

Siehe [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype).

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




### resetRanges(String dataRange, boolean isVertical, CellArea locationRange) {#resetRanges-java.lang.String-boolean-com.aspose.cells.CellArea-}
```
public void resetRanges(String dataRange, boolean isVertical, CellArea locationRange)
```


Setzt den Datenbereich und den Positionsbereich der Sparkline-Gruppe zurück. Diese Methode löscht die ursprünglichen Sparkline-Elemente in der Gruppe und erstellt neue Sparkline-Elemente für die neuen Bereiche.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dataRange | java.lang.String | Gibt den neuen Datenbereich der Sparkline-Gruppe an. |
| isVertical | boolean | Gibt an, ob die Sparklines aus dem neuen Datenbereich zeilenweise oder spaltenweise dargestellt werden sollen. |
| locationRange | [CellArea](../../com.aspose.cells/cellarea) | Gibt an, wo die Sparklines platziert werden sollen. |

### setDisplayHidden(boolean value) {#setDisplayHidden-boolean-}
```
public void setDisplayHidden(boolean value)
```


Gibt an, ob Daten in ausgeblendeten Zeilen und Spalten angezeigt werden sollen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setFirstPointColor(CellsColor value) {#setFirstPointColor-com.aspose.cells.CellsColor-}
```
public void setFirstPointColor(CellsColor value)
```


Legt die Farbe des ersten Datenpunkts in der Sparkline‑Gruppe fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setHighPointColor(CellsColor value) {#setHighPointColor-com.aspose.cells.CellsColor-}
```
public void setHighPointColor(CellsColor value)
```


Legt die Farbe der höchsten Datenpunkte in der Sparkline‑Gruppe fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setHorizontalAxisColor(CellsColor value) {#setHorizontalAxisColor-com.aspose.cells.CellsColor-}
```
public void setHorizontalAxisColor(CellsColor value)
```


Legt die Farbe der horizontalen Achse in der Sparkline‑Gruppe fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setHorizontalAxisDateRange(String value) {#setHorizontalAxisDateRange-java.lang.String-}
```
public void setHorizontalAxisDateRange(String value)
```


Stellt den Bereich dar, der die Datumswerte für die Sparkline-Daten enthält.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setLastPointColor(CellsColor value) {#setLastPointColor-com.aspose.cells.CellsColor-}
```
public void setLastPointColor(CellsColor value)
```


Legt die Farbe des letzten Datenpunkts in der Sparkline‑Gruppe fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setLineWeight(double value) {#setLineWeight-double-}
```
public void setLineWeight(double value)
```


Legt die Linienstärke in jeder Linien‑Sparkline der Sparkline‑Gruppe fest, gemessen in Punkten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setLowPointColor(CellsColor value) {#setLowPointColor-com.aspose.cells.CellsColor-}
```
public void setLowPointColor(CellsColor value)
```


Legt die Farbe der niedrigsten Datenpunkte in der Sparkline‑Gruppe fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setMarkersColor(CellsColor value) {#setMarkersColor-com.aspose.cells.CellsColor-}
```
public void setMarkersColor(CellsColor value)
```


Legt die Farbe der Punkte in jeder Linien‑Sparkline der Sparkline‑Gruppe fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setNegativePointsColor(CellsColor value) {#setNegativePointsColor-com.aspose.cells.CellsColor-}
```
public void setNegativePointsColor(CellsColor value)
```


Legt die Farbe der negativen Werte in der Sparkline‑Gruppe fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setPlotEmptyCellsType(int value) {#setPlotEmptyCellsType-int-}
```
public void setPlotEmptyCellsType(int value)
```


Gibt an, wie leere Zellen dargestellt werden.

Siehe [PlotEmptyCellsType](../../com.aspose.cells/plotemptycellstype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setPlotRightToLeft(boolean value) {#setPlotRightToLeft-boolean-}
```
public void setPlotRightToLeft(boolean value)
```


Gibt an, ob die Plot-Daten von rechts nach links verlaufen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setPresetStyle(int value) {#setPresetStyle-int-}
```
public void setPresetStyle(int value)
```


Legt den voreingestellten Stiltyp der Sparkline‑Gruppe fest.

Siehe [SparklinePresetStyleType](../../com.aspose.cells/sparklinepresetstyletype).

**Remarks**

Wenn diese Eigenschaft gesetzt ist, werden diese Eigenschaften: SeriesColor,NegativePointsColor,HorizontalAxisColor,MarkersColor,FirstPointColor,LastPointColor,HighPointColor,LowPointColor überschrieben. Bitte setzen Sie zuerst die Eigenschaft und dann die anderen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setSeriesColor(CellsColor value) {#setSeriesColor-com.aspose.cells.CellsColor-}
```
public void setSeriesColor(CellsColor value)
```


Legt die Farbe der Sparklines in der Sparkline‑Gruppe fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setShowFirstPoint(boolean value) {#setShowFirstPoint-boolean-}
```
public void setShowFirstPoint(boolean value)
```


Gibt an, ob der erste Datenpunkt in der Sparkline-Gruppe hervorgehoben werden soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowHighPoint(boolean value) {#setShowHighPoint-boolean-}
```
public void setShowHighPoint(boolean value)
```


Gibt an, ob die höchsten Datenpunkte in der Sparkline‑Gruppe hervorgehoben werden sollen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowHorizontalAxis(boolean value) {#setShowHorizontalAxis-boolean-}
```
public void setShowHorizontalAxis(boolean value)
```


Gibt an, ob die horizontale Achse der Sparkline angezeigt werden soll. Die horizontale Achse erscheint, wenn die Sparkline Daten enthält, die die Nullachse überschreiten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowLastPoint(boolean value) {#setShowLastPoint-boolean-}
```
public void setShowLastPoint(boolean value)
```


Gibt an, ob der letzte Datenpunkt in der Sparkline‑Gruppe hervorgehoben werden soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowLowPoint(boolean value) {#setShowLowPoint-boolean-}
```
public void setShowLowPoint(boolean value)
```


Gibt an, ob die niedrigsten Datenpunkte in der Sparkline‑Gruppe hervorgehoben werden sollen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowMarkers(boolean value) {#setShowMarkers-boolean-}
```
public void setShowMarkers(boolean value)
```


Gibt an, ob jeder Punkt in jeder Linien‑Sparkline der Sparkline‑Gruppe hervorgehoben werden soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowNegativePoints(boolean value) {#setShowNegativePoints-boolean-}
```
public void setShowNegativePoints(boolean value)
```


Gibt an, ob die negativen Werte in der Sparkline‑Gruppe mit einer anderen Farbe oder Markierung hervorgehoben werden sollen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Gibt den Sparkline‑Typ der Sparkline‑Gruppe an.

Siehe [SparklineType](../../com.aspose.cells/sparklinetype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setVerticalAxisMaxValue(double value) {#setVerticalAxisMaxValue-double-}
```
public void setVerticalAxisMaxValue(double value)
```


Legt den benutzerdefinierten Maximalwert für die vertikale Achse fest.

**Remarks**

Wenn diese Eigenschaft gesetzt ist, wird [getVerticalAxisMaxValueType()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMaxValueType--) [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM) sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setVerticalAxisMaxValue(int type, double value) {#setVerticalAxisMaxValue-int-double-}
```
public void setVerticalAxisMaxValue(int type, double value)
```


Legt den benutzerdefinierten Maximalwert für die vertikale Sparkline‑Achse mit dem angegebenen Achsenwerttyp fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| type | int | [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype). Typ, der angibt, wie der maximale Achsenwert angewendet wird. |
| value | double | Benutzerdefinierter Maximalwert der vertikalen Achse. Wird ignoriert, wenn der Typ nicht [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM) ist. |

### setVerticalAxisMaxValueType(int value) {#setVerticalAxisMaxValueType-int-}
```
public void setVerticalAxisMaxValueType(int value)
```


Stellt den Typ des maximalen Achsenwerts für die vertikale Achse dar.

Siehe [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setVerticalAxisMinValue(double value) {#setVerticalAxisMinValue-double-}
```
public void setVerticalAxisMinValue(double value)
```


Legt den benutzerdefinierten Minimalwert für die vertikale Achse fest.

**Remarks**

Wenn diese Eigenschaft gesetzt ist, wird [getVerticalAxisMinValueType()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMinValueType--) [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM) sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setVerticalAxisMinValue(int type, double value) {#setVerticalAxisMinValue-int-double-}
```
public void setVerticalAxisMinValue(int type, double value)
```


Legt den benutzerdefinierten Minimalwert für die vertikale Achse der Sparkline mit dem angegebenen Achsenwerttyp fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| type | int | [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype). Typ, der angibt, wie der minimale Achsenwert angewendet wird. |
| value | double | Benutzerdefinierter Minimalwert der vertikalen Achse. Wird ignoriert, wenn der Typ nicht [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM) ist. |

### setVerticalAxisMinValueType(int value) {#setVerticalAxisMinValueType-int-}
```
public void setVerticalAxisMinValueType(int value)
```


Stellt den Typ des minimalen Achsenwerts für die vertikale Achse dar.

Siehe [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype).

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

