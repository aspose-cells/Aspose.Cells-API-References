---
title: "ChartPoint.YValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartPoint. Obtiene o establece el valor Y del punto del gráfico"
type: docs
url: /es/net/aspose.cells.charts/chartpoint/yvalue/
---
## ChartPoint.YValue property

Obtiene o establece el valor Y del punto del gráfico.

```csharp
public object YValue { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPointPropertyYValueDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["A5"].PutValue("D");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Agregar un gráfico de columnas
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Obtener los puntos de la primera serie
            Series series = chart.NSeries[0];
            var points = series.Points;

            // Demostrar la propiedad YValue
            Console.WriteLine("Y Values of Chart Points:");
            for (int i = 0; i < points.Count; i++)
            {
                Console.WriteLine($"Point {i + 1}: {points[i].YValue}");
            }

            // Modificar el YValue de un punto
            points[2].YValue = 50;
            Console.WriteLine($"\nModified Point 3 YValue to: {points[2].YValue}");

            // Guarda el libro de trabajo
            workbook.Save("ChartPointYValueDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


