---
title: "Chart.PlotBy"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Chart. Obtiene y establece si se traza por fila o columna"
type: docs
url: /es/net/aspose.cells.charts/chart/plotby/
---
## Chart.PlotBy property

Obtiene y establece si se traza por fila o columna.

```csharp
public PlotDataByType PlotBy { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyPlotByDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["C1"].PutValue("Series 2");
            worksheet.Cells["C2"].PutValue(15);
            worksheet.Cells["C3"].PutValue(25);
            worksheet.Cells["C4"].PutValue(35);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Establecer origen de datos del Chart
            chart.SetChartDataRange("A1:C4", true);

            // Demostrar la propiedad PlotBy
            Console.WriteLine("Default PlotBy: " + chart.PlotBy);
            
            // Crear un nuevo gráfico con una configuración de plot by diferente
            int newChartIndex = worksheet.Charts.Add(ChartType.Column, 25, 0, 40, 8);
            Aspose.Cells.Charts.Chart newChart = worksheet.Charts[newChartIndex];
            newChart.SetChartDataRange("A1:C4", false); // Plot by row
            Console.WriteLine("New chart PlotBy: " + newChart.PlotBy);

            // Guarda el libro de trabajo
            workbook.Save("ChartPropertyPlotByDemo_out.xlsx");
        }
    }
}
```

### Ver también

* enum [PlotDataByType](../../plotdatabytype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


