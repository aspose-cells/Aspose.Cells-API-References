---
title: "Axis.MinValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Axis. Representa el valor mínimo en el eje de valores"
type: docs
url: /es/net/aspose.cells.charts/axis/minvalue/
---
## Axis.MinValue property

Representa el valor mínimo en el eje de valores.

```csharp
public object MinValue { get; set; }
```

### Observaciones

El tipo minValue solo puede ser double o DateTime

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyMinValueDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceda a la primera hoja de cálculo y agregue datos de muestra
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["B1"].PutValue(40);
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(60);

            // Agregar un gráfico y establecer el rango de datos
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 5, 15, 15);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B3", false);

            // Configurar propiedades del eje de valores
            chart.ValueAxis.MinValue = 15;  // Setting minimum value
            chart.ValueAxis.MaxValue = 70;
            chart.ValueAxis.MajorUnit = 10;

            // Guarda el libro de trabajo
            workbook.Save("AxisMinValueDemo.xlsx");

            Console.WriteLine("Chart created with MinValue set to 15.");
        }
    }
}
```

### Ver también

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


