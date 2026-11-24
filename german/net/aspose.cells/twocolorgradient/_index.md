---
title: "Klasse TwoColorGradient"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.TwoColorGradient Klasse. Stellt einen Zweifarbverlauf dar"
type: docs
url: /de/net/aspose.cells/twocolorgradient/
---
## TwoColorGradient class

Stellt einen Zweifarbverlauf dar.

```csharp
public class TwoColorGradient
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [TwoColorGradient](twocolorgradient/)(Color, Color, GradientStyleType, int) |  |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Color1](../../aspose.cells/twocolorgradient/color1/) { get; set; } | Liest und setzt die erste Verlauffarbe. |
| [Color2](../../aspose.cells/twocolorgradient/color2/) { get; set; } | Liest und setzt die zweite Verlauffarbe. |
| [GradientStyleType](../../aspose.cells/twocolorgradient/gradientstyletype/) { get; set; } | Liest und setzt den Verlaufsschattierungsstil. |
| [Variant](../../aspose.cells/twocolorgradient/variant/) { get; set; } | Liest und setzt die Verlaufvariante. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class CellsClassTwoColorGradientDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Initialisieren Sie TwoColorGradient mit Konstruktorparametern
            TwoColorGradient gradient = new TwoColorGradient(
                Color.LightSkyBlue, 
                Color.DarkBlue, 
                GradientStyleType.DiagonalUp, 
                2);

            // Ändern Sie die Verlaufseigenschaften nach der Initialisierung
            gradient.GradientStyleType = GradientStyleType.DiagonalDown;

            // Erstellen Sie den Zellenstil und wenden Sie den Verlauf an
            Style style = workbook.CreateStyle();
            style.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);

            // Wenden Sie den Stil auf die Zelle an und fügen Sie Inhalt hinzu
            Cell cell = worksheet.Cells["B2"];
            cell.PutValue("Aspose.Cells TwoColorGradient Demo");
            cell.SetStyle(style);

            // Passen Sie die Zellengrößen für die Sichtbarkeit an
            worksheet.Cells.SetRowHeight(1, 45);
            worksheet.Cells.SetColumnWidth(1, 55);

            // Speichern Sie das Ergebnis mit Verlaufformatierung
            workbook.Save("TwoColorGradientDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


