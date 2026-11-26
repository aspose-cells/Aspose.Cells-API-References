---
title: "AxisBins.Width"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad AxisBins. Obtiene o establece el ancho del contenedor de eje"
type: docs
url: /es/net/aspose.cells.charts/axisbins/width/
---
## AxisBins.Width property

Obtiene o establece el ancho del contenedor de eje.

```csharp
public double Width { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisBinsPropertyWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Datos de ejemplo
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["C1"].PutValue(20);
            worksheet.Cells["D1"].PutValue(15);
            worksheet.Cells["B2"].PutValue(35);
            worksheet.Cells["C2"].PutValue(32);
            worksheet.Cells["D2"].PutValue(31);

            // Crear gráfico de histograma
            int chartIndex = worksheet.Charts.Add(ChartType.Histogram, 7, 1, 25, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:D2", false);
            chart.NSeries.CategoryData = "B1:D1";

            // Establecer ancho del contenedor
            chart.CategoryAxis.Bins.Width = 12;

            // Guardar y demostrar el resultado
            workbook.Save("AxisBinsPropertyWidthDemo_out.xlsx");

            Console.WriteLine("Example executed successfully with bin width set to 12.");
        }
    }
}
```

### Ver también

* class [AxisBins](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


