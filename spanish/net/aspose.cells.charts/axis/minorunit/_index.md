---
title: "Axis.MinorUnit"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Axis. Representa las unidades menores del eje"
type: docs
url: /es/net/aspose.cells.charts/axis/minorunit/
---
## Axis.MinorUnit property

Representa las unidades menores del eje.

```csharp
public double MinorUnit { get; set; }
```

### Observaciones

Las unidades menores deben ser mayores que cero.

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyMinorUnitDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Agregar datos de ejemplo
            cells["A1"].PutValue("Region");
            cells["A2"].PutValue("France");
            cells["A3"].PutValue("Germany");
            cells["A4"].PutValue("England");
            cells["B1"].PutValue("Sales");
            cells["B2"].PutValue(70000);
            cells["B3"].PutValue(55000);
            cells["B4"].PutValue(30000);

            // Crear gráfico
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 1, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // Configurar datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Configurar eje de valores
            chart.ValueAxis.Title.Text = "Sales Amount";
            chart.ValueAxis.MajorUnit = 20000;
            chart.ValueAxis.MinorUnit = 5000; // Demonstrate MinorUnit property
            chart.ValueAxis.MinValue = 0;
            chart.ValueAxis.MaxValue = 80000;

            // Guarda el libro de trabajo
            workbook.Save("AxisPropertyMinorUnitDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


