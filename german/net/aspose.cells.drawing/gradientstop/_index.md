---
title: "Klasse GradientStop"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.GradientStop-Klasse. Stellt den Gradient-Stopp dar"
type: docs
url: /de/net/aspose.cells.drawing/gradientstop/
---
## GradientStop class

Stellt den Gradient-Stopp dar.

```csharp
public class GradientStop
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [CellsColor](../../aspose.cells.drawing/gradientstop/cellscolor/) { get; } | Liest die Farbe dieses Gradient-Stops. |
| [Position](../../aspose.cells.drawing/gradientstop/position/) { get; set; } | Die Position des Stops. |
| [Transparency](../../aspose.cells.drawing/gradientstop/transparency/) { get; set; } | Gibt den Transparenzgrad des Bereichs zurück oder legt ihn fest, als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent). |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class DrawingClassGradientStopDemo
    {
        public static void Run()
        {
            // Erstellt ein neues Arbeitsbuch für die Demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Fügen Sie eine Form mit Farbverlauffüllung hinzu
                Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 300);
                shape.Fill.FillType = FillType.Gradient;
                GradientFill gradientFill = shape.Fill.GradientFill;
                gradientFill.SetGradient(GradientFillType.Linear, 0, GradientDirectionType.FromUpperLeftCorner);

                // Farbe für Gradient-Stopp erstellen
                CellsColor color = workbook.CreateCellsColor();
                color.Color = Color.Blue;

                // Gradient-Stopp hinzufügen
                gradientFill.GradientStops.Add(0, color, 30);

                // Zugriff auf den Gradient-Stopp
                GradientStop stop = gradientFill.GradientStops[0];

                // Demonstriere grundlegende Funktionalität
                Console.WriteLine("GradientStop instance created successfully");
                Console.WriteLine("Position: " + stop.Position);
                Console.WriteLine("Transparency: " + stop.Transparency);
                Console.WriteLine("CellsColor Type: " + stop.CellsColor.Type);

                // Eigenschaften ändern
                stop.Position = 0.5;
                stop.Transparency = 0.7;

                Console.WriteLine("Modified Position: " + stop.Position);
                Console.WriteLine("Modified Transparency: " + stop.Transparency);

                // Speichere die Arbeitsmappe
                workbook.Save("GradientStopDemo.xlsx");
                Console.WriteLine("Demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with GradientStop: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


