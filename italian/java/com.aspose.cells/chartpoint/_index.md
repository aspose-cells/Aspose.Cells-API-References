---
title: "ChartPoint"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta un singolo punto in una serie di un grafico."
type: docs
url: /it/java/com.aspose.cells/chartpoint/
---

**Inheritance:**
java.lang.Object
```
public class ChartPoint
```

Rappresenta un singolo punto in una serie di un grafico.

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
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArcEndPointXPx()](#getArcEndPointXPx--) | Restituisce la coordinata x del punto finale della sezione a torta dopo aver chiamato il metodo Chart.Calculate(). |
| [getArcEndPointYPx()](#getArcEndPointYPx--) | Restituisce la coordinata y del punto finale della sezione a torta dopo aver chiamato il metodo Chart.Calculate(). |
| [getArcStartPointXPx()](#getArcStartPointXPx--) | Ottiene la coordinata x del punto di partenza della sezione a torta dopo aver chiamato il metodo Chart.Calculate(). |
| [getArcStartPointYPx()](#getArcStartPointYPx--) | Ottiene la coordinata y del punto di partenza della sezione a torta dopo aver chiamato il metodo Chart.Calculate(). |
| [getArea()](#getArea--) | Ottiene il [getArea()](../../com.aspose.cells/chartpoint\#getArea--). |
| [getBorder()](#getBorder--) | Ottiene il [Line](../../com.aspose.cells/line). |
| [getBorderWidthPx()](#getBorderWidthPx--) | Ottiene la larghezza del bordo in unità di pixel dopo aver chiamato il metodo Chart.Calculate(). |
| [getBottomPointCount()](#getBottomPointCount--) | Ottiene il numero di punti inferiori dopo aver chiamato il metodo Chart.Calculate(). |
| [getBottomPointXPx(int index)](#getBottomPointXPx-int-) | Ottiene la coordinata x del punto inferiore della forma dopo aver chiamato il metodo Chart.Calculate(). |
| [getBottomPointYPx(int index)](#getBottomPointYPx-int-) | Ottiene la coordinata y del punto inferiore della forma dopo aver chiamato il metodo Chart.Calculate(). |
| [getClass()](#getClass--) |  |
| [getDataLabels()](#getDataLabels--) | Restituisce un oggetto [getDataLabels()](../../com.aspose.cells/chartpoint\#getDataLabels--) che rappresenta l'etichetta dati associata a questo punto del grafico. |
| [getDoughnutInnerRadius()](#getDoughnutInnerRadius--) | Ottiene il raggio interno della fetta di ciambella in unità di pixel dopo aver chiamato il metodo Chart.Calculate(). |
| [getEndAngle()](#getEndAngle--) | Ottiene l'angolo finale della sezione a torta, misurato in gradi in senso orario dall'asse x dopo aver chiamato il metodo Chart.Calculate(). |
| [getExplosion()](#getExplosion--) | La distanza di una fetta di torta aperta dal centro del grafico a torta è espressa come percentuale del diametro della torta. |
| [getInnerArcEndPointXPx()](#getInnerArcEndPointXPx--) | Restituisce la coordinata x del punto finale della sezione a torta dopo aver chiamato il metodo Chart.Calculate(). |
| [getInnerArcEndPointYPx()](#getInnerArcEndPointYPx--) | Restituisce la coordinata y del punto finale della sezione a torta dopo aver chiamato il metodo Chart.Calculate(). |
| [getInnerArcStartPointXPx()](#getInnerArcStartPointXPx--) | Ottiene la coordinata x del punto di partenza della sezione a torta dopo aver chiamato il metodo Chart.Calculate(). |
| [getInnerArcStartPointYPx()](#getInnerArcStartPointYPx--) | Ottiene la coordinata y del punto di partenza della sezione a torta dopo aver chiamato il metodo Chart.Calculate(). |
| [getInnerRadiusPx()](#getInnerRadiusPx--) | Ottiene il raggio interno della fetta di ciambella in unità di pixel dopo aver chiamato il metodo Chart.Calculate(). |
| [getMarker()](#getMarker--) | Ottiene il [getMarker()](../../com.aspose.cells/chartpoint\#getMarker--). |
| [getOnCategoryAxisPointCount()](#getOnCategoryAxisPointCount--) | Ottiene il numero dei punti sull'asse delle categorie dopo aver chiamato il metodo Chart.Calculate(). |
| [getOnCategoryAxisPointXPx(int index)](#getOnCategoryAxisPointXPx-int-) | Ottiene la coordinata x del punto sull'asse delle categorie dopo aver chiamato il metodo Chart.Calculate(). |
| [getOnCategoryAxisPointYPx(int index)](#getOnCategoryAxisPointYPx-int-) | Ottiene la coordinata y del punto sull'asse delle categorie dopo aver chiamato il metodo Chart.Calculate(). |
| [getRadiusPx()](#getRadiusPx--) | Ottiene il raggio di bolla, torta o ciambella in unità di pixel dopo aver chiamato il metodo Chart.Calculate(). |
| [getShadow()](#getShadow--) | Vero se il punto del grafico ha un'ombra. |
| [getShapeHeight()](#getShapeHeight--) | Ottiene l'altezza in unità di 1/4000 dell'altezza del grafico dopo aver chiamato il metodo Chart.Calculate(). |
| [getShapeHeightPx()](#getShapeHeightPx--) | Ottiene l'altezza in unità di pixel dopo aver chiamato il metodo Chart.Calculate(). |
| [getShapeProperties()](#getShapeProperties--) | Ottiene l'oggetto [ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection) che contiene le proprietà visive della forma del ChartPoint. |
| [getShapeWidth()](#getShapeWidth--) | Ottiene la larghezza in unità di 1/4000 della larghezza del grafico dopo aver chiamato il metodo Chart.Calculate(). |
| [getShapeWidthPx()](#getShapeWidthPx--) | Ottiene la larghezza in unità di pixel dopo aver chiamato il metodo Chart.Calculate(). |
| [getShapeX()](#getShapeX--) | Ottiene la coordinata x dell'angolo in alto a sinistra in unità di 1/4000 della larghezza del grafico dopo aver chiamato il metodo Chart.Calculate(). |
| [getShapeXPx()](#getShapeXPx--) | Ottiene la coordinata x dell'angolo in alto a sinistra in unità di pixel dopo aver chiamato il metodo Chart.Calculate(). |
| [getShapeY()](#getShapeY--) | Restituisce la coordinata y dell'angolo in alto a sinistra in unità di 1/4000 dell'altezza del grafico dopo aver chiamato il metodo Chart.Calculate(). |
| [getShapeYPx()](#getShapeYPx--) | Restituisce la coordinata y dell'angolo in alto a sinistra in unità di pixel dopo aver chiamato il metodo Chart.Calculate(). |
| [getStartAngle()](#getStartAngle--) | Restituisce l'angolo iniziale della sezione a torta, misurato in gradi in senso orario dall'asse x dopo aver chiamato il metodo Chart.Calculate(). |
| [getTopPointCount()](#getTopPointCount--) | Restituisce il numero di punti superiori dopo aver chiamato il metodo Chart.Calculate(). |
| [getTopPointXPx(int index)](#getTopPointXPx-int-) | Restituisce la coordinata x del punto superiore della forma dopo aver chiamato il metodo Chart.Calculate(). |
| [getTopPointYPx(int index)](#getTopPointYPx-int-) | Restituisce la coordinata y del punto superiore della forma dopo aver chiamato il metodo Chart.Calculate(). |
| [getXValue()](#getXValue--) | Restituisce il valore X del punto del grafico. |
| [getXValueType()](#getXValueType--) | Restituisce il tipo di valore X del punto del grafico. |
| [getYValue()](#getYValue--) | Restituisce il valore Y del punto del grafico. |
| [getYValueType()](#getYValueType--) | Restituisce il tipo di valore Y del punto del grafico. |
| [hashCode()](#hashCode--) |  |
| [isInSecondaryPlot()](#isInSecondaryPlot--) | Restituisce un valore che indica se questo punto dati è nella seconda torta o barra in un grafico a torta di torta o barra di torta. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setExplosion(int value)](#setExplosion-int-) | La distanza di una fetta di torta aperta dal centro del grafico a torta è espressa come percentuale del diametro della torta. |
| [setInSecondaryPlot(boolean value)](#setInSecondaryPlot-boolean-) | Imposta un valore che indica se questo punto dati è nella seconda torta o barra in un grafico a torta di torta o barra di torta. |
| [setShadow(boolean value)](#setShadow-boolean-) | Vero se il punto del grafico ha un'ombra. |
| [setXValue(Object value)](#setXValue-java.lang.Object-) | Imposta il valore X del punto del grafico. |
| [setYValue(Object value)](#setYValue-java.lang.Object-) | Imposta il valore Y del punto del grafico. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getArcEndPointXPx() {#getArcEndPointXPx--}
```
public float getArcEndPointXPx()
```


Restituisce la coordinata x del punto finale della sezione a torta dopo aver chiamato il metodo Chart.Calculate(). Si applica ai grafici a torta e ciambella.

**Returns:**
float
### getArcEndPointYPx() {#getArcEndPointYPx--}
```
public float getArcEndPointYPx()
```


Restituisce la coordinata y del punto finale della sezione a torta dopo aver chiamato il metodo Chart.Calculate(). Si applica ai grafici a torta e ciambella.

**Returns:**
float
### getArcStartPointXPx() {#getArcStartPointXPx--}
```
public float getArcStartPointXPx()
```


Restituisce la coordinata x del punto iniziale della sezione a torta dopo aver chiamato il metodo Chart.Calculate(). Si applica ai grafici a torta e ciambella.

**Returns:**
float
### getArcStartPointYPx() {#getArcStartPointYPx--}
```
public float getArcStartPointYPx()
```


Restituisce la coordinata y del punto iniziale della sezione a torta dopo aver chiamato il metodo Chart.Calculate(). Si applica ai grafici a torta e ciambella.

**Returns:**
float
### getArea() {#getArea--}
```
public Area getArea()
```


Ottiene il [getArea()](../../com.aspose.cells/chartpoint\#getArea--).

**Returns:**
[Area](../../com.aspose.cells/area)
### getBorder() {#getBorder--}
```
public Line getBorder()
```


Ottiene il [Line](../../com.aspose.cells/line).

**Returns:**
[Line](../../com.aspose.cells/line)
### getBorderWidthPx() {#getBorderWidthPx--}
```
public int getBorderWidthPx()
```


Ottiene la larghezza del bordo in unità di pixel dopo aver chiamato il metodo Chart.Calculate().

**Returns:**
int
### getBottomPointCount() {#getBottomPointCount--}
```
public int getBottomPointCount()
```


Ottiene il numero di punti inferiori dopo aver chiamato il metodo Chart.Calculate().

**Returns:**
int
### getBottomPointXPx(int index) {#getBottomPointXPx-int-}
```
public float getBottomPointXPx(int index)
```


Restituisce la coordinata x del punto inferiore della forma dopo aver chiamato il metodo Chart.Calculate(). Si applica ai grafici 3D: Column3D, Bar3D, Cone, Cylinder, Pyramid.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int |  |

**Returns:**
float
### getBottomPointYPx(int index) {#getBottomPointYPx-int-}
```
public float getBottomPointYPx(int index)
```


Restituisce la coordinata y del punto inferiore della forma dopo aver chiamato il metodo Chart.Calculate(). Si applica ai grafici 3D: Column3D, Bar3D, Cone, Cylinder, Pyramid.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int |  |

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


Restituisce un oggetto [getDataLabels()](../../com.aspose.cells/chartpoint\#getDataLabels--) che rappresenta l'etichetta dati associata a questo punto del grafico.

**Returns:**
[DataLabels](../../com.aspose.cells/datalabels)
### getDoughnutInnerRadius() {#getDoughnutInnerRadius--}
```
public int getDoughnutInnerRadius()
```


Restituisce il raggio interno della fetta di ciambella in unità di pixel dopo aver chiamato il metodo Chart.Calculate(). Si applica al grafico ciambella.

**Returns:**
int
### getEndAngle() {#getEndAngle--}
```
public float getEndAngle()
```


Restituisce l'angolo finale della sezione a torta, misurato in gradi in senso orario dall'asse x dopo aver chiamato il metodo Chart.Calculate(). Si applica al grafico a torta.

**Returns:**
float
### getExplosion() {#getExplosion--}
```
public int getExplosion()
```


La distanza di una fetta di torta aperta dal centro del grafico a torta è espressa come percentuale del diametro della torta.

**Returns:**
int
### getInnerArcEndPointXPx() {#getInnerArcEndPointXPx--}
```
public float getInnerArcEndPointXPx()
```


Restituisce la coordinata x del punto finale della sezione a torta dopo aver chiamato il metodo Chart.Calculate(). Si applica ai grafici ciambella.

**Returns:**
float
### getInnerArcEndPointYPx() {#getInnerArcEndPointYPx--}
```
public float getInnerArcEndPointYPx()
```


Restituisce la coordinata y del punto finale della sezione a torta dopo aver chiamato il metodo Chart.Calculate(). Si applica al grafico ciambella.

**Returns:**
float
### getInnerArcStartPointXPx() {#getInnerArcStartPointXPx--}
```
public float getInnerArcStartPointXPx()
```


Restituisce la coordinata x del punto iniziale della sezione a torta dopo aver chiamato il metodo Chart.Calculate(). Si applica al grafico ciambella.

**Returns:**
float
### getInnerArcStartPointYPx() {#getInnerArcStartPointYPx--}
```
public float getInnerArcStartPointYPx()
```


Restituisce la coordinata y del punto di partenza della sezione a torta dopo le chiamate al metodo Chart.Calculate(). Si applica al grafico a ciambella.

**Returns:**
float
### getInnerRadiusPx() {#getInnerRadiusPx--}
```
public int getInnerRadiusPx()
```


Restituisce il raggio interno della fetta di ciambella in unità di pixel dopo le chiamate al metodo Chart.Calculate(). Si applica al grafico a ciambella.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà ChartPoint.DoughnutInnerRadius. Questa proprietà sarà rimossa 12 mesi dopo, a partire da giugno 2024. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
int
### getMarker() {#getMarker--}
```
public Marker getMarker()
```


Ottiene il [getMarker()](../../com.aspose.cells/chartpoint\#getMarker--).

**Returns:**
[Marker](../../com.aspose.cells/marker)
### getOnCategoryAxisPointCount() {#getOnCategoryAxisPointCount--}
```
public int getOnCategoryAxisPointCount()
```


Restituisce il numero di punti sull'asse delle categorie dopo aver chiamato il metodo Chart.Calculate(). Si applica solo ai grafici ad area.

**Remarks**

Il grafico area 2D restituisce 1, il grafico area 3D restituisce 2.

**Returns:**
int
### getOnCategoryAxisPointXPx(int index) {#getOnCategoryAxisPointXPx-int-}
```
public float getOnCategoryAxisPointXPx(int index)
```


Restituisce la coordinata x del punto sull'asse delle categorie dopo le chiamate al metodo Chart.Calculate(). Si applica solo al grafico ad area.

**Remarks**

Grafico area 2D: l'indice è 0. Grafico area 3D: l'indice è 0 o 1.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int |  |

**Returns:**
float
### getOnCategoryAxisPointYPx(int index) {#getOnCategoryAxisPointYPx-int-}
```
public float getOnCategoryAxisPointYPx(int index)
```


Restituisce la coordinata y del punto sull'asse delle categorie dopo aver chiamato il metodo Chart.Calculate(). Si applica solo al grafico ad area.

**Remarks**

Grafico area 2D: l'indice è 0. Grafico area 3D: l'indice è 0 o 1.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int |  |

**Returns:**
float
### getRadiusPx() {#getRadiusPx--}
```
public int getRadiusPx()
```


Ottiene il raggio di bolla, torta o ciambella in unità di pixel dopo aver chiamato il metodo Chart.Calculate().

**Returns:**
int
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


Vero se il punto del grafico ha un'ombra.

**Returns:**
boolean
### getShapeHeight() {#getShapeHeight--}
```
public int getShapeHeight()
```


Ottiene l'altezza in unità di 1/4000 dell'altezza del grafico dopo aver chiamato il metodo Chart.Calculate().

**Returns:**
int
### getShapeHeightPx() {#getShapeHeightPx--}
```
public int getShapeHeightPx()
```


Ottiene l'altezza in unità di pixel dopo aver chiamato il metodo Chart.Calculate().

**Returns:**
int
### getShapeProperties() {#getShapeProperties--}
```
public ShapePropertyCollection getShapeProperties()
```


Ottiene l'oggetto [ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection) che contiene le proprietà visive della forma del ChartPoint.

**Returns:**
[ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection)
### getShapeWidth() {#getShapeWidth--}
```
public int getShapeWidth()
```


Ottiene la larghezza in unità di 1/4000 della larghezza del grafico dopo aver chiamato il metodo Chart.Calculate().

**Returns:**
int
### getShapeWidthPx() {#getShapeWidthPx--}
```
public int getShapeWidthPx()
```


Ottiene la larghezza in unità di pixel dopo aver chiamato il metodo Chart.Calculate().

**Returns:**
int
### getShapeX() {#getShapeX--}
```
public int getShapeX()
```


Ottiene la coordinata x dell'angolo in alto a sinistra in unità di 1/4000 della larghezza del grafico dopo aver chiamato il metodo Chart.Calculate().

**Returns:**
int
### getShapeXPx() {#getShapeXPx--}
```
public int getShapeXPx()
```


Ottiene la coordinata x dell'angolo in alto a sinistra in unità di pixel dopo aver chiamato il metodo Chart.Calculate().

**Returns:**
int
### getShapeY() {#getShapeY--}
```
public int getShapeY()
```


Restituisce la coordinata y dell'angolo in alto a sinistra in unità di 1/4000 dell'altezza del grafico dopo aver chiamato il metodo Chart.Calculate().

**Returns:**
int
### getShapeYPx() {#getShapeYPx--}
```
public int getShapeYPx()
```


Restituisce la coordinata y dell'angolo in alto a sinistra in unità di pixel dopo aver chiamato il metodo Chart.Calculate().

**Returns:**
int
### getStartAngle() {#getStartAngle--}
```
public float getStartAngle()
```


Restituisce l'angolo di partenza per la sezione a torta, misurato in gradi in senso orario dall'asse x dopo aver chiamato il metodo Chart.Calculate(). Si applica al grafico a torta.

**Returns:**
float
### getTopPointCount() {#getTopPointCount--}
```
public int getTopPointCount()
```


Restituisce il numero di punti superiori dopo aver chiamato il metodo Chart.Calculate().

**Returns:**
int
### getTopPointXPx(int index) {#getTopPointXPx-int-}
```
public float getTopPointXPx(int index)
```


Restituisce la coordinata x del punto superiore della forma dopo le chiamate al metodo Chart.Calculate(). Si applica ai grafici 3D: Column3D, Bar3D, Cone, Cylinder, Pyramid e Area3D

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int |  |

**Returns:**
float
### getTopPointYPx(int index) {#getTopPointYPx-int-}
```
public float getTopPointYPx(int index)
```


Restituisce la coordinata y del punto superiore della forma dopo aver chiamato il metodo Chart.Calculate(). Si applica ai grafici 3D: Column3D, Bar3D, Cone, Cylinder, Pyramid e Area3D.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int |  |

**Returns:**
float
### getXValue() {#getXValue--}
```
public Object getXValue()
```


Restituisce il valore X del punto del grafico.

**Returns:**
java.lang.Object
### getXValueType() {#getXValueType--}
```
public int getXValueType()
```


Restituisce il tipo di valore X del punto del grafico.

Vedi [CellValueType](../../com.aspose.cells/cellvaluetype).

**Returns:**
int
### getYValue() {#getYValue--}
```
public Object getYValue()
```


Restituisce il valore Y del punto del grafico.

**Returns:**
java.lang.Object
### getYValueType() {#getYValueType--}
```
public int getYValueType()
```


Restituisce il tipo di valore Y del punto del grafico.

Vedi [CellValueType](../../com.aspose.cells/cellvaluetype).

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


Restituisce un valore che indica se questo punto dati è nella seconda torta o barra in un grafico a torta di torta o barra di torta.

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


La distanza di una fetta di torta aperta dal centro del grafico a torta è espressa come percentuale del diametro della torta.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setInSecondaryPlot(boolean value) {#setInSecondaryPlot-boolean-}
```
public void setInSecondaryPlot(boolean value)
```


Imposta un valore che indica se questo punto dati è nella seconda torta o barra in un grafico a torta di torta o barra di torta.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


Vero se il punto del grafico ha un'ombra.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setXValue(Object value) {#setXValue-java.lang.Object-}
```
public void setXValue(Object value)
```


Imposta il valore X del punto del grafico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.Object |  |

### setYValue(Object value) {#setYValue-java.lang.Object-}
```
public void setYValue(Object value)
```


Imposta il valore Y del punto del grafico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.Object |  |

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

