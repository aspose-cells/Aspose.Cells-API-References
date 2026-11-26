---
title: "Trendline.DisplayEquation"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Trendline. Indica si la ecuación de la línea de tendencia se muestra en el gráfico en la misma etiqueta de datos que el valor de R al cuadrado. Establecer esta propiedad en True activa automáticamente las etiquetas de datos"
type: docs
url: /es/net/aspose.cells.charts/trendline/displayequation/
---
## Trendline.DisplayEquation property

Representa si la ecuación de la línea de tendencia se muestra en el gráfico (en la misma etiqueta de datos que el valor R-cuadrado). Establecer esta propiedad en True activa automáticamente las etiquetas de datos.

```csharp
public bool DisplayEquation { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyDisplayEquationDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Agregar serie y línea de tendencia
            chart.NSeries.Add("A1:B4", true);
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            
            // Configurar propiedades de la línea de tendencia
            trendline.DisplayEquation = true;
            trendline.DisplayRSquared = false;
            trendline.Color = Color.Blue;

            workbook.Save("TrendlineDisplayEquationDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


