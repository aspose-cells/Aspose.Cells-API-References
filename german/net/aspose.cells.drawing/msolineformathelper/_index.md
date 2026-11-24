---
title: "Klasse MsoLineFormatHelper"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.MsoLineFormatHelper Klasse. Stellt die Formatierung von Linien und Pfeilspitzen dar"
type: docs
url: /de/net/aspose.cells.drawing/msolineformathelper/
---
## MsoLineFormatHelper class

Stellt die Linien- und Pfeilspitzenformatierung dar.

```csharp
public class MsoLineFormatHelper
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [BackColor](../../aspose.cells.drawing/msolineformathelper/backcolor/) { get; set; } | Liest und setzt die Hintergrundfarbe der Randlinie. |
| [DashStyle](../../aspose.cells.drawing/msolineformathelper/dashstyle/) { get; set; } | Liest oder setzt den Strichstil für die angegebene Linie. |
| [ForeColor](../../aspose.cells.drawing/msolineformathelper/forecolor/) { get; set; } | Liest und setzt die Vorderfarbe der Randlinie. |
| [IsVisible](../../aspose.cells.drawing/msolineformathelper/isvisible/) { get; set; } | Gibt an, ob das Objekt sichtbar ist. |
| [Style](../../aspose.cells.drawing/msolineformathelper/style/) { get; set; } | Gibt ein Style-Objekt zurück, das den Stil des angegebenen Bereichs darstellt. |
| [Transparency](../../aspose.cells.drawing/msolineformathelper/transparency/) { get; set; } | Gibt den Transparenzgrad der angegebenen Füllung zurück oder setzt ihn, als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent). |
| [Weight](../../aspose.cells.drawing/msolineformathelper/weight/) { get; set; } | Gibt das Gewicht der Linie zurück oder setzt es, in pt-Einheiten. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class DrawingClassMsoLineFormatHelperDemo
    {
        public static void Run()
        {
            // Erstellt ein neues Arbeitsbuch für die Demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Erstelle eine Form, um die Linienformatierung zu demonstrieren
                Shape shape = worksheet.Shapes.AddLine(10, 10, 100, 100, 0, 0);

                // Hole das Linienformat direkt aus der Form
                MsoLineFormat lineFormat = shape.LineFormat;

                // Setze Eigenschaften direkt am Linienformat
                lineFormat.IsVisible = true;
                lineFormat.Style = MsoLineStyle.Single;
                lineFormat.ForeColor = Color.Blue;
                lineFormat.BackColor = Color.LightGray;
                lineFormat.DashStyle = MsoLineDashStyle.Solid;
                lineFormat.Transparency = 0.2;
                lineFormat.Weight = 2.5;

                // Zeige die konfigurierten Eigenschaften an
                Console.WriteLine($"Line is visible: {lineFormat.IsVisible}");
                Console.WriteLine($"Line style: {lineFormat.Style}");
                Console.WriteLine($"Fore color: {lineFormat.ForeColor}");
                Console.WriteLine($"Back color: {lineFormat.BackColor}");
                Console.WriteLine($"Dash style: {lineFormat.DashStyle}");
                Console.WriteLine($"Transparency: {lineFormat.Transparency}");
                Console.WriteLine($"Weight: {lineFormat.Weight}");

                // Speichere die Arbeitsmappe
                workbook.Save("MsoLineFormatHelperDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with MsoLineFormatHelper: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


