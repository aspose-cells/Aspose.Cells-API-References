---
title: "TickLabels.ReadingOrder"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TickLabels. Representa el orden de lectura del texto"
type: docs
url: /es/net/aspose.cells.charts/ticklabels/readingorder/
---
## TickLabels.ReadingOrder property

Representa el orden de lectura del texto.

```csharp
public TextDirectionType ReadingOrder { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyReadingOrderDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);

            // Establecer el orden de lectura de las etiquetas de marcas
            TickLabels tickLabels = chart.ValueAxis.TickLabels;
            tickLabels.ReadingOrder = TextDirectionType.RightToLeft;

            // Guarda el libro de trabajo
            workbook.Save("TickLabelsReadingOrderDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [TextDirectionType](../../../aspose.cells/textdirectiontype/)
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


