---
title: "SeriesLayoutProperties.MapLabelLayout"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SeriesLayoutProperties. Obtiene y establece el diseño de las etiquetas del mapa"
type: docs
url: /es/net/aspose.cells.charts/serieslayoutproperties/maplabellayout/
---
## SeriesLayoutProperties.MapLabelLayout property

Obtiene y establece el diseño de las etiquetas del mapa.

```csharp
public MapChartLabelLayout MapLabelLayout { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesLayoutPropertiesPropertyMapLabelLayoutDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para el gráfico de mapa
            worksheet.Cells["A1"].PutValue("Country");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("United States");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Canada");
            worksheet.Cells["B3"].PutValue(80);
            worksheet.Cells["A4"].PutValue("Mexico");
            worksheet.Cells["B4"].PutValue(60);

            // Agregar un gráfico de mapa
            int chartIndex = worksheet.Charts.Add(ChartType.Map, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            Series series = chart.NSeries[0];
            series.XValues = "A2:A4";

            // Configurar propiedades de diseño del mapa
            series.LayoutProperties.MapChartProjectionType = MapChartProjectionType.Mercator;
            series.LayoutProperties.MapLabelLayout = MapChartLabelLayout.ShowAll;
            series.LayoutProperties.MapChartRegionType = MapChartRegionType.DataOnly;

            // Guarda el libro de trabajo
            workbook.Save("MapLabelLayoutDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [MapChartLabelLayout](../../mapchartlabellayout/)
* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


