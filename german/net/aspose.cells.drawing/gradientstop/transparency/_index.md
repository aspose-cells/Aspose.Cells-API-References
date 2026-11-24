---
title: "GradientStop.Transparency"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GradientStop-Eigenschaft. Gibt den Transparenzgrad des Bereichs zurück oder legt ihn fest, als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent)."
type: docs
url: /de/net/aspose.cells.drawing/gradientstop/transparency/
---
## GradientStop.Transparency property

Gibt den Transparenzgrad des Bereichs zurück oder legt ihn fest, als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent).

```csharp
public double Transparency { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientStopPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie eine Form mit Farbverlauffüllung hinzu
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 300);
            shape.Fill.FillType = FillType.Gradient;
            GradientFill gradientFill = shape.Fill.GradientFill;
            gradientFill.SetGradient(GradientFillType.Linear, 0, GradientDirectionType.FromUpperLeftCorner);

            // Farbe für Gradient-Stopp erstellen
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Blue;

            // Füge einen Gradient-Stop mit anfänglicher Transparenz hinzu.
            gradientFill.GradientStops.Add(0, color, 30);

            // Zugriff auf den Gradient-Stopp
            GradientStop stop = gradientFill.GradientStops[0];

            // Transparenz anzeigen und ändern.
            Console.WriteLine("Initial Transparency: " + stop.Transparency);
            stop.Transparency = 0.7;
            Console.WriteLine("Modified Transparency: " + stop.Transparency);

            // Füge einen weiteren Stop zum visuellen Vergleich hinzu.
            CellsColor color2 = workbook.CreateCellsColor();
            color2.Color = Color.Green;
            gradientFill.GradientStops.Add(1, color2, 30);

            // Speichere die Arbeitsmappe
            workbook.Save("GradientStopTransparencyDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [GradientStop](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


