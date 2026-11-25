---
title: "ShadowEffect.Size"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ShadowEffect. Ottiene e imposta la dimensione dell'ombra. Intervallo da 0 a 2,0. Non ha senso nell'ombra interna"
type: docs
url: /it/net/aspose.cells.drawing/shadoweffect/size/
---
## ShadowEffect.Size property

Ottiene e imposta la dimensione dell'ombra. Intervallo da 0 a 2,0. Non ha senso nelle ombre interne.

```csharp
public double Size { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShadowEffectPropertySizeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook book = new Workbook();
            
            // Accedi al primo foglio di lavoro e aggiungi una forma
            Worksheet sheet = book.Worksheets[0];
            Shape shape = sheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Ottieni l'effetto ombra e imposta le proprietà, inclusa la Dimensione
            ShadowEffect shadow = shape.ShadowEffect;
            shadow.Angle = 150;
            shadow.Blur = 30;
            shadow.Size = 1.3; // Demonstrating Size property usage
            shadow.Transparency = 0.4;
            shadow.Distance = 80;

            // Salva la cartella di lavoro
            book.Save("ShadowEffectExample.xlsx");
            
            Console.WriteLine("Shadow effect with Size property set to 1.3 has been applied.");
        }
    }
}
```

### Vedi anche

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


