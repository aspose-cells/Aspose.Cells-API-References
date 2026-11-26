---
title: "Clase ChartCalculateOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Charts.ChartCalculateOptions. Representa las opciones para calcular un gráfico"
type: docs
url: /es/net/aspose.cells.charts/chartcalculateoptions/
---
## ChartCalculateOptions class

Representa las opciones para calcular un gráfico.

```csharp
public class ChartCalculateOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [ChartCalculateOptions](chartcalculateoptions/)() | Crea las opciones para calcular el gráfico. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [UpdateAllPoints](../../aspose.cells.charts/chartcalculateoptions/updateallpoints/) { get; set; } | Indica si se actualizan todos los puntos de datos al realizar el cálculo del gráfico. Predeterminado: False. Cuando desea obtener el valor de cada punto de datos en el gráfico específicamente, configúrelo en true. Si este parámetro se establece en True, pueden generarse nuevos puntos de datos cuando se calcula el gráfico. Esto podría hacer que el archivo de Excel sea más grande. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartCalculateOptionsDemo
    {
        public static void ChartCalculateOptionsExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells[0, 0].PutValue("Category");
            worksheet.Cells[0, 1].PutValue("Value");
            worksheet.Cells[1, 0].PutValue("A");
            worksheet.Cells[1, 1].PutValue(10);
            worksheet.Cells[2, 0].PutValue("B");
            worksheet.Cells[2, 1].PutValue(20);
            worksheet.Cells[3, 0].PutValue("C");
            worksheet.Cells[3, 1].PutValue(30);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer el rango de datos para el gráfico
            chart.SetChartDataRange("A1:B4", true);

            // Crear una instancia de ChartCalculateOptions
            ChartCalculateOptions options = new ChartCalculateOptions
            {
                UpdateAllPoints = true // Set the property to update all data points
            };

            // Calcular el gráfico con las opciones especificadas
            chart.Calculate(options);

            // Guarda el libro de trabajo
            workbook.Save("ChartCalculateOptionsExample.xlsx");
            workbook.Save("ChartCalculateOptionsExample.pdf");
            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


