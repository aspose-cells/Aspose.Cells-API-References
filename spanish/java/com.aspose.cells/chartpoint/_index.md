---
title: "ChartPoint"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa un único punto en una serie de un gráfico."
type: docs
url: /es/java/com.aspose.cells/chartpoint/
---

**Inheritance:**
java.lang.Object
```
public class ChartPoint
```

Representa un único punto en una serie de un gráfico.

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
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArcEndPointXPx()](#getArcEndPointXPx--) | Obtiene la coordenada x del punto final de la sección de pastel después de llamar al método Chart.Calculate(). |
| [getArcEndPointYPx()](#getArcEndPointYPx--) | Obtiene la coordenada y del punto final de la sección de pastel después de llamar al método Chart.Calculate(). |
| [getArcStartPointXPx()](#getArcStartPointXPx--) | Obtiene la coordenada x del punto de inicio de la sección de pastel después de llamar al método Chart.Calculate(). |
| [getArcStartPointYPx()](#getArcStartPointYPx--) | Obtiene la coordenada y del punto de inicio de la sección de pastel después de llamar al método Chart.Calculate(). |
| [getArea()](#getArea--) | Obtiene el [getArea()](../../com.aspose.cells/chartpoint\#getArea--). |
| [getBorder()](#getBorder--) | Obtiene el [Line](../../com.aspose.cells/line). |
| [getBorderWidthPx()](#getBorderWidthPx--) | Obtiene el ancho del borde en unidades de píxeles después de llamar al método Chart.Calculate(). |
| [getBottomPointCount()](#getBottomPointCount--) | Obtiene el número de puntos inferiores después de llamar al método Chart.Calculate(). |
| [getBottomPointXPx(int index)](#getBottomPointXPx-int-) | Obtiene la coordenada x del punto inferior de la forma después de llamar al método Chart.Calculate(). |
| [getBottomPointYPx(int index)](#getBottomPointYPx-int-) | Obtiene la coordenada y del punto inferior de la forma después de llamar al método Chart.Calculate(). |
| [getClass()](#getClass--) |  |
| [getDataLabels()](#getDataLabels--) | Devuelve un objeto [getDataLabels()](../../com.aspose.cells/chartpoint\#getDataLabels--) que representa la etiqueta de datos asociada a este punto del gráfico. |
| [getDoughnutInnerRadius()](#getDoughnutInnerRadius--) | Obtiene el radio interno de la porción de dona en unidades de píxeles después de llamar al método Chart.Calculate(). |
| [getEndAngle()](#getEndAngle--) | Obtiene el ángulo final de la sección de pastel, medido en grados en sentido horario desde el eje x después de llamar al método Chart.Calculate(). |
| [getExplosion()](#getExplosion--) | La distancia de una porción de pastel abierta desde el centro del gráfico de pastel se expresa como un porcentaje del diámetro del pastel. |
| [getInnerArcEndPointXPx()](#getInnerArcEndPointXPx--) | Obtiene la coordenada x del punto final de la sección de pastel después de llamar al método Chart.Calculate(). |
| [getInnerArcEndPointYPx()](#getInnerArcEndPointYPx--) | Obtiene la coordenada y del punto final de la sección de pastel después de llamar al método Chart.Calculate(). |
| [getInnerArcStartPointXPx()](#getInnerArcStartPointXPx--) | Obtiene la coordenada x del punto de inicio de la sección de pastel después de llamar al método Chart.Calculate(). |
| [getInnerArcStartPointYPx()](#getInnerArcStartPointYPx--) | Obtiene la coordenada y del punto de inicio de la sección de pastel después de llamar al método Chart.Calculate(). |
| [getInnerRadiusPx()](#getInnerRadiusPx--) | Obtiene el radio interno de la porción de dona en unidades de píxeles después de llamar al método Chart.Calculate(). |
| [getMarker()](#getMarker--) | Obtiene el [getMarker()](../../com.aspose.cells/chartpoint\#getMarker--). |
| [getOnCategoryAxisPointCount()](#getOnCategoryAxisPointCount--) | Obtiene el número de puntos en el eje de categorías después de llamar al método Chart.Calculate(). |
| [getOnCategoryAxisPointXPx(int index)](#getOnCategoryAxisPointXPx-int-) | Obtiene la coordenada x del punto en el eje de categorías después de llamar al método Chart.Calculate(). |
| [getOnCategoryAxisPointYPx(int index)](#getOnCategoryAxisPointYPx-int-) | Obtiene la coordenada y del punto en el eje de categorías después de llamar al método Chart.Calculate(). |
| [getRadiusPx()](#getRadiusPx--) | Obtiene el radio de la burbuja, pastel o dona en unidades de píxeles después de llamar al método Chart.Calculate(). |
| [getShadow()](#getShadow--) | Verdadero si el punto del gráfico tiene una sombra. |
| [getShapeHeight()](#getShapeHeight--) | Obtiene la altura en unidades de 1/4000 de la altura del gráfico después de llamar al método Chart.Calculate(). |
| [getShapeHeightPx()](#getShapeHeightPx--) | Obtiene la altura en unidades de píxeles después de llamar al método Chart.Calculate(). |
| [getShapeProperties()](#getShapeProperties--) | Obtiene el objeto [ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection) que contiene las propiedades visuales de la forma del ChartPoint. |
| [getShapeWidth()](#getShapeWidth--) | Obtiene el ancho en unidades de 1/4000 del ancho del gráfico después de llamar al método Chart.Calculate(). |
| [getShapeWidthPx()](#getShapeWidthPx--) | Obtiene el ancho en unidades de píxeles después de llamar al método Chart.Calculate(). |
| [getShapeX()](#getShapeX--) | Obtiene la coordenada x de la esquina superior izquierda en unidades de 1/4000 del ancho del gráfico después de llamar al método Chart.Calculate(). |
| [getShapeXPx()](#getShapeXPx--) | Obtiene la coordenada x de la esquina superior izquierda en unidades de píxeles después de llamar al método Chart.Calculate(). |
| [getShapeY()](#getShapeY--) | Obtiene la coordenada y de la esquina superior izquierda en unidades de 1/4000 de la altura del gráfico después de llamar al método Chart.Calculate(). |
| [getShapeYPx()](#getShapeYPx--) | Obtiene la coordenada y de la esquina superior izquierda en unidades de píxeles después de llamar al método Chart.Calculate(). |
| [getStartAngle()](#getStartAngle--) | Obtiene el ángulo inicial para la sección de pastel, medido en grados en sentido horario desde el eje x después de llamar al método Chart.Calculate(). |
| [getTopPointCount()](#getTopPointCount--) | Obtiene el número de puntos superiores después de llamar al método Chart.Calculate(). |
| [getTopPointXPx(int index)](#getTopPointXPx-int-) | Obtiene la coordenada x del punto superior de la forma después de llamar al método Chart.Calculate(). |
| [getTopPointYPx(int index)](#getTopPointYPx-int-) | Obtiene la coordenada y del punto superior de la forma después de llamar al método Chart.Calculate(). |
| [getXValue()](#getXValue--) | Obtiene el valor X del punto del gráfico. |
| [getXValueType()](#getXValueType--) | Obtiene el tipo de valor X del punto del gráfico. |
| [getYValue()](#getYValue--) | Obtiene el valor Y del punto del gráfico. |
| [getYValueType()](#getYValueType--) | Obtiene el tipo de valor Y del punto del gráfico. |
| [hashCode()](#hashCode--) |  |
| [isInSecondaryPlot()](#isInSecondaryPlot--) | Obtiene un valor que indica si este punto de datos está en el segundo pastel o barra en un gráfico de pastel dentro de pastel o barra dentro de pastel. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setExplosion(int value)](#setExplosion-int-) | La distancia de una porción de pastel abierta desde el centro del gráfico de pastel se expresa como un porcentaje del diámetro del pastel. |
| [setInSecondaryPlot(boolean value)](#setInSecondaryPlot-boolean-) | Establece un valor que indica si este punto de datos está en el segundo pastel o barra en un gráfico de pastel dentro de pastel o barra dentro de pastel. |
| [setShadow(boolean value)](#setShadow-boolean-) | Verdadero si el punto del gráfico tiene una sombra. |
| [setXValue(Object value)](#setXValue-java.lang.Object-) | Establece el valor X del punto del gráfico. |
| [setYValue(Object value)](#setYValue-java.lang.Object-) | Establece el valor Y del punto del gráfico. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getArcEndPointXPx() {#getArcEndPointXPx--}
```
public float getArcEndPointXPx()
```


Obtiene la coordenada x del punto final de la sección de pastel después de llamar al método Chart.Calculate(). Se aplica a los gráficos de pastel y rosquilla.

**Returns:**
float
### getArcEndPointYPx() {#getArcEndPointYPx--}
```
public float getArcEndPointYPx()
```


Obtiene la coordenada y del punto final de la sección de pastel después de llamar al método Chart.Calculate(). Se aplica a los gráficos de pastel y rosquilla.

**Returns:**
float
### getArcStartPointXPx() {#getArcStartPointXPx--}
```
public float getArcStartPointXPx()
```


Obtiene la coordenada x del punto inicial de la sección de pastel después de llamar al método Chart.Calculate(). Se aplica a los gráficos de pastel y rosquilla.

**Returns:**
float
### getArcStartPointYPx() {#getArcStartPointYPx--}
```
public float getArcStartPointYPx()
```


Obtiene la coordenada y del punto inicial de la sección de pastel después de llamar al método Chart.Calculate(). Se aplica a los gráficos de pastel y rosquilla.

**Returns:**
float
### getArea() {#getArea--}
```
public Area getArea()
```


Obtiene el [getArea()](../../com.aspose.cells/chartpoint\#getArea--).

**Returns:**
[Area](../../com.aspose.cells/area)
### getBorder() {#getBorder--}
```
public Line getBorder()
```


Obtiene el [Line](../../com.aspose.cells/line).

**Returns:**
[Line](../../com.aspose.cells/line)
### getBorderWidthPx() {#getBorderWidthPx--}
```
public int getBorderWidthPx()
```


Obtiene el ancho del borde en unidades de píxeles después de llamar al método Chart.Calculate().

**Returns:**
int
### getBottomPointCount() {#getBottomPointCount--}
```
public int getBottomPointCount()
```


Obtiene el número de puntos inferiores después de llamar al método Chart.Calculate().

**Returns:**
int
### getBottomPointXPx(int index) {#getBottomPointXPx-int-}
```
public float getBottomPointXPx(int index)
```


Obtiene la coordenada x del punto inferior de la forma después de llamar al método Chart.Calculate(). Se aplica a los gráficos 3D: Column3D, Bar3D, Cone, Cylinder, Pyramid.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int |  |

**Returns:**
float
### getBottomPointYPx(int index) {#getBottomPointYPx-int-}
```
public float getBottomPointYPx(int index)
```


Obtiene la coordenada y del punto inferior de la forma después de llamar al método Chart.Calculate(). Se aplica a los gráficos 3D: Column3D, Bar3D, Cone, Cylinder, Pyramid.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int |  |

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


Devuelve un objeto [getDataLabels()](../../com.aspose.cells/chartpoint\#getDataLabels--) que representa la etiqueta de datos asociada a este punto del gráfico.

**Returns:**
[DataLabels](../../com.aspose.cells/datalabels)
### getDoughnutInnerRadius() {#getDoughnutInnerRadius--}
```
public int getDoughnutInnerRadius()
```


Obtiene el radio interno de la porción de rosquilla en unidades de píxeles después de llamar al método Chart.Calculate(). Se aplica al gráfico de rosquilla.

**Returns:**
int
### getEndAngle() {#getEndAngle--}
```
public float getEndAngle()
```


Obtiene el ángulo final de la sección de pastel, medido en grados en sentido horario desde el eje x después de llamar al método Chart.Calculate(). Se aplica al gráfico de pastel.

**Returns:**
float
### getExplosion() {#getExplosion--}
```
public int getExplosion()
```


La distancia de una porción de pastel abierta desde el centro del gráfico de pastel se expresa como un porcentaje del diámetro del pastel.

**Returns:**
int
### getInnerArcEndPointXPx() {#getInnerArcEndPointXPx--}
```
public float getInnerArcEndPointXPx()
```


Obtiene la coordenada x del punto final de la sección de pastel después de llamar al método Chart.Calculate(). Se aplica a los gráficos de rosquilla.

**Returns:**
float
### getInnerArcEndPointYPx() {#getInnerArcEndPointYPx--}
```
public float getInnerArcEndPointYPx()
```


Obtiene la coordenada y del punto final de la sección de pastel después de llamar al método Chart.Calculate(). Se aplica al gráfico de rosquilla.

**Returns:**
float
### getInnerArcStartPointXPx() {#getInnerArcStartPointXPx--}
```
public float getInnerArcStartPointXPx()
```


Obtiene la coordenada x del punto inicial de la sección de pastel después de llamar al método Chart.Calculate(). Se aplica al gráfico de rosquilla.

**Returns:**
float
### getInnerArcStartPointYPx() {#getInnerArcStartPointYPx--}
```
public float getInnerArcStartPointYPx()
```


Obtiene la coordenada y del punto de inicio de la sección de pastel después de llamar al método Chart.Calculate(). Se aplica al gráfico de dona.

**Returns:**
float
### getInnerRadiusPx() {#getInnerRadiusPx--}
```
public int getInnerRadiusPx()
```


Obtiene el radio interno de la porción de dona en unidades de píxeles después de llamar al método Chart.Calculate(). Se aplica al gráfico de dona.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad ChartPoint.DoughnutInnerRadius. Esta propiedad será eliminada 12 meses después desde junio de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
int
### getMarker() {#getMarker--}
```
public Marker getMarker()
```


Obtiene el [getMarker()](../../com.aspose.cells/chartpoint\#getMarker--).

**Returns:**
[Marker](../../com.aspose.cells/marker)
### getOnCategoryAxisPointCount() {#getOnCategoryAxisPointCount--}
```
public int getOnCategoryAxisPointCount()
```


Obtiene el número de puntos en el eje de categorías después de llamar al método Chart.Calculate(). Sólo se aplica a los gráficos de área.

**Remarks**

Gráfico de área 2D devuelve 1, gráfico de área 3D devuelve 2.

**Returns:**
int
### getOnCategoryAxisPointXPx(int index) {#getOnCategoryAxisPointXPx-int-}
```
public float getOnCategoryAxisPointXPx(int index)
```


Obtiene la coordenada x del punto en el eje de categorías después de llamar al método Chart.Calculate(). Sólo se aplica al gráfico de área.

**Remarks**

Gráfico de área 2D: el índice es 0. Gráfico de área 3D: el índice es 0 o 1.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int |  |

**Returns:**
float
### getOnCategoryAxisPointYPx(int index) {#getOnCategoryAxisPointYPx-int-}
```
public float getOnCategoryAxisPointYPx(int index)
```


Obtiene la coordenada y del punto en el eje de categorías después de llamar al método Chart.Calculate(). Sólo se aplica al gráfico de área.

**Remarks**

Gráfico de área 2D: el índice es 0. Gráfico de área 3D: el índice es 0 o 1.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int |  |

**Returns:**
float
### getRadiusPx() {#getRadiusPx--}
```
public int getRadiusPx()
```


Obtiene el radio de la burbuja, pastel o dona en unidades de píxeles después de llamar al método Chart.Calculate().

**Returns:**
int
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


Verdadero si el punto del gráfico tiene una sombra.

**Returns:**
boolean
### getShapeHeight() {#getShapeHeight--}
```
public int getShapeHeight()
```


Obtiene la altura en unidades de 1/4000 de la altura del gráfico después de llamar al método Chart.Calculate().

**Returns:**
int
### getShapeHeightPx() {#getShapeHeightPx--}
```
public int getShapeHeightPx()
```


Obtiene la altura en unidades de píxeles después de llamar al método Chart.Calculate().

**Returns:**
int
### getShapeProperties() {#getShapeProperties--}
```
public ShapePropertyCollection getShapeProperties()
```


Obtiene el objeto [ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection) que contiene las propiedades visuales de la forma del ChartPoint.

**Returns:**
[ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection)
### getShapeWidth() {#getShapeWidth--}
```
public int getShapeWidth()
```


Obtiene el ancho en unidades de 1/4000 del ancho del gráfico después de llamar al método Chart.Calculate().

**Returns:**
int
### getShapeWidthPx() {#getShapeWidthPx--}
```
public int getShapeWidthPx()
```


Obtiene el ancho en unidades de píxeles después de llamar al método Chart.Calculate().

**Returns:**
int
### getShapeX() {#getShapeX--}
```
public int getShapeX()
```


Obtiene la coordenada x de la esquina superior izquierda en unidades de 1/4000 del ancho del gráfico después de llamar al método Chart.Calculate().

**Returns:**
int
### getShapeXPx() {#getShapeXPx--}
```
public int getShapeXPx()
```


Obtiene la coordenada x de la esquina superior izquierda en unidades de píxeles después de llamar al método Chart.Calculate().

**Returns:**
int
### getShapeY() {#getShapeY--}
```
public int getShapeY()
```


Obtiene la coordenada y de la esquina superior izquierda en unidades de 1/4000 de la altura del gráfico después de llamar al método Chart.Calculate().

**Returns:**
int
### getShapeYPx() {#getShapeYPx--}
```
public int getShapeYPx()
```


Obtiene la coordenada y de la esquina superior izquierda en unidades de píxeles después de llamar al método Chart.Calculate().

**Returns:**
int
### getStartAngle() {#getStartAngle--}
```
public float getStartAngle()
```


Obtiene el ángulo inicial de la sección de pastel, medido en grados en sentido horario desde el eje x después de llamar al método Chart.Calculate(). Se aplica al gráfico de pastel.

**Returns:**
float
### getTopPointCount() {#getTopPointCount--}
```
public int getTopPointCount()
```


Obtiene el número de puntos superiores después de llamar al método Chart.Calculate().

**Returns:**
int
### getTopPointXPx(int index) {#getTopPointXPx-int-}
```
public float getTopPointXPx(int index)
```


Obtiene la coordenada x del punto superior de la forma después de llamar al método Chart.Calculate(). Se aplica a los gráficos 3D: Column3D, Bar3D, Cone, Cylinder, Pyramid y Area3D.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int |  |

**Returns:**
float
### getTopPointYPx(int index) {#getTopPointYPx-int-}
```
public float getTopPointYPx(int index)
```


Obtiene la coordenada y del punto superior de la forma después de llamar al método Chart.Calculate(). Se aplica a los gráficos 3D: Column3D, Bar3D, Cone, Cylinder, Pyramid y Area3D.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int |  |

**Returns:**
float
### getXValue() {#getXValue--}
```
public Object getXValue()
```


Obtiene el valor X del punto del gráfico.

**Returns:**
java.lang.Object
### getXValueType() {#getXValueType--}
```
public int getXValueType()
```


Obtiene el tipo de valor X del punto del gráfico.

Ver [CellValueType](../../com.aspose.cells/cellvaluetype).

**Returns:**
int
### getYValue() {#getYValue--}
```
public Object getYValue()
```


Obtiene el valor Y del punto del gráfico.

**Returns:**
java.lang.Object
### getYValueType() {#getYValueType--}
```
public int getYValueType()
```


Obtiene el tipo de valor Y del punto del gráfico.

Ver [CellValueType](../../com.aspose.cells/cellvaluetype).

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


Obtiene un valor que indica si este punto de datos está en el segundo pastel o barra en un gráfico de pastel dentro de pastel o barra dentro de pastel.

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


La distancia de una porción de pastel abierta desde el centro del gráfico de pastel se expresa como un porcentaje del diámetro del pastel.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setInSecondaryPlot(boolean value) {#setInSecondaryPlot-boolean-}
```
public void setInSecondaryPlot(boolean value)
```


Establece un valor que indica si este punto de datos está en el segundo pastel o barra en un gráfico de pastel dentro de pastel o barra dentro de pastel.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


Verdadero si el punto del gráfico tiene una sombra.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setXValue(Object value) {#setXValue-java.lang.Object-}
```
public void setXValue(Object value)
```


Establece el valor X del punto del gráfico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.Object |  |

### setYValue(Object value) {#setYValue-java.lang.Object-}
```
public void setYValue(Object value)
```


Establece el valor Y del punto del gráfico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.Object |  |

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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

