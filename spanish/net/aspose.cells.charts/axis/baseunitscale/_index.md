---
title: "Axis.BaseUnitScale"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad del eje. Representa la escala de unidad base para el eje de categorías"
type: docs
url: /es/net/aspose.cells.charts/axis/baseunitscale/
---
## Axis.BaseUnitScale property

Representa la escala de unidad base para el eje de categoría.

```csharp
public TimeUnit BaseUnitScale { get; set; }
```

### Observaciones

Solo tiene efecto cuando la propiedad CategoryType está configurada a TimeScale.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyBaseUnitScaleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells[$"A{i}"].PutValue(DateTime.Now.AddDays(i));
                sheet.Cells[$"B{i}"].PutValue(i * 100);
            }

            // Añade un gráfico
            int chartIndex = sheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B10", true);
            chart.NSeries.CategoryData = "A2:A10";

            // Establecer la escala de unidad base para el eje de categorías
            chart.CategoryAxis.BaseUnitScale = TimeUnit.Months;

            // Guarda el libro de trabajo
            workbook.Save("AxisPropertyBaseUnitScaleDemo_out.xlsx");
        }
    }
}
```

### Ver también

* enum [TimeUnit](../../timeunit/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


