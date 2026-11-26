---
title: "Axis.MajorUnit"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Axis. Representa las unidades principales del eje"
type: docs
url: /es/net/aspose.cells.charts/axis/majorunit/
---
## Axis.MajorUnit property

Representa las unidades principales del eje.

```csharp
public double MajorUnit { get; set; }
```

### Observaciones

Las unidades principales deben ser mayores que cero.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyMajorUnitDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Cat " + i);
                worksheet.Cells["B" + (i + 1)].PutValue(i * 10);
            }

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B11", true);
            chart.NSeries.CategoryData = "A2:A11";

            // Obtener el eje de categoría
            Axis axis = chart.CategoryAxis;

            // Mostrar la unidad principal inicial
            Console.WriteLine("Initial Major Unit: " + axis.MajorUnit);

            // Establecer nueva unidad principal
            axis.MajorUnit = 3;
            Console.WriteLine("Modified Major Unit: " + axis.MajorUnit);

            // Guarda el libro de trabajo
            workbook.Save("AxisMajorUnitDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


