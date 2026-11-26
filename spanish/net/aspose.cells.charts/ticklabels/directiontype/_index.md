---
title: "TickLabels.DirectionType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TickLabels. Obtiene y establece la dirección del texto"
type: docs
url: /es/net/aspose.cells.charts/ticklabels/directiontype/
---
## TickLabels.DirectionType property

Obtiene y establece la dirección del texto.

```csharp
public ChartTextDirectionType DirectionType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyDirectionTypeDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].Value = 50;
            worksheet.Cells["A2"].Value = 100;
            worksheet.Cells["A3"].Value = 150;
            worksheet.Cells["A4"].Value = 200;
            worksheet.Cells["B1"].Value = 60;
            worksheet.Cells["B2"].Value = 32;
            worksheet.Cells["B3"].Value = 50;
            worksheet.Cells["B4"].Value = 40;
            worksheet.Cells["C1"].Value = "清华";
            worksheet.Cells["C2"].Value = "北大";
            worksheet.Cells["C3"].Value = "人大";
            worksheet.Cells["C4"].Value = "科大";

            // Agregar gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer datos del gráfico
            chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";

            // Establecer la dirección de las etiquetas de tick a vertical
            chart.CategoryAxis.TickLabels.DirectionType = ChartTextDirectionType.Vertical;

            // Guarda el libro de trabajo
            workbook.Save("TickLabelsDirectionTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [ChartTextDirectionType](../../charttextdirectiontype/)
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


