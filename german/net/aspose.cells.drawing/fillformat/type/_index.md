---
title: "FillFormat.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FillFormat-Eigenschaft. Ruft den Fülltyp ab und legt ihn fest."
type: docs
url: /de/net/aspose.cells.drawing/fillformat/type/
---
## FillFormat.Type property

Ruft den Fülltyp ab und legt ihn fest.

```csharp
[Obsolete("Use FillFormat.FillType  instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public FillType Type { get; set; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die FillFormat.FillType-Eigenschaft. Diese Eigenschaft wird 12 Monate nach Juli 2016 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class FillFormatPropertyTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rechteckform hinzufügen
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 200);
            FillFormat fill = shape.Fill;

            // Aktuellen Type-Wert anzeigen.
            Console.WriteLine("Current Type value: " + fill.Type);

            // Typ zu Gradient ändern (veraltete Eigenschaft, die zur Demonstration verwendet wird).
            fill.Type = FillType.Gradient;

            // Zweifarbigen Farbverlaufseffekt anwenden.
            fill.SetTwoColorGradient(Color.Blue, Color.Green, GradientStyleType.Horizontal, 1);

            // Speichere die geänderte Arbeitsmappe
            workbook.Save("FillFormatTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [FillType](../../filltype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


