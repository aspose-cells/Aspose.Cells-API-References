---
title: "Axis.CrossAt"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Axis. Representa el punto en el eje de valores donde el eje de categorías lo cruza"
type: docs
url: /es/net/aspose.cells.charts/axis/crossat/
---
## Axis.CrossAt property

Representa el punto en el eje de valores donde el eje de categorías lo cruza.

```csharp
public double CrossAt { get; set; }
```

### Observaciones

El número debe ser un entero cuando se aplica al eje de categorías. Y el valor debe estar entre 1 y 31999.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyCrossAtDemo
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
            worksheet.Cells["A5"].PutValue("D");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Configurar eje de valores
            chart.ValueAxis.CrossAt = 15; // Cross at value 15
            chart.ValueAxis.MinValue = 0;
            chart.ValueAxis.MaxValue = 50;

            // Configurar eje de categorías
            chart.CategoryAxis.CrossAt = 2.5; // Cross between categories B and C
            chart.CategoryAxis.TickLabelPosition = Aspose.Cells.Charts.TickLabelPositionType.Low;

            // Guarda el libro de trabajo
            workbook.Save("AxisCrossAtDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


