---
title: "Axis.IsLogarithmic"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Axis. Representa si el tipo de escala del eje de valores es logarítmico o no"
type: docs
url: /es/net/aspose.cells.charts/axis/islogarithmic/
---
## Axis.IsLogarithmic property

Representa si el tipo de escala del eje de valores es logarítmico o no.

```csharp
public bool IsLogarithmic { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyIsLogarithmicDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(100);
            worksheet.Cells["A4"].PutValue(1000);
            worksheet.Cells["B1"].PutValue(5);
            worksheet.Cells["B2"].PutValue(25);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(100);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Agregar serie
            chart.NSeries.Add("A1:A4", true);
            chart.NSeries[0].Values = "B1:B4";

            // Configurar eje logarítmico
            chart.CategoryAxis.IsLogarithmic = true;
            chart.CategoryAxis.LogBase = 10;
            chart.CategoryAxis.MinValue = 1;
            chart.CategoryAxis.MaxValue = 10000;

            // Guarda el libro de trabajo
            workbook.Save("AxisPropertyIsLogarithmicDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


