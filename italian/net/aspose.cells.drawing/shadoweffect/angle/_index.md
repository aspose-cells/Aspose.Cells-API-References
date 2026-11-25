---
title: "ShadowEffect.Angle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ShadowEffect. Ottiene e imposta l'angolo di illuminazione. Intervallo da 0 a 359,9 gradi"
type: docs
url: /it/net/aspose.cells.drawing/shadoweffect/angle/
---
## ShadowEffect.Angle property

Ottiene e imposta l'angolo di illuminazione. Intervallo da 0 a 359,9 gradi.

```csharp
public double Angle { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShadowEffectPropertyAngleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma e imposta l'angolo dell'effetto ombra
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
            shape.ShadowEffect.Angle = 45;

            // Verifica e visualizza il valore dell'angolo
            Console.WriteLine("Shadow Effect Angle: " + shape.ShadowEffect.Angle);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


