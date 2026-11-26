---
title: "TickLabels.NumberFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TickLabels. Representa la cadena de formato para el objeto TickLabels"
type: docs
url: /es/net/aspose.cells.charts/ticklabels/numberformat/
---
## TickLabels.NumberFormat property

Representa la cadena de formato para el objeto TickLabels.

```csharp
public string NumberFormat { get; set; }
```

### Observaciones

La cadena de formato es la misma que una cadena de formato personalizado asignada a una celda. Por ejemplo, "$0".

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyNumberFormatDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(1.2345);
            worksheet.Cells["A3"].PutValue(2.3456);
            worksheet.Cells["A4"].PutValue(3.4567);

            // Crear un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer rango de datos del gráfico
            chart.NSeries.Add("A2:A4", true);

            // Establecer formato numérico para las etiquetas de marcas del eje de valores
            chart.ValueAxis.TickLabels.NumberFormat = "0.00";

            // Guarda el libro de trabajo
            workbook.Save("TickLabelsNumberFormatDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


