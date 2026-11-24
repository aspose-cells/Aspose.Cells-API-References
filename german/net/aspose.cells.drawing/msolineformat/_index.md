---
title: "Class MsoLineFormat"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.MsoLineFormat class. Stellt die Formatierung von Linien und Pfeilspitzen dar"
type: docs
url: /de/net/aspose.cells.drawing/msolineformat/
---
## MsoLineFormat class

Stellt die Linien- und Pfeilspitzenformatierung dar.

```csharp
public class MsoLineFormat
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [BackColor](../../aspose.cells.drawing/msolineformat/backcolor/) { get; set; } | Liest und setzt die Hintergrundfarbe der Randlinie. |
| [DashStyle](../../aspose.cells.drawing/msolineformat/dashstyle/) { get; set; } | Liest oder setzt den Strichstil für die angegebene Linie. |
| [ForeColor](../../aspose.cells.drawing/msolineformat/forecolor/) { get; set; } | Liest und setzt die Vorderfarbe der Randlinie. |
| [IsVisible](../../aspose.cells.drawing/msolineformat/isvisible/) { get; set; } | Gibt an, ob das Objekt sichtbar ist. |
| [Style](../../aspose.cells.drawing/msolineformat/style/) { get; set; } | Gibt ein Style-Objekt zurück, das den Stil des angegebenen Bereichs darstellt. |
| [Transparency](../../aspose.cells.drawing/msolineformat/transparency/) { get; set; } | Gibt den Transparenzgrad der angegebenen Füllung zurück oder setzt ihn, als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent). |
| [Weight](../../aspose.cells.drawing/msolineformat/weight/) { get; set; } | Gibt das Gewicht der Linie zurück oder setzt es, in pt-Einheiten. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatDemo
    {
        public static void MsoLineFormatExample()
        {
            // Instanziieren Sie ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie dem Arbeitsblatt eine Bogenform hinzu
            Aspose.Cells.Drawing.ArcShape arcShape = worksheet.Shapes.AddArc(2, 0, 2, 0, 130, 130);

            // Rufen Sie das MsoLineFormat-Objekt aus der Form ab
            MsoLineFormat lineFormat = arcShape.LineFormat;

            // Setzen Sie Eigenschaften des MsoLineFormat-Objekts
            lineFormat.IsVisible = true;
            lineFormat.Style = MsoLineStyle.ThickThin;
            lineFormat.ForeColor = Color.Red;
            lineFormat.BackColor = Color.Blue;
            lineFormat.DashStyle = MsoLineDashStyle.Solid;
            lineFormat.Transparency = 0.5;
            lineFormat.Weight = 2.0;

            // Speichere die Arbeitsmappe
            workbook.Save("MsoLineFormatExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


