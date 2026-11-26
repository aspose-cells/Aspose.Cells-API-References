---
title: "Enumeración MapChartLabelLayout"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Charts.MapChartLabelLayout. Representa la disposición de las etiquetas de los gráficos de mapa"
type: docs
url: /es/net/aspose.cells.charts/mapchartlabellayout/
---
## MapChartLabelLayout enumeration

Representa el diseño de las etiquetas del gráfico de mapa.

```csharp
public enum MapChartLabelLayout
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| BestFitOnly | `0` | Solo se utiliza el mejor ajuste. |
| ShowAll | `1` | Muestra todas las etiquetas. |
| None | `2` | No hay etiquetas. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class MapChartLabelLayoutDemo
    {
        public static void MapChartLabelLayoutExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el gráfico de mapa
            worksheet.Cells["A1"].PutValue("Country");
            worksheet.Cells["A2"].PutValue("USA");
            worksheet.Cells["A3"].PutValue("Canada");
            worksheet.Cells["A4"].PutValue("Mexico");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(150);

            // Agregar un gráfico de mapa a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Map, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer el rango de datos para el gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accede a las propiedades de diseño de la serie
            SeriesLayoutProperties layoutProperties = chart.NSeries[0].LayoutProperties;

            // Establecer la disposición de las etiquetas del gráfico de mapa
            layoutProperties.MapLabelLayout = MapChartLabelLayout.ShowAll;

            // Guarda el libro de trabajo
            workbook.Save("MapChartLabelLayoutExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


