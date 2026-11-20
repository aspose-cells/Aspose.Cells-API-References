---
title: "ChartArea"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Kapselt das Objekt, das den Diagrammbereich im Arbeitsblatt darstellt."
type: docs
url: /de/java/com.aspose.cells/chartarea/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ChartFrame](../../com.aspose.cells/chartframe)
```
public class ChartArea extends ChartFrame
```

Kapselt das Objekt, das den Diagrammbereich im Arbeitsblatt darstellt.

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
         int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 15, 5);
 
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
 
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
         chart.getNSeries().add("A1:B3", true);
 
         //Getting Chart Area
         ChartArea chartArea = chart.getChartArea();
 
         //Setting the foreground color of the chart area
         chartArea.getArea().setForegroundColor(Color.getYellow());
 
         //Setting Chart Area Shadow
         chartArea.setShadow(true);
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArea()](#getArea--) | Liefert das [getArea()](../../com.aspose.cells/chartframe\#getArea--). |
| [getAutoScaleFont()](#getAutoScaleFont--) | True, wenn der Text im Objekt die Schriftgröße ändert, wenn die Objektgröße geändert wird. |
| [getBackground()](#getBackground--) | Liefert den Anzeigemodus des Hintergrunds. |
| [getBackgroundMode()](#getBackgroundMode--) | Liefert den Anzeigemodus des Hintergrunds. |
| [getBorder()](#getBorder--) | Liefert die [Line](../../com.aspose.cells/line). |
| [getChart()](#getChart--) | Liefert das Diagramm, zu dem dieses Objekt gehört. |
| [getClass()](#getClass--) |  |
| [getDefaultHeight()](#getDefaultHeight--) | Stellt die Höhe der Standardposition in Einheiten von 1/4000 des Diagrammbereichs dar. |
| [getDefaultHeightRatioToChart()](#getDefaultHeightRatioToChart--) | Stellt die Höhe der Standardposition in Einheiten des Bruchteils des Diagrammbereichs dar. |
| [getDefaultWidth()](#getDefaultWidth--) | Stellt die Breite der Standardposition in Einheiten von 1/4000 des Diagrammbereichs dar. |
| [getDefaultWidthRatioToChart()](#getDefaultWidthRatioToChart--) | Stellt die Breite der Standardposition in Einheiten des Bruchteils des Diagrammbereichs dar. |
| [getDefaultX()](#getDefaultX--) | Stellt das x der Standardposition in Einheiten von 1/4000 des Diagrammbereichs dar. |
| [getDefaultXRatioToChart()](#getDefaultXRatioToChart--) | Stellt das x der Standardposition in Einheiten des Bruchteils des Diagrammbereichs dar. |
| [getDefaultY()](#getDefaultY--) | Stellt das y der Standardposition in Einheiten von 1/4000 des Diagrammbereichs dar. |
| [getDefaultYRatioToChart()](#getDefaultYRatioToChart--) | Stellt das y der Standardposition in Einheiten des Bruchteils des Diagrammbereichs dar. |
| [getFont()](#getFont--) | Ermittelt ein [getFont()](../../com.aspose.cells/chartarea\#getFont--)‑Objekt des angegebenen ChartArea‑Objekts. |
| [getHeight()](#getHeight--) | Ermittelt den vertikalen Versatz von seiner unteren\\u9225\\u6186ight‑Eckzeile, in Einheiten von 1/4000 des Diagrammbereichs. |
| [getHeightPixel()](#getHeightPixel--) | Ermittelt die Höhe des Rahmens in Pixeln. |
| [getHeightRatioToChart()](#getHeightRatioToChart--) | Ermittelt den vertikalen Versatz von seiner unteren rechten Eckzeile, in Verhältnis‑Einheiten des Diagrammbereichs. |
| [getShadow()](#getShadow--) | Wahr, wenn der Rahmen einen Schatten hat. |
| [getShapeProperties()](#getShapeProperties--) | Ermittelt das [getShapeProperties()](../../com.aspose.cells/chartframe\#getShapeProperties--) Objekt. |
| [getTextFont()](#getTextFont--) | Ermittelt ein [getFont()](../../com.aspose.cells/chartframe\#getFont--) Objekt des angegebenen ChartFrame-Objekts. |
| [getTextOptions()](#getTextOptions--) | Ermittelt die Optionen des Textes. |
| [getWidth()](#getWidth--) | Ermittelt den horizontalen Versatz von seiner unteren rechten Eckspalte, in Einheiten von 1/4000 des Diagrammbereichs. |
| [getWidthPixel()](#getWidthPixel--) | Ermittelt die Breite des Rahmens in Pixeln. |
| [getWidthRatioToChart()](#getWidthRatioToChart--) | Ermittelt den horizontalen Versatz von seiner unteren rechten Eckspalte, in Verhältnis‑Einheiten des Diagrammbereichs. |
| [getX()](#getX--) | Ermittelt den horizontalen Versatz von seiner oberen linken Eckspalte, in Einheiten von 1/4000 des Diagrammbereichs. |
| [getXPixel()](#getXPixel--) | Ermittelt die X‑Koordinate der oberen linken Ecke in Pixeln. |
| [getXRatioToChart()](#getXRatioToChart--) | Ermittelt den horizontalen Versatz von der oberen linken Eckspalte, als Verhältnis des Diagrammbereichs. |
| [getY()](#getY--) | Liest oder setzt den vertikalen Versatz von seiner oberen linken Zeile, in Einheiten von 1/4000 des Diagrammbereichs. |
| [getYPixel()](#getYPixel--) | Ermittelt die Y‑Koordinate der oberen linken Ecke in Pixeln. |
| [getYRatioToChart()](#getYRatioToChart--) | Liest oder setzt den vertikalen Versatz von seiner oberen linken Zeile, als Verhältnis zum Diagrammbereich. |
| [hashCode()](#hashCode--) |  |
| [isAutomaticSize()](#isAutomaticSize--) | Gibt an, ob der Diagrammrahmen automatisch dimensioniert ist. |
| [isDefaultPosBeSet()](#isDefaultPosBeSet--) | Gibt an, ob die Standardposition (DefaultX, DefaultY, DefaultWidth und DefaultHeight) festgelegt ist. |
| [isInnerMode()](#isInnerMode--) | Gibt an, ob die Größe des Plot‑Bereichs die Tick‑Markierungen und die Achsenbeschriftungen einschließt. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoScaleFont(boolean value)](#setAutoScaleFont-boolean-) | True, wenn der Text im Objekt die Schriftgröße ändert, wenn die Objektgröße geändert wird. |
| [setAutomaticSize(boolean value)](#setAutomaticSize-boolean-) | Gibt an, ob der Diagrammrahmen automatisch dimensioniert ist. |
| [setBackground(int value)](#setBackground-int-) | Legt den Anzeigemodus des Hintergrunds fest. |
| [setBackgroundMode(int value)](#setBackgroundMode-int-) | Legt den Anzeigemodus des Hintergrunds fest. |
| [setHeight(int value)](#setHeight-int-) | Setzt den vertikalen Versatz von seiner unteren\\u9225\\u6186ight Ecke Zeile, in Einheiten von 1/4000 des Diagrammbereichs. |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Legt die Höhe des Rahmens in Pixeln fest. |
| [setHeightRatioToChart(double value)](#setHeightRatioToChart-double-) | Setzt den vertikalen Versatz von seiner unteren rechten Ecke Zeile, als Verhältnis zum Diagrammbereich. |
| [setInnerMode(boolean value)](#setInnerMode-boolean-) | Gibt an, ob die Größe des Plot‑Bereichs die Tick‑Markierungen und die Achsenbeschriftungen einschließt. |
| [setPositionAuto()](#setPositionAuto--) | Setzt die Position des Rahmens auf automatisch |
| [setShadow(boolean value)](#setShadow-boolean-) | Wahr, wenn der Rahmen einen Schatten hat. |
| [setWidth(int value)](#setWidth-int-) | Setzt den horizontalen Versatz von seiner unteren rechten Ecke Spalte, in Einheiten von 1/4000 des Diagrammbereichs. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | Legt die Breite des Rahmens in Pixeln fest. |
| [setWidthRatioToChart(double value)](#setWidthRatioToChart-double-) | Setzt den horizontalen Versatz von seiner unteren rechten Ecke Spalte, als Verhältnis zum Diagrammbereich. |
| [setX(int value)](#setX-int-) | Setzt den horizontalen Versatz von seiner oberen linken Ecke Spalte, in Einheiten von 1/4000 des Diagrammbereichs. |
| [setXPixel(int value)](#setXPixel-int-) | Legt die X‑Koordinate der oberen linken Ecke in Pixeln fest. |
| [setXRatioToChart(double value)](#setXRatioToChart-double-) | Setzt den horizontalen Versatz von der oberen linken Ecke Spalte, als Verhältnis zum Diagrammbereich. |
| [setY(int value)](#setY-int-) | Liest oder setzt den vertikalen Versatz von seiner oberen linken Zeile, in Einheiten von 1/4000 des Diagrammbereichs. |
| [setYPixel(int value)](#setYPixel-int-) | Legt die Y‑Koordinate der oberen linken Ecke in Pixeln fest. |
| [setYRatioToChart(double value)](#setYRatioToChart-double-) | Liest oder setzt den vertikalen Versatz von seiner oberen linken Zeile, als Verhältnis zum Diagrammbereich. |
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
### getArea() {#getArea--}
```
public Area getArea()
```


Liefert das [getArea()](../../com.aspose.cells/chartframe\#getArea--).

**Returns:**
[Area](../../com.aspose.cells/area)
### getAutoScaleFont() {#getAutoScaleFont--}
```
public boolean getAutoScaleFont()
```


True, wenn der Text im Objekt die Schriftgröße ändert, wenn sich die Objektgröße ändert. Der Standardwert ist True.

**Returns:**
boolean
### getBackground() {#getBackground--}
```
public int getBackground()
```


Ermittelt den Anzeigemodus des Hintergrunds. Diese Eigenschaft ist nur in Excel 2003 oder früheren Versionen gültig.

Siehe [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft ChartFrame.Area.FillFormat.FillType. Beispiel: Wenn Sie den BackgroundMode auf Opaque setzen müssen, können Sie den folgenden Code verwenden: `Area.FillFormat.FillType = FillType.Solid;` `Area.FillFormat.SolidFill.Color = Color.Red;` Diese Eigenschaft wird 12 Monate später, seit JANUARY 2012, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Returns:**
int
### getBackgroundMode() {#getBackgroundMode--}
```
public int getBackgroundMode()
```


Ermittelt den Anzeigemodus des Hintergrunds. Diese Eigenschaft ist nur in Excel 2003 oder früheren Versionen gültig.

Siehe [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft ChartFrame.Area.FillFormat.FillType. Beispiel: Wenn Sie den BackgroundMode auf Opaque setzen müssen, können Sie den folgenden Code verwenden: `Area.FillFormat.FillType = FillType.Solid;` `Area.FillFormat.SolidFill.Color = Color.Red;` Diese Eigenschaft wird 12 Monate später, seit February 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Returns:**
int
### getBorder() {#getBorder--}
```
public Line getBorder()
```


Liefert die [Line](../../com.aspose.cells/line).

**Returns:**
[Line](../../com.aspose.cells/line)
### getChart() {#getChart--}
```
public Chart getChart()
```


Liefert das Diagramm, zu dem dieses Objekt gehört.

**Returns:**
[Chart](../../com.aspose.cells/chart)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDefaultHeight() {#getDefaultHeight--}
```
public int getDefaultHeight()
```


Stellt die Höhe der Standardposition in Einheiten von 1/4000 des Diagrammbereichs dar.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft ChartFrame.DefaultHeightRatioToChart. `DefaultHeight = (int)(DefaultHeightRatioToChart \* 4000);` Diese Eigenschaft wird 12 Monate später, seit February 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Returns:**
int
### getDefaultHeightRatioToChart() {#getDefaultHeightRatioToChart--}
```
public double getDefaultHeightRatioToChart()
```


Stellt die Höhe der Standardposition in Einheiten des Bruchteils des Diagrammbereichs dar.

**Returns:**
double
### getDefaultWidth() {#getDefaultWidth--}
```
public int getDefaultWidth()
```


Stellt die Breite der Standardposition in Einheiten von 1/4000 des Diagrammbereichs dar.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft ChartFrame.DefaultWidthRatioToChart. `DefaultWidth = (int)(DefaultWidthRatioToChart \* 4000);` Diese Eigenschaft wird 12 Monate später, seit February 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Returns:**
int
### getDefaultWidthRatioToChart() {#getDefaultWidthRatioToChart--}
```
public double getDefaultWidthRatioToChart()
```


Stellt die Breite der Standardposition in Einheiten des Bruchteils des Diagrammbereichs dar.

**Returns:**
double
### getDefaultX() {#getDefaultX--}
```
public int getDefaultX()
```


Stellt das x der Standardposition in Einheiten von 1/4000 des Diagrammbereichs dar.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft ChartFrame.DefaultXRatioToChart. `DefaultX = (int)(DefaultXRatioToChart \* 4000);` Diese Eigenschaft wird 12 Monate später, seit February 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Returns:**
int
### getDefaultXRatioToChart() {#getDefaultXRatioToChart--}
```
public double getDefaultXRatioToChart()
```


Stellt das x der Standardposition in Einheiten des Bruchteils des Diagrammbereichs dar.

**Returns:**
double
### getDefaultY() {#getDefaultY--}
```
public int getDefaultY()
```


Stellt das y der Standardposition in Einheiten von 1/4000 des Diagrammbereichs dar.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die Eigenschaft ChartFrame.DefaultYRatioToChart. DefaultY = (int)(DefaultYRatioToChart \* 4000); Diese Eigenschaft wird 12 Monate später, seit Februar 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Returns:**
int
### getDefaultYRatioToChart() {#getDefaultYRatioToChart--}
```
public double getDefaultYRatioToChart()
```


Stellt das y der Standardposition in Einheiten des Bruchteils des Diagrammbereichs dar.

**Returns:**
double
### getFont() {#getFont--}
```
public Font getFont()
```


Ermittelt ein [getFont()](../../com.aspose.cells/chartarea\#getFont--)‑Objekt des angegebenen ChartArea‑Objekts.

**Returns:**
[Font](../../com.aspose.cells/font)
### getHeight() {#getHeight--}
```
public int getHeight()
```


Ermittelt den vertikalen Versatz von seiner unteren\\u9225\\u6186ight‑Eckzeile, in Einheiten von 1/4000 des Diagrammbereichs.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die ChartArea.HeightRatioToChart property. Höhe = HeightRatioToChart \* 4000. Diese Eigenschaft wird 12 Monate später, seit Februar 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Returns:**
int
### getHeightPixel() {#getHeightPixel--}
```
public int getHeightPixel()
```


Ermittelt die Höhe des Rahmens in Pixeln.

**Returns:**
int
### getHeightRatioToChart() {#getHeightRatioToChart--}
```
public double getHeightRatioToChart()
```


Ermittelt den vertikalen Versatz von seiner unteren rechten Eckzeile, in Verhältnis‑Einheiten des Diagrammbereichs.

**Returns:**
double
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


Wahr, wenn der Rahmen einen Schatten hat.

**Remarks**

Nur für Diagramme in xls-Dateien.

**Returns:**
boolean
### getShapeProperties() {#getShapeProperties--}
```
public ShapePropertyCollection getShapeProperties()
```


Ermittelt das [getShapeProperties()](../../com.aspose.cells/chartframe\#getShapeProperties--) Objekt.

**Returns:**
[ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection)
### getTextFont() {#getTextFont--}
```
public Font getTextFont()
```


Ermittelt ein [getFont()](../../com.aspose.cells/chartframe\#getFont--) Objekt des angegebenen ChartFrame-Objekts.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft ChartFrame.Font. Diese Eigenschaft wird 12 Monate später, seit JANUAR 2012, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Returns:**
[Font](../../com.aspose.cells/font)
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


Ermittelt die Optionen des Textes.

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getWidth() {#getWidth--}
```
public int getWidth()
```


Ermittelt den horizontalen Versatz von seiner unteren rechten Eckspalte, in Einheiten von 1/4000 des Diagrammbereichs.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die ChartArea.WidthRatioToChart property. Breite = WidthRatioToChart \* 4000. Diese Eigenschaft wird 12 Monate später, seit Februar 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Returns:**
int
### getWidthPixel() {#getWidthPixel--}
```
public int getWidthPixel()
```


Ermittelt die Breite des Rahmens in Pixeln.

**Returns:**
int
### getWidthRatioToChart() {#getWidthRatioToChart--}
```
public double getWidthRatioToChart()
```


Ermittelt den horizontalen Versatz von seiner unteren rechten Eckspalte, in Verhältnis‑Einheiten des Diagrammbereichs.

**Returns:**
double
### getX() {#getX--}
```
public int getX()
```


Ermittelt den horizontalen Versatz von seiner oberen linken Eckspalte, in Einheiten von 1/4000 des Diagrammbereichs.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die ChartArea.XRatioToChart property. X = XRatioToChart \* 4000. Diese Eigenschaft wird 12 Monate später, seit Februar 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Returns:**
int
### getXPixel() {#getXPixel--}
```
public int getXPixel()
```


Ermittelt die X‑Koordinate der oberen linken Ecke in Pixeln.

**Returns:**
int
### getXRatioToChart() {#getXRatioToChart--}
```
public double getXRatioToChart()
```


Ermittelt den horizontalen Versatz von der oberen linken Eckspalte, als Verhältnis des Diagrammbereichs.

**Returns:**
double
### getY() {#getY--}
```
public int getY()
```


Liest oder setzt den vertikalen Versatz von seiner oberen linken Zeile, in Einheiten von 1/4000 des Diagrammbereichs.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die ChartArea.YRatioToChart property. Y = YRatioToChart \* 4000; Diese Eigenschaft wird 12 Monate später, seit Februar 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Returns:**
int
### getYPixel() {#getYPixel--}
```
public int getYPixel()
```


Ermittelt die Y‑Koordinate der oberen linken Ecke in Pixeln.

**Returns:**
int
### getYRatioToChart() {#getYRatioToChart--}
```
public double getYRatioToChart()
```


Liest oder setzt den vertikalen Versatz von seiner oberen linken Zeile, als Verhältnis zum Diagrammbereich.

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutomaticSize() {#isAutomaticSize--}
```
public boolean isAutomaticSize()
```


Gibt an, ob der Diagrammrahmen automatisch dimensioniert ist.

**Returns:**
boolean
### isDefaultPosBeSet() {#isDefaultPosBeSet--}
```
public boolean isDefaultPosBeSet()
```


Gibt an, ob die Standardposition (DefaultX, DefaultY, DefaultWidth und DefaultHeight) festgelegt ist.

**Returns:**
boolean
### isInnerMode() {#isInnerMode--}
```
public boolean isInnerMode()
```


Gibt an, ob die Größe des Plot-Bereichs die Tick-Markierungen und Achsenbeschriftungen einschließt. False bedeutet, dass die Größe den Plot-Bereich, die Tick-Markierungen und die Achsenbeschriftungen bestimmen soll.

**Remarks**

Nur für Xlsx-Dateien.

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




### setAutoScaleFont(boolean value) {#setAutoScaleFont-boolean-}
```
public void setAutoScaleFont(boolean value)
```


True, wenn der Text im Objekt die Schriftgröße ändert, wenn sich die Objektgröße ändert. Der Standardwert ist True.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAutomaticSize(boolean value) {#setAutomaticSize-boolean-}
```
public void setAutomaticSize(boolean value)
```


Gibt an, ob der Diagrammrahmen automatisch dimensioniert ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setBackground(int value) {#setBackground-int-}
```
public void setBackground(int value)
```


Legt den Anzeigemodus des Hintergrunds fest. Diese Eigenschaft ist nur in Excel 2003 oder früheren Versionen gültig.

Siehe [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft ChartFrame.Area.FillFormat.FillType. Beispiel: Wenn Sie den BackgroundMode auf Opaque setzen müssen, können Sie den folgenden Code verwenden: `Area.FillFormat.FillType = FillType.Solid;` `Area.FillFormat.SolidFill.Color = Color.Red;` Diese Eigenschaft wird 12 Monate später, seit JANUARY 2012, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setBackgroundMode(int value) {#setBackgroundMode-int-}
```
public void setBackgroundMode(int value)
```


Legt den Anzeigemodus des Hintergrunds fest. Diese Eigenschaft ist nur in Excel 2003 oder früheren Versionen gültig.

Siehe [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft ChartFrame.Area.FillFormat.FillType. Beispiel: Wenn Sie den BackgroundMode auf Opaque setzen müssen, können Sie den folgenden Code verwenden: `Area.FillFormat.FillType = FillType.Solid;` `Area.FillFormat.SolidFill.Color = Color.Red;` Diese Eigenschaft wird 12 Monate später, seit February 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setHeight(int value) {#setHeight-int-}
```
public void setHeight(int value)
```


Setzt den vertikalen Versatz von seiner unteren\\u9225\\u6186ight Ecke Zeile, in Einheiten von 1/4000 des Diagrammbereichs.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die ChartArea.HeightRatioToChart property. Höhe = HeightRatioToChart \* 4000. Diese Eigenschaft wird 12 Monate später, seit Februar 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setHeightPixel(int value) {#setHeightPixel-int-}
```
public void setHeightPixel(int value)
```


Legt die Höhe des Rahmens in Pixeln fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setHeightRatioToChart(double value) {#setHeightRatioToChart-double-}
```
public void setHeightRatioToChart(double value)
```


Setzt den vertikalen Versatz von seiner unteren rechten Ecke Zeile, als Verhältnis zum Diagrammbereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setInnerMode(boolean value) {#setInnerMode-boolean-}
```
public void setInnerMode(boolean value)
```


Gibt an, ob die Größe des Plot-Bereichs die Tick-Markierungen und Achsenbeschriftungen einschließt. False bedeutet, dass die Größe den Plot-Bereich, die Tick-Markierungen und die Achsenbeschriftungen bestimmen soll.

**Remarks**

Nur für Xlsx-Dateien.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setPositionAuto() {#setPositionAuto--}
```
public void setPositionAuto()
```


Setzt die Position des Rahmens auf automatisch

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


Wahr, wenn der Rahmen einen Schatten hat.

**Remarks**

Nur für Diagramme in xls-Dateien.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setWidth(int value) {#setWidth-int-}
```
public void setWidth(int value)
```


Setzt den horizontalen Versatz von seiner unteren rechten Ecke Spalte, in Einheiten von 1/4000 des Diagrammbereichs.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die ChartArea.WidthRatioToChart property. Breite = WidthRatioToChart \* 4000. Diese Eigenschaft wird 12 Monate später, seit Februar 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setWidthPixel(int value) {#setWidthPixel-int-}
```
public void setWidthPixel(int value)
```


Legt die Breite des Rahmens in Pixeln fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setWidthRatioToChart(double value) {#setWidthRatioToChart-double-}
```
public void setWidthRatioToChart(double value)
```


Setzt den horizontalen Versatz von seiner unteren rechten Ecke Spalte, als Verhältnis zum Diagrammbereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setX(int value) {#setX-int-}
```
public void setX(int value)
```


Setzt den horizontalen Versatz von seiner oberen linken Ecke Spalte, in Einheiten von 1/4000 des Diagrammbereichs.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die ChartArea.XRatioToChart property. X = XRatioToChart \* 4000. Diese Eigenschaft wird 12 Monate später, seit Februar 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setXPixel(int value) {#setXPixel-int-}
```
public void setXPixel(int value)
```


Legt die X‑Koordinate der oberen linken Ecke in Pixeln fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setXRatioToChart(double value) {#setXRatioToChart-double-}
```
public void setXRatioToChart(double value)
```


Setzt den horizontalen Versatz von der oberen linken Ecke Spalte, als Verhältnis zum Diagrammbereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setY(int value) {#setY-int-}
```
public void setY(int value)
```


Liest oder setzt den vertikalen Versatz von seiner oberen linken Zeile, in Einheiten von 1/4000 des Diagrammbereichs.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die ChartArea.YRatioToChart property. Y = YRatioToChart \* 4000; Diese Eigenschaft wird 12 Monate später, seit Februar 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setYPixel(int value) {#setYPixel-int-}
```
public void setYPixel(int value)
```


Legt die Y‑Koordinate der oberen linken Ecke in Pixeln fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setYRatioToChart(double value) {#setYRatioToChart-double-}
```
public void setYRatioToChart(double value)
```


Liest oder setzt den vertikalen Versatz von seiner oberen linken Zeile, als Verhältnis zum Diagrammbereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

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

