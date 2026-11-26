---
title: "Chart.GapDepth"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad del gráfico. Obtiene o establece la distancia entre las series de datos en un gráfico 3D como un porcentaje del ancho del marcador. El valor de esta propiedad debe estar entre 0 y 500"
type: docs
url: /es/net/aspose.cells.charts/chart/gapdepth/
---
## Chart.GapDepth property

Obtiene o establece la distancia entre las series de datos en un gráfico 3-D, como un porcentaje del ancho del marcador. El valor de esta propiedad debe estar entre 0 y 500.

```csharp
public int GapDepth { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyGapDepthDemo
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
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["B2"].PutValue(120);
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["B4"].PutValue(180);
            worksheet.Cells["C1"].PutValue("Series 2");
            worksheet.Cells["C2"].PutValue(90);
            worksheet.Cells["C3"].PutValue(110);
            worksheet.Cells["C4"].PutValue(130);

            // Agregar un gráfico de columnas 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:C4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Establecer la propiedad GapDepth (controla la distancia entre series de datos en gráficos 3D)
            chart.GapDepth = 150; // Value between 0-500

            // Guarda el libro de trabajo
            workbook.Save("ChartGapDepthDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


