---
title: "Axis.MajorTickMark"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Axis. Representa el tipo de marca de graduación mayor para el eje especificado"
type: docs
url: /es/net/aspose.cells.charts/axis/majortickmark/
---
## Axis.MajorTickMark property

Representa el tipo de marca de graduación principal para el eje especificado.

```csharp
public TickMarkType MajorTickMark { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyMajorTickMarkDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Agregar un gráfico de columnas
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];

            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Establecer el tipo de marca de graduación mayor a exterior
            chart.ValueAxis.MajorTickMark = TickMarkType.Outside;

            // Guarda el libro de trabajo
            workbook.Save("AxisPropertyMajorTickMarkDemo_out.xlsx");
        }
    }
}
```

### Ver también

* enum [TickMarkType](../../tickmarktype/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


