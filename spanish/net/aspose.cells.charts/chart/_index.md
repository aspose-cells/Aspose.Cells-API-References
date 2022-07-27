---
title: Chart
second_title: Referencia de API de Aspose.Cells para .NET
description: Encapsula el objeto que representa un único gráfico de Excel.
type: docs
weight: 430
url: /es/net/aspose.cells.charts/chart/
---
## Chart class

Encapsula el objeto que representa un único gráfico de Excel.

```csharp
public class Chart
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AutoScaling](../../aspose.cells.charts/chart/autoscaling) { get; set; } | Verdadero si Microsoft Excel escala un gráfico 3D para que tenga un tamaño más cercano al gráfico 2D equivalente. La propiedad RightAngleAxes debe ser True. |
| [BackWall](../../aspose.cells.charts/chart/backwall) { get; } | Devuelve un[`Walls`](./walls) objeto que representa la pared trasera de un gráfico 3-D. |
| [CategoryAxis](../../aspose.cells.charts/chart/categoryaxis) { get; } | Obtiene el eje X del gráfico. |
| [ChartArea](../../aspose.cells.charts/chart/chartarea) { get; } | Obtiene el área del gráfico en la hoja de cálculo. |
| [ChartDataTable](../../aspose.cells.charts/chart/chartdatatable) { get; } | Representa la tabla de datos del gráfico. |
| [ChartObject](../../aspose.cells.charts/chart/chartobject) { get; } | Representa la forma del gráfico; |
| [DepthPercent](../../aspose.cells.charts/chart/depthpercent) { get; set; } | Representa la profundidad de un gráfico 3D como un porcentaje del ancho del gráfico (entre 20 y 2000 por ciento). |
| [DisplayNaAsBlank](../../aspose.cells.charts/chart/displaynaasblank) { get; set; } | Indica si se muestra #N/A como valor en blanco. |
| [Elevation](../../aspose.cells.charts/chart/elevation) { get; set; } | Representa la elevación de la vista de carta 3D, en grados. |
| [FirstSliceAngle](../../aspose.cells.charts/chart/firstsliceangle) { get; set; } | Obtiene o establece el ángulo del primer sector del gráfico circular o del gráfico de anillos, en grados (en el sentido de las agujas del reloj desde la vertical). Solo se aplica a gráficos circulares, circulares 3D y de anillos, de 0 a 360. |
| [Floor](../../aspose.cells.charts/chart/floor) { get; } | Devuelve un[`Floor`](./floor) objeto que representa las paredes de un gráfico 3-D. |
| [GapDepth](../../aspose.cells.charts/chart/gapdepth) { get; set; } | Obtiene o establece la distancia entre las series de datos en un gráfico 3D, como un porcentaje del ancho del marcador. El valor de esta propiedad debe estar entre 0 y 500. |
| [GapWidth](../../aspose.cells.charts/chart/gapwidth) { get; set; } | Devuelve o establece el espacio entre grupos de barras o columnas, como porcentaje del ancho de la barra o columna. El valor de esta propiedad debe estar entre 0 y 500. |
| [HeightPercent](../../aspose.cells.charts/chart/heightpercent) { get; set; } | Devuelve o establece la altura de un gráfico 3D como un porcentaje del ancho del gráfico (entre 5 y 500 por ciento). |
| [HidePivotFieldButtons](../../aspose.cells.charts/chart/hidepivotfieldbuttons) { get; set; } | Indica si ocultar los botones de campo del gráfico dinámico solo cuando el gráfico es PivotChart. |
| [Is3D](../../aspose.cells.charts/chart/is3d) { get; } | Indica si el gráfico es un gráfico 3D. |
| [IsRectangularCornered](../../aspose.cells.charts/chart/isrectangularcornered) { get; set; } | Obtiene o establece un valor que indica si el área del gráfico tiene esquinas rectangulares. El valor predeterminado es verdadero. |
| [Legend](../../aspose.cells.charts/chart/legend) { get; } | Obtiene la leyenda del gráfico. |
| [Line](../../aspose.cells.charts/chart/line) { get; } | Obtiene la línea. |
| [Name](../../aspose.cells.charts/chart/name) { get; set; } | Obtiene y establece el nombre del gráfico. |
| [NSeries](../../aspose.cells.charts/chart/nseries) { get; } | Obtiene un[`SeriesCollection`](../seriescollection) colección que representa la serie de datos en el gráfico. |
| [PageSetup](../../aspose.cells.charts/chart/pagesetup) { get; } | Representa la descripción de configuración de página en este gráfico. |
| [Perspective](../../aspose.cells.charts/chart/perspective) { get; set; } | Devuelve o establece la perspectiva de la vista de gráfico 3D. Debe estar entre 0 y 100. Esta propiedad se ignora si la propiedad RightAngleAxes es True. |
| [PivotOptions](../../aspose.cells.charts/chart/pivotoptions) { get; } | Especifica los controles de pivote que aparecen en el gráfico |
| [PivotSource](../../aspose.cells.charts/chart/pivotsource) { get; set; } | El origen son los datos de la tabla dinámica. Si PivotSource no está vacío, el gráfico es PivotChart. |
| [Placement](../../aspose.cells.charts/chart/placement) { get; set; } | Representa la forma en que el gráfico se adjunta a las celdas debajo de él. |
| [PlotArea](../../aspose.cells.charts/chart/plotarea) { get; } | Obtiene el área de trazado del gráfico que incluye etiquetas de marca de eje. |
| [PlotBy](../../aspose.cells.charts/chart/plotby) { get; } | Obtiene y establece si se traza por fila o columna. |
| [PlotEmptyCellsType](../../aspose.cells.charts/chart/plotemptycellstype) { get; set; } | Obtiene y establece cómo trazar las celdas vacías. |
| [PlotVisibleCells](../../aspose.cells.charts/chart/plotvisiblecells) { get; set; } | Indica si solo se trazan celdas visibles. |
| [PrintSize](../../aspose.cells.charts/chart/printsize) { get; set; } | Obtiene y establece el tamaño del gráfico impreso. |
| [RightAngleAxes](../../aspose.cells.charts/chart/rightangleaxes) { get; set; } | Verdadero si los ejes del gráfico están en ángulo recto. Solo se aplica a gráficos 3D (excepto Column3D y gráficos circulares 3D). |
| [RotationAngle](../../aspose.cells.charts/chart/rotationangle) { get; set; } | Representa la rotación de la vista de gráfico 3D (la rotación del área de trazado alrededor del eje z, en grados). |
| [SecondCategoryAxis](../../aspose.cells.charts/chart/secondcategoryaxis) { get; } | Obtiene el segundo eje X del gráfico. |
| [SecondValueAxis](../../aspose.cells.charts/chart/secondvalueaxis) { get; } | Obtiene el segundo eje Y del gráfico. |
| [SeriesAxis](../../aspose.cells.charts/chart/seriesaxis) { get; } | Obtiene el eje de serie del gráfico. |
| [Shapes](../../aspose.cells.charts/chart/shapes) { get; } | Devuelve todas las formas de dibujo en este gráfico. |
| [ShowDataTable](../../aspose.cells.charts/chart/showdatatable) { get; set; } | Obtiene o establece un valor que indica si el gráfico muestra una tabla de datos. |
| [ShowLegend](../../aspose.cells.charts/chart/showlegend) { get; set; } | Obtiene o establece un valor que indica si se mostrará la leyenda del gráfico. El valor predeterminado es verdadero. |
| [SideWall](../../aspose.cells.charts/chart/sidewall) { get; } | Devuelve un[`Walls`](./walls)objeto que representa la pared lateral de un gráfico 3-D. |
| [SizeWithWindow](../../aspose.cells.charts/chart/sizewithwindow) { get; set; } | Verdadero si Microsoft Excel cambia el tamaño del gráfico para que coincida con el tamaño de la ventana de la hoja del gráfico. |
| [Style](../../aspose.cells.charts/chart/style) { get; set; } | Obtiene y establece el estilo integrado. |
| [SubTitle](../../aspose.cells.charts/chart/subtitle) { get; } | Obtiene el subtítulo del gráfico. Solo para archivos con formato ODS. |
| [Title](../../aspose.cells.charts/chart/title) { get; } | Obtiene el título del gráfico. |
| [Type](../../aspose.cells.charts/chart/type) { get; set; } | Obtiene o establece el tipo de gráfico. |
| [ValueAxis](../../aspose.cells.charts/chart/valueaxis) { get; } | Obtiene el eje Y del gráfico. |
| [Walls](../../aspose.cells.charts/chart/walls) { get; } | Devuelve un[`Walls`](./walls) objeto que representa las paredes de un gráfico 3-D. |
| [WallsAndGridlines2D](../../aspose.cells.charts/chart/wallsandgridlines2d) { get; set; } | Verdadero si las líneas de cuadrícula se dibujan bidimensionalmente en un gráfico tridimensional. |
| [Worksheet](../../aspose.cells.charts/chart/worksheet) { get; } | Obtiene la hoja de cálculo que contiene este gráfico. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Calculate](../../aspose.cells.charts/chart/calculate)() | Calcula la posición personalizada del área de trazado, ejes si la posición de ellos se asigna automáticamente. |
| [GetActualSize](../../aspose.cells.charts/chart/getactualsize)() | Obtiene el tamaño real del gráfico en unidades de píxeles. |
| [GetChartDataRange](../../aspose.cells.charts/chart/getchartdatarange)() | Obtiene el rango de origen de datos del gráfico. |
| [HasAxis](../../aspose.cells.charts/chart/hasaxis)(AxisType, bool) | Devuelve qué ejes existen en el gráfico. |
| [IsChartDataChanged](../../aspose.cells.charts/chart/ischartdatachanged)() | Detecta si la fuente de datos de un gráfico ha cambiado. |
| [Move](../../aspose.cells.charts/chart/move)(int, int, int, int) | Mueve el gráfico a una ubicación específica. |
| [RefreshPivotData](../../aspose.cells.charts/chart/refreshpivotdata)() | Actualiza los datos del gráfico dinámico desde su origen de datos dinámicos. |
| [SetChartDataRange](../../aspose.cells.charts/chart/setchartdatarange)(string, bool) | Especifica el rango de datos para un gráfico. |
| [SwitchRowColumn](../../aspose.cells.charts/chart/switchrowcolumn)() | Cambia fila/columna. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage)() | Obtiene una de 32 bits`mapa de bits` objeto del gráfico. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_1)(ImageOrPrintOptions) | Obtiene una de 32 bits`mapa de bits` objeto del gráfico. `ImageOrPrintOptions.ImageFormat` , los atributos ImageOrPrintOptions.TiffCompression e ImageOrPrintOptions.Quality se ignoran. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_6)(string) | Crea la imagen del gráfico y la guarda en un archivo. La extensión del nombre del archivo determina el formato de la imagen. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_3)(Stream, ImageOrPrintOptions) | Crea la imagen del gráfico y la guarda en una secuencia en el formato especificado. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_2)(Stream, ImageType) | Crea la imagen del gráfico y la guarda en una secuencia en el formato especificado. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_4)(Stream, long) | Crea la imagen del gráfico y la guarda en una secuencia en formato Jpeg. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_8)(string, ImageOrPrintOptions) | Crea la imagen del gráfico y la guarda en un archivo. La extensión del nombre del archivo determina el formato de la imagen. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_7)(string, ImageType) | Crea la imagen del gráfico y la guarda en un archivo con el tipo de imagen especificado. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_9)(string, long) | Crea la imagen del gráfico y la guarda en un archivo en formato Jpeg. |
| [ToPdf](../../aspose.cells.charts/chart/topdf#topdf)(Stream) | Crea el pdf del gráfico y lo guarda en una secuencia. |
| [ToPdf](../../aspose.cells.charts/chart/topdf#topdf_2)(string) | Guarda el gráfico en un archivo pdf. |
| [ToPdf](../../aspose.cells.charts/chart/topdf#topdf_1)(Stream, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) | Crea el pdf del gráfico y lo guarda en una secuencia. |
| [ToPdf](../../aspose.cells.charts/chart/topdf#topdf_3)(string, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) | Guarda el gráfico en un archivo pdf. |

### Ejemplos

```csharp
[C#]

Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];

