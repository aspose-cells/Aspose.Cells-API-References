---
title: "DataLabels.ShowSeriesName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataLabels. Indica si el nombre de la serie se muestra en las etiquetas de datos de un gráfico. Verdadero para mostrar el nombre de la serie. Falso para ocultarlo"
type: docs
url: /es/net/aspose.cells.charts/datalabels/showseriesname/
---
## DataLabels.ShowSeriesName property

Indica si el nombre de la serie se muestra en las etiquetas de datos de un gráfico. True para mostrar el nombre de la serie. False para ocultarlo.

```csharp
public bool ShowSeriesName { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyShowSeriesNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Series 1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["B1"].PutValue("Series 2");
            worksheet.Cells["B2"].PutValue(15);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(35);

            // Agregar un gráfico de columnas
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer rango de datos del gráfico
            chart.NSeries.Add("A1:A4", true);
            chart.NSeries.Add("B1:B4", true);

            // Habilitar etiquetas de datos para la primera serie
            Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;

            // Habilitar la visualización del nombre de la serie para la etiqueta de datos de un punto específico
            var points = series.Points;
            points[1].DataLabels.ShowSeriesName = true;

            // Calcular gráfico
            chart.Calculate();

            // Guarda el libro de trabajo
            workbook.Save("DataLabelsShowSeriesNameDemo.xlsx");
        }
    }
}
```

### Ver también

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


