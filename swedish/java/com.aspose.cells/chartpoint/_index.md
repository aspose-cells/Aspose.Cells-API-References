---
title: "ChartPoint"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar en enskild punkt i en serie i ett diagram."
type: docs
url: /sv/java/com.aspose.cells/chartpoint/
---

**Inheritance:**
java.lang.Object
```
public class ChartPoint
```

Representerar en enskild punkt i en serie i ett diagram.

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
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArcEndPointXPx()](#getArcEndPointXPx--) | Hämtar x-koordinaten för slutpunkten för pajsektionen efter att ha anropat metoden Chart.Calculate(). |
| [getArcEndPointYPx()](#getArcEndPointYPx--) | Hämtar y-koordinaten för slutpunkten för pajsektionen efter anrop av metoden Chart.Calculate(). |
| [getArcStartPointXPx()](#getArcStartPointXPx--) | Hämtar x-koordinaten för startpunkten för pajsektionen efter att ha anropat metoden Chart.Calculate(). |
| [getArcStartPointYPx()](#getArcStartPointYPx--) | Hämtar y-koordinaten för startpunkten för pajsektionen efter anrop av metoden Chart.Calculate(). |
| [getArea()](#getArea--) | Hämtar [getArea()](../../com.aspose.cells/chartpoint\#getArea--). |
| [getBorder()](#getBorder--) | Hämtar [Line](../../com.aspose.cells/line). |
| [getBorderWidthPx()](#getBorderWidthPx--) | Hämtar bredden på kanten i enheter av pixlar efter att ha anropat metoden Chart.Calculate(). |
| [getBottomPointCount()](#getBottomPointCount--) | Hämtar antalet bottenpunkter efter anrop av metoden Chart.Calculate(). |
| [getBottomPointXPx(int index)](#getBottomPointXPx-int-) | Hämtar x-koordinaten för bottenpunkten på formen efter att ha anropat metoden Chart.Calculate(). |
| [getBottomPointYPx(int index)](#getBottomPointYPx-int-) | Hämtar y-koordinaten för bottenpunkten på formen efter anrop av metoden Chart.Calculate(). |
| [getClass()](#getClass--) |  |
| [getDataLabels()](#getDataLabels--) | Returnerar ett [getDataLabels()](../../com.aspose.cells/chartpoint\#getDataLabels--) objekt som representerar datamärket som är associerat med denna diagrampunkt. |
| [getDoughnutInnerRadius()](#getDoughnutInnerRadius--) | Hämtar den inre radien på doughnut‑skivan i enheter av pixlar efter att ha anropat metoden Chart.Calculate(). |
| [getEndAngle()](#getEndAngle--) | Hämtar slutvinkeln för pajsektionen, mätt i grader medurs från x-axeln efter anrop av metoden Chart.Calculate(). |
| [getExplosion()](#getExplosion--) | Avståndet för en öppen pajskiva från mitten av pajdiagrammet uttrycks som en procentandel av pajens diameter. |
| [getInnerArcEndPointXPx()](#getInnerArcEndPointXPx--) | Hämtar x-koordinaten för slutpunkten för pajsektionen efter att ha anropat metoden Chart.Calculate(). |
| [getInnerArcEndPointYPx()](#getInnerArcEndPointYPx--) | Hämtar y-koordinaten för slutpunkten för pajsektionen efter anrop av metoden Chart.Calculate(). |
| [getInnerArcStartPointXPx()](#getInnerArcStartPointXPx--) | Hämtar x-koordinaten för startpunkten för pajsektionen efter att ha anropat metoden Chart.Calculate(). |
| [getInnerArcStartPointYPx()](#getInnerArcStartPointYPx--) | Hämtar y-koordinaten för startpunkten för pajsektionen efter anrop av metoden Chart.Calculate(). |
| [getInnerRadiusPx()](#getInnerRadiusPx--) | Hämtar den inre radien på donut-skivan i pixelenheter efter anrop av metoden Chart.Calculate(). |
| [getMarker()](#getMarker--) | Hämtar [getMarker()](../../com.aspose.cells/chartpoint\#getMarker--). |
| [getOnCategoryAxisPointCount()](#getOnCategoryAxisPointCount--) | Hämtar antalet punkter på kategori-axeln efter anrop av metoden Chart.Calculate(). |
| [getOnCategoryAxisPointXPx(int index)](#getOnCategoryAxisPointXPx-int-) | Hämtar x-koordinaten för punkten på kategori-axeln efter anrop av metoden Chart.Calculate(). |
| [getOnCategoryAxisPointYPx(int index)](#getOnCategoryAxisPointYPx-int-) | Hämtar y-koordinaten för punkten på kategori-axeln efter anrop av metoden Chart.Calculate(). |
| [getRadiusPx()](#getRadiusPx--) | Hämtar radien för bubbla, paj eller donut i pixelenheter efter anrop av metoden Chart.Calculate(). |
| [getShadow()](#getShadow--) | Sant om diagrampunkten har en skugga. |
| [getShapeHeight()](#getShapeHeight--) | Hämtar höjden i enheter av 1/4000 av diagrammets höjd efter anrop av metoden Chart.Calculate(). |
| [getShapeHeightPx()](#getShapeHeightPx--) | Hämtar höjden i pixelenheter efter anrop av metoden Chart.Calculate(). |
| [getShapeProperties()](#getShapeProperties--) | Hämtar objektet [ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection) som innehåller de visuella formegenskaperna för ChartPoint. |
| [getShapeWidth()](#getShapeWidth--) | Hämtar bredden i enheter av 1/4000 av diagrammets bredd efter anrop av metoden Chart.Calculate(). |
| [getShapeWidthPx()](#getShapeWidthPx--) | Hämtar bredden i pixelenheter efter anrop av metoden Chart.Calculate(). |
| [getShapeX()](#getShapeX--) | Hämtar x-koordinaten för det övre vänstra hörnet i enheter av 1/4000 av diagrammets bredd efter anrop av metoden Chart.Calculate(). |
| [getShapeXPx()](#getShapeXPx--) | Hämtar x-koordinaten för det övre vänstra hörnet i pixelenheter efter anrop av metoden Chart.Calculate(). |
| [getShapeY()](#getShapeY--) | Hämtar y-koordinaten för det övre vänstra hörnet i enheter av 1/4000 av diagrammets höjd efter anrop av metoden Chart.Calculate(). |
| [getShapeYPx()](#getShapeYPx--) | Hämtar y-koordinaten för det övre vänstra hörnet i pixelenheter efter anrop av metoden Chart.Calculate(). |
| [getStartAngle()](#getStartAngle--) | Hämtar startvinkeln för pajsektionen, mätt i grader medurs från x-axeln efter anrop av metoden Chart.Calculate(). |
| [getTopPointCount()](#getTopPointCount--) | Hämtar antalet toppunkter efter anrop av metoden Chart.Calculate(). |
| [getTopPointXPx(int index)](#getTopPointXPx-int-) | Hämtar x-koordinaten för formens toppunkt efter anrop av metoden Chart.Calculate(). |
| [getTopPointYPx(int index)](#getTopPointYPx-int-) | Hämtar y-koordinaten för formens toppunkt efter anrop av metoden Chart.Calculate(). |
| [getXValue()](#getXValue--) | Hämtar X‑värdet för diagrampunkten. |
| [getXValueType()](#getXValueType--) | Hämtar X‑värdestypen för diagrampunkten. |
| [getYValue()](#getYValue--) | Hämtar Y‑värdet för diagrampunkten. |
| [getYValueType()](#getYValueType--) | Hämtar Y‑värdestypen för diagrampunkten. |
| [hashCode()](#hashCode--) |  |
| [isInSecondaryPlot()](#isInSecondaryPlot--) | Hämtar ett värde som indikerar om denna datapunkt finns i den andra pajen eller stapeln i ett paj‑i‑paj‑eller‑stapel‑i‑paj‑diagram. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setExplosion(int value)](#setExplosion-int-) | Avståndet för en öppen pajskiva från mitten av pajdiagrammet uttrycks som en procentandel av pajens diameter. |
| [setInSecondaryPlot(boolean value)](#setInSecondaryPlot-boolean-) | Ställer in ett värde som indikerar om denna datapunkt är i den andra pie eller bar på en pie av pie eller bar i ett pie diagram |
| [setShadow(boolean value)](#setShadow-boolean-) | Sant om diagrampunkten har en skugga. |
| [setXValue(Object value)](#setXValue-java.lang.Object-) | Ställer in X‑värdet för diagrampunkten. |
| [setYValue(Object value)](#setYValue-java.lang.Object-) | Ställer in Y‑värdet för diagrampunkten. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getArcEndPointXPx() {#getArcEndPointXPx--}
```
public float getArcEndPointXPx()
```


Hämtar x‑koordinaten för slutpunkten för pie‑sektionen efter att ha anropat metoden Chart.Calculate(). Gäller för Pie‑ och Doughnut‑diagram.

**Returns:**
float
### getArcEndPointYPx() {#getArcEndPointYPx--}
```
public float getArcEndPointYPx()
```


Hämtar y‑koordinaten för slutpunkten för pie‑sektionen efter att ha anropat metoden Chart.Calculate(). Gäller för Pie‑ och Doughnut‑diagram.

**Returns:**
float
### getArcStartPointXPx() {#getArcStartPointXPx--}
```
public float getArcStartPointXPx()
```


Hämtar x‑koordinaten för startpunkten för pie‑sektionen efter att ha anropat metoden Chart.Calculate(). Gäller för Pie‑ och Doughnut‑diagram.

**Returns:**
float
### getArcStartPointYPx() {#getArcStartPointYPx--}
```
public float getArcStartPointYPx()
```


Hämtar y‑koordinaten för startpunkten för pie‑sektionen efter att ha anropat metoden Chart.Calculate(). Gäller för Pie‑ och Doughnut‑diagram.

**Returns:**
float
### getArea() {#getArea--}
```
public Area getArea()
```


Hämtar [getArea()](../../com.aspose.cells/chartpoint\#getArea--).

**Returns:**
[Area](../../com.aspose.cells/area)
### getBorder() {#getBorder--}
```
public Line getBorder()
```


Hämtar [Line](../../com.aspose.cells/line).

**Returns:**
[Line](../../com.aspose.cells/line)
### getBorderWidthPx() {#getBorderWidthPx--}
```
public int getBorderWidthPx()
```


Hämtar bredden på kanten i enheter av pixlar efter att ha anropat metoden Chart.Calculate().

**Returns:**
int
### getBottomPointCount() {#getBottomPointCount--}
```
public int getBottomPointCount()
```


Hämtar antalet bottenpunkter efter anrop av metoden Chart.Calculate().

**Returns:**
int
### getBottomPointXPx(int index) {#getBottomPointXPx-int-}
```
public float getBottomPointXPx(int index)
```


Hämtar x‑koordinaten för bottenpunkten på formen efter att ha anropat metoden Chart.Calculate(). Gäller för 3D‑diagram: Column3D, Bar3D, Cone, Cylinder, Pyramid.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int |  |

**Returns:**
float
### getBottomPointYPx(int index) {#getBottomPointYPx-int-}
```
public float getBottomPointYPx(int index)
```


Hämtar y‑koordinaten för bottenpunkten på formen efter att ha anropat metoden Chart.Calculate(). Gäller för 3D‑diagram: Column3D, Bar3D, Cone, Cylinder, Pyramid.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int |  |

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


Returnerar ett [getDataLabels()](../../com.aspose.cells/chartpoint\#getDataLabels--) objekt som representerar datamärket som är associerat med denna diagrampunkt.

**Returns:**
[DataLabels](../../com.aspose.cells/datalabels)
### getDoughnutInnerRadius() {#getDoughnutInnerRadius--}
```
public int getDoughnutInnerRadius()
```


Hämtar den inre radien för doughnut‑segmentet i pixelenheter efter att ha anropat metoden Chart.Calculate(). Gäller för Doughnut‑diagram.

**Returns:**
int
### getEndAngle() {#getEndAngle--}
```
public float getEndAngle()
```


Hämtar slutvinkeln för pie‑sektionen, mätt i grader medurs från x‑axeln efter att ha anropat metoden Chart.Calculate(). Gäller för Pie‑diagram.

**Returns:**
float
### getExplosion() {#getExplosion--}
```
public int getExplosion()
```


Avståndet för en öppen pajskiva från mitten av pajdiagrammet uttrycks som en procentandel av pajens diameter.

**Returns:**
int
### getInnerArcEndPointXPx() {#getInnerArcEndPointXPx--}
```
public float getInnerArcEndPointXPx()
```


Hämtar x‑koordinaten för slutpunkten för pie‑sektionen efter att ha anropat metoden Chart.Calculate(). Gäller för Doughnut‑diagram.

**Returns:**
float
### getInnerArcEndPointYPx() {#getInnerArcEndPointYPx--}
```
public float getInnerArcEndPointYPx()
```


Hämtar y‑koordinaten för slutpunkten för pie‑sektionen efter att ha anropat metoden Chart.Calculate(). Gäller för Doughnut‑diagram.

**Returns:**
float
### getInnerArcStartPointXPx() {#getInnerArcStartPointXPx--}
```
public float getInnerArcStartPointXPx()
```


Hämtar x‑koordinaten för startpunkten för pie‑sektionen efter att ha anropat metoden Chart.Calculate(). Gäller för Doughnut‑diagrammet.

**Returns:**
float
### getInnerArcStartPointYPx() {#getInnerArcStartPointYPx--}
```
public float getInnerArcStartPointYPx()
```


Hämtar y‑koordinaten för startpunkten för pie‑sektionen efter att ha anropat metoden Chart.Calculate(). Gäller för Doughnut‑diagram.

**Returns:**
float
### getInnerRadiusPx() {#getInnerRadiusPx--}
```
public int getInnerRadiusPx()
```


Hämtar den inre radien för doughnut‑segmentet i pixelenheter efter att ha anropat metoden Chart.Calculate(). Gäller för Doughnut‑diagram.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd i stället egenskapen ChartPoint.DoughnutInnerRadius. Denna egenskap kommer att tas bort 12 månader senare från och med juni 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
int
### getMarker() {#getMarker--}
```
public Marker getMarker()
```


Hämtar [getMarker()](../../com.aspose.cells/chartpoint\#getMarker--).

**Returns:**
[Marker](../../com.aspose.cells/marker)
### getOnCategoryAxisPointCount() {#getOnCategoryAxisPointCount--}
```
public int getOnCategoryAxisPointCount()
```


Hämtar antalet punkter på kategori‑axeln efter att ha anropat metoden Chart.Calculate(). Gäller endast för area‑diagram.

**Remarks**

Area‑2D‑diagram returnerar 1, Area‑3D‑diagram returnerar 2.

**Returns:**
int
### getOnCategoryAxisPointXPx(int index) {#getOnCategoryAxisPointXPx-int-}
```
public float getOnCategoryAxisPointXPx(int index)
```


Hämtar x‑koordinaten för punkten på kategori‑axeln efter att ha anropat metoden Chart.Calculate(). Gäller endast för Area‑diagram.

**Remarks**

Area‑2D‑diagram: index är 0. Area‑3D‑diagram: index är 0 eller 1.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int |  |

**Returns:**
float
### getOnCategoryAxisPointYPx(int index) {#getOnCategoryAxisPointYPx-int-}
```
public float getOnCategoryAxisPointYPx(int index)
```


Hämtar y‑koordinaten för punkten på kategori‑axeln efter att ha anropat metoden Chart.Calculate(). Gäller endast för Area‑diagram.

**Remarks**

Area‑2D‑diagram: index är 0. Area‑3D‑diagram: index är 0 eller 1.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int |  |

**Returns:**
float
### getRadiusPx() {#getRadiusPx--}
```
public int getRadiusPx()
```


Hämtar radien för bubbla, paj eller donut i pixelenheter efter anrop av metoden Chart.Calculate().

**Returns:**
int
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


Sant om diagrampunkten har en skugga.

**Returns:**
boolean
### getShapeHeight() {#getShapeHeight--}
```
public int getShapeHeight()
```


Hämtar höjden i enheter av 1/4000 av diagrammets höjd efter anrop av metoden Chart.Calculate().

**Returns:**
int
### getShapeHeightPx() {#getShapeHeightPx--}
```
public int getShapeHeightPx()
```


Hämtar höjden i pixelenheter efter anrop av metoden Chart.Calculate().

**Returns:**
int
### getShapeProperties() {#getShapeProperties--}
```
public ShapePropertyCollection getShapeProperties()
```


Hämtar objektet [ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection) som innehåller de visuella formegenskaperna för ChartPoint.

**Returns:**
[ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection)
### getShapeWidth() {#getShapeWidth--}
```
public int getShapeWidth()
```


Hämtar bredden i enheter av 1/4000 av diagrammets bredd efter anrop av metoden Chart.Calculate().

**Returns:**
int
### getShapeWidthPx() {#getShapeWidthPx--}
```
public int getShapeWidthPx()
```


Hämtar bredden i pixelenheter efter anrop av metoden Chart.Calculate().

**Returns:**
int
### getShapeX() {#getShapeX--}
```
public int getShapeX()
```


Hämtar x-koordinaten för det övre vänstra hörnet i enheter av 1/4000 av diagrammets bredd efter anrop av metoden Chart.Calculate().

**Returns:**
int
### getShapeXPx() {#getShapeXPx--}
```
public int getShapeXPx()
```


Hämtar x-koordinaten för det övre vänstra hörnet i pixelenheter efter anrop av metoden Chart.Calculate().

**Returns:**
int
### getShapeY() {#getShapeY--}
```
public int getShapeY()
```


Hämtar y-koordinaten för det övre vänstra hörnet i enheter av 1/4000 av diagrammets höjd efter anrop av metoden Chart.Calculate().

**Returns:**
int
### getShapeYPx() {#getShapeYPx--}
```
public int getShapeYPx()
```


Hämtar y-koordinaten för det övre vänstra hörnet i pixelenheter efter anrop av metoden Chart.Calculate().

**Returns:**
int
### getStartAngle() {#getStartAngle--}
```
public float getStartAngle()
```


Hämtar startvinkeln för pie‑sektionen, mätt i grader medurs från x‑axeln efter att ha anropat metoden Chart.Calculate(). Gäller för Pie‑diagram.

**Returns:**
float
### getTopPointCount() {#getTopPointCount--}
```
public int getTopPointCount()
```


Hämtar antalet toppunkter efter anrop av metoden Chart.Calculate().

**Returns:**
int
### getTopPointXPx(int index) {#getTopPointXPx-int-}
```
public float getTopPointXPx(int index)
```


Hämtar x‑koordinaten för toppunkten på formen efter att ha anropat metoden Chart.Calculate(). Gäller för 3D‑diagram: Column3D, Bar3D, Cone, Cylinder, Pyramid och Area3D.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int |  |

**Returns:**
float
### getTopPointYPx(int index) {#getTopPointYPx-int-}
```
public float getTopPointYPx(int index)
```


Hämtar y‑koordinaten för toppunkten på formen efter att ha anropat metoden Chart.Calculate(). Gäller för 3D‑diagram: Column3D, Bar3D, Cone, Cylinder, Pyramid och Area3D.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int |  |

**Returns:**
float
### getXValue() {#getXValue--}
```
public Object getXValue()
```


Hämtar X‑värdet för diagrampunkten.

**Returns:**
java.lang.Object
### getXValueType() {#getXValueType--}
```
public int getXValueType()
```


Hämtar X‑värdestypen för diagrampunkten.

Se [CellValueType](../../com.aspose.cells/cellvaluetype).

**Returns:**
int
### getYValue() {#getYValue--}
```
public Object getYValue()
```


Hämtar Y‑värdet för diagrampunkten.

**Returns:**
java.lang.Object
### getYValueType() {#getYValueType--}
```
public int getYValueType()
```


Hämtar Y‑värdestypen för diagrampunkten.

Se [CellValueType](../../com.aspose.cells/cellvaluetype).

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


Hämtar ett värde som indikerar om denna datapunkt finns i den andra pajen eller stapeln i ett paj‑i‑paj‑eller‑stapel‑i‑paj‑diagram.

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


Avståndet för en öppen pajskiva från mitten av pajdiagrammet uttrycks som en procentandel av pajens diameter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setInSecondaryPlot(boolean value) {#setInSecondaryPlot-boolean-}
```
public void setInSecondaryPlot(boolean value)
```


Ställer in ett värde som indikerar om denna datapunkt är i den andra pie eller bar på en pie av pie eller bar i ett pie diagram

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


Sant om diagrampunkten har en skugga.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setXValue(Object value) {#setXValue-java.lang.Object-}
```
public void setXValue(Object value)
```


Ställer in X‑värdet för diagrampunkten.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.Object |  |

### setYValue(Object value) {#setYValue-java.lang.Object-}
```
public void setYValue(Object value)
```


Ställer in Y‑värdet för diagrampunkten.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.Object |  |

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

