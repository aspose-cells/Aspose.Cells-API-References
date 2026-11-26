---
title: "Chart.AutoScaling"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Chart propiedad. Verdadero si Microsoft Excel escala un gráfico 3D de modo que su tamaño sea más cercano al del gráfico 2D equivalente. La propiedad RightAngleAxes debe ser Verdadero"
type: docs
url: /es/net/aspose.cells.charts/chart/autoscaling/
---
## Chart.AutoScaling property

Verdadero si Microsoft Excel escala un gráfico 3-D para que su tamaño sea más cercano al del gráfico 2-D equivalente. La propiedad RightAngleAxes debe ser Verdadero.

```csharp
public bool AutoScaling { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyAutoScalingDemo
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
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Demostrar la propiedad AutoScaling
            chart.AutoScaling = false;
            Console.WriteLine("Chart AutoScaling is set to: " + chart.AutoScaling);

            // Guarda el libro de trabajo
            workbook.Save("ChartAutoScalingDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


