---
title: "Enum LightRigDirectionType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.LightRigDirectionType enum. Stellt den Lichtrig-Richtungstyp dar"
type: docs
url: /de/net/aspose.cells.drawing/lightrigdirectiontype/
---
## LightRigDirectionType enumeration

Stellt den Richtungs­typ des Licht‑Riggs dar.

```csharp
public enum LightRigDirectionType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Bottom | `0` | Unten |
| BottomLeft | `1` | Unten links. |
| BottomRight | `2` | Unten rechts. |
| Left | `3` | Links. |
| Right | `4` | Rechts. |
| Top | `5` | Oben. |
| TopLeft | `6` | Oben links. |
| TopRight | `7` | Oben rechts. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassLightRigDirectionTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Form hinzu, um die Lichtrig-Richtung zu demonstrieren
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 10, 10, 200, 200, 0, 0);

            // Setze die Lichtrig-Richtung für das 3D-Format der Form
            shape.ThreeDFormat.LightingDirection = LightRigDirectionType.TopRight;

            // Demonstriere verschiedene Lichtrig-Richtungen
            Console.WriteLine("Current Light Rig Direction: " + shape.ThreeDFormat.LightingDirection);

            // Ändere die Lichtrig-Richtung
            shape.ThreeDFormat.LightingDirection = LightRigDirectionType.BottomLeft;
            Console.WriteLine("Changed Light Rig Direction: " + shape.ThreeDFormat.LightingDirection);

            // Durchlaufe alle möglichen Lichtrig-Richtungen
            Console.WriteLine("\nAll Light Rig Direction Types:");
            foreach (LightRigDirectionType direction in Enum.GetValues(typeof(LightRigDirectionType)))
            {
                Console.WriteLine(direction.ToString());
            }

            // Speichere die Arbeitsmappe
            workbook.Save("LightRigDirectionTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


