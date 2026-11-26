---
title: "TickLabels.Number"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TickLabels. Representa el número de formato para el objeto TickLabels"
type: docs
url: /es/net/aspose.cells.charts/ticklabels/number/
---
## TickLabels.Number property

Representa el número de formato para el objeto TickLabels.

```csharp
public int Number { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyNumberDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);

            // Configurar etiquetas de marcas
            TickLabels tickLabels = chart.ValueAxis.TickLabels;
            tickLabels.Number = 2; // Demonstrate Number property
            tickLabels.NumberFormat = "0.00";

            // Guarda el libro de trabajo
            workbook.Save("TickLabelsNumberDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


