---
title: "Enum AxisType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Charts.AxisType enum. Representa el tipo de eje"
type: docs
url: /es/net/aspose.cells.charts/axistype/
---
## AxisType enumeration

Representa el tipo de eje.

```csharp
public enum AxisType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Category | `0` | Eje de categoría |
| Value | `1` | Eje de valores |
| Series | `2` | Eje de series |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class AxisTypeDemo
    {
        public static void AxisTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer el rango de datos del gráfico
            chart.SetChartDataRange("A1:B4", true);

            // Determina qué ejes existen en el gráfico
            bool hasPrimaryCategoryAxis = chart.HasAxis(AxisType.Category, true);
            bool hasSecondaryCategoryAxis = chart.HasAxis(AxisType.Category, false);
            bool hasPrimaryValueAxis = chart.HasAxis(AxisType.Value, true);
            bool hasSecondaryValueAxis = chart.HasAxis(AxisType.Value, false);

            // Genere la salida de los resultados
            Console.WriteLine("Has Primary Category Axis: " + hasPrimaryCategoryAxis);
            Console.WriteLine("Has Secondary Category Axis: " + hasSecondaryCategoryAxis);
            Console.WriteLine("Has Primary Value Axis: " + hasPrimaryValueAxis);
            Console.WriteLine("Has Secondary Value Axis: " + hasSecondaryValueAxis);

            // Guarda el libro de trabajo
            workbook.Save("AxisTypeExample.xlsx");
            workbook.Save("AxisTypeExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


