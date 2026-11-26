---
title: "ChartTextFrame.TextDirection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartTextFrame. Representa el orden de lectura del texto"
type: docs
url: /es/net/aspose.cells.charts/charttextframe/textdirection/
---
## ChartTextFrame.TextDirection property

Representa el orden de lectura del texto.

```csharp
[Obsolete("Use ChartTextFrame.ReadingOrder property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public TextDirectionType TextDirection { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use la propiedad ChartTextFrame.ReadingOrder. Esta propiedad será eliminada 12 meses después desde marzo de 2020. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyTextDirectionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Configurar datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Configurar etiquetas de datos
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            dataLabels.ShowValue = true;
            
            // Demostrar la propiedad TextDirection
            dataLabels.TextDirection = TextDirectionType.LeftToRight;

            // Guarda el libro de trabajo
            workbook.Save("ChartTextDirectionDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [TextDirectionType](../../../aspose.cells/textdirectiontype/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


