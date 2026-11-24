---
title: "FillFormat.GradientColorType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FillFormat-Eigenschaft. Gibt den Farbverlauf-Farbtyp für die angegebene Füllung zurück."
type: docs
url: /de/net/aspose.cells.drawing/fillformat/gradientcolortype/
---
## FillFormat.GradientColorType property

Gibt den Farbverlauftyp für die angegebene Füllung zurück.

```csharp
public GradientColorType GradientColorType { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class FillFormatPropertyGradientColorTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Form hinzu, um die Farbverlauffüllung zu demonstrieren
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 200);

            try
            {
                // Setzen Sie eine zweifarbige Farbverlauffüllung.
                shape.Fill.SetTwoColorGradient(Color.Red, Color.Blue,
                    GradientStyleType.Horizontal, 2);

                // Greifen Sie auf FillFormat zu, um GradientColorType zu erhalten.
                FillFormat fillFormat = shape.Fill;

                // GradientColorType-Wert anzeigen.
                Console.WriteLine("GradientColorType: " + fillFormat.GradientColorType);

                // Speichere die Arbeitsmappe
                workbook.Save("GradientColorTypeDemo.xlsx");
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

* enum [GradientColorType](../../gradientcolortype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


