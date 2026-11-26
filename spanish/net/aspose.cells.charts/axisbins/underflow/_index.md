---
title: "AxisBins.Underflow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad AxisBins. Obtiene o establece el subdesbordamiento de los contenedores de eje"
type: docs
url: /es/net/aspose.cells.charts/axisbins/underflow/
---
## AxisBins.Underflow property

Obtiene o establece el subdesbordamiento de los contenedores de eje

```csharp
public double Underflow { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisBinsPropertyUnderflowDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["C1"].PutValue(20);
            worksheet.Cells["D1"].PutValue(15);
            worksheet.Cells["B2"].PutValue(35);
            worksheet.Cells["C2"].PutValue(32);
            worksheet.Cells["D2"].PutValue(31);
            worksheet.Cells["B3"].PutValue(185);
            worksheet.Cells["C3"].PutValue(202);
            worksheet.Cells["D3"].PutValue(224);

            // Agregar gráfico de histograma
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Histogram, 7, 1, 25, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:D2", false);
            chart.NSeries.Add("B3:D3", false);
            chart.NSeries.CategoryData = "B1:D1";

            // Configurar propiedades de los contenedores
            var bins = chart.CategoryAxis.Bins;
            bins.Width = 12;
            bins.Count = 3;
            bins.Overflow = 10;
            bins.Underflow = 0.5; // Demonstrate Underflow property

            // Guarda el libro de trabajo
            workbook.Save("AxisBinsPropertyUnderflowDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [AxisBins](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


