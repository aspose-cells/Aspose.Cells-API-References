---
title: "Axis.CustomDisplayUnit"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Axis. Especifica un valor personalizado para la unidad de visualización"
type: docs
url: /es/net/aspose.cells.charts/axis/customdisplayunit/
---
## Axis.CustomDisplayUnit property

Especifica un valor personalizado para la unidad de visualización.

```csharp
public double CustomDisplayUnit { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyCustomDisplayUnitDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10000000);
            worksheet.Cells["B3"].PutValue(20000000);
            worksheet.Cells["B4"].PutValue(30000000);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Establecer unidad de visualización personalizada para el eje de valores
            chart.ValueAxis.CustomDisplayUnit = 1.0E7;
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Custom;
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


