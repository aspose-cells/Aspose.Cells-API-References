---
title: "Walls.CenterY"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Walls. Obtiene la coordenada y de la esquina inferior izquierda del centro de la pared en unidades de 1/4000 de la altura del gráfico después de llamar al método Chart.Calculate."
type: docs
url: /es/net/aspose.cells.charts/walls/centery/
---
## Walls.CenterY property

Obtiene la coordenada y de la esquina inferior izquierda del centro de la pared en unidades de 1/4000 de la altura del gráfico después de llamar al método Chart.Calculate().

```csharp
public int CenterY { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class WallsPropertyCenterYDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Agregar un gráfico 3D
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column3D, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcule el gráfico para actualizar las propiedades.
            chart.Calculate();

            // Acceda a walls y demuestre la propiedad CenterY.
            Aspose.Cells.Charts.Walls walls = chart.Walls;
            Console.WriteLine("Wall CenterY position: " + walls.CenterY);

            // Guarda el libro de trabajo
            workbook.Save("WallsCenterYDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


