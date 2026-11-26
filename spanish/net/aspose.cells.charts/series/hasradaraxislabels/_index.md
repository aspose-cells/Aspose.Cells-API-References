---
title: "Series.HasRadarAxisLabels"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Series. Verdadero si un gráfico de radar tiene etiquetas de eje de categoría. Se aplica solo a gráficos de radar"
type: docs
url: /es/net/aspose.cells.charts/series/hasradaraxislabels/
---
## Series.HasRadarAxisLabels property

True si un gráfico de radar tiene etiquetas del eje de categorías. Se aplica solo a gráficos de radar.

```csharp
public bool HasRadarAxisLabels { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyHasRadarAxisLabelsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico de radar
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Cat1");
            worksheet.Cells["A3"].PutValue("Cat2");
            worksheet.Cells["A4"].PutValue("Cat3");
            
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B3"].PutValue(2);
            worksheet.Cells["B4"].PutValue(5);

            // Agregar un gráfico de radar
            int chartIndex = worksheet.Charts.Add(ChartType.Radar, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Agregar datos de la serie
            int seriesIndex = chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Obtenga la serie y establezca las etiquetas del eje de radar
            Series series = chart.NSeries[seriesIndex];
            series.HasRadarAxisLabels = true; // This is the key property being demonstrated

            // Guarda el libro de trabajo
            workbook.Save("RadarChartWithAxisLabels.xlsx");
        }
    }
}
```

### Ver también

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


