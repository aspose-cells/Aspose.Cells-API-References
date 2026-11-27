---
title: "Klass ColorHelper"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.ColorHelper-klass. Tillhandahåller hjälpfunktioner för färg"
type: docs
url: /sv/net/aspose.cells.drawing/colorhelper/
---
## ColorHelper class

Tillhandahåller hjälpfunktioner för färg.

```csharp
public class ColorHelper
```

## Metoder

| Namn | Beskrivning |
| --- | --- |
| static [FromOleColor](../../aspose.cells.drawing/colorhelper/fromolecolor/)(int) | Konvertera OLE_COLOR. |
| static [ToOleColor](../../aspose.cells.drawing/colorhelper/toolecolor/)(Color, Workbook) | Konvertera färg till OLE_COLOR |

### Exempel

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
            // Skapa en ny arbetsbok och öppna det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Konvertera OLE-färg till System.Drawing.Color (Grön)
            int oleGreen = 0x00FF00;
            Color colorFromOle = ColorHelper.FromOleColor(oleGreen);

            // Applicera konverterad färg på cell A1:s bakgrund
            Cell cellA1 = worksheet.Cells["A1"];
            Style styleA1 = cellA1.GetStyle();
            styleA1.ForegroundColor = colorFromOle;
            styleA1.Pattern = BackgroundType.Solid;
            cellA1.SetStyle(styleA1);

            // Konvertera System.Drawing.Color tillbaka till OLE-färg
            int convertedOle = ColorHelper.ToOleColor(colorFromOle, workbook);

            // Konvertera OLE-resultat tillbaka till färg (verifiering)
            Color colorFromConvertedOle = ColorHelper.FromOleColor(convertedOle);

            // Applicera återkonverterad färg på cell A2:s bakgrund
            Cell cellA2 = worksheet.Cells["A2"];
            Style styleA2 = cellA2.GetStyle();
            styleA2.ForegroundColor = colorFromConvertedOle;
            styleA2.Pattern = BackgroundType.Solid;
            cellA2.SetStyle(styleA2);

            // Spara den modifierade arbetsboken
            workbook.Save("DrawingClassColorHelperDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


