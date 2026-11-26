---
title: "Axis.CrossType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Axis. Representa el CrossType en el eje especificado donde cruza el otro eje"
type: docs
url: /es/net/aspose.cells.charts/axis/crosstype/
---
## Axis.CrossType property

Representa el `CrossType` en el eje especificado donde cruza el otro eje.

```csharp
public CrossType CrossType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyCrossTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Crear gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Configurar eje de valores
            chart.ValueAxis.MaxValue = 200;
            chart.ValueAxis.MinValue = 0;
            chart.ValueAxis.MajorUnit = 25;
            
            // Demostrar la propiedad CrossType
            chart.ValueAxis.CrossType = CrossType.Maximum;

            workbook.Save("AxisPropertyCrossTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [CrossType](../../crosstype/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


