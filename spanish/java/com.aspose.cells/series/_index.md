---
title: "Series"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Encapsula el objeto que representa una serie de datos única en un gráfico."
type: docs
url: /es/java/com.aspose.cells/series/
---

**Inheritance:**
java.lang.Object
```
public class Series
```

Encapsula el objeto que representa una serie de datos única en un gráfico.

**Example**

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
         //Adding a sample value to "A4" cell
         worksheet.getCells().get("A4").putValue(200);
         //Adding a sample value to "B1" cell
         worksheet.getCells().get("B1").putValue(60);
         //Adding a sample value to "B2" cell
         worksheet.getCells().get("B2").putValue(32);
         //Adding a sample value to "B3" cell
         worksheet.getCells().get("B3").putValue(50);
         //Adding a sample value to "B4" cell
         worksheet.getCells().get("B4").putValue(40);
         //Adding a sample value to "C1" cell as category data
         worksheet.getCells().get("C1").putValue("Q1");
         //Adding a sample value to "C2" cell as category data
         worksheet.getCells().get("C2").putValue("Q2");
         //Adding a sample value to "C3" cell as category data
         worksheet.getCells().get("C3").putValue("Y1");
         //Adding a sample value to "C4" cell as category data
         worksheet.getCells().get("C4").putValue("Y2");
         //Adding a chart to the worksheet
         int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 15, 5);
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
         int seriesIndex = chart.getNSeries().add("A1:B4", true);
         //Setting the data source for the category data of NSeries
         chart.getNSeries().setCategoryData("C1:C4");
         Series series = chart.getNSeries().get(seriesIndex);
         //Setting the values of the series.
         series.setValues("=B1:B4");
         //Changing the chart type of the series.
         series.setType(ChartType.LINE);
         //Setting marker properties.
         series.getMarker().setMarkerStyle(ChartMarkerType.CIRCLE);
         series.getMarker().setForegroundColorSetType(FormattingType.AUTOMATIC);
         series.getMarker().setForegroundColor(com.aspose.cells.Color.getBlack());
         series.getMarker().setBackgroundColorSetType(FormattingType.AUTOMATIC);
 
         //do your business
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArea()](#getArea--) | Representa el área de fondo del objeto Series. |
| [getBar3DShapeType()](#getBar3DShapeType--) | Obtiene el tipo de forma 3D utilizado con el gráfico de barras o columnas 3-D. |
| [getBorder()](#getBorder--) | Representa el borde de un objeto Series. |
| [getBubbleScale()](#getBubbleScale--) | Obtiene el factor de escala para las burbujas en el grupo de gráfico especificado. |
| [getBubbleSizeRepresents()](#getBubbleSizeRepresents--) | Obtiene lo que representa el tamaño de la burbuja en un gráfico de burbujas. |
| [getBubbleSizes()](#getBubbleSizes--) | Obtiene los valores de tamaño de burbuja de la serie del gráfico. |
| [getCachedCategoryValues()](#getCachedCategoryValues--) | Obtiene los valores de categoría almacenados en caché para la serie |
| [getCachedValues()](#getCachedValues--) | Obtiene los valores almacenados en caché para la serie |
| [getCategoryValues()](#getCategoryValues--) | Obtiene los valores reales de categoría que se utilizan para trazar cada punto de esta serie en el gráfico. |
| [getClass()](#getClass--) |  |
| [getCountOfDataValues()](#getCountOfDataValues--) | Obtiene el número de valores de datos. |
| [getDataLabels()](#getDataLabels--) | Representa el objeto DataLabels para el ASeries especificado. |
| [getDisplayName()](#getDisplayName--) | Obtiene el nombre de la serie que se muestra en el gráfico. |
| [getDoughnutHoleSize()](#getDoughnutHoleSize--) | Devuelve o establece el tamaño del agujero en un grupo de gráfico de dona. |
| [getDownBars()](#getDownBars--) | Devuelve un objeto [DropBars](../../com.aspose.cells/dropbars) que representa las barras descendentes en un gráfico de líneas. |
| [getDropLines()](#getDropLines--) | Devuelve un objeto [Line](../../com.aspose.cells/line) que representa las líneas de caída para una serie en el gráfico de líneas o de áreas. |
| [getExplosion()](#getExplosion--) | La distancia de una porción de pastel abierta desde el centro del gráfico de pastel se expresa como un porcentaje del diámetro del pastel. |
| [getFirstSliceAngle()](#getFirstSliceAngle--) | Obtiene el ángulo de la primera porción de gráfico circular o de rosquilla, en grados (en sentido horario desde la vertical). |
| [getGapWidth()](#getGapWidth--) | Devuelve o establece el espacio entre grupos de barras o columnas, como un porcentaje del ancho de la barra o columna. |
| [getHas3DEffect()](#getHas3DEffect--) | True si la serie tiene una apariencia tridimensional. |
| [getHiLoLines()](#getHiLoLines--) | Devuelve un objeto HiLoLines que representa las líneas alto-bajo para una serie en un gráfico de líneas. |
| [getLayoutProperties()](#getLayoutProperties--) | Representa las propiedades del diseño. |
| [getLeaderLines()](#getLeaderLines--) | Representa las líneas guía en un gráfico. |
| [getLegendEntry()](#getLegendEntry--) | Obtiene la entrada de la leyenda según esta serie. |
| [getMarker()](#getMarker--) | Obtiene el [getMarker()](../../com.aspose.cells/series\#getMarker--). |
| [getName()](#getName--) | Obtiene el nombre de la serie de datos. |
| [getOverlap()](#getOverlap--) | Especifica cómo se posicionan las barras y columnas. |
| [getPlotOnSecondAxis()](#getPlotOnSecondAxis--) | Indica si esta serie se traza en el segundo eje de valores. |
| [getPointValues()](#getPointValues--) | Obtiene los valores reales que se utilizan para trazar cada punto de esta serie en el gráfico. |
| [getPoints()](#getPoints--) | Obtiene la colección de puntos de una serie en un gráfico. |
| [getSecondPlotSize()](#getSecondPlotSize--) | Devuelve o establece el tamaño de la sección secundaria de un gráfico de pastel dentro de pastel o de barra dentro de pastel, como un porcentaje del tamaño del pastel principal. |
| [getSeriesLines()](#getSeriesLines--) | Devuelve un objeto SeriesLines que representa las líneas de serie para un gráfico de barras apiladas o un gráfico de columnas apiladas. |
| [getShadow()](#getShadow--) | True si la serie tiene una sombra. |
| [getShapeProperties()](#getShapeProperties--) | Obtiene el objeto [ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection) que contiene las propiedades visuales de forma de la Serie. |
| [getShowNegativeBubbles()](#getShowNegativeBubbles--) | True si se muestran burbujas negativas para el grupo de gráficos. |
| [getSizeRepresents()](#getSizeRepresents--) | Obtiene lo que representa el tamaño de la burbuja en un gráfico de burbujas. |
| [getSmooth()](#getSmooth--) | Representa el suavizado de curvas. |
| [getSplitType()](#getSplitType--) | Devuelve o establece un valor que indica cómo determinar qué puntos de datos están en el segundo pastel o barra en un gráfico de pastel dentro de pastel o barra dentro de pastel. |
| [getSplitValue()](#getSplitValue--) | Devuelve o establece un valor que se utilizará para determinar qué puntos de datos están en el segundo pastel o barra en un gráfico de pastel dentro de pastel o barra dentro de pastel. |
| [getTrendLines()](#getTrendLines--) | Devuelve todas las líneas de tendencia de esta serie. |
| [getType()](#getType--) | Obtiene el tipo de una serie de datos. |
| [getUpBars()](#getUpBars--) | Devuelve un objeto DropBars que representa las barras ascendentes en un gráfico de líneas. |
| [getValues()](#getValues--) | Representa los valores Y de esta serie de gráfico. |
| [getValuesFormatCode()](#getValuesFormatCode--) | Representa el código de formato de la lista de números de Valores. |
| [getXErrorBar()](#getXErrorBar--) | Representa la barra de error en dirección X de la serie. |
| [getXValues()](#getXValues--) | Representa los valores X de esta serie de gráfico. |
| [getXValuesFormatCode()](#getXValuesFormatCode--) | Representa el código de formato de la lista de números de Valores X. |
| [getYErrorBar()](#getYErrorBar--) | Representa la barra de error en dirección Y de la serie. |
| [hasDropLines()](#hasDropLines--) | True si el gráfico tiene líneas de caída. |
| [hasHiLoLines()](#hasHiLoLines--) | True si el gráfico de líneas tiene líneas alto-bajo. |
| [hasLeaderLines()](#hasLeaderLines--) | True si la serie tiene líneas guía. |
| [hasRadarAxisLabels()](#hasRadarAxisLabels--) | True si un gráfico de radar tiene etiquetas del eje de categorías. |
| [hasSeriesLines()](#hasSeriesLines--) | Verdadero si un gráfico de columnas apiladas o un gráfico de barras tiene líneas de serie o si un gráfico de pastel dentro de pastel o un gráfico de barra dentro de pastel tiene líneas de conexión entre las dos secciones. |
| [hasUpDownBars()](#hasUpDownBars--) | Verdadero si un gráfico de líneas tiene barras superiores e inferiores. |
| [hashCode()](#hashCode--) |  |
| [isAutoSplit()](#isAutoSplit--) | Indica si el valor del umbral es automático. |
| [isColorVaried()](#isColorVaried--) | Representa si el color de los puntos varía. |
| [isFiltered()](#isFiltered--) | Indica si la serie está seleccionada o filtrada. |
| [isVerticalValues()](#isVerticalValues--) | Indica si la fuente de datos es vertical. |
| [move(int count)](#move-int-) | Mueve la serie hacia arriba o hacia abajo. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBar3DShapeType(int value)](#setBar3DShapeType-int-) | Establece el tipo de forma 3D utilizado con el gráfico de barras o columnas 3D. |
| [setBubbleScale(int value)](#setBubbleScale-int-) | Establece el factor de escala para las burbujas en el grupo de gráficos especificado. |
| [setBubbleSizeRepresents(int value)](#setBubbleSizeRepresents-int-) | Obtiene lo que representa el tamaño de la burbuja en un gráfico de burbujas. |
| [setBubbleSizes(String value)](#setBubbleSizes-java.lang.String-) | Establece los valores de tamaño de burbuja de la serie del gráfico. |
| [setColorVaried(boolean value)](#setColorVaried-boolean-) | Representa si el color de los puntos varía. |
| [setDoughnutHoleSize(int value)](#setDoughnutHoleSize-int-) | Devuelve o establece el tamaño del agujero en un grupo de gráfico de dona. |
| [setExplosion(int value)](#setExplosion-int-) | La distancia de una porción de pastel abierta desde el centro del gráfico de pastel se expresa como un porcentaje del diámetro del pastel. |
| [setFiltered(boolean value)](#setFiltered-boolean-) | Indica si la serie está seleccionada o filtrada. |
| [setFirstSliceAngle(short value)](#setFirstSliceAngle-short-) | Establece el ángulo de la primera porción de gráfico de pastel o de rosquilla, en grados (en sentido horario desde la vertical). |
| [setGapWidth(short value)](#setGapWidth-short-) | Devuelve o establece el espacio entre grupos de barras o columnas, como un porcentaje del ancho de la barra o columna. |
| [setHas3DEffect(boolean value)](#setHas3DEffect-boolean-) | True si la serie tiene una apariencia tridimensional. |
| [setHasDropLines(boolean value)](#setHasDropLines-boolean-) | True si el gráfico tiene líneas de caída. |
| [setHasHiLoLines(boolean value)](#setHasHiLoLines-boolean-) | True si el gráfico de líneas tiene líneas alto-bajo. |
| [setHasLeaderLines(boolean value)](#setHasLeaderLines-boolean-) | True si la serie tiene líneas guía. |
| [setHasRadarAxisLabels(boolean value)](#setHasRadarAxisLabels-boolean-) | True si un gráfico de radar tiene etiquetas del eje de categorías. |
| [setHasSeriesLines(boolean value)](#setHasSeriesLines-boolean-) | Verdadero si un gráfico de columnas apiladas o un gráfico de barras tiene líneas de serie o si un gráfico de pastel dentro de pastel o un gráfico de barra dentro de pastel tiene líneas de conexión entre las dos secciones. |
| [setHasUpDownBars(boolean value)](#setHasUpDownBars-boolean-) | Verdadero si un gráfico de líneas tiene barras superiores e inferiores. |
| [setName(String value)](#setName-java.lang.String-) | Establece el nombre de la serie de datos. |
| [setOverlap(short value)](#setOverlap-short-) | Especifica cómo se posicionan las barras y columnas. |
| [setPlotOnSecondAxis(boolean value)](#setPlotOnSecondAxis-boolean-) | Indica si esta serie se traza en el segundo eje de valores. |
| [setSecondPlotSize(short value)](#setSecondPlotSize-short-) | Devuelve o establece el tamaño de la sección secundaria de un gráfico de pastel dentro de pastel o de barra dentro de pastel, como un porcentaje del tamaño del pastel principal. |
| [setShadow(boolean value)](#setShadow-boolean-) | True si la serie tiene una sombra. |
| [setShowNegativeBubbles(boolean value)](#setShowNegativeBubbles-boolean-) | True si se muestran burbujas negativas para el grupo de gráficos. |
| [setSizeRepresents(int value)](#setSizeRepresents-int-) | Establece lo que representa el tamaño de la burbuja en un gráfico de burbujas. |
| [setSmooth(boolean value)](#setSmooth-boolean-) | Representa el suavizado de curvas. |
| [setSplitType(int value)](#setSplitType-int-) | Devuelve o establece un valor que indica cómo determinar qué puntos de datos están en el segundo pastel o barra en un gráfico de pastel dentro de pastel o barra dentro de pastel. |
| [setSplitValue(double value)](#setSplitValue-double-) | Devuelve o establece un valor que se utilizará para determinar qué puntos de datos están en el segundo pastel o barra en un gráfico de pastel dentro de pastel o barra dentro de pastel. |
| [setType(int value)](#setType-int-) | Establece el tipo de una serie de datos. |
| [setValues(String value)](#setValues-java.lang.String-) | Representa los valores Y de esta serie de gráfico. |
| [setValuesFormatCode(String value)](#setValuesFormatCode-java.lang.String-) | Representa el código de formato de la lista de números de Valores. |
| [setXValues(String value)](#setXValues-java.lang.String-) | Representa los valores X de esta serie de gráfico. |
| [setXValuesFormatCode(String value)](#setXValuesFormatCode-java.lang.String-) | Representa el código de formato de la lista de números de Valores X. |
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


Representa el área de fondo del objeto Series.

**Returns:**
[Area](../../com.aspose.cells/area)
### getBar3DShapeType() {#getBar3DShapeType--}
```
public int getBar3DShapeType()
```


Obtiene el tipo de forma 3D utilizado con el gráfico de barras o columnas 3-D.

Ver [Bar3DShapeType](../../com.aspose.cells/bar3dshapetype).

**Returns:**
int
### getBorder() {#getBorder--}
```
public Line getBorder()
```


Representa el borde de un objeto Series.

**Returns:**
[Line](../../com.aspose.cells/line)
### getBubbleScale() {#getBubbleScale--}
```
public int getBubbleScale()
```


Obtiene el factor de escala para las burbujas en el grupo de gráficos especificado. Puede ser un valor entero de 0 (cero) a 300, correspondiente a un porcentaje del tamaño predeterminado. Se aplica solo a gráficos de burbujas.

**Returns:**
int
### getBubbleSizeRepresents() {#getBubbleSizeRepresents--}
```
public int getBubbleSizeRepresents()
```


Obtiene lo que representa el tamaño de la burbuja en un gráfico de burbujas.

Ver [BubbleSizeRepresents](../../com.aspose.cells/bubblesizerepresents).

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad Aspose.Cells.Charts.Series.SizeRepresents. Esta propiedad será eliminada 12 meses después desde ENERO de 2012. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
int
### getBubbleSizes() {#getBubbleSizes--}
```
public String getBubbleSizes()
```


Obtiene los valores de tamaño de burbuja de la serie del gráfico.

**Remarks**

Solo para [ChartType.BUBBLE](../../com.aspose.cells/charttype\#BUBBLE) o [ChartType.BUBBLE\_3\_D](../../com.aspose.cells/charttype\#BUBBLE-3-D).

**Returns:**
java.lang.String
### getCachedCategoryValues() {#getCachedCategoryValues--}
```
public ArrayList getCachedCategoryValues()
```


Obtiene los valores de categoría almacenados en caché para la serie

**Remarks**

NOTA: Esta propiedad es actualmente solo para uso interno. Será cambiada o eliminada en la próxima versión.

**Returns:**
java.util.ArrayList
### getCachedValues() {#getCachedValues--}
```
public ArrayList getCachedValues()
```


Obtiene los valores almacenados en caché para la serie

**Remarks**

NOTA: Esta propiedad es actualmente solo para uso interno. Será cambiada o eliminada en la próxima versión.

**Returns:**
java.util.ArrayList
### getCategoryValues() {#getCategoryValues--}
```
public ChartDataValue[][] getCategoryValues()
```


Obtiene los valores reales de categoría que se utilizan para trazar cada punto de esta serie en el gráfico.

**Remarks**

Esta propiedad ofrece una forma conveniente de obtener los valores reales correspondientes a los datos definidos por [getXValues()](../../com.aspose.cells/series\#getXValues--), especialmente cuando la fuente de datos especificada es un enlace externo, una fórmula, ...etc.

**Example**

```
         //Standalone example
         Workbook workbook = new Workbook("ExternalSourceChart.xlsx");
         Worksheet worksheet = workbook.getWorksheets().get(0);
         Chart chart = worksheet.getCharts().get(0);
         chart.calculate();
         String XValues = chart.getNSeries().get(0).getXValues();
         // XValues may be like "[External.xlsx]Sheet1!$B$2:$C$6" which is complicated
         // for user to get the actual values(the values may be linked to another workbook,
         // or cached in current workbook). Here you can use CategoryValues property
         // to get the category values actually displayed in the Excel interface
         // in the form of a two-dimensional array.
         ChartDataValue[][] v1 = chart.getNSeries().get(0).getCategoryValues();
```

**Returns:**
com.aspose.cells.ChartDataValue[][]
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCountOfDataValues() {#getCountOfDataValues--}
```
public int getCountOfDataValues()
```


Obtiene el número de valores de datos.

**Returns:**
int
### getDataLabels() {#getDataLabels--}
```
public DataLabels getDataLabels()
```


Representa el objeto DataLabels para el ASeries especificado.

**Returns:**
[DataLabels](../../com.aspose.cells/datalabels)
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Obtiene el nombre de la serie que se muestra en el gráfico.

**Returns:**
java.lang.String
### getDoughnutHoleSize() {#getDoughnutHoleSize--}
```
public int getDoughnutHoleSize()
```


Devuelve o establece el tamaño del agujero en un grupo de gráfico de rosquilla. El tamaño del agujero se expresa como un porcentaje del tamaño del gráfico, entre el 10 y el 90 por ciento.

**Returns:**
int
### getDownBars() {#getDownBars--}
```
public DropBars getDownBars()
```


Devuelve un objeto [DropBars](../../com.aspose.cells/dropbars) que representa las barras descendentes en un gráfico de líneas. Se aplica solo a gráficos de líneas.

**Returns:**
[DropBars](../../com.aspose.cells/dropbars)
### getDropLines() {#getDropLines--}
```
public Line getDropLines()
```


Devuelve un objeto [Line](../../com.aspose.cells/line) que representa las líneas de caída para una serie en el gráfico de líneas o de áreas. Se aplica solo a gráficos de líneas o de áreas.

**Returns:**
[Line](../../com.aspose.cells/line)
### getExplosion() {#getExplosion--}
```
public int getExplosion()
```


La distancia de una porción de pastel abierta desde el centro del gráfico de pastel se expresa como un porcentaje del diámetro del pastel.

**Returns:**
int
### getFirstSliceAngle() {#getFirstSliceAngle--}
```
public short getFirstSliceAngle()
```


Obtiene el ángulo de la primera porción de gráfico de pastel o de rosquilla, en grados (en sentido horario desde la vertical). Se aplica solo a gráficos de pastel, pastel 3D y rosquilla, con valores de 0 a 360.

**Returns:**
short
### getGapWidth() {#getGapWidth--}
```
public short getGapWidth()
```


Devuelve o establece el espacio entre grupos de barras o columnas, como un porcentaje del ancho de la barra o columna. El valor de esta propiedad debe estar entre 0 y 500.

**Returns:**
short
### getHas3DEffect() {#getHas3DEffect--}
```
public boolean getHas3DEffect()
```


True si la serie tiene una apariencia tridimensional.

**Remarks**

Se aplica solo a los gráficos [ChartType.BUBBLE](../../com.aspose.cells/charttype\#BUBBLE) o [ChartType.BUBBLE\_3\_D](../../com.aspose.cells/charttype\#BUBBLE-3-D).

**Returns:**
boolean
### getHiLoLines() {#getHiLoLines--}
```
public Line getHiLoLines()
```


Devuelve un objeto HiLoLines que representa las líneas alto-bajo de una serie en un gráfico de líneas. Se aplica solo a gráficos de líneas.

**Returns:**
[Line](../../com.aspose.cells/line)
### getLayoutProperties() {#getLayoutProperties--}
```
public SeriesLayoutProperties getLayoutProperties()
```


Representa las propiedades del diseño.

**Returns:**
[SeriesLayoutProperties](../../com.aspose.cells/serieslayoutproperties)
### getLeaderLines() {#getLeaderLines--}
```
public Line getLeaderLines()
```


Representa líneas guía en un gráfico. Las líneas guía conectan las etiquetas de datos con los puntos de datos. Este objeto no es una colección; no existe un objeto que represente una única línea guía.

**Returns:**
[Line](../../com.aspose.cells/line)
### getLegendEntry() {#getLegendEntry--}
```
public LegendEntry getLegendEntry()
```


Obtiene la entrada de la leyenda según esta serie.

**Returns:**
[LegendEntry](../../com.aspose.cells/legendentry)
### getMarker() {#getMarker--}
```
public Marker getMarker()
```


Obtiene el [getMarker()](../../com.aspose.cells/series\#getMarker--).

**Returns:**
[Marker](../../com.aspose.cells/marker)
### getName() {#getName--}
```
public String getName()
```


Obtiene el nombre de la serie de datos.

**Example**

```
         //Reference name to a cell
         chart.getNSeries().get(0).setName("=A1");
 
         //Set a string to name
         chart.getNSeries().get(0).setName("First Series");
```

**Returns:**
java.lang.String
### getOverlap() {#getOverlap--}
```
public short getOverlap()
```


Especifica cómo se posicionan las barras y columnas. Puede ser un valor entre -100 y 100. Se aplica solo a gráficos de barras 2-D y columnas 2-D.

**Returns:**
short
### getPlotOnSecondAxis() {#getPlotOnSecondAxis--}
```
public boolean getPlotOnSecondAxis()
```


Indica si esta serie se traza en el segundo eje de valores.

**Returns:**
boolean
### getPointValues() {#getPointValues--}
```
public ChartDataValue[] getPointValues()
```


Obtiene los valores reales que se utilizan para trazar cada punto de esta serie en el gráfico.

**Remarks**

Esta propiedad ofrece una forma práctica de obtener los valores reales correspondientes a los datos definidos por [getValues()](../../com.aspose.cells/series\#getValues--), especialmente cuando la fuente de datos especificada es un enlace externo, una fórmula, etc.

**Example**

```
         Workbook workbook = new Workbook("ExternalSourceChart.xlsx");
         Worksheet worksheet = workbook.getWorksheets().get(0);
         Chart chart = worksheet.getCharts().get(0);
         chart.calculate();
         String Values = chart.getNSeries().get(0).getValues();
         // Values could be like "[External.xlsx]Sheet1!$A$1:$A$6" which is complicated
         // for user to get the actual values(the values may be linked to another workbook,
         // or cached in current workbook). Here you can use PointValues property
         // to get the values actually displayed in the Excel interface
         // in the form of an array.
         ChartDataValue[] v1 = chart.getNSeries().get(0).getPointValues();
```

**Returns:**
com.aspose.cells.ChartDataValue[]
### getPoints() {#getPoints--}
```
public ChartPointCollection getPoints()
```


Obtiene la colección de puntos de una serie en un gráfico.

**Remarks**

Cuando el gráfico es Pie of Pie o Bar of Pie, el último punto es otro punto en la primera porción del pastel.

**Returns:**
[ChartPointCollection](../../com.aspose.cells/chartpointcollection)
### getSecondPlotSize() {#getSecondPlotSize--}
```
public short getSecondPlotSize()
```


Devuelve o establece el tamaño de la sección secundaria de un gráfico Pie of Pie o Bar of Pie, como porcentaje del tamaño del pastel principal. Puede ser un valor de 5 a 200.

**Returns:**
short
### getSeriesLines() {#getSeriesLines--}
```
public Line getSeriesLines()
```


Devuelve un objeto SeriesLines que representa las líneas de serie para un gráfico de barras apiladas o un gráfico de columnas apiladas. Se aplica solo a gráficos de barras apiladas y columnas apiladas.

**Returns:**
[Line](../../com.aspose.cells/line)
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


True si la serie tiene una sombra.

**Returns:**
boolean
### getShapeProperties() {#getShapeProperties--}
```
public ShapePropertyCollection getShapeProperties()
```


Obtiene el objeto [ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection) que contiene las propiedades visuales de forma de la Serie.

**Returns:**
[ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection)
### getShowNegativeBubbles() {#getShowNegativeBubbles--}
```
public boolean getShowNegativeBubbles()
```


True si se muestran burbujas negativas para el grupo de gráficos. Válido solo para gráficos de burbujas.

**Returns:**
boolean
### getSizeRepresents() {#getSizeRepresents--}
```
public int getSizeRepresents()
```


Obtiene lo que representa el tamaño de la burbuja en un gráfico de burbujas.

Ver [BubbleSizeRepresents](../../com.aspose.cells/bubblesizerepresents).

**Remarks**

BubbleSizeRepresents.SizeIsArea indica que el valor [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) es el área de la burbuja. BubbleSizeRepresents.SizeIsWidth indica que el valor [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) es el ancho de la burbuja.

**Returns:**
int
### getSmooth() {#getSmooth--}
```
public boolean getSmooth()
```


Representa el suavizado de curvas. True si el suavizado de curvas está activado para el gráfico de líneas o de dispersión. Se aplica solo a gráficos de líneas y gráficos de dispersión con líneas.

**Returns:**
boolean
### getSplitType() {#getSplitType--}
```
public int getSplitType()
```


Devuelve o establece un valor que indica cómo determinar qué puntos de datos están en el segundo pastel o barra en un gráfico de pastel dentro de pastel o barra dentro de pastel.

Ver [ChartSplitType](../../com.aspose.cells/chartsplittype).

**Returns:**
int
### getSplitValue() {#getSplitValue--}
```
public double getSplitValue()
```


Devuelve o establece un valor que se utilizará para determinar qué puntos de datos están en el segundo pastel o barra en un gráfico de pastel dentro de pastel o barra dentro de pastel.

**Returns:**
double
### getTrendLines() {#getTrendLines--}
```
public TrendlineCollection getTrendLines()
```


Devuelve todas las líneas de tendencia de esta serie.

**Returns:**
[TrendlineCollection](../../com.aspose.cells/trendlinecollection)
### getType() {#getType--}
```
public int getType()
```


Obtiene el tipo de una serie de datos.

Ver [ChartType](../../com.aspose.cells/charttype).

**Returns:**
int
### getUpBars() {#getUpBars--}
```
public DropBars getUpBars()
```


Devuelve un objeto DropBars que representa las barras ascendentes en un gráfico de líneas. Se aplica solo a gráficos de líneas.

**Returns:**
[DropBars](../../com.aspose.cells/dropbars)
### getValues() {#getValues--}
```
public String getValues()
```


Representa los valores Y de esta serie de gráfico.

**Remarks**

Para obtener los valores reales (correspondientes a cada punto de esta serie) definidos por esta propiedad, utilice [getPointValues()](../../com.aspose.cells/series\#getPointValues--).

**Returns:**
java.lang.String
### getValuesFormatCode() {#getValuesFormatCode--}
```
public String getValuesFormatCode()
```


Representa el código de formato de la lista de números de Valores.

**Returns:**
java.lang.String
### getXErrorBar() {#getXErrorBar--}
```
public ErrorBar getXErrorBar()
```


Representa la barra de error en dirección X de la serie.

**Returns:**
[ErrorBar](../../com.aspose.cells/errorbar)
### getXValues() {#getXValues--}
```
public String getXValues()
```


Representa los valores X de esta serie de gráfico.

**Remarks**

Solo para gráficos de dispersión y burbujas. Por favor, use [SeriesCollection.getCategoryData()](../../com.aspose.cells/seriescollection\#getCategoryData--) para otros tipos de gráficos; [getCategoryValues()](../../com.aspose.cells/series\#getCategoryValues--) se utiliza para obtener los valores de categoría reales de esta serie.

**Returns:**
java.lang.String
### getXValuesFormatCode() {#getXValuesFormatCode--}
```
public String getXValuesFormatCode()
```


Representa el código de formato de la lista de números de Valores X.

**Returns:**
java.lang.String
### getYErrorBar() {#getYErrorBar--}
```
public ErrorBar getYErrorBar()
```


Representa la barra de error en dirección Y de la serie.

**Returns:**
[ErrorBar](../../com.aspose.cells/errorbar)
### hasDropLines() {#hasDropLines--}
```
public boolean hasDropLines()
```


True si el gráfico tiene líneas de caída. Se aplica solo a gráficos de líneas o de áreas.

**Returns:**
boolean
### hasHiLoLines() {#hasHiLoLines--}
```
public boolean hasHiLoLines()
```


True si el gráfico de líneas tiene líneas alto-bajo. Se aplica solo a gráficos de líneas.

**Returns:**
boolean
### hasLeaderLines() {#hasLeaderLines--}
```
public boolean hasLeaderLines()
```


True si la serie tiene líneas guía.

**Returns:**
boolean
### hasRadarAxisLabels() {#hasRadarAxisLabels--}
```
public boolean hasRadarAxisLabels()
```


True si un gráfico de radar tiene etiquetas en el eje de categorías. Se aplica solo a gráficos de radar.

**Returns:**
boolean
### hasSeriesLines() {#hasSeriesLines--}
```
public boolean hasSeriesLines()
```


True si un gráfico de columnas apiladas o de barras tiene líneas de serie o si un gráfico Pie of Pie o Bar of Pie tiene líneas de conexión entre las dos secciones. Se aplica solo a gráficos de columnas apiladas, gráficos de barras, gráficos Pie of Pie o Bar of Pie.

**Returns:**
boolean
### hasUpDownBars() {#hasUpDownBars--}
```
public boolean hasUpDownBars()
```


True si un gráfico de líneas tiene barras ascendentes y descendentes. Se aplica solo a gráficos de líneas.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoSplit() {#isAutoSplit--}
```
public boolean isAutoSplit()
```


Indica si el valor del umbral es automático.

**Returns:**
boolean
### isColorVaried() {#isColorVaried--}
```
public boolean isColorVaried()
```


Representa si el color de los puntos varía. El gráfico debe contener solo una serie o ser un gráfico de pastel.

**Returns:**
boolean
### isFiltered() {#isFiltered--}
```
public boolean isFiltered()
```


Indica si la serie está seleccionada o filtrada. True indica que esta serie está filtrada y no se mostrará en el gráfico.

**Returns:**
boolean
### isVerticalValues() {#isVerticalValues--}
```
public boolean isVerticalValues()
```


Indica si la fuente de datos es vertical.

**Returns:**
boolean
### move(int count) {#move-int-}
```
public void move(int count)
```


Mueve la serie hacia arriba o hacia abajo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| recuento | int | El número de movimientos hacia arriba o abajo. Mueva la serie hacia arriba si este valor es menor que cero; mueva la serie hacia abajo si es mayor que cero. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setBar3DShapeType(int value) {#setBar3DShapeType-int-}
```
public void setBar3DShapeType(int value)
```


Establece el tipo de forma 3D utilizado con el gráfico de barras o columnas 3D.

Ver [Bar3DShapeType](../../com.aspose.cells/bar3dshapetype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setBubbleScale(int value) {#setBubbleScale-int-}
```
public void setBubbleScale(int value)
```


Establece el factor de escala para las burbujas en el grupo de gráficos especificado. Puede ser un valor entero de 0 (cero) a 300, correspondiente a un porcentaje del tamaño predeterminado. Se aplica solo a gráficos de burbujas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setBubbleSizeRepresents(int value) {#setBubbleSizeRepresents-int-}
```
public void setBubbleSizeRepresents(int value)
```


Obtiene lo que representa el tamaño de la burbuja en un gráfico de burbujas.

Ver [BubbleSizeRepresents](../../com.aspose.cells/bubblesizerepresents).

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad Aspose.Cells.Charts.Series.SizeRepresents. Esta propiedad será eliminada 12 meses después desde ENERO de 2012. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setBubbleSizes(String value) {#setBubbleSizes-java.lang.String-}
```
public void setBubbleSizes(String value)
```


Establece los valores de tamaño de burbuja de la serie del gráfico.

**Remarks**

Solo para [ChartType.BUBBLE](../../com.aspose.cells/charttype\#BUBBLE) o [ChartType.BUBBLE\_3\_D](../../com.aspose.cells/charttype\#BUBBLE-3-D).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setColorVaried(boolean value) {#setColorVaried-boolean-}
```
public void setColorVaried(boolean value)
```


Representa si el color de los puntos varía. El gráfico debe contener solo una serie o ser un gráfico de pastel.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setDoughnutHoleSize(int value) {#setDoughnutHoleSize-int-}
```
public void setDoughnutHoleSize(int value)
```


Devuelve o establece el tamaño del agujero en un grupo de gráfico de rosquilla. El tamaño del agujero se expresa como un porcentaje del tamaño del gráfico, entre el 10 y el 90 por ciento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setExplosion(int value) {#setExplosion-int-}
```
public void setExplosion(int value)
```


La distancia de una porción de pastel abierta desde el centro del gráfico de pastel se expresa como un porcentaje del diámetro del pastel.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setFiltered(boolean value) {#setFiltered-boolean-}
```
public void setFiltered(boolean value)
```


Indica si la serie está seleccionada o filtrada. True indica que esta serie está filtrada y no se mostrará en el gráfico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setFirstSliceAngle(short value) {#setFirstSliceAngle-short-}
```
public void setFirstSliceAngle(short value)
```


Establece el ángulo de la primera porción de gráfico circular o de rosquilla, en grados (en sentido horario desde la vertical). Se aplica solo a gráficos circulares, circulares 3D y de rosquilla, con valores de 0 a 360.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | short |  |

### setGapWidth(short value) {#setGapWidth-short-}
```
public void setGapWidth(short value)
```


Devuelve o establece el espacio entre grupos de barras o columnas, como un porcentaje del ancho de la barra o columna. El valor de esta propiedad debe estar entre 0 y 500.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | short |  |

### setHas3DEffect(boolean value) {#setHas3DEffect-boolean-}
```
public void setHas3DEffect(boolean value)
```


True si la serie tiene una apariencia tridimensional.

**Remarks**

Se aplica solo a los gráficos [ChartType.BUBBLE](../../com.aspose.cells/charttype\#BUBBLE) o [ChartType.BUBBLE\_3\_D](../../com.aspose.cells/charttype\#BUBBLE-3-D).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setHasDropLines(boolean value) {#setHasDropLines-boolean-}
```
public void setHasDropLines(boolean value)
```


True si el gráfico tiene líneas de caída. Se aplica solo a gráficos de líneas o de áreas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setHasHiLoLines(boolean value) {#setHasHiLoLines-boolean-}
```
public void setHasHiLoLines(boolean value)
```


True si el gráfico de líneas tiene líneas alto-bajo. Se aplica solo a gráficos de líneas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setHasLeaderLines(boolean value) {#setHasLeaderLines-boolean-}
```
public void setHasLeaderLines(boolean value)
```


True si la serie tiene líneas guía.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setHasRadarAxisLabels(boolean value) {#setHasRadarAxisLabels-boolean-}
```
public void setHasRadarAxisLabels(boolean value)
```


True si un gráfico de radar tiene etiquetas en el eje de categorías. Se aplica solo a gráficos de radar.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setHasSeriesLines(boolean value) {#setHasSeriesLines-boolean-}
```
public void setHasSeriesLines(boolean value)
```


True si un gráfico de columnas apiladas o de barras tiene líneas de serie o si un gráfico Pie of Pie o Bar of Pie tiene líneas de conexión entre las dos secciones. Se aplica solo a gráficos de columnas apiladas, gráficos de barras, gráficos Pie of Pie o Bar of Pie.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setHasUpDownBars(boolean value) {#setHasUpDownBars-boolean-}
```
public void setHasUpDownBars(boolean value)
```


True si un gráfico de líneas tiene barras ascendentes y descendentes. Se aplica solo a gráficos de líneas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Establece el nombre de la serie de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setOverlap(short value) {#setOverlap-short-}
```
public void setOverlap(short value)
```


Especifica cómo se posicionan las barras y columnas. Puede ser un valor entre -100 y 100. Se aplica solo a gráficos de barras 2-D y columnas 2-D.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | short |  |

### setPlotOnSecondAxis(boolean value) {#setPlotOnSecondAxis-boolean-}
```
public void setPlotOnSecondAxis(boolean value)
```


Indica si esta serie se traza en el segundo eje de valores.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSecondPlotSize(short value) {#setSecondPlotSize-short-}
```
public void setSecondPlotSize(short value)
```


Devuelve o establece el tamaño de la sección secundaria de un gráfico Pie of Pie o Bar of Pie, como porcentaje del tamaño del pastel principal. Puede ser un valor de 5 a 200.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | short |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


True si la serie tiene una sombra.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowNegativeBubbles(boolean value) {#setShowNegativeBubbles-boolean-}
```
public void setShowNegativeBubbles(boolean value)
```


True si se muestran burbujas negativas para el grupo de gráficos. Válido solo para gráficos de burbujas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSizeRepresents(int value) {#setSizeRepresents-int-}
```
public void setSizeRepresents(int value)
```


Establece lo que representa el tamaño de la burbuja en un gráfico de burbujas.

Ver [BubbleSizeRepresents](../../com.aspose.cells/bubblesizerepresents).

**Remarks**

BubbleSizeRepresents.SizeIsArea indica que el valor [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) es el área de la burbuja. BubbleSizeRepresents.SizeIsWidth indica que el valor [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) es el ancho de la burbuja.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setSmooth(boolean value) {#setSmooth-boolean-}
```
public void setSmooth(boolean value)
```


Representa el suavizado de curvas. True si el suavizado de curvas está activado para el gráfico de líneas o de dispersión. Se aplica solo a gráficos de líneas y gráficos de dispersión con líneas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSplitType(int value) {#setSplitType-int-}
```
public void setSplitType(int value)
```


Devuelve o establece un valor que indica cómo determinar qué puntos de datos están en el segundo pastel o barra en un gráfico de pastel dentro de pastel o barra dentro de pastel.

Ver [ChartSplitType](../../com.aspose.cells/chartsplittype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setSplitValue(double value) {#setSplitValue-double-}
```
public void setSplitValue(double value)
```


Devuelve o establece un valor que se utilizará para determinar qué puntos de datos están en el segundo pastel o barra en un gráfico de pastel dentro de pastel o barra dentro de pastel.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Establece el tipo de una serie de datos.

Ver [ChartType](../../com.aspose.cells/charttype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setValues(String value) {#setValues-java.lang.String-}
```
public void setValues(String value)
```


Representa los valores Y de esta serie de gráfico.

**Remarks**

Para obtener los valores reales (correspondientes a cada punto de esta serie) definidos por esta propiedad, utilice [getPointValues()](../../com.aspose.cells/series\#getPointValues--).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setValuesFormatCode(String value) {#setValuesFormatCode-java.lang.String-}
```
public void setValuesFormatCode(String value)
```


Representa el código de formato de la lista de números de Valores.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setXValues(String value) {#setXValues-java.lang.String-}
```
public void setXValues(String value)
```


Representa los valores X de esta serie de gráfico.

**Remarks**

Solo para gráficos de dispersión y burbujas. Por favor, use [SeriesCollection.getCategoryData()](../../com.aspose.cells/seriescollection\#getCategoryData--) para otros tipos de gráficos; [getCategoryValues()](../../com.aspose.cells/series\#getCategoryValues--) se utiliza para obtener los valores de categoría reales de esta serie.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setXValuesFormatCode(String value) {#setXValuesFormatCode-java.lang.String-}
```
public void setXValuesFormatCode(String value)
```


Representa el código de formato de la lista de números de Valores X.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

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

