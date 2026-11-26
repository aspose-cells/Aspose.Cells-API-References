---
title: "Series.BubbleSizes"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Series. Obtiene o establece los valores de tamaño de burbuja de la serie del gráfico"
type: docs
url: /es/net/aspose.cells.charts/series/bubblesizes/
---
## Series.BubbleSizes property

Obtiene o establece los valores de tamaño de burbuja de la serie del gráfico.

```csharp
public string BubbleSizes { get; set; }
```

### Observaciones

Solo para Bubble o Bubble3D.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyBubbleSizesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el gráfico de burbujas
            worksheet.Cells["A1"].PutValue("X Values");
            worksheet.Cells["B1"].PutValue("Y Values");
            worksheet.Cells["C1"].PutValue("Bubble Sizes");
            
            for (int i = 2; i <= 5; i++)
            {
                worksheet.Cells["A" + i].PutValue(i);
                worksheet.Cells["B" + i].PutValue(i * 2);
                worksheet.Cells["C" + i].PutValue(i * 0.5);
            }

            // Agregar un gráfico de burbujas
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Bubble, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Establecer datos de la serie usando la propiedad BubbleSizes
            chart.NSeries.Add("A2:A5", true);
            chart.NSeries[0].XValues = "B2:B5";
            chart.NSeries[0].BubbleSizes = "C2:C5";

            // Guarda el libro de trabajo
            workbook.Save("BubbleChartDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


