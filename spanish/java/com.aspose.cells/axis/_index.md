---
title: "Axis"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Encapsula el objeto que representa un eje de un gráfico."
type: docs
url: /es/java/com.aspose.cells/axis/
---

**Inheritance:**
java.lang.Object
```
public class Axis
```

Encapsula el objeto que representa un eje de un gráfico.

**Example**

Con los siguientes códigos, puedes aprender cómo establecer la unidad, el valor máximo y mínimo del Axis.

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Adding a new worksheet to the Excel object
         int sheetIndex = workbook.getWorksheets().add();
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(sheetIndex);
         //Adding a sample value to "A1" cell
         worksheet.getCells().get("A1").putValue(50);
         //Adding a sample value to "A2" cell
         worksheet.getCells().get("A2").putValue(100);
         //Adding a sample value to "A3" cell
         worksheet.getCells().get("A3").putValue(150);
         //Adding a sample value to "B1" cell
         worksheet.getCells().get("B1").putValue(4);
         //Adding a sample value to "B2" cell
         worksheet.getCells().get("B2").putValue(20);
         //Adding a sample value to "B3" cell
         worksheet.getCells().get("B3").putValue(50);
         //Adding a chart to the worksheet
         int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 25, 5);
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
         chart.getNSeries().add("A1:B3", true);
         //Set the max value of value axis
         chart.getValueAxis().setMaxValue(200);
         //Set the min value of value axis
         chart.getValueAxis().setMinValue(0);
         //Set the major unit
         chart.getValueAxis().setMajorUnit(25);
         //Category(X) axis crosses at the maxinum value.
         chart.getValueAxis().setCrossType(CrossType.MAXIMUM);
         //Set he number of categories or series between tick-mark labels. 
         chart.getCategoryAxis().setTickLabelSpacing(2);
 
         //do your business
 
         //Saving the Excel file
         workbook.save("book1.xlsx");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArea()](#getArea--) | Obtiene el [getArea()](../../com.aspose.cells/axis\#getArea--). |
| [getAxisBetweenCategories()](#getAxisBetweenCategories--) | Representa si el eje de valores cruza el eje de categorías entre categorías. |
| [getAxisLabels()](#getAxisLabels--) | Obtiene las etiquetas del eje después de llamar al método Chart.Calculate(). |
| [getAxisLine()](#getAxisLine--) | Obtiene la apariencia de un Axis. |
| [getAxisTexts()](#getAxisTexts--) | Obtiene las etiquetas del eje después de llamar al método Chart.Calculate(). |
| [getBaseUnitScale()](#getBaseUnitScale--) | Representa la escala de unidad base para el eje de categorías. |
| [getBins()](#getBins--) | Representa los contenedores en el eje de un gráfico (Histograma/Pareto) |
| [getCategoryType()](#getCategoryType--) | Representa el tipo del eje de categorías. |
| [getClass()](#getClass--) |  |
| [getCrossAt()](#getCrossAt--) | Representa el punto en el eje de valores donde el eje de categorías lo cruza. |
| [getCrossType()](#getCrossType--) | Representa el [getCrossType()](../../com.aspose.cells/axis\#getCrossType--) en el eje especificado donde cruza el otro eje. |
| [getCustUnit()](#getCustUnit--) | Especifica un valor personalizado para la unidad de visualización. |
| [getCustomDisplayUnit()](#getCustomDisplayUnit--) | Especifica un valor personalizado para la unidad de visualización. |
| [getCustomUnit()](#getCustomUnit--) | Especifica un valor personalizado para la unidad de visualización. |
| [getDisplayUnit()](#getDisplayUnit--) | Representa la etiqueta de unidad para el eje especificado. |
| [getDisplayUnitLabel()](#getDisplayUnitLabel--) | Representa una etiqueta de unidad en un eje del gráfico especificado. |
| [getLogBase()](#getLogBase--) | Representa la base logarítmica. |
| [getMajorGridLines()](#getMajorGridLines--) | Representa las líneas de cuadrícula principales en el eje de un gráfico. |
| [getMajorTickMark()](#getMajorTickMark--) | Representa el tipo de marca de graduación mayor para el eje especificado. |
| [getMajorUnit()](#getMajorUnit--) | Representa las unidades mayores para el eje. |
| [getMajorUnitScale()](#getMajorUnitScale--) | Representa la escala de la unidad mayor para el eje de categorías. |
| [getMaxValue()](#getMaxValue--) | Representa el valor máximo en el eje de valores. |
| [getMinValue()](#getMinValue--) | Representa el valor mínimo en el eje de valores. |
| [getMinorGridLines()](#getMinorGridLines--) | Representa las líneas de cuadrícula menores en un eje de gráfico. |
| [getMinorTickMark()](#getMinorTickMark--) | Representa el tipo de marca de graduación menor para el eje especificado. |
| [getMinorUnit()](#getMinorUnit--) | Representa las unidades menores para el eje. |
| [getMinorUnitScale()](#getMinorUnitScale--) | Representa la escala de la unidad mayor para el eje de categorías. |
| [getTickLabelPosition()](#getTickLabelPosition--) | Representa la posición de las etiquetas de marcas de graduación en el eje especificado. |
| [getTickLabelSpacing()](#getTickLabelSpacing--) | Representa el número de categorías o series entre las etiquetas de marcas de graduación. |
| [getTickLabels()](#getTickLabels--) | Devuelve un objeto [getTickLabels()](../../com.aspose.cells/axis\#getTickLabels--) que representa las etiquetas de marcas de graduación para el eje especificado. |
| [getTickMarkSpacing()](#getTickMarkSpacing--) | Devuelve o establece el número de categorías o series entre marcas de graduación. |
| [getTitle()](#getTitle--) | Obtiene el título de este eje en el gráfico. |
| [hasMultiLevelLabels()](#hasMultiLevelLabels--) | Indica si las etiquetas se mostrarán en varios niveles. |
| [hashCode()](#hashCode--) |  |
| [isAutoTickLabelSpacing()](#isAutoTickLabelSpacing--) | Indica si el espaciado de la etiqueta de graduación es automático |
| [isAutomaticMajorUnit()](#isAutomaticMajorUnit--) | Indica si la unidad mayor del eje se asigna automáticamente. |
| [isAutomaticMaxValue()](#isAutomaticMaxValue--) | Indica si el valor máximo se asigna automáticamente. |
| [isAutomaticMinValue()](#isAutomaticMinValue--) | Indica si el valor mínimo se asigna automáticamente. |
| [isAutomaticMinorUnit()](#isAutomaticMinorUnit--) | Indica si la unidad menor del eje se asigna automáticamente. |
| [isBaseUnitAuto()](#isBaseUnitAuto--) | Representa si la unidad base es automática. |
| [isDisplayUnitLabelShown()](#isDisplayUnitLabelShown--) | Representa si la etiqueta de unidad de visualización se muestra en el eje especificado. |
| [isLogarithmic()](#isLogarithmic--) | Representa si el tipo de escala del eje de valores es logarítmico o no. |
| [isPlotOrderReversed()](#isPlotOrderReversed--) | Representa si Microsoft Excel traza los puntos de datos de último a primero. |
| [isVisible()](#isVisible--) | Representa si el eje es visible. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoTickLabelSpacing(boolean value)](#setAutoTickLabelSpacing-boolean-) | Indica si el espaciado de la etiqueta de graduación es automático |
| [setAutomaticMajorUnit(boolean value)](#setAutomaticMajorUnit-boolean-) | Indica si la unidad mayor del eje se asigna automáticamente. |
| [setAutomaticMaxValue(boolean value)](#setAutomaticMaxValue-boolean-) | Indica si el valor máximo se asigna automáticamente. |
| [setAutomaticMinValue(boolean value)](#setAutomaticMinValue-boolean-) | Indica si el valor mínimo se asigna automáticamente. |
| [setAutomaticMinorUnit(boolean value)](#setAutomaticMinorUnit-boolean-) | Indica si la unidad menor del eje se asigna automáticamente. |
| [setAxisBetweenCategories(boolean value)](#setAxisBetweenCategories-boolean-) | Representa si el eje de valores cruza el eje de categorías entre categorías. |
| [setBaseUnitAuto(boolean value)](#setBaseUnitAuto-boolean-) | Representa si la unidad base es automática. |
| [setBaseUnitScale(int value)](#setBaseUnitScale-int-) | Representa la escala de unidad base para el eje de categorías. |
| [setCategoryType(int value)](#setCategoryType-int-) | Representa el tipo del eje de categorías. |
| [setCrossAt(double value)](#setCrossAt-double-) | Representa el punto en el eje de valores donde el eje de categorías lo cruza. |
| [setCrossType(int value)](#setCrossType-int-) | Representa el [getCrossType()](../../com.aspose.cells/axis\#getCrossType--) en el eje especificado donde cruza el otro eje. |
| [setCustUnit(int value)](#setCustUnit-int-) | Especifica un valor personalizado para la unidad de visualización. |
| [setCustomDisplayUnit(double value)](#setCustomDisplayUnit-double-) | Especifica un valor personalizado para la unidad de visualización. |
| [setCustomUnit(int value)](#setCustomUnit-int-) | Especifica un valor personalizado para la unidad de visualización. |
| [setDisplayUnit(int value)](#setDisplayUnit-int-) | Representa la etiqueta de unidad para el eje especificado. |
| [setDisplayUnitLabelShown(boolean value)](#setDisplayUnitLabelShown-boolean-) | Representa si la etiqueta de unidad de visualización se muestra en el eje especificado. |
| [setHasMultiLevelLabels(boolean value)](#setHasMultiLevelLabels-boolean-) | Indica si las etiquetas se mostrarán en varios niveles. |
| [setLogBase(double value)](#setLogBase-double-) | Representa la base logarítmica. |
| [setLogarithmic(boolean value)](#setLogarithmic-boolean-) | Representa si el tipo de escala del eje de valores es logarítmico o no. |
| [setMajorTickMark(int value)](#setMajorTickMark-int-) | Representa el tipo de marca de graduación mayor para el eje especificado. |
| [setMajorUnit(double value)](#setMajorUnit-double-) | Representa las unidades mayores para el eje. |
| [setMajorUnitScale(int value)](#setMajorUnitScale-int-) | Representa la escala de la unidad mayor para el eje de categorías. |
| [setMaxValue(Object value)](#setMaxValue-java.lang.Object-) | Representa el valor máximo en el eje de valores. |
| [setMinValue(Object value)](#setMinValue-java.lang.Object-) | Representa el valor mínimo en el eje de valores. |
| [setMinorTickMark(int value)](#setMinorTickMark-int-) | Representa el tipo de marca de graduación menor para el eje especificado. |
| [setMinorUnit(double value)](#setMinorUnit-double-) | Representa las unidades menores para el eje. |
| [setMinorUnitScale(int value)](#setMinorUnitScale-int-) | Representa la escala de la unidad mayor para el eje de categorías. |
| [setPlotOrderReversed(boolean value)](#setPlotOrderReversed-boolean-) | Representa si Microsoft Excel traza los puntos de datos de último a primero. |
| [setTickLabelPosition(int value)](#setTickLabelPosition-int-) | Representa la posición de las etiquetas de marcas de graduación en el eje especificado. |
| [setTickLabelSpacing(int value)](#setTickLabelSpacing-int-) | Representa el número de categorías o series entre las etiquetas de marcas de graduación. |
| [setTickMarkSpacing(int value)](#setTickMarkSpacing-int-) | Devuelve o establece el número de categorías o series entre marcas de graduación. |
| [setVisible(boolean value)](#setVisible-boolean-) | Representa si el eje es visible. |
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
### getArea() {#getArea--}
```
public Area getArea()
```


Obtiene el [getArea()](../../com.aspose.cells/axis\#getArea--).

**Returns:**
[Area](../../com.aspose.cells/area)
### getAxisBetweenCategories() {#getAxisBetweenCategories--}
```
public boolean getAxisBetweenCategories()
```


Representa si el eje de valores cruza el eje de categorías entre categorías.

**Remarks**

Esta propiedad se aplica solo a ejes de categorías, y no se aplica a gráficos 3D.

**Returns:**
boolean
### getAxisLabels() {#getAxisLabels--}
```
public ArrayList getAxisLabels()
```


Obtiene las etiquetas del eje después de llamar al método Chart.Calculate().

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use el método Axis.GetAxisTexts. Esta propiedad será eliminada 12 meses después a partir de noviembre de 2023. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Returns:**
java.util.ArrayList
### getAxisLine() {#getAxisLine--}
```
public Line getAxisLine()
```


Obtiene la apariencia de un Axis.

**Returns:**
[Line](../../com.aspose.cells/line)
### getAxisTexts() {#getAxisTexts--}
```
public String[] getAxisTexts()
```


Obtiene las etiquetas del eje después de llamar al método Chart.Calculate().

**Returns:**
java.lang.String[]
### getBaseUnitScale() {#getBaseUnitScale--}
```
public int getBaseUnitScale()
```


Representa la escala de unidad base para el eje de categorías.

Ver [TimeUnit](../../com.aspose.cells/timeunit).

**Remarks**

Solo tiene efecto cuando la propiedad CategoryType está establecida en TimeScale.

**Returns:**
int
### getBins() {#getBins--}
```
public AxisBins getBins()
```


Representa los contenedores en el eje de un gráfico (Histograma/Pareto)

**Remarks**

Solo para el gráfico Histogram o Pareto.

**Returns:**
[AxisBins](../../com.aspose.cells/axisbins)
### getCategoryType() {#getCategoryType--}
```
public int getCategoryType()
```


Representa el tipo del eje de categorías.

Ver [CategoryType](../../com.aspose.cells/categorytype).

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCrossAt() {#getCrossAt--}
```
public double getCrossAt()
```


Representa el punto en el eje de valores donde el eje de categorías lo cruza.

**Remarks**

El número debe ser un entero cuando se aplica al eje de categoría. Y el valor debe estar entre 1 y 31999.

**Returns:**
double
### getCrossType() {#getCrossType--}
```
public int getCrossType()
```


Representa el [getCrossType()](../../com.aspose.cells/axis\#getCrossType--) en el eje especificado donde cruza el otro eje.

Ver [CrossType](../../com.aspose.cells/crosstype).

**Returns:**
int
### getCustUnit() {#getCustUnit--}
```
public int getCustUnit()
```


Especifica un valor personalizado para la unidad de visualización.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, por favor use la propiedad Axis.CustomUnit. Esta propiedad será eliminada 12 meses después a partir de enero de 2023. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Returns:**
int
### getCustomDisplayUnit() {#getCustomDisplayUnit--}
```
public double getCustomDisplayUnit()
```


Especifica un valor personalizado para la unidad de visualización.

**Returns:**
double
### getCustomUnit() {#getCustomUnit--}
```
public int getCustomUnit()
```


Especifica un valor personalizado para la unidad de visualización.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, por favor use la propiedad Axis.CustomDisplayUnit. Esta propiedad será eliminada 12 meses después a partir de febrero de 2025. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Returns:**
int
### getDisplayUnit() {#getDisplayUnit--}
```
public int getDisplayUnit()
```


Representa la etiqueta de unidad para el eje especificado.

Ver [DisplayUnitType](../../com.aspose.cells/displayunittype).

**Returns:**
int
### getDisplayUnitLabel() {#getDisplayUnitLabel--}
```
public DisplayUnitLabel getDisplayUnitLabel()
```


Representa una etiqueta de unidad en un eje del gráfico especificado. Las etiquetas de unidad son útiles para graficar valores grandes, por ejemplo, en millones o miles de millones.

**Returns:**
[DisplayUnitLabel](../../com.aspose.cells/displayunitlabel)
### getLogBase() {#getLogBase--}
```
public double getLogBase()
```


Representa la base logarítmica. El valor predeterminado es 10.

**Returns:**
double
### getMajorGridLines() {#getMajorGridLines--}
```
public Line getMajorGridLines()
```


Representa las líneas de cuadrícula principales en el eje de un gráfico.

**Example**

```
         chart.getValueAxis().getMajorGridLines().setVisible(false);
         chart.getCategoryAxis().getMajorGridLines().setVisible(true);
```

**Returns:**
[Line](../../com.aspose.cells/line)
### getMajorTickMark() {#getMajorTickMark--}
```
public int getMajorTickMark()
```


Representa el tipo de marca de graduación mayor para el eje especificado.

Ver [TickMarkType](../../com.aspose.cells/tickmarktype).

**Returns:**
int
### getMajorUnit() {#getMajorUnit--}
```
public double getMajorUnit()
```


Representa las unidades mayores para el eje.

**Remarks**

Las unidades principales deben ser mayores que cero.

**Returns:**
double
### getMajorUnitScale() {#getMajorUnitScale--}
```
public int getMajorUnitScale()
```


Representa la escala de la unidad mayor para el eje de categorías.

Ver [TimeUnit](../../com.aspose.cells/timeunit).

**Example**

```
         chart.getCategoryAxis().setCategoryType(CategoryType.TIME_SCALE);
         /*TimeUnit*/int majorUnitScale = chart.getCategoryAxis().getMajorUnitScale(); //get
         chart.getCategoryAxis().setMajorUnitScale(majorUnitScale); //set
         chart.getCategoryAxis().setMajorUnit(2);
```

**Returns:**
int
### getMaxValue() {#getMaxValue--}
```
public Object getMaxValue()
```


Representa el valor máximo en el eje de valores.

**Remarks**

El tipo maxValue solo puede ser double o DateTime.

**Returns:**
java.lang.Object
### getMinValue() {#getMinValue--}
```
public Object getMinValue()
```


Representa el valor mínimo en el eje de valores.

**Remarks**

El tipo minValue solo puede ser double o DateTime.

**Returns:**
java.lang.Object
### getMinorGridLines() {#getMinorGridLines--}
```
public Line getMinorGridLines()
```


Representa las líneas de cuadrícula menores en un eje de gráfico.

**Returns:**
[Line](../../com.aspose.cells/line)
### getMinorTickMark() {#getMinorTickMark--}
```
public int getMinorTickMark()
```


Representa el tipo de marca de graduación menor para el eje especificado.

Ver [TickMarkType](../../com.aspose.cells/tickmarktype).

**Returns:**
int
### getMinorUnit() {#getMinorUnit--}
```
public double getMinorUnit()
```


Representa las unidades menores para el eje.

**Remarks**

Las unidades menores deben ser mayores que cero.

**Returns:**
double
### getMinorUnitScale() {#getMinorUnitScale--}
```
public int getMinorUnitScale()
```


Representa la escala de la unidad mayor para el eje de categorías.

Ver [TimeUnit](../../com.aspose.cells/timeunit).

**Example**

```
         chart.getCategoryAxis().setCategoryType(CategoryType.TIME_SCALE);
         chart.getCategoryAxis().setMinorUnitScale(TimeUnit.MONTHS);
         chart.getCategoryAxis().setMinorUnit(2);
```

**Returns:**
int
### getTickLabelPosition() {#getTickLabelPosition--}
```
public int getTickLabelPosition()
```


Representa la posición de las etiquetas de marcas de graduación en el eje especificado.

Ver [TickLabelPositionType](../../com.aspose.cells/ticklabelpositiontype).

**Returns:**
int
### getTickLabelSpacing() {#getTickLabelSpacing--}
```
public int getTickLabelSpacing()
```


Representa el número de categorías o series entre las etiquetas de marcas de graduación. Se aplica solo a los ejes de categoría y series.

**Remarks**

El número debe estar entre 1 y 31999.

**Returns:**
int
### getTickLabels() {#getTickLabels--}
```
public TickLabels getTickLabels()
```


Devuelve un objeto [getTickLabels()](../../com.aspose.cells/axis\#getTickLabels--) que representa las etiquetas de marcas de graduación para el eje especificado.

**Returns:**
[TickLabels](../../com.aspose.cells/ticklabels)
### getTickMarkSpacing() {#getTickMarkSpacing--}
```
public int getTickMarkSpacing()
```


Devuelve o establece el número de categorías o series entre marcas de graduación. Se aplica solo a los ejes de categoría y series.

**Remarks**

El número debe estar entre 1 y 31999.

**Returns:**
int
### getTitle() {#getTitle--}
```
public Title getTitle()
```


Obtiene el título de este eje en el gráfico.

**Returns:**
[Title](../../com.aspose.cells/title)
### hasMultiLevelLabels() {#hasMultiLevelLabels--}
```
public boolean hasMultiLevelLabels()
```


Indica si las etiquetas se mostrarán en varios niveles.

**Remarks**

Solo válido para el eje de categoría.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoTickLabelSpacing() {#isAutoTickLabelSpacing--}
```
public boolean isAutoTickLabelSpacing()
```


Indica si el espaciado de la etiqueta de graduación es automático

**Returns:**
boolean
### isAutomaticMajorUnit() {#isAutomaticMajorUnit--}
```
public boolean isAutomaticMajorUnit()
```


Indica si la unidad mayor del eje se asigna automáticamente.

**Returns:**
boolean
### isAutomaticMaxValue() {#isAutomaticMaxValue--}
```
public boolean isAutomaticMaxValue()
```


Indica si el valor máximo se asigna automáticamente.

**Returns:**
boolean
### isAutomaticMinValue() {#isAutomaticMinValue--}
```
public boolean isAutomaticMinValue()
```


Indica si el valor mínimo se asigna automáticamente.

**Returns:**
boolean
### isAutomaticMinorUnit() {#isAutomaticMinorUnit--}
```
public boolean isAutomaticMinorUnit()
```


Indica si la unidad menor del eje se asigna automáticamente.

**Returns:**
boolean
### isBaseUnitAuto() {#isBaseUnitAuto--}
```
public boolean isBaseUnitAuto()
```


Representa si la unidad base es automática.

**Returns:**
boolean
### isDisplayUnitLabelShown() {#isDisplayUnitLabelShown--}
```
public boolean isDisplayUnitLabelShown()
```


Representa si la etiqueta de unidad de visualización se muestra en el eje especificado.

**Remarks**

El valor predeterminado es True. Solo funciona cuando [getDisplayUnit()](../../com.aspose.cells/axis\#getDisplayUnit--) no es [DisplayUnitType.NONE](../../com.aspose.cells/displayunittype\#NONE).

**Returns:**
boolean
### isLogarithmic() {#isLogarithmic--}
```
public boolean isLogarithmic()
```


Representa si el tipo de escala del eje de valores es logarítmico o no.

**Returns:**
boolean
### isPlotOrderReversed() {#isPlotOrderReversed--}
```
public boolean isPlotOrderReversed()
```


Representa si Microsoft Excel traza los puntos de datos de último a primero.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Representa si el eje es visible.

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




### setAutoTickLabelSpacing(boolean value) {#setAutoTickLabelSpacing-boolean-}
```
public void setAutoTickLabelSpacing(boolean value)
```


Indica si el espaciado de la etiqueta de graduación es automático

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAutomaticMajorUnit(boolean value) {#setAutomaticMajorUnit-boolean-}
```
public void setAutomaticMajorUnit(boolean value)
```


Indica si la unidad mayor del eje se asigna automáticamente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAutomaticMaxValue(boolean value) {#setAutomaticMaxValue-boolean-}
```
public void setAutomaticMaxValue(boolean value)
```


Indica si el valor máximo se asigna automáticamente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAutomaticMinValue(boolean value) {#setAutomaticMinValue-boolean-}
```
public void setAutomaticMinValue(boolean value)
```


Indica si el valor mínimo se asigna automáticamente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAutomaticMinorUnit(boolean value) {#setAutomaticMinorUnit-boolean-}
```
public void setAutomaticMinorUnit(boolean value)
```


Indica si la unidad menor del eje se asigna automáticamente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAxisBetweenCategories(boolean value) {#setAxisBetweenCategories-boolean-}
```
public void setAxisBetweenCategories(boolean value)
```


Representa si el eje de valores cruza el eje de categorías entre categorías.

**Remarks**

Esta propiedad se aplica solo a ejes de categorías, y no se aplica a gráficos 3D.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setBaseUnitAuto(boolean value) {#setBaseUnitAuto-boolean-}
```
public void setBaseUnitAuto(boolean value)
```


Representa si la unidad base es automática.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setBaseUnitScale(int value) {#setBaseUnitScale-int-}
```
public void setBaseUnitScale(int value)
```


Representa la escala de unidad base para el eje de categorías.

Ver [TimeUnit](../../com.aspose.cells/timeunit).

**Remarks**

Solo tiene efecto cuando la propiedad CategoryType está establecida en TimeScale.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setCategoryType(int value) {#setCategoryType-int-}
```
public void setCategoryType(int value)
```


Representa el tipo del eje de categorías.

Ver [CategoryType](../../com.aspose.cells/categorytype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setCrossAt(double value) {#setCrossAt-double-}
```
public void setCrossAt(double value)
```


Representa el punto en el eje de valores donde el eje de categorías lo cruza.

**Remarks**

El número debe ser un entero cuando se aplica al eje de categoría. Y el valor debe estar entre 1 y 31999.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setCrossType(int value) {#setCrossType-int-}
```
public void setCrossType(int value)
```


Representa el [getCrossType()](../../com.aspose.cells/axis\#getCrossType--) en el eje especificado donde cruza el otro eje.

Ver [CrossType](../../com.aspose.cells/crosstype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setCustUnit(int value) {#setCustUnit-int-}
```
public void setCustUnit(int value)
```


Especifica un valor personalizado para la unidad de visualización.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, por favor use la propiedad Axis.CustomUnit. Esta propiedad será eliminada 12 meses después a partir de enero de 2023. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setCustomDisplayUnit(double value) {#setCustomDisplayUnit-double-}
```
public void setCustomDisplayUnit(double value)
```


Especifica un valor personalizado para la unidad de visualización.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setCustomUnit(int value) {#setCustomUnit-int-}
```
public void setCustomUnit(int value)
```


Especifica un valor personalizado para la unidad de visualización.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, por favor use la propiedad Axis.CustomDisplayUnit. Esta propiedad será eliminada 12 meses después a partir de febrero de 2025. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setDisplayUnit(int value) {#setDisplayUnit-int-}
```
public void setDisplayUnit(int value)
```


Representa la etiqueta de unidad para el eje especificado.

Ver [DisplayUnitType](../../com.aspose.cells/displayunittype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setDisplayUnitLabelShown(boolean value) {#setDisplayUnitLabelShown-boolean-}
```
public void setDisplayUnitLabelShown(boolean value)
```


Representa si la etiqueta de unidad de visualización se muestra en el eje especificado.

**Remarks**

El valor predeterminado es True. Solo funciona cuando [getDisplayUnit()](../../com.aspose.cells/axis\#getDisplayUnit--) no es [DisplayUnitType.NONE](../../com.aspose.cells/displayunittype\#NONE).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setHasMultiLevelLabels(boolean value) {#setHasMultiLevelLabels-boolean-}
```
public void setHasMultiLevelLabels(boolean value)
```


Indica si las etiquetas se mostrarán en varios niveles.

**Remarks**

Solo válido para el eje de categoría.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setLogBase(double value) {#setLogBase-double-}
```
public void setLogBase(double value)
```


Representa la base logarítmica. El valor predeterminado es 10.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setLogarithmic(boolean value) {#setLogarithmic-boolean-}
```
public void setLogarithmic(boolean value)
```


Representa si el tipo de escala del eje de valores es logarítmico o no.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setMajorTickMark(int value) {#setMajorTickMark-int-}
```
public void setMajorTickMark(int value)
```


Representa el tipo de marca de graduación mayor para el eje especificado.

Ver [TickMarkType](../../com.aspose.cells/tickmarktype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setMajorUnit(double value) {#setMajorUnit-double-}
```
public void setMajorUnit(double value)
```


Representa las unidades mayores para el eje.

**Remarks**

Las unidades principales deben ser mayores que cero.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setMajorUnitScale(int value) {#setMajorUnitScale-int-}
```
public void setMajorUnitScale(int value)
```


Representa la escala de la unidad mayor para el eje de categorías.

Ver [TimeUnit](../../com.aspose.cells/timeunit).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setMaxValue(Object value) {#setMaxValue-java.lang.Object-}
```
public void setMaxValue(Object value)
```


Representa el valor máximo en el eje de valores.

**Remarks**

El tipo maxValue solo puede ser double o DateTime.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.Object |  |

### setMinValue(Object value) {#setMinValue-java.lang.Object-}
```
public void setMinValue(Object value)
```


Representa el valor mínimo en el eje de valores.

**Remarks**

El tipo minValue solo puede ser double o DateTime.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.Object |  |

### setMinorTickMark(int value) {#setMinorTickMark-int-}
```
public void setMinorTickMark(int value)
```


Representa el tipo de marca de graduación menor para el eje especificado.

Ver [TickMarkType](../../com.aspose.cells/tickmarktype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setMinorUnit(double value) {#setMinorUnit-double-}
```
public void setMinorUnit(double value)
```


Representa las unidades menores para el eje.

**Remarks**

Las unidades menores deben ser mayores que cero.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setMinorUnitScale(int value) {#setMinorUnitScale-int-}
```
public void setMinorUnitScale(int value)
```


Representa la escala de la unidad mayor para el eje de categorías.

Ver [TimeUnit](../../com.aspose.cells/timeunit).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setPlotOrderReversed(boolean value) {#setPlotOrderReversed-boolean-}
```
public void setPlotOrderReversed(boolean value)
```


Representa si Microsoft Excel traza los puntos de datos de último a primero.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setTickLabelPosition(int value) {#setTickLabelPosition-int-}
```
public void setTickLabelPosition(int value)
```


Representa la posición de las etiquetas de marcas de graduación en el eje especificado.

Ver [TickLabelPositionType](../../com.aspose.cells/ticklabelpositiontype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setTickLabelSpacing(int value) {#setTickLabelSpacing-int-}
```
public void setTickLabelSpacing(int value)
```


Representa el número de categorías o series entre las etiquetas de marcas de graduación. Se aplica solo a los ejes de categoría y series.

**Remarks**

El número debe estar entre 1 y 31999.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setTickMarkSpacing(int value) {#setTickMarkSpacing-int-}
```
public void setTickMarkSpacing(int value)
```


Devuelve o establece el número de categorías o series entre marcas de graduación. Se aplica solo a los ejes de categoría y series.

**Remarks**

El número debe estar entre 1 y 31999.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Representa si el eje es visible.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

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

