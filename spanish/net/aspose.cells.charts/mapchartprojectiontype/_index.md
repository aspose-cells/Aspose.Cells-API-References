---
title: "Enumeración MapChartProjectionType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Charts.MapChartProjectionType enum. Representa el tipo de proyección del gráfico de mapa"
type: docs
url: /es/net/aspose.cells.charts/mapchartprojectiontype/
---
## MapChartProjectionType enumeration

Representa el tipo de proyección del gráfico de mapa.

```csharp
public enum MapChartProjectionType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Automatic | `0` | Automático |
| Mercator | `1` | Mercator |
| Miller | `2` | Miller |
| Albers | `3` | Albers |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class MapChartProjectionTypeDemo
    {
        public static void MapChartProjectionTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra a la hoja de cálculo para el gráfico de mapa
            worksheet.Cells["A1"].PutValue("Country");
            worksheet.Cells["A2"].PutValue("USA");
            worksheet.Cells["A3"].PutValue("Canada");
            worksheet.Cells["A4"].PutValue("Mexico");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(80);
            worksheet.Cells["B4"].PutValue(60);

            // Agregar un gráfico de mapa a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Map, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer el rango de datos del gráfico
            chart.SetChartDataRange("A1:B4", true);

            // Establecer el tipo de proyección para el gráfico de mapa
            chart.NSeries[0].LayoutProperties.MapChartProjectionType = MapChartProjectionType.Mercator;

            // Salida del tipo de proyección
            Console.WriteLine("Map Chart Projection Type: " + chart.NSeries[0].LayoutProperties.MapChartProjectionType);

            // Guarda el libro de trabajo
            workbook.Save("MapChartProjectionTypeExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


