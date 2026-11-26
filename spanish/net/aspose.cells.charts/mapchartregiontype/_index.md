---
title: "Enumeración MapChartRegionType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Charts.MapChartRegionType. Representa el tipo de región del gráfico de mapa"
type: docs
url: /es/net/aspose.cells.charts/mapchartregiontype/
---
## MapChartRegionType enumeration

Representa el tipo de región del gráfico de mapa.

```csharp
public enum MapChartRegionType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Automatic | `0` | Automático |
| DataOnly | `1` | Contiene solo datos. |
| CountryRegionList | `2` | Lista de regiones de países. |
| World | `3` | Mundo. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class MapChartRegionTypeDemo
    {
        public static void MapChartRegionTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Country");
            worksheet.Cells["A2"].PutValue("USA");
            worksheet.Cells["A3"].PutValue("Canada");
            worksheet.Cells["A4"].PutValue("Mexico");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // Agregar un gráfico de mapa a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Map, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer el rango de datos del gráfico
            chart.SetChartDataRange("A1:B4", true);

            // Establecer el tipo de región del gráfico de mapa
            foreach (Series series in chart.NSeries)
            {
                series.LayoutProperties.MapChartRegionType = MapChartRegionType.CountryRegionList;
            }

            // Guarda el libro de trabajo
            workbook.Save("MapChartRegionTypeExample.xlsx");

            // Mostrar el resultado
            Console.WriteLine("Map chart with region type 'CountryRegionList' created successfully.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


