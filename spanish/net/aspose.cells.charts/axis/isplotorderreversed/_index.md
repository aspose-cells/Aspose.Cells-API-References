---
title: "Axis.IsPlotOrderReversed"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Axis. Representa si Microsoft Excel traza los puntos de datos de último a primero"
type: docs
url: /es/net/aspose.cells.charts/axis/isplotorderreversed/
---
## Axis.IsPlotOrderReversed property

Representa si Microsoft Excel traza los puntos de datos de último a primero.

```csharp
public bool IsPlotOrderReversed { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyIsPlotOrderReversedDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Agregar un gráfico de columnas
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Establecer origen de datos del Chart
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Invertir el orden de trazado de las categorías
            chart.CategoryAxis.IsPlotOrderReversed = true;

            // Guarda el libro de trabajo
            workbook.Save("AxisPropertyIsPlotOrderReversedDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


