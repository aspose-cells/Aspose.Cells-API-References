---
title: "GradientStopCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà GradientStopCollection. Ottiene la fermata di gradiente per indice"
type: docs
url: /it/net/aspose.cells.drawing/gradientstopcollection/item/
---
## GradientStopCollection indexer

Ottiene la fermata del gradiente per indice.

```csharp
public GradientStop this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice. |

### Valore di ritorno

La fermata di gradiente.

### Esempi

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
            
            // Dimostra l'uso della proprietà Item
            GradientStop stop = shape.Fill.GradientFill.GradientStops[1];
            Console.WriteLine("Gradient stop position: " + stop.Position);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [GradientStop](../../gradientstop/)
* class [GradientStopCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


