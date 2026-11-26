---
title: "Series.FirstSliceAngle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Series. Obtiene o establece el ángulo de la primera porción de piechart o doughnutchart en grados en sentido horario desde la vertical. Se aplica solo a gráficos de pie, 3D pie y doughnut con valores de 0 a 360"
type: docs
url: /es/net/aspose.cells.charts/series/firstsliceangle/
---
## Series.FirstSliceAngle property

Obtiene o establece el ángulo de la primera porción de pastel o dona, en grados (en sentido horario desde la vertical). Se aplica solo a gráficos de pastel, pastel 3D y dona, con valores de 0 a 360.

```csharp
public short FirstSliceAngle { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyFirstSliceAngleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para el gráfico de pastel
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Agregar gráfico circular
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Obtener la primera serie y establecer FirstSliceAngle
            Series series = chart.NSeries[0];
            series.FirstSliceAngle = 45; // Rotate pie chart by 45 degrees

            workbook.Save("PieChartWithFirstSliceAngle.xlsx");
        }
    }
}
```

### Ver también

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


