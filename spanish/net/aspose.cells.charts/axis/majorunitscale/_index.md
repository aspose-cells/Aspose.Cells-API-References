---
title: "Axis.MajorUnitScale"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Axis. Representa la escala de unidad mayor para el eje de categorías"
type: docs
url: /es/net/aspose.cells.charts/axis/majorunitscale/
---
## Axis.MajorUnitScale property

Representa la escala de unidad principal para el eje de categorías.

```csharp
public TimeUnit MajorUnitScale { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyMajorUnitScaleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra de escala de tiempo
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 3, 1));
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 5, 1));
            worksheet.Cells["B4"].PutValue(30);
            
            // Crear gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);
            
            // Configurar el eje de categorías como escala de tiempo con unidad mayor cada 2 meses
            chart.CategoryAxis.CategoryType = CategoryType.TimeScale;
            chart.CategoryAxis.MajorUnitScale = TimeUnit.Months;
            chart.CategoryAxis.MajorUnit = 2;
            
            workbook.Save("AxisPropertyMajorUnitScaleDemo_out.xlsx");
        }
    }
}
```

### Ver también

* enum [TimeUnit](../../timeunit/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


