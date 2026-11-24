---
title: "ShadowEffect.Blur"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShadowEffect-Eigenschaft. Gibt die Unschärfe des Schattens zurück und legt sie fest. Bereich von 0 bis 100 Punkten"
type: docs
url: /de/net/aspose.cells.drawing/shadoweffect/blur/
---
## ShadowEffect.Blur property

Liest und setzt die Unschärfe des Schattens. Bereich von 0 bis 100 Punkten.

```csharp
public double Blur { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Eine Beispiel-Form hinzufügen
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            
            // Hole den Schatteneffekt
            ShadowEffect shadow = shape.ShadowEffect;
            
            // Setze Schatteneigenschaften, einschließlich Unschärfe
            shadow.Angle = 150;
            shadow.Blur = 30;
            shadow.Size = 1.3;
            shadow.Transparency = 0.4;
            shadow.Distance = 80;
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
            
            Console.WriteLine("Shadow effect with blur applied successfully.");
        }
    }
}
```

### Siehe auch

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


