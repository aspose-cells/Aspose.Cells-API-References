---
title: "GradientStopCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad GradientStopCollection. Obtiene la parada de degradado por el índice"
type: docs
url: /es/net/aspose.cells.drawing/gradientstopcollection/item/
---
## GradientStopCollection indexer

Obtiene la parada de degradado por el índice.

```csharp
public GradientStop this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice. |

### Valor de retorno

La parada de degradado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class GradientStopCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;
            shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            Shape shape = shapes[0];

            shape.Fill.FillType = FillType.Gradient;
            shape.Fill.GradientFill.SetPresetThemeGradient(PresetThemeGradientType.BottomSpotlight, ThemeColorType.Accent5);
            
            // Demostrar el uso de la propiedad Item
            GradientStop stop = shape.Fill.GradientFill.GradientStops[1];
            Console.WriteLine("Gradient stop position: " + stop.Position);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [GradientStop](../../gradientstop/)
* class [GradientStopCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


