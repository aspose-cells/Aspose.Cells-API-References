---
title: "Chart.Walls"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Chart. Devuelve un objeto Walls que representa las paredes de un gráfico 3D"
type: docs
url: /es/net/aspose.cells.charts/chart/walls/
---
## Chart.Walls property

Devuelve un objeto `Walls` que representa las paredes de un gráfico 3-D.

```csharp
public Walls Walls { get; }
```

### Observaciones

Esta propiedad no se aplica a los gráficos de pastel 3-D.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPropertyWallsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(35);

            // Crear gráfico de columnas cilíndricas
            int chartIndex = worksheet.Charts.Add(ChartType.Cylinder, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Configurar conceptos básicos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            chart.IsRectangularCornered = true;
            chart.RotationAngle = 20;

            // Configurar propiedades de paredes
            Walls walls = chart.Walls;
            walls.BackgroundColor = Color.LightGray;
            walls.ForegroundColor = Color.Transparent;
            walls.FillFormat.SetPresetColorGradient(GradientPresetType.CalmWater, GradientStyleType.Horizontal, 1);

            // Guardar el resultado
            workbook.Save("ChartWallsDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [Walls](../../walls/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


