---
title: "Axis.MinorGridLines"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Axis. Representa líneas de cuadrícula menores en el eje de un gráfico"
type: docs
url: /es/net/aspose.cells.charts/axis/minorgridlines/
---
## Axis.MinorGridLines property

Representa las líneas de cuadrícula menores en el eje de un gráfico.

```csharp
public Line MinorGridLines { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyMinorGridLinesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
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
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Habilitar líneas de cuadrícula mayores y menores para el eje de valores
            chart.ValueAxis.MajorGridLines.IsVisible = true;
            chart.ValueAxis.MinorGridLines.IsVisible = true;
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Line](../../../aspose.cells.drawing/line/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


