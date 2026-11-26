---
title: "Enum TimeUnit"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Charts.TimeUnit enum. Representa la unidad base para el eje de categoría"
type: docs
url: /es/net/aspose.cells.charts/timeunit/
---
## TimeUnit enumeration

Representa la unidad base para el eje de categorías.

```csharp
public enum TimeUnit
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Days | `0` | Días |
| Months | `1` | Meses |
| Years | `2` | Años |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TimeUnitDemo
    {
        public static void TimeUnitExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            // Agregar una nueva hoja de trabajo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].PutValue(new DateTime(2023, 1, 1));
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 2, 1));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 3, 1));
            worksheet.Cells["B1"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["B3"].PutValue(300);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 25, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Agregar series al gráfico
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Establece el eje de categoría para usar unidades de tiempo
            Axis categoryAxis = chart.CategoryAxis;
            categoryAxis.CategoryType = CategoryType.TimeScale;
            categoryAxis.BaseUnitScale = TimeUnit.Months;
            categoryAxis.MajorUnitScale = TimeUnit.Months;
            categoryAxis.MinorUnitScale = TimeUnit.Days;

            // Personaliza la apariencia del gráfico
            chart.Title.Text = "Sample Chart with Time Units";
            chart.ValueAxis.Title.Text = "Values";
            chart.CategoryAxis.Title.Text = "Dates";

            // Guarda el libro de trabajo
            workbook.Save("TimeUnitExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


