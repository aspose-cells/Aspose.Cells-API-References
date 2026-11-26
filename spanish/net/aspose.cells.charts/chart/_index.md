---
title: "Clase Chart"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Charts.Chart. Encapsula el objeto que representa un único gráfico de Excel"
type: docs
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
| [ActualChartSize](../../aspose.cells.charts/chart/actualchartsize/) { get; } | (**Obsolete.**) Obtiene el tamaño real del gráfico en unidades de píxeles. |
| [AutoScaling](../../aspose.cells.charts/chart/autoscaling/) { get; set; } | Verdadero si Microsoft Excel escala un gráfico 3-D para que su tamaño sea más cercano al del gráfico 2-D equivalente. La propiedad RightAngleAxes debe ser Verdadero. |
| [BackWall](../../aspose.cells.charts/chart/backwall/) { get; } | Devuelve un objeto [`Walls`](./walls/) que representa la pared trasera de un gráfico 3-D. |
| [CategoryAxis](../../aspose.cells.charts/chart/categoryaxis/) { get; } | Obtiene el eje X del gráfico. |
| [ChartArea](../../aspose.cells.charts/chart/chartarea/) { get; } | Obtiene el área del gráfico en la hoja de cálculo. |
| [ChartDataTable](../../aspose.cells.charts/chart/chartdatatable/) { get; } | Representa la tabla de datos del gráfico. |
| [ChartObject](../../aspose.cells.charts/chart/chartobject/) { get; } | Representa el chartShape; |
| [DepthPercent](../../aspose.cells.charts/chart/depthpercent/) { get; set; } | Representa la profundidad de un gráfico 3-D como un porcentaje del ancho del gráfico (entre el 20 y el 2000 por ciento). |
| [DisplayNaAsBlank](../../aspose.cells.charts/chart/displaynaasblank/) { get; set; } | Indica si se debe mostrar #N/A como un valor en blanco. |
| [Elevation](../../aspose.cells.charts/chart/elevation/) { get; set; } | Representa la elevación de la vista del gráfico 3-D, en grados. |
| [FilteredNSeries](../../aspose.cells.charts/chart/filterednseries/) { get; } | Obtiene una colección [`SeriesCollection`](../seriescollection/) que representa las series de datos que están filtradas en el gráfico. |
| [FirstSliceAngle](../../aspose.cells.charts/chart/firstsliceangle/) { get; set; } | Obtiene o establece el ángulo de la primera porción de gráfico de pastel o de rosquilla, en grados (en sentido horario desde la vertical). Se aplica solo a gráficos de pastel, pastel 3-D y rosquilla, de 0 a 360. |
| [Floor](../../aspose.cells.charts/chart/floor/) { get; } | Devuelve un objeto [`Floor`](./floor/) que representa las paredes de un gráfico 3-D. |
| [GapDepth](../../aspose.cells.charts/chart/gapdepth/) { get; set; } | Obtiene o establece la distancia entre las series de datos en un gráfico 3-D, como un porcentaje del ancho del marcador. El valor de esta propiedad debe estar entre 0 y 500. |
| [GapWidth](../../aspose.cells.charts/chart/gapwidth/) { get; set; } | Devuelve o establece el espacio entre grupos de barras o columnas, como un porcentaje del ancho de la barra o columna. El valor de esta propiedad debe estar entre 0 y 500. |
| [HeightPercent](../../aspose.cells.charts/chart/heightpercent/) { get; set; } | Devuelve o establece la altura de un gráfico 3-D como un porcentaje del ancho del gráfico (entre el 5 y el 500 por ciento). |
| [HidePivotFieldButtons](../../aspose.cells.charts/chart/hidepivotfieldbuttons/) { get; set; } | Indica si se ocultan los botones de campo del gráfico dinámico solo cuando el gráfico es PivotChart. |
| [Is3D](../../aspose.cells.charts/chart/is3d/) { get; } | Indica si el gráfico es un gráfico 3D. |
| [IsRectangularCornered](../../aspose.cells.charts/chart/isrectangularcornered/) { get; set; } | Obtiene o establece un valor que indica si el área del gráfico tiene esquinas rectangulares. El valor predeterminado es true. |
| [Legend](../../aspose.cells.charts/chart/legend/) { get; } | Obtiene la leyenda del gráfico. |
| [Line](../../aspose.cells.charts/chart/line/) { get; } | Obtiene la línea. |
| [Name](../../aspose.cells.charts/chart/name/) { get; set; } | Obtiene y establece el nombre del gráfico. |
| [NSeries](../../aspose.cells.charts/chart/nseries/) { get; } | Obtiene una colección [`SeriesCollection`](../seriescollection/) que representa las series de datos en el gráfico. |
| [PageSetup](../../aspose.cells.charts/chart/pagesetup/) { get; } | Representa la descripción de la configuración de página en este gráfico. |
| [Perspective](../../aspose.cells.charts/chart/perspective/) { get; set; } | Devuelve o establece la perspectiva para la vista del gráfico tridimensional. Debe estar entre 0 y 100. Esta propiedad se ignora si la propiedad RightAngleAxes es True. |
| [PivotOptions](../../aspose.cells.charts/chart/pivotoptions/) { get; } | Especifica los controles dinámicos que aparecen en el gráfico. |
| [PivotSource](../../aspose.cells.charts/chart/pivotsource/) { get; set; } | La fuente son los datos de la tabla dinámica. Si PivotSource no está vacío, el gráfico es PivotChart. |
| [Placement](../../aspose.cells.charts/chart/placement/) { get; set; } | Representa la forma en que el gráfico está unido a las celdas debajo de él. |
| [PlotArea](../../aspose.cells.charts/chart/plotarea/) { get; } | Obtiene el área de trazado del gráfico que incluye las etiquetas de marcas del eje. |
| [PlotBy](../../aspose.cells.charts/chart/plotby/) { get; } | Obtiene y establece si se traza por fila o columna. |
| [PlotEmptyCellsType](../../aspose.cells.charts/chart/plotemptycellstype/) { get; set; } | Obtiene y establece cómo trazar las celdas vacías. |
| [PlotVisibleCells](../../aspose.cells.charts/chart/plotvisiblecells/) { get; set; } | (**Obsolete.**) Indica si solo se trazan celdas visibles. |
| [PlotVisibleCellsOnly](../../aspose.cells.charts/chart/plotvisiblecellsonly/) { get; set; } | Indica si solo se trazan celdas visibles del gráfico. |
| [PrintSize](../../aspose.cells.charts/chart/printsize/) { get; set; } | Obtiene y establece el tamaño impreso del gráfico. |
| [RightAngleAxes](../../aspose.cells.charts/chart/rightangleaxes/) { get; set; } | True si los ejes del gráfico forman ángulos rectos. Se aplica solo a gráficos 3-D (excepto Column3D y gráficos de pastel 3-D). |
| [RotationAngle](../../aspose.cells.charts/chart/rotationangle/) { get; set; } | Representa la rotación de la vista del gráfico 3-D (la rotación del área de trazado alrededor del eje z, en grados). |
| [SecondCategoryAxis](../../aspose.cells.charts/chart/secondcategoryaxis/) { get; } | Obtiene el segundo eje X del gráfico. |
| [SecondValueAxis](../../aspose.cells.charts/chart/secondvalueaxis/) { get; } | Obtiene el segundo eje Y del gráfico. |
| [SeriesAxis](../../aspose.cells.charts/chart/seriesaxis/) { get; } | Obtiene el eje de series del gráfico. |
| [Shapes](../../aspose.cells.charts/chart/shapes/) { get; } | Devuelve todas las formas de dibujo en este gráfico. |
| [ShowDataTable](../../aspose.cells.charts/chart/showdatatable/) { get; set; } | Obtiene o establece un valor que indica si el gráfico muestra una tabla de datos. |
| [ShowLegend](../../aspose.cells.charts/chart/showlegend/) { get; set; } | Obtiene o establece un valor que indica si se mostrará la leyenda del gráfico. El valor predeterminado es true. |
| [SideWall](../../aspose.cells.charts/chart/sidewall/) { get; } | Devuelve un objeto [`Walls`](./walls/) que representa la pared lateral de un gráfico 3-D. |
| [SizeWithWindow](../../aspose.cells.charts/chart/sizewithwindow/) { get; set; } | True si Microsoft Excel redimensiona el gráfico para que coincida con el tamaño de la ventana de la hoja del gráfico. |
| [Style](../../aspose.cells.charts/chart/style/) { get; set; } | Obtiene y establece el estilo incorporado. |
| [SubTitle](../../aspose.cells.charts/chart/subtitle/) { get; } | Obtiene el subtítulo del gráfico. Solo se aplica a archivos ODS. |
| [Title](../../aspose.cells.charts/chart/title/) { get; } | Obtiene el título del gráfico. |
| [Type](../../aspose.cells.charts/chart/type/) { get; set; } | Obtiene o establece el tipo de un gráfico. |
| [ValueAxis](../../aspose.cells.charts/chart/valueaxis/) { get; } | Obtiene el eje Y del gráfico. |
| [Walls](../../aspose.cells.charts/chart/walls/) { get; } | Devuelve un objeto [`Walls`](./walls/) que representa las paredes de un gráfico 3-D. |
| [WallsAndGridlines2D](../../aspose.cells.charts/chart/wallsandgridlines2d/) { get; set; } | True si las líneas de cuadrícula se dibujan bidimensionalmente en un gráfico 3-D. |
| [Worksheet](../../aspose.cells.charts/chart/worksheet/) { get; } | Obtiene la hoja de cálculo que contiene este gráfico. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Calculate](../../aspose.cells.charts/chart/calculate/#calculate)() | Calcula las posiciones personalizadas del área de trazado y los ejes si sus posiciones se asignan automáticamente. |
| [Calculate](../../aspose.cells.charts/chart/calculate/#calculate_1)(ChartCalculateOptions) | Calcula la posición personalizada del área de trazado y los ejes si su posición se asigna automáticamente, con Opciones de cálculo del gráfico. |
| [ChangeTemplate](../../aspose.cells.charts/chart/changetemplate/)(byte[]) | Cambiar el tipo de gráfico con una plantilla predefinida. |
| [GetActualSize](../../aspose.cells.charts/chart/getactualsize/)() | Obtiene el tamaño real del gráfico en unidades de píxeles. |
| [GetChartDataRange](../../aspose.cells.charts/chart/getchartdatarange/)() | Obtiene el rango de origen de datos del gráfico. |
| [HasAxis](../../aspose.cells.charts/chart/hasaxis/)(AxisType, bool) | Devuelve qué ejes existen en el gráfico. |
| [IsCellReferedByChart](../../aspose.cells.charts/chart/iscellreferedbychart/)(int, int, int) | Devuelve si la celda es referenciada por el gráfico. |
| [IsChartDataChanged](../../aspose.cells.charts/chart/ischartdatachanged/)() | Detecta si el origen de datos de un gráfico ha cambiado. |
| [IsReferedByChart](../../aspose.cells.charts/chart/isreferedbychart/)(int, int) | (**Obsolete.**) Devuelve si la celda es referenciada por el gráfico. |
| [Move](../../aspose.cells.charts/chart/move/)(int, int, int, int) | Mueve el gráfico a una ubicación especificada. |
| [RefreshPivotData](../../aspose.cells.charts/chart/refreshpivotdata/)() | Actualiza los datos del gráfico desde la tabla dinámica. |
| [SetChartDataRange](../../aspose.cells.charts/chart/setchartdatarange/)(string, bool) | Especifica el rango de datos para un gráfico. |
| [SwitchRowColumn](../../aspose.cells.charts/chart/switchrowcolumn/)() | Intercambia fila/columna. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage)() | Obtiene un objeto `Bitmap` de 32 bits del gráfico. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_1)(ImageOrPrintOptions) | Obtiene un objeto `Bitmap` de 32 bits del gráfico. Los atributos `ImageOrPrintOptions.ImageFormat`, ImageOrPrintOptions.TiffCompression y ImageOrPrintOptions.Quality se ignoran. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_6)(string) | Crea la imagen del gráfico y la guarda en un archivo. La extensión del nombre del archivo determina el formato de la imagen. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_5)(Stream, ImageFormat) | (**Obsolete.**) Crea la imagen del gráfico y la guarda en un flujo en el formato especificado. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_3)(Stream, ImageOrPrintOptions) | Crea la imagen del gráfico y la guarda en un flujo en el formato especificado. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_2)(Stream, ImageType) | Crea la imagen del gráfico y la guarda en un flujo en el formato especificado. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_4)(Stream, long) | Crea la imagen del gráfico y la guarda en un flujo en formato Jpeg. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_10)(string, ImageFormat) | (**Obsolete.**) Crea la imagen del gráfico y la guarda en un archivo en el formato especificado. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_8)(string, ImageOrPrintOptions) | Crea la imagen del gráfico y la guarda en un archivo. La extensión del nombre del archivo determina el formato de la imagen. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_7)(string, ImageType) | Crea la imagen del gráfico y la guarda en un archivo en el tipo de imagen especificado. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_9)(string, long) | (**Obsolete.**) Crea la imagen del gráfico y la guarda en un archivo en formato Jpeg. |
| [ToPdf](../../aspose.cells.charts/chart/topdf/#topdf)(Stream) | Crea el PDF del gráfico y lo guarda en un flujo. |
| [ToPdf](../../aspose.cells.charts/chart/topdf/#topdf_2)(string) | Guarda el gráfico en un archivo PDF. |
| [ToPdf](../../aspose.cells.charts/chart/topdf/#topdf_1)(Stream, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) | Crea el PDF del gráfico y lo guarda en un flujo. |
| [ToPdf](../../aspose.cells.charts/chart/topdf/#topdf_3)(string, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) | Guarda el gráfico en un archivo PDF. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class ChartDemo
    {
        public static void ChartExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells[0, 1].PutValue("Income");
            worksheet.Cells[1, 0].PutValue("Company A");
            worksheet.Cells[2, 0].PutValue("Company B");
            worksheet.Cells[3, 0].PutValue("Company C");
            worksheet.Cells[1, 1].PutValue(10000);
            worksheet.Cells[2, 1].PutValue(20000);
            worksheet.Cells[3, 1].PutValue(30000);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer el rango de datos para el gráfico
            chart.SetChartDataRange("A1:B4", true);

            // Establecer propiedades del gráfico
            chart.ShowLegend = true;
            chart.Title.Text = "Income Analysis";
            chart.Style = 2; // Built-in style

            // Personalizar la apariencia del gráfico
            chart.ChartObject.Name = "IncomeChart";
            chart.PlotEmptyCellsType = PlotEmptyCellsType.NotPlotted;
            chart.PlotVisibleCells = true;
            chart.DisplayNaAsBlank = true;
            chart.SizeWithWindow = true;

            // Personalizar los ejes del gráfico
            chart.CategoryAxis.Title.Text = "Companies";
            chart.ValueAxis.Title.Text = "Income";
            chart.CategoryAxis.MajorTickMark = TickMarkType.Outside;
            chart.ValueAxis.MajorTickMark = TickMarkType.Outside;

            // Personalizar la leyenda del gráfico
            chart.Legend.Position = LegendPositionType.Bottom;
            chart.Legend.IsOverLay = false;

            // Personaliza el área de trazado del gráfico
            chart.PlotArea.Area.ForegroundColor = Color.LightYellow;
            chart.PlotArea.Border.IsVisible = false;

            // Personaliza el área del gráfico
            chart.ChartArea.Area.ForegroundColor = Color.LightBlue;
            chart.ChartArea.Border.IsVisible = false;

            // Guarda el libro de trabajo
            workbook.Save("ChartExample.xlsx");
            workbook.Save("ChartExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


