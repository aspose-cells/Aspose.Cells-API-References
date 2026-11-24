---
title: "FillFormat.Transparency"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FillFormat-Eigenschaft. Gibt den Transparenzgrad des Bereichs zurück oder legt ihn fest, als Wert von 0.0 undurchsichtig bis 1.0 klar"
type: docs
url: /de/net/aspose.cells.drawing/fillformat/transparency/
---
## FillFormat.Transparency property

Gibt den Transparenzgrad des Bereichs zurück oder legt ihn fest, als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent).

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
    public class FillFormatPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Form hinzu, um Transparenz zu demonstrieren
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 200, 100, 50, 50);

            // Füllungseigenschaften mit Transparenz festlegen
            shape.Fill.FillType = FillType.Solid;
            shape.Fill.SolidFill.Color = System.Drawing.Color.Blue;
            shape.Fill.Transparency = 0.3; // 30% transparent

            // Speichere die Arbeitsmappe
            workbook.Save("FillFormatTransparencyDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


