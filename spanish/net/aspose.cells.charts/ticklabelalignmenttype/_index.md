---
title: "Enumeración TickLabelAlignmentType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Charts.TickLabelAlignmentType enum. Representa el tipo de alineación de texto para las etiquetas de marcas en el eje"
type: docs
url: /es/net/aspose.cells.charts/ticklabelalignmenttype/
---
## TickLabelAlignmentType enumeration

Representa el tipo de alineación de texto para las etiquetas de marcas de graduación en el eje

```csharp
public enum TickLabelAlignmentType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Center | `0` | Especifica que el texto está centrado. |
| Left | `1` | Especifica que el texto está alineado a la izquierda. |
| Right | `2` | Especifica que el texto está alineado a la derecha.. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TickLabelAlignmentTypeDemo
    {
        public static void TickLabelAlignmentTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Agregar series al gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Acceder a las etiquetas de marcas del eje de categorías
            TickLabels tickLabels = chart.CategoryAxis.TickLabels;

            // Establecer el tipo de alineación para las etiquetas de marcas
            tickLabels.AlignmentType = TickLabelAlignmentType.Center;

            // Guarda el libro de trabajo
            workbook.Save("TickLabelAlignmentTypeExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


