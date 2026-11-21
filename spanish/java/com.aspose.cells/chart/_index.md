---
title: "Gráfico"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Encapsula el objeto que representa un único gráfico de Excel."
type: docs
url: /es/java/com.aspose.cells/chart/
---

**Inheritance:**
java.lang.Object
```
public class Chart
```

Encapsula el objeto que representa un único gráfico de Excel.

**Example**

El siguiente código muestra cómo crear un gráfico con código .NET.

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
         	chart.setShowLegend(true);
         	chart.getTitle().setText("Income Analysis");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [calculate()](#calculate--) | Calcula las posiciones personalizadas del área de trazado y los ejes si sus posiciones se asignan automáticamente. |
| [calculate(ChartCalculateOptions calculateOptions)](#calculate-com.aspose.cells.ChartCalculateOptions-) | Calcula la posición personalizada del área de trazado y los ejes si su posición se asigna automáticamente, con Opciones de Cálculo de Gráfico. |
| [changeTemplate(byte[] data)](#changeTemplate-byte---) | Cambiar el tipo de gráfico con una plantilla predefinida. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActualChartSize()](#getActualChartSize--) | Obtiene el tamaño real del gráfico en unidades de píxeles. |
| [getActualSize()](#getActualSize--) | Obtiene el tamaño real del gráfico en unidades de píxeles. |
| [getAutoScaling()](#getAutoScaling--) | True si Microsoft Excel escala un gráfico 3D para que su tamaño sea más cercano al del gráfico 2D equivalente. |
| [getBackWall()](#getBackWall--) | Devuelve un objeto [getWalls()](../../com.aspose.cells/chart\\#getWalls--) que representa la pared trasera de un gráfico 3D. |
| [getCategoryAxis()](#getCategoryAxis--) | Obtiene el eje X del gráfico. |
| [getChartArea()](#getChartArea--) | Obtiene el área del gráfico en la hoja de cálculo. |
| [getChartDataRange()](#getChartDataRange--) | Obtiene el rango de origen de datos del gráfico. |
| [getChartDataTable()](#getChartDataTable--) | Representa la tabla de datos del gráfico. |
| [getChartObject()](#getChartObject--) | Representa el chartShape; |
| [getChartShape()](#getChartShape--) | Representa el chartShape; |
| [getClass()](#getClass--) |  |
| [getDepthPercent()](#getDepthPercent--) | Representa la profundidad de un gráfico 3-D como un porcentaje del ancho del gráfico (entre el 20 y el 2000 por ciento). |
| [getDisplayNaAsBlank()](#getDisplayNaAsBlank--) | Indica si se debe mostrar \#N/A como un valor en blanco. |
| [getElevation()](#getElevation--) | Representa la elevación de la vista del gráfico 3-D, en grados. |
| [getFilteredNSeries()](#getFilteredNSeries--) | Obtiene una colección [SeriesCollection](../../com.aspose.cells/seriescollection) que representa las series de datos que se filtran en el gráfico. |
| [getFirstSliceAngle()](#getFirstSliceAngle--) | Obtiene el ángulo de la primera porción de gráfico circular o de rosquilla, en grados (en sentido horario desde la vertical). |
| [getFloor()](#getFloor--) | Devuelve un objeto [getFloor()](../../com.aspose.cells/chart\#getFloor--) que representa las paredes de un gráfico 3-D. |
| [getGapDepth()](#getGapDepth--) | Obtiene la distancia entre las series de datos en un gráfico 3-D, como un porcentaje del ancho del marcador. |
| [getGapWidth()](#getGapWidth--) | Devuelve o establece el espacio entre grupos de barras o columnas, como un porcentaje del ancho de la barra o columna. |
| [getHeightPercent()](#getHeightPercent--) | Devuelve o establece la altura de un gráfico 3-D como un porcentaje del ancho del gráfico (entre el 5 y el 500 por ciento). |
| [getHidePivotFieldButtons()](#getHidePivotFieldButtons--) | Indica si se ocultan los botones de campo del gráfico dinámico solo cuando el gráfico es PivotChart. |
| [getIs3D()](#getIs3D--) | Indica si el gráfico es un gráfico 3d. |
| [getLegend()](#getLegend--) | Obtiene la leyenda del gráfico. |
| [getLine()](#getLine--) | Obtiene la línea. |
| [getNSeries()](#getNSeries--) | Obtiene una colección [SeriesCollection](../../com.aspose.cells/seriescollection) que representa las series de datos en el gráfico. |
| [getName()](#getName--) | Obtiene el nombre del gráfico. |
| [getPageSetup()](#getPageSetup--) | Representa la descripción de la configuración de página en este gráfico. |
| [getPerspective()](#getPerspective--) | Devuelve o establece la perspectiva para la vista del gráfico three\u9225\u6178dimensional. |
| [getPivotOptions()](#getPivotOptions--) | Especifica los controles dinámicos que aparecen en el gráfico. |
| [getPivotSource()](#getPivotSource--) | El origen son los datos de la tabla dinámica. |
| [getPlacement()](#getPlacement--) | Representa la forma en que el gráfico está unido a las celdas debajo de él. |
| [getPlotArea()](#getPlotArea--) | Obtiene el área de trazado del gráfico que incluye las etiquetas de marcas del eje. |
| [getPlotBy()](#getPlotBy--) | Obtiene si la representación es por fila o columna. |
| [getPlotEmptyCellsType()](#getPlotEmptyCellsType--) | Obtiene cómo representar las celdas vacías. |
| [getPlotVisibleCells()](#getPlotVisibleCells--) | Indica si solo se representan celdas visibles. |
| [getPlotVisibleCellsOnly()](#getPlotVisibleCellsOnly--) | Indica si solo se representan celdas visibles. |
| [getPrintSize()](#getPrintSize--) | Obtiene el tamaño impreso del gráfico. |
| [getRightAngleAxes()](#getRightAngleAxes--) | True si los ejes del gráfico forman ángulos rectos. |
| [getRotationAngle()](#getRotationAngle--) | Representa la rotación de la vista del gráfico 3-D (la rotación del área de trazado alrededor del eje z, en grados). |
| [getSecondCategoryAxis()](#getSecondCategoryAxis--) | Obtiene el segundo eje X del gráfico. |
| [getSecondValueAxis()](#getSecondValueAxis--) | Obtiene el segundo eje Y del gráfico. |
| [getSeriesAxis()](#getSeriesAxis--) | Obtiene el eje de series del gráfico. |
| [getShapes()](#getShapes--) | Devuelve todas las formas de dibujo en este gráfico. |
| [getShowDataTable()](#getShowDataTable--) | Obtiene un valor que indica si el gráfico muestra una tabla de datos. |
| [getShowLegend()](#getShowLegend--) | Obtiene un valor que indica si se mostrará la leyenda del gráfico. |
| [getSideWall()](#getSideWall--) | Devuelve un objeto [getWalls()](../../com.aspose.cells/chart\#getWalls--) que representa la pared lateral de un gráfico 3-D. |
| [getSizeWithWindow()](#getSizeWithWindow--) | True si Microsoft Excel redimensiona el gráfico para que coincida con el tamaño de la ventana de la hoja de gráfico. |
| [getStyle()](#getStyle--) | Obtiene el estilo incorporado. |
| [getSubTitle()](#getSubTitle--) | Obtiene el subtítulo del gráfico. |
| [getTitle()](#getTitle--) | Obtiene el título del gráfico. |
| [getType()](#getType--) | Obtiene el tipo de un gráfico. |
| [getValueAxis()](#getValueAxis--) | Obtiene el eje Y del gráfico. |
| [getWalls()](#getWalls--) | Devuelve un objeto [getWalls()](../../com.aspose.cells/chart\#getWalls--) que representa las paredes de un gráfico 3-D. |
| [getWallsAndGridlines2D()](#getWallsAndGridlines2D--) | True si las líneas de cuadrícula se dibujan bidimensionalmente en un gráfico 3-D. |
| [getWorksheet()](#getWorksheet--) | Obtiene la hoja de cálculo que contiene este gráfico. |
| [hasAxis(int aixsType, boolean isPrimary)](#hasAxis-int-boolean-) | Devuelve qué ejes existen en el gráfico. |
| [hashCode()](#hashCode--) |  |
| [isCellReferedByChart(int sheetIndex, int rowIndex, int columnIndex)](#isCellReferedByChart-int-int-int-) | Devuelve si la celda referenciada por el gráfico. |
| [isChartDataChanged()](#isChartDataChanged--) | Detecta si la fuente de datos de un gráfico ha cambiado. |
| [isRectangularCornered()](#isRectangularCornered--) | Obtiene un valor que indica si el área del gráfico tiene esquinas rectangulares. |
| [isReferedByChart(int rowIndex, int columnIndex)](#isReferedByChart-int-int-) | Devuelve si la celda es referenciada por el gráfico. |
| [move(int topRow, int leftColumn, int bottomRow, int rightColumn)](#move-int-int-int-int-) | Mueve el gráfico a una ubicación especificada. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshPivotData()](#refreshPivotData--) | Actualiza los datos del gráfico desde la tabla dinámica. |
| [setAutoScaling(boolean value)](#setAutoScaling-boolean-) | True si Microsoft Excel escala un gráfico 3D para que su tamaño sea más cercano al del gráfico 2D equivalente. |
| [setChartDataRange(String area, boolean isVertical)](#setChartDataRange-java.lang.String-boolean-) | Especifica el rango de datos para un gráfico. |
| [setDepthPercent(int value)](#setDepthPercent-int-) | Representa la profundidad de un gráfico 3-D como un porcentaje del ancho del gráfico (entre el 20 y el 2000 por ciento). |
| [setDisplayNaAsBlank(boolean value)](#setDisplayNaAsBlank-boolean-) | Indica si se debe mostrar \#N/A como un valor en blanco. |
| [setElevation(int value)](#setElevation-int-) | Representa la elevación de la vista del gráfico 3-D, en grados. |
| [setFirstSliceAngle(int value)](#setFirstSliceAngle-int-) | Establece el ángulo de la primera porción de gráfico de pastel o de rosquilla, en grados (en sentido horario desde la vertical). |
| [setGapDepth(int value)](#setGapDepth-int-) | Establece la distancia entre las series de datos en un gráfico 3D, como un porcentaje del ancho del marcador. |
| [setGapWidth(int value)](#setGapWidth-int-) | Devuelve o establece el espacio entre grupos de barras o columnas, como un porcentaje del ancho de la barra o columna. |
| [setHeightPercent(int value)](#setHeightPercent-int-) | Devuelve o establece la altura de un gráfico 3-D como un porcentaje del ancho del gráfico (entre el 5 y el 500 por ciento). |
| [setHidePivotFieldButtons(boolean value)](#setHidePivotFieldButtons-boolean-) | Indica si se ocultan los botones de campo del gráfico dinámico solo cuando el gráfico es PivotChart. |
| [setName(String value)](#setName-java.lang.String-) | Establece el nombre del gráfico. |
| [setPerspective(short value)](#setPerspective-short-) | Devuelve o establece la perspectiva para la vista del gráfico three\u9225\u6178dimensional. |
| [setPivotSource(String value)](#setPivotSource-java.lang.String-) | El origen son los datos de la tabla dinámica. |
| [setPlacement(int value)](#setPlacement-int-) | Representa la forma en que el gráfico está unido a las celdas debajo de él. |
| [setPlotEmptyCellsType(int value)](#setPlotEmptyCellsType-int-) | Establece cómo trazar las celdas vacías. |
| [setPlotVisibleCells(boolean value)](#setPlotVisibleCells-boolean-) | Indica si solo se representan celdas visibles. |
| [setPlotVisibleCellsOnly(boolean value)](#setPlotVisibleCellsOnly-boolean-) | Indica si solo se representan celdas visibles. |
| [setPrintSize(int value)](#setPrintSize-int-) | Establece el tamaño impreso del gráfico. |
| [setRectangularCornered(boolean value)](#setRectangularCornered-boolean-) | Establece un valor que indica si el área del gráfico tiene esquinas rectangulares. |
| [setRightAngleAxes(boolean value)](#setRightAngleAxes-boolean-) | True si los ejes del gráfico forman ángulos rectos. |
| [setRotationAngle(int value)](#setRotationAngle-int-) | Representa la rotación de la vista del gráfico 3-D (la rotación del área de trazado alrededor del eje z, en grados). |
| [setShowDataTable(boolean value)](#setShowDataTable-boolean-) | Establece un valor que indica si el gráfico muestra una tabla de datos. |
| [setShowLegend(boolean value)](#setShowLegend-boolean-) | Establece un valor que indica si se mostrará la leyenda del gráfico. |
| [setSizeWithWindow(boolean value)](#setSizeWithWindow-boolean-) | True si Microsoft Excel redimensiona el gráfico para que coincida con el tamaño de la ventana de la hoja de gráfico. |
| [setStyle(int value)](#setStyle-int-) | Establece el estilo incorporado. |
| [setType(int value)](#setType-int-) | Establece el tipo de un gráfico. |
| [setWallsAndGridlines2D(boolean value)](#setWallsAndGridlines2D-boolean-) | True si las líneas de cuadrícula se dibujan bidimensionalmente en un gráfico 3-D. |
| [switchRowColumn()](#switchRowColumn--) | Intercambia fila/columna. |
| [toImage(OutputStream stream, ImageOrPrintOptions options)](#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-) | Crea la imagen del gráfico y la guarda en un flujo en el formato especificado. |
| [toImage(String imageFile)](#toImage-java.lang.String-) | Crea la imagen del gráfico y la guarda en un archivo. |
| [toImage(String imageFile, ImageFormat imageFormat)](#toImage-java.lang.String-com.aspose.cells.ImageFormat-) | Crea la imagen del gráfico y la guarda en un archivo en el formato especificado. |
| [toImage(String imageFile, ImageOrPrintOptions options)](#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-) | Crea la imagen del gráfico y la guarda en un archivo. |
| [toImage(String imageFile, int imageType)](#toImage-java.lang.String-int-) | Crea la imagen del gráfico y la guarda en un archivo en el tipo de imagen especificado. |
| [toImage(String imageFile, long jpegQuality)](#toImage-java.lang.String-long-) | Crea la imagen del gráfico y la guarda en un archivo en formato JPEG. |
| [toPdf(OutputStream stream)](#toPdf-java.io.OutputStream-) | Crea el PDF del gráfico y lo guarda en un flujo. |
| [toPdf(OutputStream stream, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType)](#toPdf-java.io.OutputStream-float-float-int-int-) | Crea el PDF del gráfico y lo guarda en un flujo. |
| [toPdf(String fileName)](#toPdf-java.lang.String-) | Guarda el gráfico en un archivo PDF. |
| [toPdf(String fileName, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType)](#toPdf-java.lang.String-float-float-int-int-) | Guarda el gráfico en un archivo PDF. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### calculate() {#calculate--}
```
public void calculate()
```


Calcula las posiciones personalizadas del área de trazado y los ejes si sus posiciones se asignan automáticamente.

### calculate(ChartCalculateOptions calculateOptions) {#calculate-com.aspose.cells.ChartCalculateOptions-}
```
public void calculate(ChartCalculateOptions calculateOptions)
```


Calcula la posición personalizada del área de trazado y los ejes si su posición se asigna automáticamente, con Opciones de Cálculo de Gráfico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| calculateOptions | [ChartCalculateOptions](../../com.aspose.cells/chartcalculateoptions) |  |

### changeTemplate(byte[] data) {#changeTemplate-byte---}
```
public void changeTemplate(byte[] data)
```


Cambiar el tipo de gráfico con una plantilla predefinida.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| datos | byte[] | Los datos del archivo de plantilla de gráfico (.crtx). |

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
### getActualChartSize() {#getActualChartSize--}
```
public int[] getActualChartSize()
```


Obtiene el tamaño real del gráfico en unidades de píxeles.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice el método Chart.getActualSize(). Esta propiedad será eliminada 12 meses después, a partir de julio de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
int[] - Tamaño real en una matriz (anchura y altura). [0] es anchura; [1] es altura.
### getActualSize() {#getActualSize--}
```
public int[] getActualSize()
```


Obtiene el tamaño real del gráfico en unidades de píxeles.

**Returns:**
int[] - Tamaño real en una matriz (anchura y altura). [0] es anchura; [1] es altura.
### getAutoScaling() {#getAutoScaling--}
```
public boolean getAutoScaling()
```


True si Microsoft Excel escala un gráfico 3-D de modo que su tamaño sea más cercano al del gráfico 2-D equivalente. La propiedad RightAngleAxes debe ser True.

**Returns:**
boolean
### getBackWall() {#getBackWall--}
```
public Walls getBackWall()
```


Devuelve un objeto [getWalls()](../../com.aspose.cells/chart\\#getWalls--) que representa la pared trasera de un gráfico 3D.

**Returns:**
[Walls](../../com.aspose.cells/walls)
### getCategoryAxis() {#getCategoryAxis--}
```
public Axis getCategoryAxis()
```


Obtiene el eje X del gráfico.

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getChartArea() {#getChartArea--}
```
public ChartArea getChartArea()
```


Obtiene el área del gráfico en la hoja de cálculo.

**Returns:**
[ChartArea](../../com.aspose.cells/chartarea)
### getChartDataRange() {#getChartDataRange--}
```
public String getChartDataRange()
```


Obtiene el rango de origen de datos del gráfico.

**Remarks**

Solo admite rangos. Si Series.Values, Name y XValues están en un rango continuo, se devolverá un rango que los contenga.

**Returns:**
java.lang.String - La fuente de datos.
### getChartDataTable() {#getChartDataTable--}
```
public ChartDataTable getChartDataTable()
```


Representa la tabla de datos del gráfico.

**Returns:**
[ChartDataTable](../../com.aspose.cells/chartdatatable)
### getChartObject() {#getChartObject--}
```
public ChartShape getChartObject()
```


Representa el chartShape;

**Returns:**
[ChartShape](../../com.aspose.cells/chartshape)
### getChartShape() {#getChartShape--}
```
public ChartShape getChartShape()
```


Representa el chartShape;

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad Aspose.Cells.Charts.Chart.ChartObject. Esta propiedad será eliminada 12 meses después, a partir de ENERO de 2012. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
[ChartShape](../../com.aspose.cells/chartshape)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDepthPercent() {#getDepthPercent--}
```
public int getDepthPercent()
```


Representa la profundidad de un gráfico 3-D como un porcentaje del ancho del gráfico (entre el 20 y el 2000 por ciento).

**Returns:**
int
### getDisplayNaAsBlank() {#getDisplayNaAsBlank--}
```
public boolean getDisplayNaAsBlank()
```


Indica si se debe mostrar \#N/A como un valor en blanco.

**Returns:**
boolean
### getElevation() {#getElevation--}
```
public int getElevation()
```


Representa la elevación de la vista del gráfico 3-D, en grados.

**Remarks**

La elevación del gráfico es la altura a la que se visualiza el gráfico, en grados. El valor predeterminado es 15 para la mayoría de los tipos de gráfico. El valor de esta propiedad debe estar entre -90 y 90, excepto para los gráficos de barras 3-D, donde debe estar entre 0 y 44.

**Returns:**
int
### getFilteredNSeries() {#getFilteredNSeries--}
```
public SeriesCollection getFilteredNSeries()
```


Obtiene una colección [SeriesCollection](../../com.aspose.cells/seriescollection) que representa las series de datos que se filtran en el gráfico.

**Returns:**
[SeriesCollection](../../com.aspose.cells/seriescollection)
### getFirstSliceAngle() {#getFirstSliceAngle--}
```
public int getFirstSliceAngle()
```


Obtiene el ángulo de la primera porción de gráfico circular o de rosquilla, en grados (en sentido horario desde la vertical). Se aplica solo a gráficos de pastel, pastel 3-D y rosquilla, de 0 a 360.

**Returns:**
int
### getFloor() {#getFloor--}
```
public Floor getFloor()
```


Devuelve un objeto [getFloor()](../../com.aspose.cells/chart\#getFloor--) que representa las paredes de un gráfico 3-D.

**Remarks**

Esta propiedad no se aplica a los gráficos de pastel 3-D.

**Returns:**
[Floor](../../com.aspose.cells/floor)
### getGapDepth() {#getGapDepth--}
```
public int getGapDepth()
```


Obtiene la distancia entre las series de datos en un gráfico 3-D, como un porcentaje del ancho del marcador. El valor de esta propiedad debe estar entre 0 y 500.

**Returns:**
int
### getGapWidth() {#getGapWidth--}
```
public int getGapWidth()
```


Devuelve o establece el espacio entre grupos de barras o columnas, como un porcentaje del ancho de la barra o columna. El valor de esta propiedad debe estar entre 0 y 500.

**Returns:**
int
### getHeightPercent() {#getHeightPercent--}
```
public int getHeightPercent()
```


Devuelve o establece la altura de un gráfico 3-D como un porcentaje del ancho del gráfico (entre el 5 y el 500 por ciento).

**Returns:**
int
### getHidePivotFieldButtons() {#getHidePivotFieldButtons--}
```
public boolean getHidePivotFieldButtons()
```


Indica si se ocultan los botones de campo del gráfico dinámico solo cuando el gráfico es PivotChart.

**Returns:**
boolean
### getIs3D() {#getIs3D--}
```
public boolean getIs3D()
```


Indica si el gráfico es un gráfico 3d.

**Returns:**
boolean
### getLegend() {#getLegend--}
```
public Legend getLegend()
```


Obtiene la leyenda del gráfico.

**Returns:**
[Legend](../../com.aspose.cells/legend)
### getLine() {#getLine--}
```
public Line getLine()
```


Obtiene la línea.

**Returns:**
[Line](../../com.aspose.cells/line)
### getNSeries() {#getNSeries--}
```
public SeriesCollection getNSeries()
```


Obtiene una colección [SeriesCollection](../../com.aspose.cells/seriescollection) que representa las series de datos en el gráfico.

**Returns:**
[SeriesCollection](../../com.aspose.cells/seriescollection)
### getName() {#getName--}
```
public String getName()
```


Obtiene el nombre del gráfico.

**Returns:**
java.lang.String
### getPageSetup() {#getPageSetup--}
```
public PageSetup getPageSetup()
```


Representa la descripción de la configuración de página en este gráfico.

**Returns:**
[PageSetup](../../com.aspose.cells/pagesetup)
### getPerspective() {#getPerspective--}
```
public short getPerspective()
```


Devuelve o establece la perspectiva para la vista del gráfico tridimensional three\u9225\u6178. Debe estar entre 0 y 100. Esta propiedad se ignora si la propiedad RightAngleAxes es True.

**Returns:**
short
### getPivotOptions() {#getPivotOptions--}
```
public PivotOptions getPivotOptions()
```


Especifica los controles dinámicos que aparecen en el gráfico.

**Returns:**
[PivotOptions](../../com.aspose.cells/pivotoptions)
### getPivotSource() {#getPivotSource--}
```
public String getPivotSource()
```


La fuente es los datos de la tabla dinámica. Si PivotSource no está vacío, el gráfico es un PivotChart.

**Remarks**

Si la tabla dinámica "PivotTable1" está en la hoja "Sheet1" del archivo "Book1.xls". El pivotSource podría ser "[Book1.xls]Sheet1!PivotTable1" si el gráfico y la tabla dinámica no están en el mismo libro. Si establece esta propiedad, la configuración anterior de la fuente de datos se perderá.

**Returns:**
java.lang.String
### getPlacement() {#getPlacement--}
```
public int getPlacement()
```


Representa la forma en que el gráfico está unido a las celdas debajo de él.

Ver [PlacementType](../../com.aspose.cells/placementtype).

**Returns:**
int
### getPlotArea() {#getPlotArea--}
```
public PlotArea getPlotArea()
```


Obtiene el área de trazado del gráfico que incluye las etiquetas de marcas del eje.

**Remarks**

**Returns:**
[PlotArea](../../com.aspose.cells/plotarea)
### getPlotBy() {#getPlotBy--}
```
public int getPlotBy()
```


Obtiene si la representación es por fila o columna.

Ver [PlotDataByType](../../com.aspose.cells/plotdatabytype).

**Returns:**
int
### getPlotEmptyCellsType() {#getPlotEmptyCellsType--}
```
public int getPlotEmptyCellsType()
```


Obtiene cómo representar las celdas vacías.

Ver [PlotEmptyCellsType](../../com.aspose.cells/plotemptycellstype).

**Returns:**
int
### getPlotVisibleCells() {#getPlotVisibleCells--}
```
public boolean getPlotVisibleCells()
```


Indica si solo se representan celdas visibles.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad PlotVisibleCellsOnly. Este método será eliminado 12 meses después, a partir de diciembre de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
boolean
### getPlotVisibleCellsOnly() {#getPlotVisibleCellsOnly--}
```
public boolean getPlotVisibleCellsOnly()
```


Indica si solo se representan celdas visibles.

**Returns:**
boolean
### getPrintSize() {#getPrintSize--}
```
public int getPrintSize()
```


Obtiene el tamaño impreso del gráfico.

Ver [PrintSizeType](../../com.aspose.cells/printsizetype).

**Returns:**
int
### getRightAngleAxes() {#getRightAngleAxes--}
```
public boolean getRightAngleAxes()
```


True si los ejes del gráfico están a ángulos rectos. Se aplica solo a gráficos 3-D (excepto Column3D y gráficos de pastel 3-D).

**Remarks**

Si esta propiedad es True, la propiedad Perspective se ignora.

**Returns:**
boolean
### getRotationAngle() {#getRotationAngle--}
```
public int getRotationAngle()
```


Representa la rotación de la vista del gráfico 3-D (la rotación del área de trazado alrededor del eje z, en grados).

**Remarks**

El valor de esta propiedad debe estar entre 0 y 360, excepto para los gráficos de barras 3-D, donde el valor debe estar entre 0 y 44. El valor predeterminado es 20. Se aplica solo a gráficos 3-D.

**Returns:**
int
### getSecondCategoryAxis() {#getSecondCategoryAxis--}
```
public Axis getSecondCategoryAxis()
```


Obtiene el segundo eje X del gráfico.

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getSecondValueAxis() {#getSecondValueAxis--}
```
public Axis getSecondValueAxis()
```


Obtiene el segundo eje Y del gráfico.

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getSeriesAxis() {#getSeriesAxis--}
```
public Axis getSeriesAxis()
```


Obtiene el eje de series del gráfico.

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getShapes() {#getShapes--}
```
public ShapeCollection getShapes()
```


Devuelve todas las formas de dibujo en este gráfico.

**Returns:**
[ShapeCollection](../../com.aspose.cells/shapecollection)
### getShowDataTable() {#getShowDataTable--}
```
public boolean getShowDataTable()
```


Obtiene un valor que indica si el gráfico muestra una tabla de datos.

**Returns:**
boolean
### getShowLegend() {#getShowLegend--}
```
public boolean getShowLegend()
```


Obtiene un valor que indica si se mostrará la leyenda del gráfico. El valor predeterminado es true.

**Returns:**
boolean
### getSideWall() {#getSideWall--}
```
public Walls getSideWall()
```


Devuelve un objeto [getWalls()](../../com.aspose.cells/chart\#getWalls--) que representa la pared lateral de un gráfico 3-D.

**Returns:**
[Walls](../../com.aspose.cells/walls)
### getSizeWithWindow() {#getSizeWithWindow--}
```
public boolean getSizeWithWindow()
```


True si Microsoft Excel redimensiona el gráfico para que coincida con el tamaño de la ventana de la hoja de gráfico.

**Returns:**
boolean
### getStyle() {#getStyle--}
```
public int getStyle()
```


Obtiene el estilo incorporado.

**Remarks**

Debe estar entre 1 y 48. Devuelve -1 si no está configurado.

**Returns:**
int
### getSubTitle() {#getSubTitle--}
```
public Title getSubTitle()
```


Obtiene el subtítulo del gráfico. Solo se aplica a archivos ODS.

**Returns:**
[Title](../../com.aspose.cells/title)
### getTitle() {#getTitle--}
```
public Title getTitle()
```


Obtiene el título del gráfico.

**Returns:**
[Title](../../com.aspose.cells/title)
### getType() {#getType--}
```
public int getType()
```


Obtiene el tipo de un gráfico.

Ver [ChartType](../../com.aspose.cells/charttype).

**Returns:**
int
### getValueAxis() {#getValueAxis--}
```
public Axis getValueAxis()
```


Obtiene el eje Y del gráfico.

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getWalls() {#getWalls--}
```
public Walls getWalls()
```


Devuelve un objeto [getWalls()](../../com.aspose.cells/chart\#getWalls--) que representa las paredes de un gráfico 3-D.

**Remarks**

Esta propiedad no se aplica a los gráficos de pastel 3-D.

**Returns:**
[Walls](../../com.aspose.cells/walls)
### getWallsAndGridlines2D() {#getWallsAndGridlines2D--}
```
public boolean getWallsAndGridlines2D()
```


True si las líneas de cuadrícula se dibujan bidimensionalmente en un gráfico 3-D.

**Returns:**
boolean
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Obtiene la hoja de cálculo que contiene este gráfico.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### hasAxis(int aixsType, boolean isPrimary) {#hasAxis-int-boolean-}
```
public boolean hasAxis(int aixsType, boolean isPrimary)
```


Devuelve qué ejes existen en el gráfico.

**Remarks**

Normalmente, Pie, PieExploded, PiePie,PieBar, Pie3D, Pie3DExploded,Doughnut, DoughnutExploded no tiene eje.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| aixsType | int |  |
| isPrimary | boolean |  |

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCellReferedByChart(int sheetIndex, int rowIndex, int columnIndex) {#isCellReferedByChart-int-int-int-}
```
public boolean isCellReferedByChart(int sheetIndex, int rowIndex, int columnIndex)
```


Devuelve si la celda referenciada por el gráfico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetIndex | int | El índice de hoja -1 significa la hoja de cálculo que contiene el gráfico actual. |
| rowIndex | int | El índice de fila |
| columnIndex | int | El índice de columna |

**Returns:**
boolean -
### isChartDataChanged() {#isChartDataChanged--}
```
public boolean isChartDataChanged()
```


Detecta si la fuente de datos de un gráfico ha cambiado.

**Remarks**

El método detecta los cambios en la fuente de datos del gráfico antes de renderizar el gráfico al formato de imagen. En la primera llamada a Chart.toImage, los datos de origen del gráfico (p. ej., XValuesParseData, ValuesParseData) se registrarán. Antes de volver a llamar al método Chart.toImage, invoque el método IsChartDataChanged para comprobar si el gráfico necesita volver a renderizarse.

**Returns:**
boolean - Devuelve true si el gráfico ha cambiado, de lo contrario devuelve false
### isRectangularCornered() {#isRectangularCornered--}
```
public boolean isRectangularCornered()
```


Obtiene un valor que indica si el área del gráfico tiene esquinas rectangulares. El valor predeterminado es true.

**Returns:**
boolean
### isReferedByChart(int rowIndex, int columnIndex) {#isReferedByChart-int-int-}
```
public boolean isReferedByChart(int rowIndex, int columnIndex)
```


Devuelve si la celda es referenciada por el gráfico.

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método IsCellReferedByChart(int,int,int). Este método será eliminado 12 meses después desde abril de 2023. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | int | El índice de fila |
| columnIndex | int | El índice de columna |

**Returns:**
boolean -
### move(int topRow, int leftColumn, int bottomRow, int rightColumn) {#move-int-int-int-int-}
```
public void move(int topRow, int leftColumn, int bottomRow, int rightColumn)
```


Mueve el gráfico a una ubicación especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | int | Índice de fila superior izquierda. |
| leftColumn | int | Índice de columna superior izquierda. |
| bottomRow | int | Índice de fila inferior derecha |
| rightColumn | int | Índice de columna inferior derecha |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refreshPivotData() {#refreshPivotData--}
```
public void refreshPivotData()
```


Actualiza los datos del gráfico desde la tabla dinámica.

**Remarks**

Recopilaremos datos de la fuente de datos pivote al informe de tabla dinámica. Este método solo se usa para recopilar todos los datos en un gráfico dinámico.

### setAutoScaling(boolean value) {#setAutoScaling-boolean-}
```
public void setAutoScaling(boolean value)
```


True si Microsoft Excel escala un gráfico 3-D de modo que su tamaño sea más cercano al del gráfico 2-D equivalente. La propiedad RightAngleAxes debe ser True.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setChartDataRange(String area, boolean isVertical) {#setChartDataRange-java.lang.String-boolean-}
```
public void setChartDataRange(String area, boolean isVertical)
```


Especifica el rango de datos para un gráfico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| area | java.lang.String | Especifica los valores desde los cuales trazar la serie de datos |
| isVertical | boolean | Especifica si se debe trazar la serie a partir de un rango de valores de celdas por fila o por columna. |

### setDepthPercent(int value) {#setDepthPercent-int-}
```
public void setDepthPercent(int value)
```


Representa la profundidad de un gráfico 3-D como un porcentaje del ancho del gráfico (entre el 20 y el 2000 por ciento).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setDisplayNaAsBlank(boolean value) {#setDisplayNaAsBlank-boolean-}
```
public void setDisplayNaAsBlank(boolean value)
```


Indica si se debe mostrar \#N/A como un valor en blanco.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setElevation(int value) {#setElevation-int-}
```
public void setElevation(int value)
```


Representa la elevación de la vista del gráfico 3-D, en grados.

**Remarks**

La elevación del gráfico es la altura a la que se visualiza el gráfico, en grados. El valor predeterminado es 15 para la mayoría de los tipos de gráfico. El valor de esta propiedad debe estar entre -90 y 90, excepto para los gráficos de barras 3-D, donde debe estar entre 0 y 44.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setFirstSliceAngle(int value) {#setFirstSliceAngle-int-}
```
public void setFirstSliceAngle(int value)
```


Establece el ángulo de la primera porción de gráfico de pastel o de dona, en grados (en sentido horario desde la vertical). Se aplica solo a gráficos de pastel, pastel 3D y dona, de 0 a 360.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setGapDepth(int value) {#setGapDepth-int-}
```
public void setGapDepth(int value)
```


Establece la distancia entre las series de datos en un gráfico 3D, como un porcentaje del ancho del marcador. El valor de esta propiedad debe estar entre 0 y 500.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setGapWidth(int value) {#setGapWidth-int-}
```
public void setGapWidth(int value)
```


Devuelve o establece el espacio entre grupos de barras o columnas, como un porcentaje del ancho de la barra o columna. El valor de esta propiedad debe estar entre 0 y 500.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setHeightPercent(int value) {#setHeightPercent-int-}
```
public void setHeightPercent(int value)
```


Devuelve o establece la altura de un gráfico 3-D como un porcentaje del ancho del gráfico (entre el 5 y el 500 por ciento).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setHidePivotFieldButtons(boolean value) {#setHidePivotFieldButtons-boolean-}
```
public void setHidePivotFieldButtons(boolean value)
```


Indica si se ocultan los botones de campo del gráfico dinámico solo cuando el gráfico es PivotChart.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Establece el nombre del gráfico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setPerspective(short value) {#setPerspective-short-}
```
public void setPerspective(short value)
```


Devuelve o establece la perspectiva para la vista del gráfico tridimensional three\u9225\u6178. Debe estar entre 0 y 100. Esta propiedad se ignora si la propiedad RightAngleAxes es True.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | short |  |

### setPivotSource(String value) {#setPivotSource-java.lang.String-}
```
public void setPivotSource(String value)
```


La fuente es los datos de la tabla dinámica. Si PivotSource no está vacío, el gráfico es un PivotChart.

**Remarks**

Si la tabla dinámica "PivotTable1" está en la hoja "Sheet1" del archivo "Book1.xls". El pivotSource podría ser "[Book1.xls]Sheet1!PivotTable1" si el gráfico y la tabla dinámica no están en el mismo libro. Si establece esta propiedad, la configuración anterior de la fuente de datos se perderá.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setPlacement(int value) {#setPlacement-int-}
```
public void setPlacement(int value)
```


Representa la forma en que el gráfico está unido a las celdas debajo de él.

Ver [PlacementType](../../com.aspose.cells/placementtype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setPlotEmptyCellsType(int value) {#setPlotEmptyCellsType-int-}
```
public void setPlotEmptyCellsType(int value)
```


Establece cómo trazar las celdas vacías.

Ver [PlotEmptyCellsType](../../com.aspose.cells/plotemptycellstype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setPlotVisibleCells(boolean value) {#setPlotVisibleCells-boolean-}
```
public void setPlotVisibleCells(boolean value)
```


Indica si solo se representan celdas visibles.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad PlotVisibleCellsOnly. Este método será eliminado 12 meses después, a partir de diciembre de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setPlotVisibleCellsOnly(boolean value) {#setPlotVisibleCellsOnly-boolean-}
```
public void setPlotVisibleCellsOnly(boolean value)
```


Indica si solo se representan celdas visibles.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setPrintSize(int value) {#setPrintSize-int-}
```
public void setPrintSize(int value)
```


Establece el tamaño impreso del gráfico.

Ver [PrintSizeType](../../com.aspose.cells/printsizetype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setRectangularCornered(boolean value) {#setRectangularCornered-boolean-}
```
public void setRectangularCornered(boolean value)
```


Establece un valor que indica si el área del gráfico tiene esquinas rectangulares. El valor predeterminado es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setRightAngleAxes(boolean value) {#setRightAngleAxes-boolean-}
```
public void setRightAngleAxes(boolean value)
```


True si los ejes del gráfico están a ángulos rectos. Se aplica solo a gráficos 3-D (excepto Column3D y gráficos de pastel 3-D).

**Remarks**

Si esta propiedad es True, la propiedad Perspective se ignora.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setRotationAngle(int value) {#setRotationAngle-int-}
```
public void setRotationAngle(int value)
```


Representa la rotación de la vista del gráfico 3-D (la rotación del área de trazado alrededor del eje z, en grados).

**Remarks**

El valor de esta propiedad debe estar entre 0 y 360, excepto para los gráficos de barras 3-D, donde el valor debe estar entre 0 y 44. El valor predeterminado es 20. Se aplica solo a gráficos 3-D.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setShowDataTable(boolean value) {#setShowDataTable-boolean-}
```
public void setShowDataTable(boolean value)
```


Establece un valor que indica si el gráfico muestra una tabla de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowLegend(boolean value) {#setShowLegend-boolean-}
```
public void setShowLegend(boolean value)
```


Establece un valor que indica si la leyenda del gráfico se mostrará. El valor predeterminado es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSizeWithWindow(boolean value) {#setSizeWithWindow-boolean-}
```
public void setSizeWithWindow(boolean value)
```


True si Microsoft Excel redimensiona el gráfico para que coincida con el tamaño de la ventana de la hoja de gráfico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setStyle(int value) {#setStyle-int-}
```
public void setStyle(int value)
```


Establece el estilo incorporado.

**Remarks**

Debe estar entre 1 y 48. Devuelve -1 si no está configurado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Establece el tipo de un gráfico.

Ver [ChartType](../../com.aspose.cells/charttype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setWallsAndGridlines2D(boolean value) {#setWallsAndGridlines2D-boolean-}
```
public void setWallsAndGridlines2D(boolean value)
```


True si las líneas de cuadrícula se dibujan bidimensionalmente en un gráfico 3-D.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### switchRowColumn() {#switchRowColumn--}
```
public boolean switchRowColumn()
```


Intercambia fila/columna.

**Returns:**
boolean - False significa que el cambio de fila/columna falla.
### toImage(OutputStream stream, ImageOrPrintOptions options) {#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(OutputStream stream, ImageOrPrintOptions options)
```


Crea la imagen del gráfico y la guarda en un flujo en el formato especificado.

**Remarks**

El formato de la imagen se especifica usando `options.ImageFormat`. Los siguientes formatos son compatibles: ImageFormat.Bmp, ImageFormat.Gif, ImageFormat.Png, ImageFormat.Jpeg, ImageFormat.Tiff, ImageFormat.Emf.

Si el ancho o la altura es cero o el gráfico no es compatible según la Lista de Gráficos Compatibles, este método no hará nada. Consulte la [Supported Charts List][] para más detalles.


[Supported Charts List]: http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.OutputStream | El flujo de salida. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | Opciones adicionales de creación de imagen |

### toImage(String imageFile) {#toImage-java.lang.String-}
```
public void toImage(String imageFile)
```


Crea la imagen del gráfico y la guarda en un archivo. La extensión del nombre del archivo determina el formato de la imagen.

**Remarks**

El formato de la imagen se especifica usando la extensión del nombre del archivo. Por ejemplo, si especifica \"myfile.png\", la imagen se guardará en formato PNG. Las siguientes extensiones de archivo son reconocidas: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

Si el ancho o la altura es cero o el gráfico no es compatible según la Lista de Gráficos Compatibles, este método no hará nada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| imageFile | java.lang.String | El nombre del archivo de imagen con ruta completa. |

### toImage(String imageFile, ImageFormat imageFormat) {#toImage-java.lang.String-com.aspose.cells.ImageFormat-}
```
public void toImage(String imageFile, ImageFormat imageFormat)
```


Crea la imagen del gráfico y la guarda en un archivo en el formato especificado.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice el método Chart.ToImage(string, ImageType). Esta propiedad será eliminada 12 meses después desde julio de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| imageFile | java.lang.String | El nombre del archivo de imagen con ruta completa. |
| imageFormat | [ImageFormat](../../com.aspose.cells/imageformat) | El formato en el que guardar la imagen. |

### toImage(String imageFile, ImageOrPrintOptions options) {#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(String imageFile, ImageOrPrintOptions options)
```


Crea la imagen del gráfico y la guarda en un archivo. La extensión del nombre del archivo determina el formato de la imagen.

**Remarks**

El formato de la imagen se especifica usando la extensión del nombre del archivo. Por ejemplo, si especifica \"myfile.png\", la imagen se guardará en formato PNG. Las siguientes extensiones de archivo son reconocidas: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

Si el ancho o la altura es cero o el gráfico no es compatible según la Lista de Gráficos Compatibles, este método no hará nada. Consulte la [Supported Charts List][] para más detalles.

**Example**

Guarda en Tiff con 300 dpi y compresión CCITT4.

```
         ImageOrPrintOptions options = new ImageOrPrintOptions();
         options.setHorizontalResolution(300);
         options.setVerticalResolution(300);
         options.setTiffCompression(TiffCompression.COMPRESSION_CCITT_4);
 
         Workbook book = new Workbook("test.xls");
         book.getWorksheets().get(0).getCharts().get(0).toImage("chart.Tiff", options);
```


[Supported Charts List]: http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| imageFile | java.lang.String | El nombre del archivo de imagen con ruta completa. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | Opciones adicionales de creación de imagen |

### toImage(String imageFile, int imageType) {#toImage-java.lang.String-int-}
```
public void toImage(String imageFile, int imageType)
```


Crea la imagen del gráfico y la guarda en un archivo en el tipo de imagen especificado.

**Remarks**

El tipo de la imagen se especifica usando `imageType`. Los siguientes tipos son compatibles: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Si el ancho o la altura es cero o el gráfico no es compatible según la Lista de Gráficos Compatibles, este método no hará nada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| imageFile | java.lang.String | El nombre del archivo de imagen con ruta completa. |
| imageType | int | [ImageType](../../com.aspose.cells/imagetype). El tipo de imagen en el que guardar la imagen. |

### toImage(String imageFile, long jpegQuality) {#toImage-java.lang.String-long-}
```
public void toImage(String imageFile, long jpegQuality)
```


Crea la imagen del gráfico y la guarda en un archivo en formato JPEG.

**Remarks**

Si el ancho o la altura son cero o el gráfico no es compatible según la Lista de Gráficos Compatibles, este método no hará nada. NOTA: Este método está ahora obsoleto. En su lugar, utilice el método ToImage(string,ImageOrPrintOptions) con la calidad especificada. Este método será eliminado 12 meses después desde marzo de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| imageFile | java.lang.String | El nombre del archivo de imagen con ruta completa. |
| jpegQuality | long | Calidad JPEG. |

### toPdf(OutputStream stream) {#toPdf-java.io.OutputStream-}
```
public void toPdf(OutputStream stream)
```


Crea el PDF del gráfico y lo guarda en un flujo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.OutputStream | El flujo de salida. |

### toPdf(OutputStream stream, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType) {#toPdf-java.io.OutputStream-float-float-int-int-}
```
public void toPdf(OutputStream stream, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType)
```


Crea el PDF del gráfico y lo guarda en un flujo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.OutputStream | El flujo de salida. |
| desiredPageWidth | float | El ancho de página deseado en pulgadas. |
| desiredPageHeight | float | La altura de página deseada en pulgadas. |
| hAlignmentType | int | [PageLayoutAlignmentType](../../com.aspose.cells/pagelayoutalignmenttype). El tipo de alineación horizontal del gráfico en la página de salida. |
| vAlignmentType | int | [PageLayoutAlignmentType](../../com.aspose.cells/pagelayoutalignmenttype). El tipo de alineación vertical del gráfico en la página de salida. |

### toPdf(String fileName) {#toPdf-java.lang.String-}
```
public void toPdf(String fileName)
```


Guarda el gráfico en un archivo PDF.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | java.lang.String | el nombre del archivo pdf con ruta completa |

### toPdf(String fileName, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType) {#toPdf-java.lang.String-float-float-int-int-}
```
public void toPdf(String fileName, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType)
```


Guarda el gráfico en un archivo PDF.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | java.lang.String | el nombre del archivo pdf con ruta completa |
| desiredPageWidth | float | El ancho de página deseado en pulgadas. |
| desiredPageHeight | float | La altura de página deseada en pulgadas. |
| hAlignmentType | int | [PageLayoutAlignmentType](../../com.aspose.cells/pagelayoutalignmenttype). El tipo de alineación horizontal del gráfico en la página de salida. |
| vAlignmentType | int | [PageLayoutAlignmentType](../../com.aspose.cells/pagelayoutalignmenttype). El tipo de alineación vertical del gráfico en la página de salida. |

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

