---
title: "ThreeDFormat.Equals"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ThreeDFormat-Methode."
type: docs
url: /de/net/aspose.cells.drawing/threedformat/equals/
---
## ThreeDFormat.Equals method

```csharp
public override bool Equals(object obj)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | Object |  |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Form hinzu, um 3D-Formate zu vergleichen
            Shape shape1 = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 0, 0, 100, 100, 0, 0);
            Shape shape2 = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 0, 150, 100, 100, 0, 0);

            // Erhalte die 3D-Formate der Formen
            ThreeDFormat format1 = shape1.ThreeDFormat;
            ThreeDFormat format2 = shape2.ThreeDFormat;

            // Konfiguriere identische 3D-Einstellungen
            format1.BottomBevelWidth = 10;
            format1.BottomBevelHeight = 10;
            format1.BottomBevelType = BevelType.ArtDeco;

            format2.BottomBevelWidth = 10;
            format2.BottomBevelHeight = 10;
            format2.BottomBevelType = BevelType.ArtDeco;

            try
            {
                // Rufen Sie die Equals-Methode auf, um die 3D-Formate zu vergleichen
                bool areEqual = format1.Equals((object)format2);

                // Ergebnis anzeigen
                Console.WriteLine($"The 3D formats are equal: {areEqual}");

                // Ändern Sie eine Eigenschaft, um sie unterschiedlich zu machen
                format2.BottomBevelWidth = 15;
                areEqual = format1.Equals((object)format2);
                Console.WriteLine($"After modification, the 3D formats are equal: {areEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("ThreeDFormatEqualsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


