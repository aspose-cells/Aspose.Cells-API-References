---
title: "Chart.DepthPercent"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad del gráfico. Representa la profundidad de un gráfico 3D como un porcentaje del ancho del gráfico entre 20 y 2000 por ciento."
type: docs
url: /es/net/aspose.cells.charts/chart/depthpercent/
---
## Chart.DepthPercent property

Representa la profundidad de un gráfico 3-D como un porcentaje del ancho del gráfico (entre el 20 y el 2000 por ciento).

```csharp
public int DepthPercent { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyDepthPercentDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);
            worksheet.Cells["C1"].PutValue("Series2");
            worksheet.Cells["C2"].PutValue(150);
            worksheet.Cells["C3"].PutValue(250);
            worksheet.Cells["C4"].PutValue(350);

            // Agregar un gráfico de columnas 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:C4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Establecer la propiedad DepthPercent (controla la profundidad del gráfico 3D como porcentaje del ancho del gráfico)
            chart.DepthPercent = 150; // 150% depth

            // Guarda el libro de trabajo
            workbook.Save("ChartDepthPercentDemo.xlsx");

            Console.WriteLine("Chart with DepthPercent 150% created successfully.");
        }
    }
}
```

### Ver también

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


