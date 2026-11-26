---
title: "Axis.MinorUnitScale"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Axis. Representa la escala de unidad mayor para el eje de categorías"
type: docs
url: /es/net/aspose.cells.charts/axis/minorunitscale/
---
## Axis.MinorUnitScale property

Representa la escala de unidad principal para el eje de categorías.

```csharp
public TimeUnit MinorUnitScale { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyMinorUnitScaleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra basados en tiempo
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells[$"A{i}"].PutValue(DateTime.Now.AddMonths(i - 2));
                worksheet.Cells[$"B{i}"].PutValue(i * 100);
            }

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B10", true);
            chart.NSeries.CategoryData = "A2:A10";

            // Configurar el eje de categorías como escala de tiempo
            chart.CategoryAxis.CategoryType = CategoryType.TimeScale;
            chart.CategoryAxis.MinorUnitScale = TimeUnit.Months;
            chart.CategoryAxis.MinorUnit = 2;

            // Guarda el libro de trabajo
            workbook.Save("AxisPropertyMinorUnitScaleDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [TimeUnit](../../timeunit/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


