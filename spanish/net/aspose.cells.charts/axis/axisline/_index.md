---
title: "Axis.AxisLine"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Axis. Obtiene la apariencia de un eje"
type: docs
url: /es/net/aspose.cells.charts/axis/axisline/
---
## Axis.AxisLine property

Obtiene la apariencia de un eje.

```csharp
public Line AxisLine { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AxisPropertyAxisLineDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Acceder al eje de valores
            Axis valueAxis = chart.ValueAxis;

            // Personalizar las propiedades de la línea del eje
            valueAxis.AxisLine.Color = Color.Red;
            valueAxis.AxisLine.Style = LineType.DashDot;
            valueAxis.AxisLine.Weight = WeightType.MediumLine;

            // Guarda el libro de trabajo
            workbook.Save("AxisLineDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Line](../../../aspose.cells.drawing/line/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


