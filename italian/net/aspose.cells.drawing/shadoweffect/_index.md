---
title: "Class ShadowEffect"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.ShadowEffect class. Questa classe specifica l'effetto di ombra dell'elemento grafico o della forma"
type: docs
url: /it/net/aspose.cells.drawing/shadoweffect/
---
## ShadowEffect class

Questa classe specifica l'effetto ombra dell'elemento del grafico o della forma.

```csharp
public class ShadowEffect
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Angle](../../aspose.cells.drawing/shadoweffect/angle/) { get; set; } | Ottiene e imposta l'angolo di illuminazione. Intervallo da 0 a 359,9 gradi. |
| [Blur](../../aspose.cells.drawing/shadoweffect/blur/) { get; set; } | Ottiene e imposta la sfocatura dell'ombra. Intervallo da 0 a 100 punti. |
| [Color](../../aspose.cells.drawing/shadoweffect/color/) { get; set; } | Ottiene e imposta il colore dell'ombra. |
| [Distance](../../aspose.cells.drawing/shadoweffect/distance/) { get; set; } | Ottiene e imposta la distanza dell'ombra. Intervallo da 0 a 200 punti. |
| [PresetType](../../aspose.cells.drawing/shadoweffect/presettype/) { get; set; } | Ottiene e imposta il tipo di ombra predefinito dell'ombra. |
| [Size](../../aspose.cells.drawing/shadoweffect/size/) { get; set; } | Ottiene e imposta la dimensione dell'ombra. Intervallo da 0 a 2,0. Non ha senso nelle ombre interne. |
| [Transparency](../../aspose.cells.drawing/shadoweffect/transparency/) { get; set; } | Ottiene e imposta il grado di trasparenza dell'ombra. Intervallo da 0,0 (opaco) a 1,0 (trasparente). |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassShadowEffectDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma di esempio con tutti i parametri richiesti
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 100);

            // Ottieni l'effetto ombra della forma
            ShadowEffect shadow = shape.ShadowEffect;

            // Imposta le proprietà dell'ombra
            shadow.Angle = 150;
            shadow.Blur = 30;
            shadow.Size = 1.3;
            shadow.Transparency = 0.4;
            shadow.Distance = 80;

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");

            Console.WriteLine("Shadow effect demo completed successfully.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