Cells cells = sheet.Cells;
cells[0,1].PutValue("Income");
cells[1,0].PutValue("Company A");
cells[2,0].PutValue("Company B");
cells[3,0].PutValue("Company C");
cells[1,1].PutValue(10000);
cells[2,1].PutValue(20000);
cells[3,1].PutValue(30000);
		
int chartIndex = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);

Chart chart = sheet.Charts[chartIndex];
chart.SetChartDataRange("A1:B4", true);
chart.ShowLegend = true;
chart.Title.Text = "Income Analysis";

[Visual Basic]

Dim workbook as Workbook = new Workbook()
Dim sheet as Worksheet = workbook.Worksheets(0)

Dim cells as Cells = sheet.Cells
cells(0,1).PutValue("Income")
cells(1,0).PutValue("Company A")
cells(2,0).PutValue("Company B")
cells(3,0).PutValue("Company C")
cells(1,1).PutValue(10000)
cells(2,1).PutValue(20000)
cells(3,1).PutValue(30000)
		
Dim chartIndex as Integer = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15)

Dim chart as Chart = sheet.Charts(chartIndex) 
chart.SetChartDataRange("A1:B4", True);
chart.ShowLegend = True
chart.Title.Text = "Income Analysis"
```

### Ver también

* espacio de nombres [Aspose.Cells.Charts](../../aspose.cells.charts)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
