---
title: "ShadowEffect.Color"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShadowEffect-Eigenschaft. Gibt die Farbe des Schattens zurück oder legt sie fest"
type: docs
url: /de/net/aspose.cells.drawing/shadoweffect/color/
---
## ShadowEffect.Color property

Liest und setzt die Farbe des Schattens.

```csharp
public CellsColor Color { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class ShadowEffectPropertyColorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Rechteckform hinzu, um den Schatteneffekt zu demonstrieren
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            try
            {
                // Hole den Schatteneffekt von der Form
                ShadowEffect shadowEffect = shape.ShadowEffect;

                // Erstelle ein neues CellsColor-Objekt
                CellsColor shadowColor = workbook.CreateCellsColor();

                // Setze die Farbe auf Rot mittels RGB-Werten
                shadowColor.Color = Color.Red;

                // Wende die Farbe auf den Schatteneffekt an
                shadowEffect.Color = shadowColor;

                // Zeige den aktuellen Farbwert an
                Console.WriteLine("Shadow Color (RGB): " + shadowEffect.Color.Color.ToString());
                Console.WriteLine("Shadow Color (ARGB): " + shadowEffect.Color.Argb);

                // Speichere die Arbeitsmappe, um die Wirkung zu demonstrieren
                workbook.Save("ShadowEffectColorDemo.xlsx");

                // Lade die Arbeitsmappe erneut, um zu überprüfen, dass die Farbe gespeichert wurde
                Workbook loadedWorkbook = new Workbook("ShadowEffectColorDemo.xlsx");
                ShadowEffect loadedShadowEffect = loadedWorkbook.Worksheets[0].Shapes[0].ShadowEffect;

                // Zeige den geladenen Farbwert an
                Console.WriteLine("Loaded Shadow Color (RGB): " + loadedShadowEffect.Color.Color.ToString());
                Console.WriteLine("Loaded Shadow Color (ARGB): " + loadedShadowEffect.Color.Argb);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


