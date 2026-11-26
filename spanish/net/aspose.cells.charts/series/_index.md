---
title: "Clase Series"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Charts.Series class. Encapsula el objeto que representa una única serie de datos en un gráfico"
type: docs
url: /es/net/aspose.cells.charts/series/
---
## Series class

Encapsula el objeto que representa una única serie de datos en un gráfico.

```csharp
public class Series
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Area](../../aspose.cells.charts/series/area/) { get; } | Representa el área de fondo del objeto Series. |
| [Bar3DShapeType](../../aspose.cells.charts/series/bar3dshapetype/) { get; set; } | Obtiene o establece el tipo de forma 3D utilizado con el gráfico de barras o columnas 3D. |
| [Border](../../aspose.cells.charts/series/border/) { get; } | Representa el borde de un objeto Series. |
| [BubbleScale](../../aspose.cells.charts/series/bubblescale/) { get; set; } | Obtiene o establece el factor de escala para las burbujas en el grupo de gráfico especificado. Puede ser un valor entero de 0 (cero) a 300, correspondiente a un porcentaje del tamaño predeterminado. Se aplica solo a gráficos de burbujas. |
| [BubbleSizes](../../aspose.cells.charts/series/bubblesizes/) { get; set; } | Obtiene o establece los valores de tamaño de burbuja de la serie del gráfico. |
| [CachedCategoryValues](../../aspose.cells.charts/series/cachedcategoryvalues/) { get; } | (**Obsolete.**) Obtiene los valores de categoría en caché de la serie |
| [CachedValues](../../aspose.cells.charts/series/cachedvalues/) { get; } | (**Obsolete.**) Obtiene los valores en caché de la serie |
| [CategoryValues](../../aspose.cells.charts/series/categoryvalues/) { get; } | Obtiene los valores reales de categoría que se utilizan para trazar cada punto de esta serie en el gráfico. |
| [CountOfDataValues](../../aspose.cells.charts/series/countofdatavalues/) { get; } | Obtiene el número de los valores de datos. |
| [DataLabels](../../aspose.cells.charts/series/datalabels/) { get; } | Representa el objeto DataLabels para el ASeries especificado. |
| [DisplayName](../../aspose.cells.charts/series/displayname/) { get; } | Obtiene el nombre de la serie que se muestra en el gráfico. |
| [DoughnutHoleSize](../../aspose.cells.charts/series/doughnutholesize/) { get; set; } | Devuelve o establece el tamaño del agujero en un grupo de gráfico de dona. El tamaño del agujero se expresa como un porcentaje del tamaño del gráfico, entre el 10 y el 90 por ciento. |
| [DownBars](../../aspose.cells.charts/series/downbars/) { get; } | Devuelve un objeto [`DropBars`](../dropbars/) que representa las barras descendentes en un gráfico de líneas. Se aplica solo a gráficos de líneas. |
| [DropLines](../../aspose.cells.charts/series/droplines/) { get; } | Devuelve un objeto [`Line`](../../aspose.cells.drawing/line/) que representa las líneas de caída para una serie en el gráfico de líneas o de áreas. Se aplica solo a gráficos de líneas o de áreas. |
| [Explosion](../../aspose.cells.charts/series/explosion/) { get; set; } | La distancia de una porción de pastel abierta desde el centro del gráfico de pastel se expresa como un porcentaje del diámetro del pastel. |
| [FirstSliceAngle](../../aspose.cells.charts/series/firstsliceangle/) { get; set; } | Obtiene o establece el ángulo de la primera porción de pastel o dona, en grados (en sentido horario desde la vertical). Se aplica solo a gráficos de pastel, pastel 3D y dona, con valores de 0 a 360. |
| [GapWidth](../../aspose.cells.charts/series/gapwidth/) { get; set; } | Devuelve o establece el espacio entre grupos de barras o columnas, como un porcentaje del ancho de la barra o columna. El valor de esta propiedad debe estar entre 0 y 500. |
| [Has3DEffect](../../aspose.cells.charts/series/has3deffect/) { get; set; } | True si la serie tiene una apariencia tridimensional. |
| [HasDropLines](../../aspose.cells.charts/series/hasdroplines/) { get; set; } | True si el gráfico tiene líneas de caída. Se aplica solo a gráficos de líneas o de áreas. |
| [HasHiLoLines](../../aspose.cells.charts/series/hashilolines/) { get; set; } | True si el gráfico de líneas tiene líneas alto-bajo. Se aplica solo a gráficos de líneas. |
| [HasLeaderLines](../../aspose.cells.charts/series/hasleaderlines/) { get; set; } | True si la serie tiene líneas guía. |
| [HasRadarAxisLabels](../../aspose.cells.charts/series/hasradaraxislabels/) { get; set; } | True si un gráfico de radar tiene etiquetas del eje de categorías. Se aplica solo a gráficos de radar. |
| [HasSeriesLines](../../aspose.cells.charts/series/hasserieslines/) { get; set; } | True si un gráfico de columnas apiladas o de barras tiene líneas de serie o si un gráfico Pie of Pie o Bar of Pie tiene líneas de conexión entre las dos secciones. Se aplica solo a gráficos de columnas apiladas, gráficos de barras, gráficos Pie of Pie o Bar of Pie. |
| [HasUpDownBars](../../aspose.cells.charts/series/hasupdownbars/) { get; set; } | True si un gráfico de líneas tiene barras arriba y abajo. Se aplica solo a gráficos de líneas. |
| [HiLoLines](../../aspose.cells.charts/series/hilolines/) { get; } | Devuelve un objeto HiLoLines que representa las líneas alto-bajo para una serie en un gráfico de líneas. Se aplica solo a gráficos de líneas. |
| [IsAutoSplit](../../aspose.cells.charts/series/isautosplit/) { get; } | Indica si el valor del umbral es automático. |
| [IsColorVaried](../../aspose.cells.charts/series/iscolorvaried/) { get; set; } | Representa si el color de los puntos varía. El gráfico debe contener solo una serie o ser un gráfico de pastel. |
| [IsFiltered](../../aspose.cells.charts/series/isfiltered/) { get; set; } | Indica si la serie está seleccionada o filtrada. True indica que esta serie está filtrada y no se mostrará en el gráfico. |
| [IsVerticalValues](../../aspose.cells.charts/series/isverticalvalues/) { get; } | Indica si la fuente de datos es vertical. |
| [LayoutProperties](../../aspose.cells.charts/series/layoutproperties/) { get; } | Representa las propiedades del diseño. |
| [LeaderLines](../../aspose.cells.charts/series/leaderlines/) { get; } | Representa líneas guía en un gráfico. Las líneas guía conectan las etiquetas de datos con los puntos de datos. Este objeto no es una colección; no hay un objeto que represente una sola línea guía. |
| [LegendEntry](../../aspose.cells.charts/series/legendentry/) { get; } | Obtiene la entrada de leyenda correspondiente a esta serie. |
| [Marker](../../aspose.cells.charts/series/marker/) { get; } | Obtiene el [`marker`](./marker/). |
| [Name](../../aspose.cells.charts/series/name/) { get; set; } | Obtiene o establece el nombre de la serie de datos. |
| [Overlap](../../aspose.cells.charts/series/overlap/) { get; set; } | Especifica cómo se posicionan las barras y columnas. Puede ser un valor entre -100 y 100. Se aplica solo a gráficos de barras 2D y gráficos de columnas 2D. |
| [PlotOnSecondAxis](../../aspose.cells.charts/series/plotonsecondaxis/) { get; set; } | Indica si esta serie se dibuja en el segundo eje de valores. |
| [Points](../../aspose.cells.charts/series/points/) { get; } | Obtiene la colección de puntos en una serie de un gráfico. |
| [PointValues](../../aspose.cells.charts/series/pointvalues/) { get; } | Obtiene los valores reales que se utilizan para trazar cada punto de esta serie en el gráfico. |
| [SecondPlotSize](../../aspose.cells.charts/series/secondplotsize/) { get; set; } | Devuelve o establece el tamaño de la sección secundaria de un gráfico de pastel dentro de pastel o de barra dentro de pastel, como un porcentaje del tamaño del pastel principal. Puede ser un valor de 5 a 200. |
| [SeriesLines](../../aspose.cells.charts/series/serieslines/) { get; } | Devuelve un objeto SeriesLines que representa las líneas de serie para un gráfico de barras apiladas o un gráfico de columnas apiladas. Se aplica solo a gráficos de barras apiladas y columnas apiladas. |
| [Shadow](../../aspose.cells.charts/series/shadow/) { get; set; } | True si la serie tiene una sombra. |
| [ShapeProperties](../../aspose.cells.charts/series/shapeproperties/) { get; } | Obtiene el objeto [`ShapePropertyCollection`](../../aspose.cells.drawing/shapepropertycollection/) que contiene las propiedades visuales de forma de la Serie. |
| [ShowNegativeBubbles](../../aspose.cells.charts/series/shownegativebubbles/) { get; set; } | True si se muestran burbujas negativas para el grupo de gráfico. Válido solo para gráficos de burbujas. |
| [SizeRepresents](../../aspose.cells.charts/series/sizerepresents/) { get; set; } | Obtiene o establece lo que representa el tamaño de la burbuja en un gráfico de burbujas. |
| [Smooth](../../aspose.cells.charts/series/smooth/) { get; set; } | Representa el suavizado de curvas. True si el suavizado de curvas está activado para el gráfico de líneas o de dispersión. Se aplica solo a gráficos de líneas y gráficos de dispersión con líneas. |
| [SplitType](../../aspose.cells.charts/series/splittype/) { get; set; } | Devuelve o establece un valor que indica cómo determinar qué puntos de datos están en el segundo pastel o barra en un gráfico de pastel dentro de pastel o barra dentro de pastel. |
| [SplitValue](../../aspose.cells.charts/series/splitvalue/) { get; set; } | Devuelve o establece un valor que se utilizará para determinar qué puntos de datos están en el segundo pastel o barra en un gráfico de pastel dentro de pastel o barra dentro de pastel. |
| [TrendLines](../../aspose.cells.charts/series/trendlines/) { get; } | Devuelve todas las líneas de tendencia de esta serie. |
| [Type](../../aspose.cells.charts/series/type/) { get; set; } | Obtiene o establece el tipo de una serie de datos. |
| [UpBars](../../aspose.cells.charts/series/upbars/) { get; } | Devuelve un objeto DropBars que representa las barras ascendentes en un gráfico de líneas. Se aplica solo a gráficos de líneas. |
| [Values](../../aspose.cells.charts/series/values/) { get; set; } | Representa los valores Y de esta serie de gráfico. |
| [ValuesFormatCode](../../aspose.cells.charts/series/valuesformatcode/) { get; set; } | Representa el código de formato de la lista de números de Valores. |
| [XErrorBar](../../aspose.cells.charts/series/xerrorbar/) { get; } | Representa la barra de error en dirección X de la serie. |
| [XValues](../../aspose.cells.charts/series/xvalues/) { get; set; } | Representa los valores X de esta serie de gráfico. |
| [XValuesFormatCode](../../aspose.cells.charts/series/xvaluesformatcode/) { get; set; } | Representa el código de formato de la lista de números de Valores X. |
| [YErrorBar](../../aspose.cells.charts/series/yerrorbar/) { get; } | Representa la barra de error en dirección Y de la serie. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Move](../../aspose.cells.charts/series/move/)(int) | Mueve la serie hacia arriba o hacia abajo. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesDemo
    {
        public static void SeriesExample()
        {
            // Instanciando un objeto Workbook
            Workbook workbook = new Workbook();
            // Añadiendo una nueva hoja de cálculo al objeto Excel
            int sheetIndex = workbook.Worksheets.Add();
            // Obteniendo la referencia de la hoja de cálculo recién añadida pasando su índice de hoja
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            // Agregar valores de muestra a celdas
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            // Accediendo a la instancia del gráfico recién agregado
            Chart chart = worksheet.Charts[chartIndex];
            // Agregar NSeries (fuente de datos del gráfico) al gráfico que abarca desde la celda "A1" hasta "B4"
            int seriesIndex = chart.NSeries.Add("A1:B4", true);
            // Estableciendo la fuente de datos para los datos de categoría de NSeries
            chart.NSeries.CategoryData = "C1:C4";

            // Accediendo a la serie
            Series series = chart.NSeries[seriesIndex];

            // Configurando los valores de la serie
            series.Values = "=B1:B4";
            // Cambiar el tipo de gráfico de la serie
            series.Type = ChartType.Line;
            // Establecer propiedades del marcador
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.ForegroundColorSetType = FormattingType.Automatic;
            series.Marker.ForegroundColor = System.Drawing.Color.Black;
            series.Marker.BackgroundColorSetType = FormattingType.Automatic;

            // Configurando propiedades adicionales
            series.Name = "First Series";
            series.IsFiltered = false;
            series.ValuesFormatCode = "0.00";
            series.XValues = "=A1:A4";
            series.BubbleSizes = "=B1:B4";
            series.Smooth = true;
            series.Shadow = true;
            series.Has3DEffect = true;
            series.Bar3DShapeType = Bar3DShapeType.Cylinder;
            series.PlotOnSecondAxis = false;
            series.HasHiLoLines = false;
            series.HasSeriesLines = false;
            series.HasDropLines = false;
            series.HasUpDownBars = false;
            series.IsColorVaried = false;
            series.GapWidth = 150;
            series.FirstSliceAngle = 45;
            series.Overlap = 0;
            series.SecondPlotSize = 100;
            series.SplitType = ChartSplitType.Position;
            series.SplitValue = 10.0;
            series.BubbleScale = 100;
            series.SizeRepresents = BubbleSizeRepresents.SizeIsArea;
            series.ShowNegativeBubbles = true;
            series.DoughnutHoleSize = 50;
            series.Explosion = 10;
            series.HasRadarAxisLabels = false;
            series.HasLeaderLines = true;

            // Guardando el archivo Excel
            workbook.Save("SeriesExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


