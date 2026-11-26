---
title: "Enumeración PageLayoutAlignmentType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.PageLayoutAlignmentType enum. Enumera los tipos de alineación del diseño de página"
type: docs
url: /es/net/aspose.cells/pagelayoutalignmenttype/
---
## PageLayoutAlignmentType enumeration

Enumera los tipos de alineación del diseño de página.

```csharp
public enum PageLayoutAlignmentType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Bottom | `0` | Representa la alineación inferior del diseño de página. |
| Center | `1` | Representa la alineación central del diseño de página. |
| Left | `2` | Representa la alineación izquierda del diseño de página. |
| Right | `3` | Representa la alineación derecha del diseño de página. |
| Top | `4` | Representa la alineación superior del diseño de página. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PageLayoutAlignmentTypeDemo
    {
        public static void PageLayoutAlignmentTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(456);
            worksheet.Cells["A4"].PutValue(789);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Establecer el rango de datos para el gráfico
            chart.SetChartDataRange("A1:A4", true);

            // Establecer el título del gráfico
            chart.Title.Text = "Sample Chart";

            // Guardar el libro de trabajo en un archivo
            workbook.Save("PageLayoutAlignmentTypeExample.xlsx");

            // Exportar el gráfico a PDF con una alineación de diseño de página específica
            chart.ToPdf("ChartExample.pdf", 8.5f, 11f, PageLayoutAlignmentType.Center, PageLayoutAlignmentType.Center);

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


