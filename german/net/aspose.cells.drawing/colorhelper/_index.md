---
title: "Klasse ColorHelper"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.ColorHelper Klasse. Stellt Hilfsfunktionen für Farben bereit"
type: docs
url: /de/net/aspose.cells.drawing/colorhelper/
---
## ColorHelper class

Stellt Hilfsfunktionen für Farben bereit.

```csharp
public class ColorHelper
```

## Methoden

| Name | Beschreibung |
| --- | --- |
| static [FromOleColor](../../aspose.cells.drawing/colorhelper/fromolecolor/)(int) | OLE_COLOR konvertieren. |
| static [ToOleColor](../../aspose.cells.drawing/colorhelper/toolecolor/)(Color, Workbook) | Farbe in OLE_COLOR konvertieren |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class DrawingClassColorHelperDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe und greife auf das erste Arbeitsblatt zu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // OLE-Farbe in System.Drawing.Color (Grün) konvertieren
            int oleGreen = 0x00FF00;
            Color colorFromOle = ColorHelper.FromOleColor(oleGreen);

            // Konvertierte Farbe auf den Hintergrund von Zelle A1 anwenden
            Cell cellA1 = worksheet.Cells["A1"];
            Style styleA1 = cellA1.GetStyle();
            styleA1.ForegroundColor = colorFromOle;
            styleA1.Pattern = BackgroundType.Solid;
            cellA1.SetStyle(styleA1);

            // System.Drawing.Color zurück in OLE-Farbe konvertieren
            int convertedOle = ColorHelper.ToOleColor(colorFromOle, workbook);

            // OLE-Ergebnis zurück in Farbe konvertieren (Verifizierung)
            Color colorFromConvertedOle = ColorHelper.FromOleColor(convertedOle);

            // Rekonvertierte Farbe auf den Hintergrund von Zelle A2 anwenden
            Cell cellA2 = worksheet.Cells["A2"];
            Style styleA2 = cellA2.GetStyle();
            styleA2.ForegroundColor = colorFromConvertedOle;
            styleA2.Pattern = BackgroundType.Solid;
            cellA2.SetStyle(styleA2);

            // Speichere die geänderte Arbeitsmappe
            workbook.Save("DrawingClassColorHelperDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


