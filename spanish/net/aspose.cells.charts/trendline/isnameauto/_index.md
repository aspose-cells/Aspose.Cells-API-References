---
title: "Trendline.IsNameAuto"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Trendline. Indica si Microsoft Excel determina automáticamente el nombre de la línea de tendencia"
type: docs
url: /es/net/aspose.cells.charts/trendline/isnameauto/
---
## Trendline.IsNameAuto property

Devuelve si Microsoft Excel determina automáticamente el nombre de la línea de tendencia.

```csharp
public bool IsNameAuto { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyIsNameAutoDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["B1"].PutValue("Y");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue(i);
                worksheet.Cells["B" + i].PutValue(i * 2);
            }

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Agregar serie al gráfico
            chart.NSeries.Add("B2:B10", true);
            chart.NSeries.CategoryData = "A2:A10";

            // Agregar línea de tendencia - modificado para asegurar la creación adecuada del objeto Trendline
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            
            // Demostrar la propiedad IsNameAuto
            Console.WriteLine("Initial IsNameAuto value: " + trendline.IsNameAuto);
            
            // Establecer nombre personalizado (desactiva la asignación automática de nombres)
            trendline.Name = "Custom Trendline Name";
            Console.WriteLine("After setting custom name, IsNameAuto: " + trendline.IsNameAuto);
            
            // Restablecer al nombre automático
            trendline.IsNameAuto = true;
            Console.WriteLine("After setting IsNameAuto=true, Name: " + trendline.Name);
        }
    }
}
```

### Ver también

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


