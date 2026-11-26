---
title: "ShapePropertyCollection.Format3D"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "ShapePropertyCollection propiedad. Representa un objeto Format3D que especifica propiedades de forma 3D para el elemento o forma del gráfico"
type: docs
url: /es/net/aspose.cells.drawing/shapepropertycollection/format3d/
---
## ShapePropertyCollection.Format3D property

Representa un objeto `Format3D` que especifica propiedades de forma 3D para el elemento o forma del gráfico.

```csharp
public Format3D Format3D { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyCollectionPropertyFormat3DDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Sample 3D Chart");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);

            // Agregar gráfico de columnas 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:A4", false);

            // Acceder a las propiedades de forma de la serie
            Series series = chart.NSeries[0];
            ShapePropertyCollection shapeProperties = series.ShapeProperties;

            // Aplicar formato 3D
            Format3D format3D = shapeProperties.Format3D;
            format3D.SurfaceLightingType = LightRigType.BrightRoom;
            format3D.LightingAngle = 30;
            format3D.TopBevel.Type = BevelPresetType.ArtDeco;
            format3D.TopBevel.Height = 8;
            format3D.TopBevel.Width = 8;

            workbook.Save("Format3DDemo.xlsx");
            Console.WriteLine("3D formatting applied and saved to Format3DDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Format3D](../../format3d/)
* class [ShapePropertyCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


