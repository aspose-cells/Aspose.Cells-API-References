---
title: "Walls.Height"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Walls. Obtiene la altura de arriba a abajo en unidades de 1/4000 de la altura del gráfico después de llamar al método Chart.Calculate."
type: docs
url: /es/net/aspose.cells.charts/walls/height/
---
## Walls.Height property

Obtiene la altura de arriba a abajo en unidades de 1/4000 de la altura del gráfico después de llamar al método Chart.Calculate().

```csharp
public int Height { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class WallsPropertyHeightDemo
    {
        public static void Run()
        {
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

            // Agregar gráfico 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            chart.Calculate();

            // Acceda a walls y demuestre la propiedad Height.
            Walls walls = chart.Walls;
            Console.WriteLine("Wall Height: " + walls.Height);
            Console.WriteLine("Wall Height in Pixels: " + walls.HeightPx);

            // Modifique el tamaño del área del gráfico en lugar de la propiedad Height directa.
            chart.ChartObject.Height = 400;
            chart.Calculate();
            Console.WriteLine("After resizing - Wall Height: " + walls.Height);
            Console.WriteLine("After resizing - Wall Height in Pixels: " + walls.HeightPx);

            workbook.Save("WallsHeightDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


