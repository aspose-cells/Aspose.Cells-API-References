---
title: "Clase SeriesLayoutProperties"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Charts.SeriesLayoutProperties. Representa las propiedades del diseño de series"
type: docs
url: /es/net/aspose.cells.charts/serieslayoutproperties/
---
## SeriesLayoutProperties class

Representa las propiedades del diseño de series.

```csharp
public class SeriesLayoutProperties
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [SeriesLayoutProperties](serieslayoutproperties/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [IsIntervalLeftClosed](../../aspose.cells.charts/serieslayoutproperties/isintervalleftclosed/) { get; set; } | Indica si el intervalo está cerrado en el lado izquierdo. |
| [MapChartProjectionType](../../aspose.cells.charts/serieslayoutproperties/mapchartprojectiontype/) { get; set; } | Obtiene y establece el tipo de proyección del mapa. |
| [MapChartRegionType](../../aspose.cells.charts/serieslayoutproperties/mapchartregiontype/) { get; set; } | Obtiene y establece el tipo de región del mapa. |
| [MapLabelLayout](../../aspose.cells.charts/serieslayoutproperties/maplabellayout/) { get; set; } | Obtiene y establece el diseño de las etiquetas del mapa. |
| [QuartileCalculation](../../aspose.cells.charts/serieslayoutproperties/quartilecalculation/) { get; set; } | Representa las propiedades estadísticas de la serie. |
| [ShowConnectorLines](../../aspose.cells.charts/serieslayoutproperties/showconnectorlines/) { get; set; } | Indica si se muestran líneas de conexión entre los puntos de datos. |
| [ShowInnerPoints](../../aspose.cells.charts/serieslayoutproperties/showinnerpoints/) { get; set; } | Indica si se muestran puntos de datos que no son valores atípicos. |
| [ShowMeanLine](../../aspose.cells.charts/serieslayoutproperties/showmeanline/) { get; set; } | Indica si se muestra la línea que conecta todos los puntos de media. |
| [ShowMeanMarker](../../aspose.cells.charts/serieslayoutproperties/showmeanmarker/) { get; set; } | Indica si se muestran los marcadores que denotan la media. |
| [ShowOutlierPoints](../../aspose.cells.charts/serieslayoutproperties/showoutlierpoints/) { get; set; } | Indica si se muestran los puntos de datos atípicos. |
| [Subtotals](../../aspose.cells.charts/serieslayoutproperties/subtotals/) { get; set; } | Representa el índice de un punto de datos subtotal. |

### Observaciones

Solo aplicable a los gráficos BoxWhisker,Funnel,ParetoLine,Sunburst,Treemap,Waterfall y Histogram.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesLayoutPropertiesDemo
    {
        public static void SeriesLayoutPropertiesExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la hoja de cálculo
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
            Chart chart = worksheet.Charts[chartIndex];

            // Agregar series al gráfico
            int seriesIndex = chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";
            Series series = chart.NSeries[seriesIndex];

            // Establece los valores de la serie
            series.Values = "=B1:B4";

            // Accede al objeto SeriesLayoutProperties
            SeriesLayoutProperties layoutProperties = series.LayoutProperties;

            // Establece las propiedades de SeriesLayoutProperties
            layoutProperties.ShowConnectorLines = true;
            layoutProperties.ShowMeanLine = true;
            layoutProperties.ShowOutlierPoints = true;
            layoutProperties.ShowMeanMarker = true;
            layoutProperties.ShowInnerPoints = true;
            layoutProperties.QuartileCalculation = QuartileCalculationType.Inclusive;
            layoutProperties.MapLabelLayout = MapChartLabelLayout.ShowAll;
            layoutProperties.IsIntervalLeftClosed = true;
            layoutProperties.MapChartRegionType = MapChartRegionType.World;
            layoutProperties.MapChartProjectionType = MapChartProjectionType.Mercator;

            // Guarda el libro de trabajo
            workbook.Save("SeriesLayoutPropertiesExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


