---
title: "Trendline.Backward"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Trendline. Devuelve o establece el número de períodos o unidades en un gráfico de dispersión que la línea de tendencia se extiende hacia atrás. El número de períodos debe ser mayor o igual a cero. Si el tipo de gráfico es columna, el número de períodos debe estar entre 0 y 0.5"
type: docs
url: /es/net/aspose.cells.charts/trendline/backward/
---
## Trendline.Backward property

Devuelve o establece el número de períodos (o unidades en un gráfico de dispersión) que la línea de tendencia se extiende hacia atrás. El número de períodos debe ser mayor o igual a cero. Si el tipo de gráfico es columna, el número de períodos debe estar entre 0 y 0,5

```csharp
public double Backward { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyBackwardDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);

            // Crear gráfico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B4", true);

            // Agregar línea de tendencia y obtenerla por índice
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(Aspose.Cells.Charts.TrendlineType.Linear);
            Aspose.Cells.Charts.Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.Name = "Linear Trend";
            trendline.DisplayEquation = true;
            
            // Establecer la propiedad backward para extender la línea de tendencia hacia atrás en 0.5 unidades
            trendline.Backward = 0.5;
            
            workbook.Save("TrendlineBackwardDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


