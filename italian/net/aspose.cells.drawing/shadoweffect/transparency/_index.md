---
title: "ShadowEffect.Transparency"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ShadowEffect. Ottiene e imposta il grado di trasparenza dell'ombra. Intervallo da 0,0 opaco a 1,0 trasparente"
type: docs
url: /it/net/aspose.cells.drawing/shadoweffect/transparency/
---
## ShadowEffect.Transparency property

Ottiene e imposta il grado di trasparenza dell'ombra. Intervallo da 0,0 (opaco) a 1,0 (trasparente).

```csharp
public double Transparency { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShadowEffectPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi una forma per dimostrare l'effetto ombra
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            
            // Ottieni l'effetto ombra e imposta le proprietà, inclusa la Trasparenza
            ShadowEffect shadow = shape.ShadowEffect;
            shadow.Angle = 150;
            shadow.Blur = 30;
            shadow.Size = 1.3;
            shadow.Transparency = 0.4; // Setting transparency to 40%
            shadow.Distance = 80;
            
            // Salva la cartella di lavoro
            workbook.Save("ShadowEffectDemo.xlsx");
            
            Console.WriteLine("Workbook saved with shadow effect transparency set to 0.4");
        }
    }
}
```

### Vedi anche

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


