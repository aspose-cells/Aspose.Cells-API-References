---
title: "ChartPoint.XValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartPoint. Obtiene o establece el valor X del punto del gráfico"
type: docs
url: /es/net/aspose.cells.charts/chartpoint/xvalue/
---
## ChartPoint.XValue property

Obtiene o establece el valor X del punto del gráfico.

```csharp
public object XValue { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPointPropertyXValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Añadiendo datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(50);
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(150);

            // Añadiendo un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Estableciendo la fuente de datos del gráfico
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Personalizando los puntos de datos
            for (int i = 0; i < chart.NSeries[0].Points.Count; i++)
            {
                ChartPoint point = chart.NSeries[0].Points[i];
                
                // Demostrando el uso de la propiedad XValue
                point.XValue = "Modified " + (i + 1);
                
                // Formato adicional para mayor visibilidad
                point.Area.ForegroundColor = Color.FromArgb(100 + i * 50, 150, 200);
            }

            workbook.Save("ChartPointXValueDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


