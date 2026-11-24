---
title: "TwoColorGradient.TwoColorGradient"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TwoColorGradient-Konstruktor."
type: docs
url: /de/net/aspose.cells/twocolorgradient/twocolorgradient/
---
## TwoColorGradient constructor

```csharp
public TwoColorGradient(Color color1, Color color2, GradientStyleType gradientStyleType, 
    int variant)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| color1 | Farbe |  |
| color2 | Farbe |  |
| gradientStyleType | GradientStyleType |  |
| Variante | Int32 |  |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class TwoColorGradientMethodSharpctorWithColorColorGradientStyleTyInt32Demo
    {
        public static void Run()
        {
            try
            {
                // Erstelle eine TwoColorGradient-Instanz mit dem Konstruktor und allen Parametern
                TwoColorGradient gradient = new TwoColorGradient(
                    Color.LightBlue,
                    Color.DarkBlue,
                    GradientStyleType.Horizontal,
                    1);

                // Zeige die Gradient-Eigenschaften an, um die Initialisierung zu überprüfen
                Console.WriteLine($"Gradient created with:");
                Console.WriteLine($"Color1: {gradient.Color1}");
                Console.WriteLine($"Color2: {gradient.Color2}");
                Console.WriteLine($"GradientStyleType: {gradient.GradientStyleType}");
                Console.WriteLine($"Variant: {gradient.Variant}");

                // Erstelle eine Arbeitsmappe und wende den Verlauf an, um die Funktionalität zu demonstrieren
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Wende den Verlauf auf eine Zelle an
                Style style = workbook.CreateStyle();
                style.SetTwoColorGradient(
                    gradient.Color1,
                    gradient.Color2,
                    gradient.GradientStyleType,
                    gradient.Variant);

                worksheet.Cells["A1"].PutValue("TwoColorGradient Demo");
                worksheet.Cells["A1"].SetStyle(style);

                // Speichere die Arbeitsmappe
                workbook.Save("TwoColorGradientDemo.xlsx");
                Console.WriteLine("Gradient applied successfully to workbook.");
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

* enum [GradientStyleType](../../../aspose.cells.drawing/gradientstyletype/)
* class [TwoColorGradient](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


