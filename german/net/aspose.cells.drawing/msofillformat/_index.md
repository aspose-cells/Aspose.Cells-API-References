---
title: "Klasse MsoFillFormat"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.MsoFillFormat-Klasse. Stellt die Füllformatierung für ein Formobjekt dar"
type: docs
url: /de/net/aspose.cells.drawing/msofillformat/
---
## MsoFillFormat class

Stellt die Füllformatierung für eine Form dar.

```csharp
public class MsoFillFormat
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [BackColor](../../aspose.cells.drawing/msofillformat/backcolor/) { get; set; } | Liest und setzt die Hintergrundfarbe der Füllung. |
| [ForeColor](../../aspose.cells.drawing/msofillformat/forecolor/) { get; set; } | Liest und setzt die Vordergrundfarbe der Füllung. |
| [ImageData](../../aspose.cells.drawing/msofillformat/imagedata/) { get; set; } | Liest und setzt die Textur- und Bildfüllungsdaten. |
| [IsVisible](../../aspose.cells.drawing/msofillformat/isvisible/) { get; set; } | Gibt an, ob eine Füllung vorhanden ist. |
| [Texture](../../aspose.cells.drawing/msofillformat/texture/) { get; } | Liest den Texturfülltyp. |
| [Transparency](../../aspose.cells.drawing/msofillformat/transparency/) { get; set; } | Gibt den Transparenzgrad der angegebenen Füllung zurück oder setzt ihn, als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent). |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [SetOneColorGradient](../../aspose.cells.drawing/msofillformat/setonecolorgradient/)(Color, double, GradientStyleType, int) | Setzt die angegebene Füllung auf einen Einfarbverlauf. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatDemo
    {
        public static void MsoFillFormatExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie dem Arbeitsblatt eine Bogenform hinzu
            Aspose.Cells.Drawing.ArcShape arcShape = worksheet.Shapes.AddArc(2, 0, 2, 0, 130, 130);

            // Greifen Sie auf das Füllformat des Formobjekts zu
            MsoFillFormat fillFormat = arcShape.FillFormat;

            // Setzt die Vordergrundfarbe der Füllung
            fillFormat.ForeColor = Color.Blue;

            // Setzt die Hintergrundfarbe der Füllung
            fillFormat.BackColor = Color.LightBlue;

            // Setzt die Transparenz
            fillFormat.Transparency = 0.5;

            // Prüft, ob die Füllung sichtbar ist
            bool isVisible = fillFormat.IsVisible;
            Console.WriteLine("Is Fill Visible: " + isVisible);

            // Setzt eine einfarbige Verlauffüllung
            fillFormat.SetOneColorGradient(Color.Green, 0.3, GradientStyleType.Horizontal, 1);

            // Speichere die Arbeitsmappe
            workbook.Save("MsoFillFormatExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


