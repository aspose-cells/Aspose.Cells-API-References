---
title: "TickLabels.IsAutomaticRotation"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TickLabels. Indica si el ángulo de rotación es automático"
type: docs
url: /es/net/aspose.cells.charts/ticklabels/isautomaticrotation/
---
## TickLabels.IsAutomaticRotation property

Indica si el ángulo de rotación es automático

```csharp
public bool IsAutomaticRotation { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyIsAutomaticRotationDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Agregar gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Configurar etiquetas de marcas
            TickLabels tickLabels = chart.ValueAxis.TickLabels;
            tickLabels.IsAutomaticRotation = false; // Disable automatic rotation
            tickLabels.RotationAngle = 45; // Set manual rotation angle

            workbook.Save("TickLabelsRotationDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


