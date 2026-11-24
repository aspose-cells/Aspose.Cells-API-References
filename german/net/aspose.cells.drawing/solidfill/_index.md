---
title: "Klasse SolidFill"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.SolidFill Klasse. Kapselt das Objekt, das das Format einer einfarbigen Füllung darstellt"
type: docs
url: /de/net/aspose.cells.drawing/solidfill/
---
## SolidFill class

Kapselt das Objekt, das das Format einer einfarbigen Füllung darstellt

```csharp
public class SolidFill : Fill
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [CellsColor](../../aspose.cells.drawing/solidfill/cellscolor/) { get; set; } | Liest und setzt das [`CellsColor`](./cellscolor/) Objekt. |
| [Color](../../aspose.cells.drawing/solidfill/color/) { get; set; } | Liest oder setzt die Farbe. |
| [Transparency](../../aspose.cells.drawing/solidfill/transparency/) { get; set; } | Gibt den Transparenzgrad des Bereichs zurück oder legt ihn fest, als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent). |

## Methoden

| Name | Beschreibung |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/solidfill/equals/)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/solidfill/gethashcode/)() | Liest den Hash‑Code. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using System;
    using System.Drawing;
    using Aspose.Cells;
    using Aspose.Cells.Drawing;

    public class DrawingClassSolidFillDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            try
            {
                // Füge dem Blatt eine einfache Rechteckform hinzu
                Shape rect = sheet.Shapes.AddRectangle(2, 0, 2, 0, 150, 100);

                // Konfiguriere die Form, um eine einfarbige Füllung zu verwenden
                rect.Fill.FillType = FillType.Solid;

                // Erhalte das SolidFill-Objekt
                SolidFill solidFill = rect.Fill.SolidFill;

                // Setze Eigenschaften für die einfarbige Füllung
                solidFill.Color = Color.CornflowerBlue;   // System.Drawing.Color
                solidFill.Transparency = 0.25;            // 0 = opaque, 1 = fully transparent

                // Greife auf die CellsColor-Eigenschaft zu (lesen/schreiben)
                CellsColor cellsColor = solidFill.CellsColor;
                if (cellsColor != null)
                {
                    Console.WriteLine("CellsColor object is available.");
                }
                else
                {
                    Console.WriteLine("CellsColor is null (default).");
                }

                Console.WriteLine($"SolidFill created with Color={solidFill.Color.Name}, Transparency={solidFill.Transparency}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SolidFill: {ex.Message}");
            }

            // Speichere die Arbeitsmappe, um das Aussehen der Form zu überprüfen
            workbook.Save("DrawingClassSolidFillDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


