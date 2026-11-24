---
title: "ShadowEffect.Transparency"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShadowEffect-Eigenschaft. Gibt den Transparenzgrad des Schattens zurück oder legt ihn fest. Bereich von 0,0 (undurchsichtig) bis 1,0 (transparent)"
type: docs
url: /de/net/aspose.cells.drawing/shadoweffect/transparency/
---
## ShadowEffect.Transparency property

Liest und setzt den Transparenzgrad des Schattens. Bereich von 0,0 (undurchsichtig) bis 1,0 (transparent).

```csharp
public double Transparency { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge eine Form hinzu, um den Schatteneffekt zu demonstrieren
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            
            // Hole den Schatteneffekt und setze Eigenschaften, einschließlich Transparenz
            ShadowEffect shadow = shape.ShadowEffect;
            shadow.Angle = 150;
            shadow.Blur = 30;
            shadow.Size = 1.3;
            shadow.Transparency = 0.4; // Setting transparency to 40%
            shadow.Distance = 80;
            
            // Speichere die Arbeitsmappe
            workbook.Save("ShadowEffectDemo.xlsx");
            
            Console.WriteLine("Workbook saved with shadow effect transparency set to 0.4");
        }
    }
}
```

### Siehe auch

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


