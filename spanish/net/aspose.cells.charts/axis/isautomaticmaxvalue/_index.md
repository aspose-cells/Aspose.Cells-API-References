---
title: "Axis.IsAutomaticMaxValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Axis. Indica si el valor máximo se asigna automáticamente"
type: docs
url: /es/net/aspose.cells.charts/axis/isautomaticmaxvalue/
---
## Axis.IsAutomaticMaxValue property

Indica si el valor máximo se asigna automáticamente.

```csharp
public bool IsAutomaticMaxValue { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyIsAutomaticMaxValueDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
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

            // Obtener el eje de valores
            Axis valueAxis = chart.ValueAxis;

            // Demostrar la propiedad IsAutomaticMaxValue
            Console.WriteLine("Initial IsAutomaticMaxValue: " + valueAxis.IsAutomaticMaxValue);
            Console.WriteLine("Initial MaxValue: " + valueAxis.MaxValue);

            // Desactivar el valor máximo automático y establecer un valor personalizado
            valueAxis.IsAutomaticMaxValue = false;
            valueAxis.MaxValue = 40;
            Console.WriteLine("After change - IsAutomaticMaxValue: " + valueAxis.IsAutomaticMaxValue);
            Console.WriteLine("After change - MaxValue: " + valueAxis.MaxValue);

            // Reactivar el valor máximo automático
            valueAxis.IsAutomaticMaxValue = true;
            Console.WriteLine("After re-enabling - IsAutomaticMaxValue: " + valueAxis.IsAutomaticMaxValue);
            Console.WriteLine("After re-enabling - MaxValue: " + valueAxis.MaxValue);

            // Guarda el libro de trabajo
            workbook.Save("AxisPropertyIsAutomaticMaxValueDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


