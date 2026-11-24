---
title: "PatternFill.BackTransparency"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PatternFill-Eigenschaft. Ruft die Transparenz der Hintergrundfarbe ab oder legt sie fest"
type: docs
url: /de/net/aspose.cells.drawing/patternfill/backtransparency/
---
## PatternFill.BackTransparency property

Liest oder setzt die Transparenz der Hintergrundfarbe.

```csharp
public double BackTransparency { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class PatternFillPropertyBackTransparencyDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Rechteck-Shape zum Arbeitsblatt hinzu
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 200, 200);

            // Hole die vorhandene PatternFill-Instanz aus der Form und konfiguriere die Eigenschaften
            shape.Fill.FillType = FillType.Pattern;
            PatternFill patternFill = shape.Fill.PatternFill;
            patternFill.Pattern = FillPattern.Solid;
            patternFill.BackgroundColor = Color.Blue;

            // Zeige den anfänglichen BackTransparency-Wert an
            Console.WriteLine("Current BackTransparency value: " + patternFill.BackTransparency);

            // Setze einen neuen BackTransparency-Wert (50 % Transparenz)
            patternFill.BackTransparency = 0.5;

            // Speichere die geänderte Arbeitsmappe
            workbook.Save("PatternFillBackTransparencyDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


