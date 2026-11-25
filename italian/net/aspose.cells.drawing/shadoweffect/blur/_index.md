---
title: "ShadowEffect.Blur"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ShadowEffect. Ottiene e imposta la sfocatura dell'ombra. Intervallo da 0 a 100 punti"
type: docs
url: /it/net/aspose.cells.drawing/shadoweffect/blur/
---
## ShadowEffect.Blur property

Ottiene e imposta la sfocatura dell'ombra. Intervallo da 0 a 100 punti.

```csharp
public double Blur { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShadowEffectPropertyBlurDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi una forma di esempio
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            
            // Ottieni l'effetto ombra
            ShadowEffect shadow = shape.ShadowEffect;
            
            // Imposta le proprietà dell'ombra, inclusa la Sfocatura
            shadow.Angle = 150;
            shadow.Blur = 30;
            shadow.Size = 1.3;
            shadow.Transparency = 0.4;
            shadow.Distance = 80;
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
            
            Console.WriteLine("Shadow effect with blur applied successfully.");
        }
    }
}
```

### Vedi anche

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


