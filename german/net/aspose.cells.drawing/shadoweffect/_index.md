---
title: "Klasse ShadowEffect"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.ShadowEffect Klasse. Diese Klasse gibt den Schatteneffekt des Diagrammelements oder der Form an."
type: docs
url: /de/net/aspose.cells.drawing/shadoweffect/
---
## ShadowEffect class

Diese Klasse gibt den Schatteneffekt des Diagrammelements oder der Form an.

```csharp
public class ShadowEffect
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Angle](../../aspose.cells.drawing/shadoweffect/angle/) { get; set; } | Liest und setzt den Beleuchtungswinkel. Bereich von 0 bis 359,9 Grad. |
| [Blur](../../aspose.cells.drawing/shadoweffect/blur/) { get; set; } | Liest und setzt die Unschärfe des Schattens. Bereich von 0 bis 100 Punkten. |
| [Color](../../aspose.cells.drawing/shadoweffect/color/) { get; set; } | Liest und setzt die Farbe des Schattens. |
| [Distance](../../aspose.cells.drawing/shadoweffect/distance/) { get; set; } | Liest und setzt den Abstand des Schattens. Bereich von 0 bis 200 Punkten. |
| [PresetType](../../aspose.cells.drawing/shadoweffect/presettype/) { get; set; } | Liest und setzt den voreingestellten Schatten‑typ des Schattens. |
| [Size](../../aspose.cells.drawing/shadoweffect/size/) { get; set; } | Liest und setzt die Größe des Schattens. Bereich von 0 bis 2,0. Bedeutungslose bei innerem Schatten. |
| [Transparency](../../aspose.cells.drawing/shadoweffect/transparency/) { get; set; } | Liest und setzt den Transparenzgrad des Schattens. Bereich von 0,0 (undurchsichtig) bis 1,0 (transparent). |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispielhafte Form mit allen erforderlichen Parametern hinzufügen
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 100);

            // Den Schatteneffekt der Form abrufen
            ShadowEffect shadow = shape.ShadowEffect;

            // Schatteneigenschaften festlegen
            shadow.Angle = 150;
            shadow.Blur = 30;
            shadow.Size = 1.3;
            shadow.Transparency = 0.4;
            shadow.Distance = 80;

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");

            Console.WriteLine("Shadow effect demo completed successfully.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


