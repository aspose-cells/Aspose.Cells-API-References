---
title: "Enum RectangleAlignmentType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.RectangleAlignmentType‑Enum. Gibt an, wie zwei Rechtecke relativ zueinander positioniert werden"
type: docs
url: /de/net/aspose.cells.drawing/rectanglealignmenttype/
---
## RectangleAlignmentType enumeration

Stellt dar, wie zwei Rechtecke relativ zueinander positioniert werden.

```csharp
public enum RectangleAlignmentType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Bottom | `0` | Unten |
| BottomLeft | `1` | UntenLinks |
| BottomRight | `2` | UntenRechts |
| Center | `3` | Mitte |
| Left | `4` | Links |
| Right | `5` | Rechts |
| Top | `6` | Oben |
| TopLeft | `7` | ObenLinks |
| TopRight | `8` | ObenRechts |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassRectangleAlignmentTypeDemo
    {
        public static void Run()
        {
            // Erstellt ein neues Arbeitsbuch für die Demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Füge eine Rechteckform hinzu, um die Ausrichtung zu demonstrieren
                Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 0, 200, 100, 100);

                // Demonstriere verschiedene Ausrichtungstypen
                Console.WriteLine("Available RectangleAlignmentType values:");
                Console.WriteLine("Bottom: " + RectangleAlignmentType.Bottom);
                Console.WriteLine("BottomLeft: " + RectangleAlignmentType.BottomLeft);
                Console.WriteLine("BottomRight: " + RectangleAlignmentType.BottomRight);
                Console.WriteLine("Center: " + RectangleAlignmentType.Center);
                Console.WriteLine("Left: " + RectangleAlignmentType.Left);
                Console.WriteLine("Right: " + RectangleAlignmentType.Right);
                Console.WriteLine("Top: " + RectangleAlignmentType.Top);
                Console.WriteLine("TopLeft: " + RectangleAlignmentType.TopLeft);
                Console.WriteLine("TopRight: " + RectangleAlignmentType.TopRight);

                // Setze die Ausrichtung basierend auf einem der Enum-Werte
                rectangle.TextHorizontalAlignment = TextAlignmentType.Center;
                rectangle.TextVerticalAlignment = TextAlignmentType.Center;

                // Speichere die Arbeitsmappe
                workbook.Save("RectangleAlignmentTypeDemo.xlsx");
                Console.WriteLine("RectangleAlignmentType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating RectangleAlignmentType: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


