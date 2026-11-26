---
title: "Chart.Perspective"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Chart. Devuelve o establece la perspectiva para la vista del gráfico tridimensional. Debe estar entre 0 y 100. Esta propiedad se ignora si la propiedad RightAngleAxes es True"
type: docs
url: /es/net/aspose.cells.charts/chart/perspective/
---
## Chart.Perspective property

Devuelve o establece la perspectiva para la vista del gráfico tridimensional. Debe estar entre 0 y 100. Esta propiedad se ignora si la propiedad RightAngleAxes es True.

```csharp
public short Perspective { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyPerspectiveDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Agregar un gráfico de columnas 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Establecer propiedades de perspectiva del gráfico 3D
            chart.Perspective = 30; // Perspective angle (0-100)
            chart.RotationAngle = 15; // Rotation angle
            chart.Elevation = 20; // Elevation angle
            chart.RightAngleAxes = false; // Enable perspective projection
            chart.AutoScaling = true; // Auto scale the chart

            // Guarda el libro de trabajo
            workbook.Save("ChartPerspectiveDemo.xlsx");

            Console.WriteLine("Chart with perspective settings created successfully.");
        }
    }
}
```

### Ver también

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


