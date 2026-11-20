---
title: "Legende"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Kapselt das Objekt, das die Diagrammlegende darstellt."
type: docs
url: /de/java/com.aspose.cells/legend/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ChartFrame](../../com.aspose.cells/chartframe), [com.aspose.cells.ChartTextFrame](../../com.aspose.cells/charttextframe)
```
public class Legend extends ChartTextFrame
```

Kapselt das Objekt, das die Diagrammlegende darstellt.

**Example**

```
         Workbook workbook = new Workbook();
         	Worksheet sheet = workbook.getWorksheets().get(0);
 
         	Cells cells = sheet.getCells();
         	cells.get(0,1).putValue("Income");
         	cells.get(1,0).putValue("Company A");
         	cells.get(2,0).putValue("Company B");
         	cells.get(3,0).putValue("Company C");
         	cells.get(1,1).putValue(10000);
         	cells.get(2,1).putValue(20000);
         	cells.get(3,1).putValue(30000);
 
         	int chartIndex = sheet.getCharts().add(ChartType.COLUMN, 9, 9, 21, 15);
         	Chart chart = sheet.getCharts().get(chartIndex);
         	chart.setChartDataRange("A1:B4", true);
         //Set Legend's width and height
         Legend legend = chart.getLegend();
 
         //Legend is at right side of chart by default.
         //If the legend is at left or right side of the chart, setting Legend.X property will not take effect.
         //If the legend is at top or bottom side of the chart, setting Legend.Y property will not take effect.
         legend.setY(1500);
         legend.setWidth(50);
         legend.setHeight(50); 
         //Set legend's position
         legend.setPosition(LegendPositionType.LEFT);
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [characters(int startIndex, int length)](#characters-int-int-) | Gibt ein Characters‑Objekt zurück, das einen Zeichenbereich im Text darstellt. |
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
| [getDirectionType()](#getDirectionType--) | Ermittelt die Schreibrichtung. |
| [getFont()](#getFont--) | Ermittelt ein [getFont()](../../com.aspose.cells/chartframe\#getFont--) Objekt des angegebenen ChartFrame-Objekts. |
| [getHeight()](#getHeight--) | Ermittelt die Höhe des Rahmens in Einheiten von 1/4000 des Diagrammbereichs. |
| [getHeightPixel()](#getHeightPixel--) | Ermittelt die Höhe des Rahmens in Pixeln. |
| [getHeightRatioToChart()](#getHeightRatioToChart--) | Ermittelt die Höhe des Rahmens in Einheiten des Verhältnisses des Diagrammbereichs. |
| [getLegendEntries()](#getLegendEntries--) | Ruft eine Sammlung aller LegendEntry-Objekte in der angegebenen Diagrammlegende ab. |
| [getLegendEntriesLabels()](#getLegendEntriesLabels--) | Ruft die Bezeichnungen der Legendeinträge ab, nachdem die Methode Chart.Calculate() aufgerufen wurde. |
| [getLegendLabels()](#getLegendLabels--) | Ruft die Bezeichnungen der Legendeinträge ab, nachdem Chart.Calculate() aufgerufen wurde. |
| [getLinkedSource()](#getLinkedSource--) | Ermittelt eine Referenz auf das Arbeitsblatt. |
| [getPosition()](#getPosition--) | Ruft den Legendenpositionstyp ab. |
| [getReadingOrder()](#getReadingOrder--) | Stellt die Lesereihenfolge des Textes dar. |
| [getRotationAngle()](#getRotationAngle--) | Stellt den Drehwinkel des Textes dar. |
| [getShadow()](#getShadow--) | Wahr, wenn der Rahmen einen Schatten hat. |
| [getShapeProperties()](#getShapeProperties--) | Ermittelt das [getShapeProperties()](../../com.aspose.cells/chartframe\#getShapeProperties--) Objekt. |
| [getText()](#getText--) | Ermittelt den Text des Titels eines Rahmens. |
| [getTextDirection()](#getTextDirection--) | Stellt die Lesereihenfolge des Textes dar. |
| [getTextFont()](#getTextFont--) | Ermittelt ein [getFont()](../../com.aspose.cells/chartframe\#getFont--) Objekt des angegebenen ChartFrame-Objekts. |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--) | Ermittelt die horizontale Ausrichtung des Textes. |
| [getTextOptions()](#getTextOptions--) | Ermittelt die Optionen des Textes. |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--) | Ermittelt die vertikale Ausrichtung des Textes. |
| [getWidth()](#getWidth--) | Ermittelt die Breite des Rahmens in Einheiten von 1/4000 des Diagrammbereichs. |
| [getWidthPixel()](#getWidthPixel--) | Ermittelt die Breite des Rahmens in Pixeln. |
| [getWidthRatioToChart()](#getWidthRatioToChart--) | Ermittelt die Breite des Rahmens in Einheiten des Verhältnisses zum Diagrammbereich. |
| [getX()](#getX--) | Liefert die x‑Koordinate der oberen linken Ecke in Einheiten von 1/4000 des Diagrammbereichs. |
| [getXPixel()](#getXPixel--) | Ermittelt die X‑Koordinate der oberen linken Ecke in Pixeln. |
| [getXRatioToChart()](#getXRatioToChart--) | Liefert die x‑Koordinate der oberen linken Ecke in Einheiten des Verhältnisses des Diagrammbereichs. |
| [getY()](#getY--) | Ermittelt die Y‑Koordinate der oberen linken Ecke in Einheiten von 1/4000 des Diagrammbereichs. |
| [getYPixel()](#getYPixel--) | Ermittelt die Y‑Koordinate der oberen linken Ecke in Pixeln. |
| [getYRatioToChart()](#getYRatioToChart--) | Liefert die y‑Koordinate der oberen linken Ecke in Einheiten des Verhältnisses des Diagrammbereichs. |
| [hashCode()](#hashCode--) |  |
| [isAutoText()](#isAutoText--) | Gibt an, dass der Text automatisch generiert wird. |
| [isAutomaticRotation()](#isAutomaticRotation--) | Gibt an, ob der Text des Diagramms automatisch gedreht wird. |
| [isAutomaticSize()](#isAutomaticSize--) | Gibt an, ob der Diagrammrahmen automatisch dimensioniert ist. |
| [isDefaultPosBeSet()](#isDefaultPosBeSet--) | Gibt an, ob die Standardposition (DefaultX, DefaultY, DefaultWidth und DefaultHeight) festgelegt ist. |
| [isDeleted()](#isDeleted--) | Gibt an, ob diese Datenbeschriftung gelöscht ist. |
| [isInnerMode()](#isInnerMode--) | Gibt an, ob die Größe des Plot‑Bereichs die Tick‑Markierungen und die Achsenbeschriftungen einschließt. |
| [isOverLay()](#isOverLay--) | Ruft ab, ob die Legende angezeigt wird, ohne das Diagramm zu überlappen. |
| [isResizeShapeToFitText()](#isResizeShapeToFitText--) | Ermittelt, ob eine Form automatisch angepasst werden soll, um den darin beschriebenen Text vollständig zu enthalten. |
| [isTextWrapped()](#isTextWrapped--) | Ermittelt einen Wert, der angibt, ob der Text umgebrochen ist. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoScaleFont(boolean value)](#setAutoScaleFont-boolean-) | True, wenn der Text im Objekt die Schriftgröße ändert, wenn die Objektgröße geändert wird. |
| [setAutoText(boolean value)](#setAutoText-boolean-) | Gibt an, dass der Text automatisch generiert wird. |
| [setAutomaticSize(boolean value)](#setAutomaticSize-boolean-) | Gibt an, ob der Diagrammrahmen automatisch dimensioniert ist. |
| [setBackground(int value)](#setBackground-int-) | Legt den Anzeigemodus des Hintergrunds fest. |
| [setBackgroundMode(int value)](#setBackgroundMode-int-) | Legt den Anzeigemodus des Hintergrunds fest. |
| [setDeleted(boolean value)](#setDeleted-boolean-) | Gibt an, ob diese Datenbeschriftung gelöscht ist. |
| [setDirectionType(int value)](#setDirectionType-int-) | Legt die Textausrichtung fest. |
| [setHeight(int value)](#setHeight-int-) | Legt die Höhe des Rahmens in Einheiten von 1/4000 des Diagrammbereichs fest. |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Legt die Höhe des Rahmens in Pixeln fest. |
| [setHeightRatioToChart(double value)](#setHeightRatioToChart-double-) | Legt die Höhe des Rahmens in Einheiten des Verhältnisses zum Diagrammbereich fest. |
| [setInnerMode(boolean value)](#setInnerMode-boolean-) | Gibt an, ob die Größe des Plot‑Bereichs die Tick‑Markierungen und die Achsenbeschriftungen einschließt. |
| [setLinkedSource(String value)](#setLinkedSource-java.lang.String-) | Legt eine Referenz auf das Arbeitsblatt fest. |
| [setOverLay(boolean value)](#setOverLay-boolean-) | Legt fest, ob die Legende angezeigt wird, ohne das Diagramm zu überlappen. |
| [setPosition(int value)](#setPosition-int-) | Legt den Legendenpositionstyp fest. |
| [setPositionAuto()](#setPositionAuto--) | Setzt die Position des Rahmens auf automatisch |
| [setReadingOrder(int value)](#setReadingOrder-int-) | Stellt die Lesereihenfolge des Textes dar. |
| [setResizeShapeToFitText(boolean value)](#setResizeShapeToFitText-boolean-) | Legt fest, ob eine Form automatisch angepasst werden soll, um den darin beschriebenen Text vollständig zu enthalten. |
| [setRotationAngle(int value)](#setRotationAngle-int-) | Stellt den Drehwinkel des Textes dar. |
| [setShadow(boolean value)](#setShadow-boolean-) | Wahr, wenn der Rahmen einen Schatten hat. |
| [setText(String value)](#setText-java.lang.String-) | Legt den Text des Titels eines Rahmens fest. |
| [setTextDirection(int value)](#setTextDirection-int-) | Stellt die Lesereihenfolge des Textes dar. |
| [setTextHorizontalAlignment(int value)](#setTextHorizontalAlignment-int-) | Legt die horizontale Ausrichtung des Textes fest. |
| [setTextVerticalAlignment(int value)](#setTextVerticalAlignment-int-) | Legt die vertikale Ausrichtung des Textes fest. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Legt einen Wert fest, der angibt, ob der Text umgebrochen wird. |
| [setWidth(int value)](#setWidth-int-) | Legt die Breite des Rahmens in Einheiten von 1/4000 des Diagrammbereichs fest. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | Legt die Breite des Rahmens in Pixeln fest. |
| [setWidthRatioToChart(double value)](#setWidthRatioToChart-double-) | Legt die Breite des Rahmens im Verhältnis zum Diagrammbereich fest. |
| [setX(int value)](#setX-int-) | Setzt die x‑Koordinate der oberen linken Ecke in Einheiten von 1/4000 des Diagrammbereichs. |
| [setXPixel(int value)](#setXPixel-int-) | Legt die X‑Koordinate der oberen linken Ecke in Pixeln fest. |
| [setXRatioToChart(double value)](#setXRatioToChart-double-) | Setzt die x‑Koordinate der oberen linken Ecke in Einheiten des Verhältnisses des Diagrammbereichs. |
| [setY(int value)](#setY-int-) | Legt die Y‑Koordinate der oberen linken Ecke in Einheiten von 1/4000 des Diagrammbereichs fest. |
| [setYPixel(int value)](#setYPixel-int-) | Legt die Y‑Koordinate der oberen linken Ecke in Pixeln fest. |
| [setYRatioToChart(double value)](#setYRatioToChart-double-) | Setzt die y‑Koordinate der oberen linken Ecke in Einheiten des Verhältnisses des Diagrammbereichs. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### characters(int startIndex, int length) {#characters-int-int-}
```
public FontSetting characters(int startIndex, int length)
```


Gibt ein Characters‑Objekt zurück, das einen Zeichenbereich im Text darstellt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startIndex | int | Der Index des Beginns des Zeichens. |
| length | int | Die Anzahl der Zeichen. |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - Characters object.
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
### getDirectionType() {#getDirectionType--}
```
public int getDirectionType()
```


Ermittelt die Schreibrichtung.

Siehe [ChartTextDirectionType](../../com.aspose.cells/charttextdirectiontype).

**Returns:**
int
### getFont() {#getFont--}
```
public Font getFont()
```


Ermittelt ein [getFont()](../../com.aspose.cells/chartframe\#getFont--) Objekt des angegebenen ChartFrame-Objekts.

**Returns:**
[Font](../../com.aspose.cells/font)
### getHeight() {#getHeight--}
```
public int getHeight()
```


Ermittelt die Höhe des Rahmens in Einheiten von 1/4000 des Diagrammbereichs.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die Eigenschaft ChartFrame.HeightRatioToChart. Height = HeightRatioToChart \* 4000. Diese Eigenschaft wird 12 Monate später, seit Februar 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

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


Ermittelt die Höhe des Rahmens in Einheiten des Verhältnisses des Diagrammbereichs.

**Remarks**

Dies ist ein Bruchwert, sein gültiger Bereich liegt zwischen 0-1. Wie konvertiert man Verhältnis-Einheiten in Pixel? HeightPixel = HeightRatioToChart \* Chart.ChartObject.Height;

**Returns:**
double
### getLegendEntries() {#getLegendEntries--}
```
public LegendEntryCollection getLegendEntries()
```


Ruft eine Sammlung aller LegendEntry-Objekte in der angegebenen Diagrammlegende ab. Das Festlegen der Legendeinträge für ein Oberflächendiagramm wird nicht unterstützt. Daher wird null zurückgegeben, wenn der Diagrammtyp ein Oberflächendiagramm ist.

**Returns:**
[LegendEntryCollection](../../com.aspose.cells/legendentrycollection)
### getLegendEntriesLabels() {#getLegendEntriesLabels--}
```
public ArrayList getLegendEntriesLabels()
```


Ruft die Bezeichnungen der Legendeinträge ab, nachdem die Methode Chart.Calculate() aufgerufen wurde.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode Legend.GetLegendLabels. Diese Eigenschaft wird 12 Monate nach November 2023 entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Returns:**
java.util.ArrayList
### getLegendLabels() {#getLegendLabels--}
```
public String[] getLegendLabels()
```


Ruft die Bezeichnungen der Legendeinträge ab, nachdem Chart.Calculate() aufgerufen wurde.

**Returns:**
java.lang.String[]
### getLinkedSource() {#getLinkedSource--}
```
public String getLinkedSource()
```


Ermittelt eine Referenz auf das Arbeitsblatt.

**Returns:**
java.lang.String
### getPosition() {#getPosition--}
```
public int getPosition()
```


Ruft den Legendenpositionstyp ab.

Siehe [LegendPositionType](../../com.aspose.cells/legendpositiontype).

**Remarks**


Standardposition ist rechts.

Wenn die Legende sich auf der linken oder rechten Seite des Diagramms befindet, hat das Setzen der Eigenschaft Legend.X keine Wirkung.

Wenn die Legende sich oben oder unten am Diagramm befindet, hat das Setzen der Eigenschaft Legend.Y keine Wirkung.


**Returns:**
int
### getReadingOrder() {#getReadingOrder--}
```
public int getReadingOrder()
```


Stellt die Lesereihenfolge des Textes dar.

Siehe [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Returns:**
int
### getRotationAngle() {#getRotationAngle--}
```
public int getRotationAngle()
```


Stellt den Drehwinkel des Textes dar.

**Remarks**


0: Nicht gedreht.

255: Oben nach unten.

\-90: Abwärts.

90: Aufwärts.


**Returns:**
int
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
### getText() {#getText--}
```
public String getText()
```


Ermittelt den Text des Titels eines Rahmens.

**Returns:**
java.lang.String
### getTextDirection() {#getTextDirection--}
```
public int getTextDirection()
```


Stellt die Lesereihenfolge des Textes dar.

Siehe [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft ChartTextFrame.ReadingOrder. Diese Eigenschaft wird 12 Monate später, seit März 2020, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Returns:**
int
### getTextFont() {#getTextFont--}
```
public Font getTextFont()
```


Ermittelt ein [getFont()](../../com.aspose.cells/chartframe\#getFont--) Objekt des angegebenen ChartFrame-Objekts.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft ChartFrame.Font. Diese Eigenschaft wird 12 Monate später, seit JANUAR 2012, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Returns:**
[Font](../../com.aspose.cells/font)
### getTextHorizontalAlignment() {#getTextHorizontalAlignment--}
```
public int getTextHorizontalAlignment()
```


Ermittelt die horizontale Ausrichtung des Textes.

Siehe [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


Ermittelt die Optionen des Textes.

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getTextVerticalAlignment() {#getTextVerticalAlignment--}
```
public int getTextVerticalAlignment()
```


Ermittelt die vertikale Ausrichtung des Textes.

Siehe [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getWidth() {#getWidth--}
```
public int getWidth()
```


Ermittelt die Breite des Rahmens in Einheiten von 1/4000 des Diagrammbereichs.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die Eigenschaft ChartFrame.WidthRatioToChart. Width = WidthRatioToChart \* 4000; Diese Eigenschaft wird 12 Monate später, seit Februar 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

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


Ermittelt die Breite des Rahmens in Einheiten des Verhältnisses zum Diagrammbereich.

**Remarks**

Dies ist ein Bruchwert, sein gültiger Bereich liegt zwischen 0-1. Wie konvertiert man Verhältnis-Einheiten in Pixel? WidthPixel = WidthRatioToChart \* Chart.ChartObject.Width;

**Returns:**
double
### getX() {#getX--}
```
public int getX()
```


Liefert die x‑Koordinate der oberen linken Ecke in Einheiten von 1/4000 des Diagrammbereichs.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die Eigenschaft ChartFrame.XRatioToChart. X = XRatioToChart \* 4000. Diese Eigenschaft wird 12 Monate später, seit February 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

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


Liefert die x‑Koordinate der oberen linken Ecke in Einheiten des Verhältnisses des Diagrammbereichs.

**Remarks**

Dies ist ein Bruchwert, sein gültiger Bereich liegt zwischen 0‑1. Wie konvertiert man Einheiten des Verhältnisses in Pixel? XPixel = XRatioToChart \* Chart.ChartObject.Width;

**Returns:**
double
### getY() {#getY--}
```
public int getY()
```


Ermittelt die Y‑Koordinate der oberen linken Ecke in Einheiten von 1/4000 des Diagrammbereichs.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die Eigenschaft ChartFrame.YRatioToChart. Y = YRatioToChart \* 4000. Diese Eigenschaft wird 12 Monate später, seit February 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

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


Liefert die y‑Koordinate der oberen linken Ecke in Einheiten des Verhältnisses des Diagrammbereichs.

**Remarks**

Dies ist ein Bruchwert, sein gültiger Bereich liegt zwischen 0‑1. Wie konvertiert man Einheiten des Verhältnisses in Pixel? YPixel = YRatioToChart \* Chart.ChartObject.Height;

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoText() {#isAutoText--}
```
public boolean isAutoText()
```


Gibt an, dass der Text automatisch generiert wird.

**Returns:**
boolean
### isAutomaticRotation() {#isAutomaticRotation--}
```
public boolean isAutomaticRotation()
```


Gibt an, ob der Text des Diagramms automatisch gedreht wird.

**Returns:**
boolean
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
### isDeleted() {#isDeleted--}
```
public boolean isDeleted()
```


Gibt an, ob diese Datenbeschriftung gelöscht ist.

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
### isOverLay() {#isOverLay--}
```
public boolean isOverLay()
```


Ruft ab, ob die Legende angezeigt wird, ohne das Diagramm zu überlappen.

**Returns:**
boolean
### isResizeShapeToFitText() {#isResizeShapeToFitText--}
```
public boolean isResizeShapeToFitText()
```


Ermittelt, ob eine Form automatisch angepasst werden soll, um den darin beschriebenen Text vollständig zu enthalten. Auto-Fit bedeutet, dass der Text innerhalb einer Form skaliert wird, um den gesamten Text aufzunehmen.

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


Ermittelt einen Wert, der angibt, ob der Text umgebrochen ist.

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

### setAutoText(boolean value) {#setAutoText-boolean-}
```
public void setAutoText(boolean value)
```


Gibt an, dass der Text automatisch generiert wird.

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

### setDeleted(boolean value) {#setDeleted-boolean-}
```
public void setDeleted(boolean value)
```


Gibt an, ob diese Datenbeschriftung gelöscht ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setDirectionType(int value) {#setDirectionType-int-}
```
public void setDirectionType(int value)
```


Legt die Textausrichtung fest.

Siehe [ChartTextDirectionType](../../com.aspose.cells/charttextdirectiontype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setHeight(int value) {#setHeight-int-}
```
public void setHeight(int value)
```


Legt die Höhe des Rahmens in Einheiten von 1/4000 des Diagrammbereichs fest.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die Eigenschaft ChartFrame.HeightRatioToChart. Height = HeightRatioToChart \* 4000. Diese Eigenschaft wird 12 Monate später, seit Februar 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

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


Legt die Höhe des Rahmens in Einheiten des Verhältnisses zum Diagrammbereich fest.

**Remarks**

Dies ist ein Bruchwert, sein gültiger Bereich liegt zwischen 0-1. Wie konvertiert man Verhältnis-Einheiten in Pixel? HeightPixel = HeightRatioToChart \* Chart.ChartObject.Height;

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

### setLinkedSource(String value) {#setLinkedSource-java.lang.String-}
```
public void setLinkedSource(String value)
```


Legt eine Referenz auf das Arbeitsblatt fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setOverLay(boolean value) {#setOverLay-boolean-}
```
public void setOverLay(boolean value)
```


Legt fest, ob die Legende angezeigt wird, ohne das Diagramm zu überlappen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setPosition(int value) {#setPosition-int-}
```
public void setPosition(int value)
```


Legt den Legendenpositionstyp fest.

Siehe [LegendPositionType](../../com.aspose.cells/legendpositiontype).

**Remarks**


Standardposition ist rechts.

Wenn die Legende sich auf der linken oder rechten Seite des Diagramms befindet, hat das Setzen der Eigenschaft Legend.X keine Wirkung.

Wenn die Legende sich oben oder unten am Diagramm befindet, hat das Setzen der Eigenschaft Legend.Y keine Wirkung.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setPositionAuto() {#setPositionAuto--}
```
public void setPositionAuto()
```


Setzt die Position des Rahmens auf automatisch

### setReadingOrder(int value) {#setReadingOrder-int-}
```
public void setReadingOrder(int value)
```


Stellt die Lesereihenfolge des Textes dar.

Siehe [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setResizeShapeToFitText(boolean value) {#setResizeShapeToFitText-boolean-}
```
public void setResizeShapeToFitText(boolean value)
```


Legt fest, ob eine Form automatisch angepasst werden soll, um den darin beschriebenen Text vollständig zu enthalten. Auto-Anpassung bedeutet, dass der Text innerhalb einer Form skaliert wird, um den gesamten Text aufzunehmen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setRotationAngle(int value) {#setRotationAngle-int-}
```
public void setRotationAngle(int value)
```


Stellt den Drehwinkel des Textes dar.

**Remarks**


0: Nicht gedreht.

255: Oben nach unten.

\-90: Abwärts.

90: Aufwärts.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

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

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Legt den Text des Titels eines Rahmens fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setTextDirection(int value) {#setTextDirection-int-}
```
public void setTextDirection(int value)
```


Stellt die Lesereihenfolge des Textes dar.

Siehe [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft ChartTextFrame.ReadingOrder. Diese Eigenschaft wird 12 Monate später, seit März 2020, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setTextHorizontalAlignment(int value) {#setTextHorizontalAlignment-int-}
```
public void setTextHorizontalAlignment(int value)
```


Legt die horizontale Ausrichtung des Textes fest.

Siehe [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setTextVerticalAlignment(int value) {#setTextVerticalAlignment-int-}
```
public void setTextVerticalAlignment(int value)
```


Legt die vertikale Ausrichtung des Textes fest.

Siehe [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setTextWrapped(boolean value) {#setTextWrapped-boolean-}
```
public void setTextWrapped(boolean value)
```


Legt einen Wert fest, der angibt, ob der Text umgebrochen wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setWidth(int value) {#setWidth-int-}
```
public void setWidth(int value)
```


Legt die Breite des Rahmens in Einheiten von 1/4000 des Diagrammbereichs fest.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die Eigenschaft ChartFrame.WidthRatioToChart. Width = WidthRatioToChart \* 4000; Diese Eigenschaft wird 12 Monate später, seit Februar 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

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


Legt die Breite des Rahmens im Verhältnis zum Diagrammbereich fest.

**Remarks**

Dies ist ein Bruchwert, sein gültiger Bereich liegt zwischen 0-1. Wie konvertiert man Verhältnis-Einheiten in Pixel? WidthPixel = WidthRatioToChart \* Chart.ChartObject.Width;

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setX(int value) {#setX-int-}
```
public void setX(int value)
```


Setzt die x‑Koordinate der oberen linken Ecke in Einheiten von 1/4000 des Diagrammbereichs.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die Eigenschaft ChartFrame.XRatioToChart. X = XRatioToChart \* 4000. Diese Eigenschaft wird 12 Monate später, seit February 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

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


Setzt die x‑Koordinate der oberen linken Ecke in Einheiten des Verhältnisses des Diagrammbereichs.

**Remarks**

Dies ist ein Bruchwert, sein gültiger Bereich liegt zwischen 0‑1. Wie konvertiert man Einheiten des Verhältnisses in Pixel? XPixel = XRatioToChart \* Chart.ChartObject.Width;

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setY(int value) {#setY-int-}
```
public void setY(int value)
```


Legt die Y‑Koordinate der oberen linken Ecke in Einheiten von 1/4000 des Diagrammbereichs fest.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die Eigenschaft ChartFrame.YRatioToChart. Y = YRatioToChart \* 4000. Diese Eigenschaft wird 12 Monate später, seit February 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

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


Setzt die y‑Koordinate der oberen linken Ecke in Einheiten des Verhältnisses des Diagrammbereichs.

**Remarks**

Dies ist ein Bruchwert, sein gültiger Bereich liegt zwischen 0‑1. Wie konvertiert man Einheiten des Verhältnisses in Pixel? YPixel = YRatioToChart \* Chart.ChartObject.Height;

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

