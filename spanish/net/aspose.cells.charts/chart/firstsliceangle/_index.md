---
title: "Chart.FirstSliceAngle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Chart property. Obtiene o establece el ángulo de la primera porción de piechart o doughnutchart en grados, en sentido horario desde la vertical. Se aplica solo a gráficos pie 3D y doughnut de 0 a 360"
type: docs
url: /es/net/aspose.cells.charts/chart/firstsliceangle/
---
## Chart.FirstSliceAngle property

Obtiene o establece el ángulo de la primera porción de gráfico de pastel o de rosquilla, en grados (en sentido horario desde la vertical). Se aplica solo a gráficos de pastel, pastel 3-D y rosquilla, de 0 a 360.

```csharp
public int FirstSliceAngle { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyFirstSliceAngleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Agregar gráfico circular
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Pie, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Establecer el ángulo de la primera porción a 45 grados
            chart.FirstSliceAngle = 45;
            
            // Guarda el libro de trabajo
            workbook.Save("PieChartWithFirstSliceAngle.xlsx");
        }
    }
}
```

### Ver también

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


