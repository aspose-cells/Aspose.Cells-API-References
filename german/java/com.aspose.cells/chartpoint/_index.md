---
title: "ChartPoint"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt einen einzelnen Punkt in einer Serie eines Diagramms dar."
type: docs
url: /de/java/com.aspose.cells/chartpoint/
---

**Inheritance:**
java.lang.Object
```
public class ChartPoint
```

Stellt einen einzelnen Punkt in einer Serie eines Diagramms dar.

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
         int chartIndex = worksheet.getCharts().add(ChartType.PIE_EXPLODED, 5, 0, 25, 10);
 
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
 
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
         chart.getNSeries().add("A1:B3", true);
 
         //Show Data Labels 
         chart.getNSeries().get(0).getDataLabels().setShowValue(true);
 
         for (int i = 0; i  <chart.getNSeries().get(0).getPoints().getCount(); i++)
         {
             //Get Data Point
             ChartPoint point = chart.getNSeries().get(0).getPoints().get(i);
             //Set Pir Explosion
             point.setExplosion(15);
             //Set Border Color
             point.getBorder().setColor(com.aspose.cells.Color.getRed());
         }
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArcEndPointXPx()](#getArcEndPointXPx--) | Ermittelt die x‑Koordinate des Endpunkts des Kuchensegments nach Aufruf der Methode Chart.Calculate(). |
| [getArcEndPointYPx()](#getArcEndPointYPx--) | Ermittelt die y‑Koordinate des Endpunkts des Kuchensegments nach Aufruf der Methode Chart.Calculate(). |
| [getArcStartPointXPx()](#getArcStartPointXPx--) | Ermittelt die x‑Koordinate des Startpunkts des Kuchensegments nach Aufruf der Methode Chart.Calculate(). |
| [getArcStartPointYPx()](#getArcStartPointYPx--) | Ermittelt die y‑Koordinate des Startpunkts des Kuchensegments nach Aufruf der Methode Chart.Calculate(). |
| [getArea()](#getArea--) | Ermittelt die [getArea()](../../com.aspose.cells/chartpoint\#getArea--). |
| [getBorder()](#getBorder--) | Liefert die [Line](../../com.aspose.cells/line). |
| [getBorderWidthPx()](#getBorderWidthPx--) | Ermittelt die Breite des Rahmens in Pixeln nach Aufruf der Methode Chart.Calculate(). |
| [getBottomPointCount()](#getBottomPointCount--) | Ermittelt die Anzahl der unteren Punkte nach Aufruf der Methode Chart.Calculate(). |
| [getBottomPointXPx(int index)](#getBottomPointXPx-int-) | Ermittelt die x‑Koordinate des unteren Punkts der Form nach Aufruf der Methode Chart.Calculate(). |
| [getBottomPointYPx(int index)](#getBottomPointYPx-int-) | Ermittelt die y‑Koordinate des unteren Punkts der Form nach Aufruf der Methode Chart.Calculate(). |
| [getClass()](#getClass--) |  |
| [getDataLabels()](#getDataLabels--) | Gibt ein [getDataLabels()](../../com.aspose.cells/chartpoint\#getDataLabels--) Objekt zurück, das das mit diesem Diagrammpunkt verbundene Datenbeschriftungsobjekt darstellt. |
| [getDoughnutInnerRadius()](#getDoughnutInnerRadius--) | Ermittelt den inneren Radius des Donut‑Segments in Pixeln nach Aufruf der Methode Chart.Calculate(). |
| [getEndAngle()](#getEndAngle--) | Ermittelt den Endwinkel des Kuchensegments, gemessen in Grad im Uhrzeigersinn von der x‑Achse nach Aufruf der Methode Chart.Calculate(). |
| [getExplosion()](#getExplosion--) | Der Abstand eines offenen Kuchensegments vom Zentrum des Kuchendiagramms wird als Prozentsatz des Durchmessers des Kuchens angegeben. |
| [getInnerArcEndPointXPx()](#getInnerArcEndPointXPx--) | Ermittelt die x‑Koordinate des Endpunkts des Kuchensegments nach Aufruf der Methode Chart.Calculate(). |
| [getInnerArcEndPointYPx()](#getInnerArcEndPointYPx--) | Ermittelt die y‑Koordinate des Endpunkts des Kuchensegments nach Aufruf der Methode Chart.Calculate(). |
| [getInnerArcStartPointXPx()](#getInnerArcStartPointXPx--) | Ermittelt die x‑Koordinate des Startpunkts des Kuchensegments nach Aufruf der Methode Chart.Calculate(). |
| [getInnerArcStartPointYPx()](#getInnerArcStartPointYPx--) | Ermittelt die y‑Koordinate des Startpunkts des Kuchensegments nach Aufruf der Methode Chart.Calculate(). |
| [getInnerRadiusPx()](#getInnerRadiusPx--) | Ermittelt den inneren Radius des Donut‑Segments in Pixeln nach Aufruf der Methode Chart.Calculate(). |
| [getMarker()](#getMarker--) | Ruft das [getMarker()](../../com.aspose.cells/chartpoint\#getMarker--) ab. |
| [getOnCategoryAxisPointCount()](#getOnCategoryAxisPointCount--) | Ruft die Anzahl der Punkte auf der Kategorienachse nach dem Aufruf der Methode Chart.Calculate() ab. |
| [getOnCategoryAxisPointXPx(int index)](#getOnCategoryAxisPointXPx-int-) | Ruft die x-Koordinate des Punktes auf der Kategorienachse nach dem Aufruf der Methode Chart.Calculate() ab. |
| [getOnCategoryAxisPointYPx(int index)](#getOnCategoryAxisPointYPx-int-) | Ruft die y-Koordinate des Punktes auf der Kategorienachse nach dem Aufruf der Methode Chart.Calculate() ab. |
| [getRadiusPx()](#getRadiusPx--) | Ruft den Radius von Blase, Kuchen oder Donut in Pixeln nach dem Aufruf der Methode Chart.Calculate() ab. |
| [getShadow()](#getShadow--) | True, wenn der Diagrammpunkt einen Schatten hat. |
| [getShapeHeight()](#getShapeHeight--) | Ruft die Höhe in Einheiten von 1/4000 der Diagrammhöhe nach dem Aufruf der Methode Chart.Calculate() ab. |
| [getShapeHeightPx()](#getShapeHeightPx--) | Ruft die Höhe in Pixeln nach dem Aufruf der Methode Chart.Calculate() ab. |
| [getShapeProperties()](#getShapeProperties--) | Ruft das [ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection)-Objekt ab, das die visuellen Formeigenschaften des Diagrammpunkts enthält. |
| [getShapeWidth()](#getShapeWidth--) | Ruft die Breite in Einheiten von 1/4000 der Diagrammbreite nach dem Aufruf der Methode Chart.Calculate() ab. |
| [getShapeWidthPx()](#getShapeWidthPx--) | Ruft die Breite in Pixeln nach dem Aufruf der Methode Chart.Calculate() ab. |
| [getShapeX()](#getShapeX--) | Ruft die x-Koordinate der oberen linken Ecke in Einheiten von 1/4000 der Diagrammbreite nach dem Aufruf der Methode Chart.Calculate() ab. |
| [getShapeXPx()](#getShapeXPx--) | Ruft die x-Koordinate der oberen linken Ecke in Pixeln nach dem Aufruf der Methode Chart.Calculate() ab. |
| [getShapeY()](#getShapeY--) | Ruft die y-Koordinate der oberen linken Ecke in Einheiten von 1/4000 der Diagrammhöhe nach dem Aufruf der Methode Chart.Calculate() ab. |
| [getShapeYPx()](#getShapeYPx--) | Ruft die y-Koordinate der oberen linken Ecke in Pixeln nach dem Aufruf der Methode Chart.Calculate() ab. |
| [getStartAngle()](#getStartAngle--) | Ruft den Startwinkel für das Kuchensegment ab, gemessen in Grad im Uhrzeigersinn von der x-Achse nach dem Aufruf der Methode Chart.Calculate(). |
| [getTopPointCount()](#getTopPointCount--) | Ruft die Anzahl der oberen Punkte nach dem Aufruf der Methode Chart.Calculate() ab. |
| [getTopPointXPx(int index)](#getTopPointXPx-int-) | Ruft die x-Koordinate des oberen Punkts der Form nach dem Aufruf der Methode Chart.Calculate() ab. |
| [getTopPointYPx(int index)](#getTopPointYPx-int-) | Ruft die y-Koordinate des oberen Punkts der Form nach dem Aufruf der Methode Chart.Calculate() ab. |
| [getXValue()](#getXValue--) | Ruft den X-Wert des Diagrammpunkts ab. |
| [getXValueType()](#getXValueType--) | Ruft den Typ des X-Werts des Diagrammpunkts ab. |
| [getYValue()](#getYValue--) | Ruft den Y-Wert des Diagrammpunkts ab. |
| [getYValueType()](#getYValueType--) | Ruft den Typ des Y-Werts des Diagrammpunkts ab. |
| [hashCode()](#hashCode--) |  |
| [isInSecondaryPlot()](#isInSecondaryPlot--) | Ruft einen Wert ab, der angibt, ob dieser Datenpunkt im zweiten Kuchen oder Balken eines Kuchen‑oder Balkendiagramms liegt. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setExplosion(int value)](#setExplosion-int-) | Der Abstand eines offenen Kuchensegments vom Zentrum des Kuchendiagramms wird als Prozentsatz des Durchmessers des Kuchens angegeben. |
| [setInSecondaryPlot(boolean value)](#setInSecondaryPlot-boolean-) | Setzt einen Wert, der angibt, ob dieser Datenpunkt im zweiten Kuchen oder Balken eines Kuchen‑oder Balkendiagramms liegt. |
| [setShadow(boolean value)](#setShadow-boolean-) | True, wenn der Diagrammpunkt einen Schatten hat. |
| [setXValue(Object value)](#setXValue-java.lang.Object-) | Legt den X-Wert des Diagrammpunkts fest. |
| [setYValue(Object value)](#setYValue-java.lang.Object-) | Legt den Y-Wert des Diagrammpunkts fest. |
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
### getArcEndPointXPx() {#getArcEndPointXPx--}
```
public float getArcEndPointXPx()
```


Ermittelt die x-Koordinate des Endpunkts für das Pie-Segment nach Aufruf der Methode Chart.Calculate(). Gilt für Pie- und Doughnut-Diagramme.

**Returns:**
float
### getArcEndPointYPx() {#getArcEndPointYPx--}
```
public float getArcEndPointYPx()
```


Ermittelt die y-Koordinate des Endpunkts für das Pie-Segment nach Aufruf der Methode Chart.Calculate(). Gilt für Pie- und Doughnut-Diagramme.

**Returns:**
float
### getArcStartPointXPx() {#getArcStartPointXPx--}
```
public float getArcStartPointXPx()
```


Ermittelt die x-Koordinate des Startpunkts für das Pie-Segment nach Aufruf der Methode Chart.Calculate(). Gilt für Pie- und Doughnut-Diagramme.

**Returns:**
float
### getArcStartPointYPx() {#getArcStartPointYPx--}
```
public float getArcStartPointYPx()
```


Ermittelt die y-Koordinate des Startpunkts für das Pie-Segment nach Aufruf der Methode Chart.Calculate(). Gilt für Pie- und Doughnut-Diagramme.

**Returns:**
float
### getArea() {#getArea--}
```
public Area getArea()
```


Ermittelt die [getArea()](../../com.aspose.cells/chartpoint\#getArea--).

**Returns:**
[Area](../../com.aspose.cells/area)
### getBorder() {#getBorder--}
```
public Line getBorder()
```


Liefert die [Line](../../com.aspose.cells/line).

**Returns:**
[Line](../../com.aspose.cells/line)
### getBorderWidthPx() {#getBorderWidthPx--}
```
public int getBorderWidthPx()
```


Ermittelt die Breite des Rahmens in Pixeln nach Aufruf der Methode Chart.Calculate().

**Returns:**
int
### getBottomPointCount() {#getBottomPointCount--}
```
public int getBottomPointCount()
```


Ermittelt die Anzahl der unteren Punkte nach Aufruf der Methode Chart.Calculate().

**Returns:**
int
### getBottomPointXPx(int index) {#getBottomPointXPx-int-}
```
public float getBottomPointXPx(int index)
```


Ermittelt die x-Koordinate des unteren Punktes der Form nach Aufruf der Methode Chart.Calculate(). Gilt für 3D-Diagramme: Column3D, Bar3D, Cone, Cylinder, Pyramid.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int |  |

**Returns:**
float
### getBottomPointYPx(int index) {#getBottomPointYPx-int-}
```
public float getBottomPointYPx(int index)
```


Ermittelt die y-Koordinate des unteren Punktes der Form nach Aufruf der Methode Chart.Calculate(). Gilt für 3D-Diagramme: Column3D, Bar3D, Cone, Cylinder, Pyramid.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int |  |

**Returns:**
float
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDataLabels() {#getDataLabels--}
```
public DataLabels getDataLabels()
```


Gibt ein [getDataLabels()](../../com.aspose.cells/chartpoint\#getDataLabels--) Objekt zurück, das das mit diesem Diagrammpunkt verbundene Datenbeschriftungsobjekt darstellt.

**Returns:**
[DataLabels](../../com.aspose.cells/datalabels)
### getDoughnutInnerRadius() {#getDoughnutInnerRadius--}
```
public int getDoughnutInnerRadius()
```


Ermittelt den inneren Radius des Donut‑Segments in Pixeln nach Aufruf der Methode Chart.Calculate(). Gilt für Doughnut-Diagramme.

**Returns:**
int
### getEndAngle() {#getEndAngle--}
```
public float getEndAngle()
```


Ermittelt den Endwinkel für das Pie-Segment, gemessen in Grad im Uhrzeigersinn von der x-Achse nach Aufruf der Methode Chart.Calculate(). Gilt für Pie-Diagramme.

**Returns:**
float
### getExplosion() {#getExplosion--}
```
public int getExplosion()
```


Der Abstand eines offenen Kuchensegments vom Zentrum des Kuchendiagramms wird als Prozentsatz des Durchmessers des Kuchens angegeben.

**Returns:**
int
### getInnerArcEndPointXPx() {#getInnerArcEndPointXPx--}
```
public float getInnerArcEndPointXPx()
```


Ermittelt die x-Koordinate des Endpunkts für das Pie-Segment nach Aufruf der Methode Chart.Calculate(). Gilt für Doughnut-Diagramme.

**Returns:**
float
### getInnerArcEndPointYPx() {#getInnerArcEndPointYPx--}
```
public float getInnerArcEndPointYPx()
```


Ermittelt die y-Koordinate des Endpunkts für das Pie-Segment nach Aufruf der Methode Chart.Calculate(). Gilt für Doughnut-Diagramme.

**Returns:**
float
### getInnerArcStartPointXPx() {#getInnerArcStartPointXPx--}
```
public float getInnerArcStartPointXPx()
```


Ermittelt die x-Koordinate des Startpunkts für das Pie-Segment nach Aufruf der Methode Chart.Calculate(). Gilt für das Doughnut-Diagramm.

**Returns:**
float
### getInnerArcStartPointYPx() {#getInnerArcStartPointYPx--}
```
public float getInnerArcStartPointYPx()
```


Ermittelt die y-Koordinate des Startpunkts für das Pie-Segment nach Aufruf der Methode Chart.Calculate(). Gilt für Doughnut-Diagramme.

**Returns:**
float
### getInnerRadiusPx() {#getInnerRadiusPx--}
```
public int getInnerRadiusPx()
```


Ermittelt den inneren Radius des Donut‑Segments in Pixeln nach Aufruf der Methode Chart.Calculate(). Gilt für Doughnut-Diagramme.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft ChartPoint.DoughnutInnerRadius. Diese Eigenschaft wird 12 Monate nach Juni 2024 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Returns:**
int
### getMarker() {#getMarker--}
```
public Marker getMarker()
```


Ruft das [getMarker()](../../com.aspose.cells/chartpoint\#getMarker--) ab.

**Returns:**
[Marker](../../com.aspose.cells/marker)
### getOnCategoryAxisPointCount() {#getOnCategoryAxisPointCount--}
```
public int getOnCategoryAxisPointCount()
```


Ermittelt die Anzahl der Punkte auf der Kategorienachse nach Aufruf der Methode Chart.Calculate(). Gilt nur für Flächendiagramme.

**Remarks**

Flächen-2D-Diagramm gibt 1 zurück, Flächen-3D-Diagramm gibt 2 zurück.

**Returns:**
int
### getOnCategoryAxisPointXPx(int index) {#getOnCategoryAxisPointXPx-int-}
```
public float getOnCategoryAxisPointXPx(int index)
```


Ermittelt die x-Koordinate des Punktes auf der Kategorienachse nach Aufruf der Methode Chart.Calculate(). Gilt nur für Flächendiagramme.

**Remarks**

Flächen-2D-Diagramm: Index ist 0. Flächen-3D-Diagramm: Index ist 0 oder 1.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int |  |

**Returns:**
float
### getOnCategoryAxisPointYPx(int index) {#getOnCategoryAxisPointYPx-int-}
```
public float getOnCategoryAxisPointYPx(int index)
```


Ermittelt die y-Koordinate des Punktes auf der Kategorienachse nach Aufruf der Methode Chart.Calculate(). Gilt nur für Flächendiagramme.

**Remarks**

Flächen-2D-Diagramm: Index ist 0. Flächen-3D-Diagramm: Index ist 0 oder 1.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int |  |

**Returns:**
float
### getRadiusPx() {#getRadiusPx--}
```
public int getRadiusPx()
```


Ruft den Radius von Blase, Kuchen oder Donut in Pixeln nach dem Aufruf der Methode Chart.Calculate() ab.

**Returns:**
int
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


True, wenn der Diagrammpunkt einen Schatten hat.

**Returns:**
boolean
### getShapeHeight() {#getShapeHeight--}
```
public int getShapeHeight()
```


Ruft die Höhe in Einheiten von 1/4000 der Diagrammhöhe nach dem Aufruf der Methode Chart.Calculate() ab.

**Returns:**
int
### getShapeHeightPx() {#getShapeHeightPx--}
```
public int getShapeHeightPx()
```


Ruft die Höhe in Pixeln nach dem Aufruf der Methode Chart.Calculate() ab.

**Returns:**
int
### getShapeProperties() {#getShapeProperties--}
```
public ShapePropertyCollection getShapeProperties()
```


Ruft das [ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection)-Objekt ab, das die visuellen Formeigenschaften des Diagrammpunkts enthält.

**Returns:**
[ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection)
### getShapeWidth() {#getShapeWidth--}
```
public int getShapeWidth()
```


Ruft die Breite in Einheiten von 1/4000 der Diagrammbreite nach dem Aufruf der Methode Chart.Calculate() ab.

**Returns:**
int
### getShapeWidthPx() {#getShapeWidthPx--}
```
public int getShapeWidthPx()
```


Ruft die Breite in Pixeln nach dem Aufruf der Methode Chart.Calculate() ab.

**Returns:**
int
### getShapeX() {#getShapeX--}
```
public int getShapeX()
```


Ruft die x-Koordinate der oberen linken Ecke in Einheiten von 1/4000 der Diagrammbreite nach dem Aufruf der Methode Chart.Calculate() ab.

**Returns:**
int
### getShapeXPx() {#getShapeXPx--}
```
public int getShapeXPx()
```


Ruft die x-Koordinate der oberen linken Ecke in Pixeln nach dem Aufruf der Methode Chart.Calculate() ab.

**Returns:**
int
### getShapeY() {#getShapeY--}
```
public int getShapeY()
```


Ruft die y-Koordinate der oberen linken Ecke in Einheiten von 1/4000 der Diagrammhöhe nach dem Aufruf der Methode Chart.Calculate() ab.

**Returns:**
int
### getShapeYPx() {#getShapeYPx--}
```
public int getShapeYPx()
```


Ruft die y-Koordinate der oberen linken Ecke in Pixeln nach dem Aufruf der Methode Chart.Calculate() ab.

**Returns:**
int
### getStartAngle() {#getStartAngle--}
```
public float getStartAngle()
```


Ermittelt den Startwinkel für das Pie-Segment, gemessen in Grad im Uhrzeigersinn von der x-Achse nach Aufruf der Methode Chart.Calculate(). Gilt für Pie-Diagramme.

**Returns:**
float
### getTopPointCount() {#getTopPointCount--}
```
public int getTopPointCount()
```


Ruft die Anzahl der oberen Punkte nach dem Aufruf der Methode Chart.Calculate() ab.

**Returns:**
int
### getTopPointXPx(int index) {#getTopPointXPx-int-}
```
public float getTopPointXPx(int index)
```


Ermittelt die x-Koordinate des oberen Punktes der Form nach Aufruf der Methode Chart.Calculate(). Gilt für 3D-Diagramme: Column3D, Bar3D, Cone, Cylinder, Pyramid und Area3D.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int |  |

**Returns:**
float
### getTopPointYPx(int index) {#getTopPointYPx-int-}
```
public float getTopPointYPx(int index)
```


Ermittelt die y-Koordinate des oberen Punktes der Form nach Aufruf der Methode Chart.Calculate(). Gilt für 3D-Diagramme: Column3D, Bar3D, Cone, Cylinder, Pyramid und Area3D.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int |  |

**Returns:**
float
### getXValue() {#getXValue--}
```
public Object getXValue()
```


Ruft den X-Wert des Diagrammpunkts ab.

**Returns:**
java.lang.Object
### getXValueType() {#getXValueType--}
```
public int getXValueType()
```


Ruft den Typ des X-Werts des Diagrammpunkts ab.

Siehe [CellValueType](../../com.aspose.cells/cellvaluetype).

**Returns:**
int
### getYValue() {#getYValue--}
```
public Object getYValue()
```


Ruft den Y-Wert des Diagrammpunkts ab.

**Returns:**
java.lang.Object
### getYValueType() {#getYValueType--}
```
public int getYValueType()
```


Ruft den Typ des Y-Werts des Diagrammpunkts ab.

Siehe [CellValueType](../../com.aspose.cells/cellvaluetype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isInSecondaryPlot() {#isInSecondaryPlot--}
```
public boolean isInSecondaryPlot()
```


Ruft einen Wert ab, der angibt, ob dieser Datenpunkt im zweiten Kuchen oder Balken eines Kuchen‑oder Balkendiagramms liegt.

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




### setExplosion(int value) {#setExplosion-int-}
```
public void setExplosion(int value)
```


Der Abstand eines offenen Kuchensegments vom Zentrum des Kuchendiagramms wird als Prozentsatz des Durchmessers des Kuchens angegeben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setInSecondaryPlot(boolean value) {#setInSecondaryPlot-boolean-}
```
public void setInSecondaryPlot(boolean value)
```


Setzt einen Wert, der angibt, ob dieser Datenpunkt im zweiten Kuchen oder Balken eines Kuchen‑oder Balkendiagramms liegt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


True, wenn der Diagrammpunkt einen Schatten hat.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setXValue(Object value) {#setXValue-java.lang.Object-}
```
public void setXValue(Object value)
```


Legt den X-Wert des Diagrammpunkts fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.Object |  |

### setYValue(Object value) {#setYValue-java.lang.Object-}
```
public void setYValue(Object value)
```


Legt den Y-Wert des Diagrammpunkts fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.Object |  |

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

