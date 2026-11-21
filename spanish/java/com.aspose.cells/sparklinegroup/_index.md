---
title: "SparklineGroup"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "está organizado en un grupo de sparkline."
type: docs
url: /es/java/com.aspose.cells/sparklinegroup/
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
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDisplayHidden()](#getDisplayHidden--) | Indica si se deben mostrar los datos en filas y columnas ocultas. |
| [getFirstPointColor()](#getFirstPointColor--) | Obtiene el color del primer punto de datos en el grupo de sparkline. |
| [getHighPointColor()](#getHighPointColor--) | Obtiene el color de los puntos más altos de datos en el grupo de sparkline. |
| [getHorizontalAxisColor()](#getHorizontalAxisColor--) | Obtiene el color del eje horizontal en el grupo de sparkline. |
| [getHorizontalAxisDateRange()](#getHorizontalAxisDateRange--) | Representa el rango que contiene los valores de fecha para los datos de sparkline. |
| [getLastPointColor()](#getLastPointColor--) | Obtiene el color del último punto de datos en el grupo de sparkline. |
| [getLineWeight()](#getLineWeight--) | Obtiene el grosor de línea en cada sparkline de línea en el grupo de sparkline, en unidades de puntos. |
| [getLowPointColor()](#getLowPointColor--) | Obtiene el color de los puntos más bajos de datos en el grupo de sparkline. |
| [getMarkersColor()](#getMarkersColor--) | Obtiene el color de los puntos en cada sparkline de línea en el grupo de sparkline. |
| [getNegativePointsColor()](#getNegativePointsColor--) | Obtiene el color de los valores negativos en el grupo de sparkline. |
| [getPlotEmptyCellsType()](#getPlotEmptyCellsType--) | Indica cómo trazar celdas vacías. |
| [getPlotRightToLeft()](#getPlotRightToLeft--) | Indica si los datos del gráfico se presentan de derecha a izquierda. |
| [getPresetStyle()](#getPresetStyle--) | Obtiene el tipo de estilo predefinido del grupo de sparkline. |
| [getSeriesColor()](#getSeriesColor--) | Obtiene el color de los sparklines en el grupo de sparkline. |
| [getShowFirstPoint()](#getShowFirstPoint--) | Indica si se debe resaltar el primer punto de datos en el grupo de sparkline. |
| [getShowHighPoint()](#getShowHighPoint--) | Indica si se deben resaltar los puntos más altos de los datos en el grupo de sparkline. |
| [getShowHorizontalAxis()](#getShowHorizontalAxis--) | Indica si se debe mostrar el eje horizontal del sparkline. |
| [getShowLastPoint()](#getShowLastPoint--) | Indica si se debe resaltar el último punto de datos en el grupo de sparkline. |
| [getShowLowPoint()](#getShowLowPoint--) | Indica si se deben resaltar los puntos más bajos de los datos en el grupo de sparkline. |
| [getShowMarkers()](#getShowMarkers--) | Indica si se debe resaltar cada punto en cada sparkline de línea en el grupo de sparkline. |
| [getShowNegativePoints()](#getShowNegativePoints--) | Indica si se deben resaltar los valores negativos en el grupo de sparkline con un color o marcador diferente. |
| [getSparklineCollection()](#getSparklineCollection--) | Obtiene la colección del objeto [Sparkline](../../com.aspose.cells/sparkline). |
| [getSparklines()](#getSparklines--) | Obtiene la colección del objeto [Sparkline](../../com.aspose.cells/sparkline). |
| [getType()](#getType--) | Indica el tipo de sparkline del grupo de sparkline. |
| [getVerticalAxisMaxValue()](#getVerticalAxisMaxValue--) | Obtiene el valor máximo personalizado para el eje vertical. |
| [getVerticalAxisMaxValueType()](#getVerticalAxisMaxValueType--) | Representa el tipo de valor máximo del eje vertical. |
| [getVerticalAxisMinValue()](#getVerticalAxisMinValue--) | Obtiene el valor mínimo personalizado para el eje vertical. |
| [getVerticalAxisMinValueType()](#getVerticalAxisMinValueType--) | Representa el tipo de valor mínimo del eje vertical. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [resetRanges(String dataRange, boolean isVertical, CellArea locationRange)](#resetRanges-java.lang.String-boolean-com.aspose.cells.CellArea-) | Restablece el rango de datos y el rango de ubicación del grupo de sparkline. |
| [setDisplayHidden(boolean value)](#setDisplayHidden-boolean-) | Indica si se deben mostrar los datos en filas y columnas ocultas. |
| [setFirstPointColor(CellsColor value)](#setFirstPointColor-com.aspose.cells.CellsColor-) | Establece el color del primer punto de datos en el grupo de sparkline. |
| [setHighPointColor(CellsColor value)](#setHighPointColor-com.aspose.cells.CellsColor-) | Establece el color de los puntos más altos de los datos en el grupo de sparkline. |
| [setHorizontalAxisColor(CellsColor value)](#setHorizontalAxisColor-com.aspose.cells.CellsColor-) | Establece el color del eje horizontal en el grupo de sparkline. |
| [setHorizontalAxisDateRange(String value)](#setHorizontalAxisDateRange-java.lang.String-) | Representa el rango que contiene los valores de fecha para los datos de sparkline. |
| [setLastPointColor(CellsColor value)](#setLastPointColor-com.aspose.cells.CellsColor-) | Establece el color del último punto de datos en el grupo de sparkline. |
| [setLineWeight(double value)](#setLineWeight-double-) | Establece el grosor de línea en cada sparkline de línea del grupo de sparkline, en unidades de puntos. |
| [setLowPointColor(CellsColor value)](#setLowPointColor-com.aspose.cells.CellsColor-) | Establece el color de los puntos más bajos de los datos en el grupo de sparkline. |
| [setMarkersColor(CellsColor value)](#setMarkersColor-com.aspose.cells.CellsColor-) | Establece el color de los puntos en cada sparkline de línea del grupo de sparkline. |
| [setNegativePointsColor(CellsColor value)](#setNegativePointsColor-com.aspose.cells.CellsColor-) | Establece el color de los valores negativos en el grupo de sparkline. |
| [setPlotEmptyCellsType(int value)](#setPlotEmptyCellsType-int-) | Indica cómo trazar celdas vacías. |
| [setPlotRightToLeft(boolean value)](#setPlotRightToLeft-boolean-) | Indica si los datos del gráfico se presentan de derecha a izquierda. |
| [setPresetStyle(int value)](#setPresetStyle-int-) | Establece el tipo de estilo predefinido del grupo de sparkline. |
| [setSeriesColor(CellsColor value)](#setSeriesColor-com.aspose.cells.CellsColor-) | Establece el color de los sparklines en el grupo de sparkline. |
| [setShowFirstPoint(boolean value)](#setShowFirstPoint-boolean-) | Indica si se debe resaltar el primer punto de datos en el grupo de sparkline. |
| [setShowHighPoint(boolean value)](#setShowHighPoint-boolean-) | Indica si se deben resaltar los puntos más altos de los datos en el grupo de sparkline. |
| [setShowHorizontalAxis(boolean value)](#setShowHorizontalAxis-boolean-) | Indica si se debe mostrar el eje horizontal del sparkline. |
| [setShowLastPoint(boolean value)](#setShowLastPoint-boolean-) | Indica si se debe resaltar el último punto de datos en el grupo de sparkline. |
| [setShowLowPoint(boolean value)](#setShowLowPoint-boolean-) | Indica si se deben resaltar los puntos más bajos de los datos en el grupo de sparkline. |
| [setShowMarkers(boolean value)](#setShowMarkers-boolean-) | Indica si se debe resaltar cada punto en cada sparkline de línea en el grupo de sparkline. |
| [setShowNegativePoints(boolean value)](#setShowNegativePoints-boolean-) | Indica si se deben resaltar los valores negativos en el grupo de sparkline con un color o marcador diferente. |
| [setType(int value)](#setType-int-) | Indica el tipo de sparkline del grupo de sparkline. |
| [setVerticalAxisMaxValue(double value)](#setVerticalAxisMaxValue-double-) | Establece el valor máximo personalizado para el eje vertical. |
| [setVerticalAxisMaxValue(int type, double value)](#setVerticalAxisMaxValue-int-double-) | Establece el valor máximo personalizado para el eje vertical del sparkline con el tipo de valor de eje especificado. |
| [setVerticalAxisMaxValueType(int value)](#setVerticalAxisMaxValueType-int-) | Representa el tipo de valor máximo del eje vertical. |
| [setVerticalAxisMinValue(double value)](#setVerticalAxisMinValue-double-) | Establece el valor mínimo personalizado para el eje vertical. |
| [setVerticalAxisMinValue(int type, double value)](#setVerticalAxisMinValue-int-double-) | Establece el valor mínimo personalizado para el eje vertical de la sparkline con el tipo de valor de eje especificado. |
| [setVerticalAxisMinValueType(int value)](#setVerticalAxisMinValueType-int-) | Representa el tipo de valor mínimo del eje vertical. |
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


Indica si se deben mostrar los datos en filas y columnas ocultas.

**Returns:**
boolean
### getFirstPointColor() {#getFirstPointColor--}
```
public CellsColor getFirstPointColor()
```


Obtiene el color del primer punto de datos en el grupo de sparkline.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getHighPointColor() {#getHighPointColor--}
```
public CellsColor getHighPointColor()
```


Obtiene el color de los puntos más altos de datos en el grupo de sparkline.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getHorizontalAxisColor() {#getHorizontalAxisColor--}
```
public CellsColor getHorizontalAxisColor()
```


Obtiene el color del eje horizontal en el grupo de sparkline.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getHorizontalAxisDateRange() {#getHorizontalAxisDateRange--}
```
public String getHorizontalAxisDateRange()
```


Representa el rango que contiene los valores de fecha para los datos de sparkline.

**Returns:**
java.lang.String
### getLastPointColor() {#getLastPointColor--}
```
public CellsColor getLastPointColor()
```


Obtiene el color del último punto de datos en el grupo de sparkline.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getLineWeight() {#getLineWeight--}
```
public double getLineWeight()
```


Obtiene el grosor de línea en cada sparkline de línea en el grupo de sparkline, en unidades de puntos.

**Returns:**
double
### getLowPointColor() {#getLowPointColor--}
```
public CellsColor getLowPointColor()
```


Obtiene el color de los puntos más bajos de datos en el grupo de sparkline.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getMarkersColor() {#getMarkersColor--}
```
public CellsColor getMarkersColor()
```


Obtiene el color de los puntos en cada sparkline de línea en el grupo de sparkline.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getNegativePointsColor() {#getNegativePointsColor--}
```
public CellsColor getNegativePointsColor()
```


Obtiene el color de los valores negativos en el grupo de sparkline.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getPlotEmptyCellsType() {#getPlotEmptyCellsType--}
```
public int getPlotEmptyCellsType()
```


Indica cómo trazar celdas vacías.

Ver [PlotEmptyCellsType](../../com.aspose.cells/plotemptycellstype).

**Returns:**
int
### getPlotRightToLeft() {#getPlotRightToLeft--}
```
public boolean getPlotRightToLeft()
```


Indica si los datos del gráfico se presentan de derecha a izquierda.

**Returns:**
boolean
### getPresetStyle() {#getPresetStyle--}
```
public int getPresetStyle()
```


Obtiene el tipo de estilo predefinido del grupo de sparkline.

Ver [SparklinePresetStyleType](../../com.aspose.cells/sparklinepresetstyletype).

**Remarks**

Si esta propiedad está establecida, estas propiedades: SeriesColor,NegativePointsColor,HorizontalAxisColor,MarkersColor,FirstPointColor,LastPointColor,HighPointColor,LowPointColor serán cubiertas. Por lo tanto, establezca primero la propiedad y luego las demás.

**Returns:**
int
### getSeriesColor() {#getSeriesColor--}
```
public CellsColor getSeriesColor()
```


Obtiene el color de los sparklines en el grupo de sparkline.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getShowFirstPoint() {#getShowFirstPoint--}
```
public boolean getShowFirstPoint()
```


Indica si se debe resaltar el primer punto de datos en el grupo de sparkline.

**Returns:**
boolean
### getShowHighPoint() {#getShowHighPoint--}
```
public boolean getShowHighPoint()
```


Indica si se deben resaltar los puntos más altos de los datos en el grupo de sparkline.

**Returns:**
boolean
### getShowHorizontalAxis() {#getShowHorizontalAxis--}
```
public boolean getShowHorizontalAxis()
```


Indica si se debe mostrar el eje horizontal de la sparkline. El eje horizontal aparece si la sparkline tiene datos que cruzan el eje cero.

**Returns:**
boolean
### getShowLastPoint() {#getShowLastPoint--}
```
public boolean getShowLastPoint()
```


Indica si se debe resaltar el último punto de datos en el grupo de sparkline.

**Returns:**
boolean
### getShowLowPoint() {#getShowLowPoint--}
```
public boolean getShowLowPoint()
```


Indica si se deben resaltar los puntos más bajos de los datos en el grupo de sparkline.

**Returns:**
boolean
### getShowMarkers() {#getShowMarkers--}
```
public boolean getShowMarkers()
```


Indica si se debe resaltar cada punto en cada sparkline de línea en el grupo de sparkline.

**Returns:**
boolean
### getShowNegativePoints() {#getShowNegativePoints--}
```
public boolean getShowNegativePoints()
```


Indica si se deben resaltar los valores negativos en el grupo de sparkline con un color o marcador diferente.

**Returns:**
boolean
### getSparklineCollection() {#getSparklineCollection--}
```
public SparklineCollection getSparklineCollection()
```


Obtiene la colección del objeto [Sparkline](../../com.aspose.cells/sparkline).

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad SparklineGroup.Sparklines. Esta propiedad será eliminada 12 meses después, a partir de noviembre de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
[SparklineCollection](../../com.aspose.cells/sparklinecollection)
### getSparklines() {#getSparklines--}
```
public SparklineCollection getSparklines()
```


Obtiene la colección del objeto [Sparkline](../../com.aspose.cells/sparkline).

**Returns:**
[SparklineCollection](../../com.aspose.cells/sparklinecollection)
### getType() {#getType--}
```
public int getType()
```


Indica el tipo de sparkline del grupo de sparkline.

Ver [SparklineType](../../com.aspose.cells/sparklinetype).

**Returns:**
int
### getVerticalAxisMaxValue() {#getVerticalAxisMaxValue--}
```
public double getVerticalAxisMaxValue()
```


Obtiene el valor máximo personalizado para el eje vertical.

**Remarks**

Si esta propiedad está establecida, [getVerticalAxisMaxValueType()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMaxValueType--) será [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM).

**Returns:**
double
### getVerticalAxisMaxValueType() {#getVerticalAxisMaxValueType--}
```
public int getVerticalAxisMaxValueType()
```


Representa el tipo de valor máximo del eje vertical.

Ver [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype).

**Returns:**
int
### getVerticalAxisMinValue() {#getVerticalAxisMinValue--}
```
public double getVerticalAxisMinValue()
```


Obtiene el valor mínimo personalizado para el eje vertical.

**Remarks**

Si esta propiedad está establecida, [getVerticalAxisMinValueType()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMinValueType--) será [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM).

**Returns:**
double
### getVerticalAxisMinValueType() {#getVerticalAxisMinValueType--}
```
public int getVerticalAxisMinValueType()
```


Representa el tipo de valor mínimo del eje vertical.

Ver [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype).

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


Restablece el rango de datos y el rango de ubicación del grupo de sparkline. Este método borrará los elementos de sparkline originales en el grupo y creará nuevos elementos de sparkline para los nuevos rangos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dataRange | java.lang.String | Especifica el nuevo rango de datos del grupo de sparkline. |
| isVertical | boolean | Especifica si se deben trazar las sparklines del nuevo rango de datos por fila o por columna. |
| locationRange | [CellArea](../../com.aspose.cells/cellarea) | Especifica dónde se colocarán las sparklines. |

### setDisplayHidden(boolean value) {#setDisplayHidden-boolean-}
```
public void setDisplayHidden(boolean value)
```


Indica si se deben mostrar los datos en filas y columnas ocultas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setFirstPointColor(CellsColor value) {#setFirstPointColor-com.aspose.cells.CellsColor-}
```
public void setFirstPointColor(CellsColor value)
```


Establece el color del primer punto de datos en el grupo de sparkline.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setHighPointColor(CellsColor value) {#setHighPointColor-com.aspose.cells.CellsColor-}
```
public void setHighPointColor(CellsColor value)
```


Establece el color de los puntos más altos de los datos en el grupo de sparkline.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setHorizontalAxisColor(CellsColor value) {#setHorizontalAxisColor-com.aspose.cells.CellsColor-}
```
public void setHorizontalAxisColor(CellsColor value)
```


Establece el color del eje horizontal en el grupo de sparkline.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setHorizontalAxisDateRange(String value) {#setHorizontalAxisDateRange-java.lang.String-}
```
public void setHorizontalAxisDateRange(String value)
```


Representa el rango que contiene los valores de fecha para los datos de sparkline.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setLastPointColor(CellsColor value) {#setLastPointColor-com.aspose.cells.CellsColor-}
```
public void setLastPointColor(CellsColor value)
```


Establece el color del último punto de datos en el grupo de sparkline.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setLineWeight(double value) {#setLineWeight-double-}
```
public void setLineWeight(double value)
```


Establece el grosor de línea en cada sparkline de línea del grupo de sparkline, en unidades de puntos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setLowPointColor(CellsColor value) {#setLowPointColor-com.aspose.cells.CellsColor-}
```
public void setLowPointColor(CellsColor value)
```


Establece el color de los puntos más bajos de los datos en el grupo de sparkline.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setMarkersColor(CellsColor value) {#setMarkersColor-com.aspose.cells.CellsColor-}
```
public void setMarkersColor(CellsColor value)
```


Establece el color de los puntos en cada sparkline de línea del grupo de sparkline.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setNegativePointsColor(CellsColor value) {#setNegativePointsColor-com.aspose.cells.CellsColor-}
```
public void setNegativePointsColor(CellsColor value)
```


Establece el color de los valores negativos en el grupo de sparkline.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setPlotEmptyCellsType(int value) {#setPlotEmptyCellsType-int-}
```
public void setPlotEmptyCellsType(int value)
```


Indica cómo trazar celdas vacías.

Ver [PlotEmptyCellsType](../../com.aspose.cells/plotemptycellstype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setPlotRightToLeft(boolean value) {#setPlotRightToLeft-boolean-}
```
public void setPlotRightToLeft(boolean value)
```


Indica si los datos del gráfico se presentan de derecha a izquierda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setPresetStyle(int value) {#setPresetStyle-int-}
```
public void setPresetStyle(int value)
```


Establece el tipo de estilo predefinido del grupo de sparkline.

Ver [SparklinePresetStyleType](../../com.aspose.cells/sparklinepresetstyletype).

**Remarks**

Si esta propiedad está establecida, estas propiedades: SeriesColor,NegativePointsColor,HorizontalAxisColor,MarkersColor,FirstPointColor,LastPointColor,HighPointColor,LowPointColor serán cubiertas. Por lo tanto, establezca primero la propiedad y luego las demás.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setSeriesColor(CellsColor value) {#setSeriesColor-com.aspose.cells.CellsColor-}
```
public void setSeriesColor(CellsColor value)
```


Establece el color de los sparklines en el grupo de sparkline.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setShowFirstPoint(boolean value) {#setShowFirstPoint-boolean-}
```
public void setShowFirstPoint(boolean value)
```


Indica si se debe resaltar el primer punto de datos en el grupo de sparkline.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowHighPoint(boolean value) {#setShowHighPoint-boolean-}
```
public void setShowHighPoint(boolean value)
```


Indica si se deben resaltar los puntos más altos de los datos en el grupo de sparkline.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowHorizontalAxis(boolean value) {#setShowHorizontalAxis-boolean-}
```
public void setShowHorizontalAxis(boolean value)
```


Indica si se debe mostrar el eje horizontal de la sparkline. El eje horizontal aparece si la sparkline tiene datos que cruzan el eje cero.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowLastPoint(boolean value) {#setShowLastPoint-boolean-}
```
public void setShowLastPoint(boolean value)
```


Indica si se debe resaltar el último punto de datos en el grupo de sparkline.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowLowPoint(boolean value) {#setShowLowPoint-boolean-}
```
public void setShowLowPoint(boolean value)
```


Indica si se deben resaltar los puntos más bajos de los datos en el grupo de sparkline.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowMarkers(boolean value) {#setShowMarkers-boolean-}
```
public void setShowMarkers(boolean value)
```


Indica si se debe resaltar cada punto en cada sparkline de línea en el grupo de sparkline.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowNegativePoints(boolean value) {#setShowNegativePoints-boolean-}
```
public void setShowNegativePoints(boolean value)
```


Indica si se deben resaltar los valores negativos en el grupo de sparkline con un color o marcador diferente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Indica el tipo de sparkline del grupo de sparkline.

Ver [SparklineType](../../com.aspose.cells/sparklinetype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setVerticalAxisMaxValue(double value) {#setVerticalAxisMaxValue-double-}
```
public void setVerticalAxisMaxValue(double value)
```


Establece el valor máximo personalizado para el eje vertical.

**Remarks**

Si esta propiedad está establecida, [getVerticalAxisMaxValueType()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMaxValueType--) será [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setVerticalAxisMaxValue(int type, double value) {#setVerticalAxisMaxValue-int-double-}
```
public void setVerticalAxisMaxValue(int type, double value)
```


Establece el valor máximo personalizado para el eje vertical del sparkline con el tipo de valor de eje especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype). Tipo que especifica cómo se aplica el valor máximo del eje. |
| value | double | Valor máximo personalizado del eje vertical. Se ignora si el tipo no es [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM). |

### setVerticalAxisMaxValueType(int value) {#setVerticalAxisMaxValueType-int-}
```
public void setVerticalAxisMaxValueType(int value)
```


Representa el tipo de valor máximo del eje vertical.

Ver [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setVerticalAxisMinValue(double value) {#setVerticalAxisMinValue-double-}
```
public void setVerticalAxisMinValue(double value)
```


Establece el valor mínimo personalizado para el eje vertical.

**Remarks**

Si esta propiedad está establecida, [getVerticalAxisMinValueType()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMinValueType--) será [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setVerticalAxisMinValue(int type, double value) {#setVerticalAxisMinValue-int-double-}
```
public void setVerticalAxisMinValue(int type, double value)
```


Establece el valor mínimo personalizado para el eje vertical de la sparkline con el tipo de valor de eje especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype). Tipo que especifica cómo se aplica el valor mínimo del eje. |
| value | double | Valor mínimo personalizado del eje vertical. Se ignora si el tipo no es [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM). |

### setVerticalAxisMinValueType(int value) {#setVerticalAxisMinValueType-int-}
```
public void setVerticalAxisMinValueType(int value)
```


Representa el tipo de valor mínimo del eje vertical.

Ver [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

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

