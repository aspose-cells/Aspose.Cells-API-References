---
title: "Aufzählung GradientColorType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.GradientColorType Aufzählung. Stellt den Farbverlauftyp für die angegebene Füllung dar"
type: docs
url: /de/net/aspose.cells.drawing/gradientcolortype/
---
## GradientColorType enumeration

Stellt den Verlauffarbtyp für die angegebene Füllung dar.

```csharp
public enum GradientColorType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| None | `0` | Kein Farbverlauf |
| OneColor | `1` | Ein Farbverlauf |
| PresetColors | `2` | Vordefinierte Farbverläufe |
| TwoColors | `3` | Zwei Farbverläufe |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassGradientColorTypeDemo
    {
        public static void Run()
        {
            // Erstellt ein neues Arbeitsbuch für die Demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Füge eine Form hinzu, um die Farbverlauffüllung zu demonstrieren
                Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 200, 200);
                FillFormat fill = shape.Fill;

                // Setze den Typ der Farbverlauffüllung
                fill.FillType = FillType.Gradient;

                // Demonstriere verschiedene Werte der GradientColorType Aufzählung
                Console.WriteLine("Available GradientColorType values:");
                Console.WriteLine("None: " + GradientColorType.None);
                Console.WriteLine("OneColor: " + GradientColorType.OneColor);
                Console.WriteLine("PresetColors: " + GradientColorType.PresetColors);
                Console.WriteLine("TwoColors: " + GradientColorType.TwoColors);

                // Lese und zeige den aktuellen Farbverlauftyp an (Eigenschaft ist schreibgeschützt)
                Console.WriteLine("Current gradient color type: " + fill.GradientColorType);

                // Speichere die Arbeitsmappe
                workbook.Save("GradientColorTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with GradientColorType: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


