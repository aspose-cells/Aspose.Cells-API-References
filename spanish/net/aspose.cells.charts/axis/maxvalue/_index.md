---
title: "Axis.MaxValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Axis. Representa el valor máximo en el eje de valores"
type: docs
url: /es/net/aspose.cells.charts/axis/maxvalue/
---
## Axis.MaxValue property

Representa el valor máximo en el eje de valores.

```csharp
public object MaxValue { get; set; }
```

### Observaciones

El tipo maxValue solo puede ser double o DateTime

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyMaxValueDemo
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
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(50);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Establecer el valor máximo del eje de valores
            chart.ValueAxis.MaxValue = 60;

            // Guarda el libro de trabajo
            workbook.Save("AxisPropertyMaxValueDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


