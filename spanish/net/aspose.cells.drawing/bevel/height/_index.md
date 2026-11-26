---
title: "Bevel.Height"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Bevel. Obtiene y establece la altura del bisel o qué tan alto sobre la forma se aplica. En unidades de puntos"
type: docs
url: /es/net/aspose.cells.drawing/bevel/height/
---
## Bevel.Height property

Obtiene y establece la altura del bisel, o cuán lejos sobre la forma se aplica. En unidades de puntos.

```csharp
public double Height { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class BevelPropertyHeightDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(1500);

            // Agregar un gráfico de columnas 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Acceder al formato 3D del área del gráfico
            Format3D format3D = chart.PlotArea.ShapeProperties.Format3D;

            // Configurar el bisel superior con la propiedad Height
            Bevel topBevel = format3D.TopBevel;
            topBevel.Type = BevelPresetType.ArtDeco;
            topBevel.Width = 8;
            topBevel.Height = 4.5; // Demonstrating Height property usage

            // Guarda el libro de trabajo
            workbook.Save("BevelHeightDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Bevel](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


