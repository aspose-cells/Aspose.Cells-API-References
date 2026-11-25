---
title: "ShadowEffect.Distance"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ShadowEffect. Ottiene e imposta la distanza dell'ombra. Intervallo da 0 a 200 punti"
type: docs
url: /it/net/aspose.cells.drawing/shadoweffect/distance/
---
## ShadowEffect.Distance property

Ottiene e imposta la distanza dell'ombra. Intervallo da 0 a 200 punti.

```csharp
public double Distance { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShadowEffectPropertyDistanceDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare
            RectangleShape rectangle = worksheet.Shapes.AddRectangle(2, 0, 2, 0, 150, 100);
            
            // Configura l'effetto ombra
            ShadowEffect shadow = rectangle.ShadowEffect;
            shadow.PresetType = PresetShadowType.OffsetDiagonalTopRight;
            
            // Crea un oggetto CellsColor e imposta i valori ARGB
            CellsColor color = workbook.CreateCellsColor();
            color.Argb = (128 << 24) | (255 << 16) | (0 << 8) | 0; // Semi-transparent red
            shadow.Color = color;
            
            shadow.Transparency = 0.3;
            shadow.Blur = 15;
            shadow.Angle = 45;
            shadow.Distance = 20; // Set distance to 20 points

            // Visualizza la distanza dell'ombra
            Console.WriteLine("Shadow Distance: " + shadow.Distance + " points");

            // Salva la cartella di lavoro con l'effetto ombra
            workbook.Save("ShadowEffectPropertyDistanceDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


