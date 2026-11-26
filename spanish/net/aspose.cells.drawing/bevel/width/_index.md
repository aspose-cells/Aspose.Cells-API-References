---
title: "Bevel.Width"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Bevel. Obtiene y establece el ancho del bisel o qué tan profundo en la forma se aplica. En unidades de puntos"
type: docs
url: /es/net/aspose.cells.drawing/bevel/width/
---
## Bevel.Width property

Obtiene y establece el ancho del bisel, o cuán lejos dentro de la forma se aplica. En unidades de puntos.

```csharp
public double Width { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class BevelPropertyWidthDemo
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

            // Agregar gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 5, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Obtener la primera serie y establecer el formato 3D
            Series series = chart.NSeries[0];
            Format3D format3D = series.ShapeProperties.Format3D;
            
            // Configurar propiedades del bisel con demostración de Width
            Bevel topBevel = format3D.TopBevel;
            topBevel.Type = BevelPresetType.Circle;
            topBevel.Width = 12; // Demonstrating Width property
            topBevel.Height = 6;

            // Guarda el libro de trabajo
            workbook.Save("BevelWidthDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Bevel](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


