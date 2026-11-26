---
title: "TickLabels.TextDirection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TickLabels. Representa el orden de lectura del texto"
type: docs
url: /es/net/aspose.cells.charts/ticklabels/textdirection/
---
## TickLabels.TextDirection property

Representa el orden de lectura del texto.

```csharp
[Obsolete("Use TickLabels.ReadingOrder property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public TextDirectionType TextDirection { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad TickLabels.ReadingOrder. Esta propiedad será eliminada 12 meses después desde marzo de 2020. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyTextDirectionDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Configurar la dirección del texto de las etiquetas de marcas
            Axis valueAxis = chart.ValueAxis;
            TickLabels tickLabels = valueAxis.TickLabels;
            tickLabels.TextDirection = TextDirectionType.LeftToRight;

            workbook.Save("TickLabelsTextDirectionDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [TextDirectionType](../../../aspose.cells/textdirectiontype/)
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


