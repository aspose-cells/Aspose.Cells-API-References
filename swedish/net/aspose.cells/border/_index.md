---
title: "Klass Border"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Border-klass. Inkapslar objektet som representerar cellens kant"
type: docs
url: /sv/net/aspose.cells/border/
---
## Border class

Inkapslar objektet som representerar cellens kant.

```csharp
public class Border
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [ArgbColor](../../aspose.cells/border/argbcolor/) { get; set; } | Hämtar och anger färgen med ett 32-bitars ARGB‑värde. |
| [Color](../../aspose.cells/border/color/) { get; set; } | Hämtar eller anger färgen på kanten. |
| [LineStyle](../../aspose.cells/border/linestyle/) { get; set; } | Hämtar eller anger cellkantens typ. |
| [ThemeColor](../../aspose.cells/border/themecolor/) { get; set; } | Hämtar och anger temafärgen för kanten. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class BorderDemo
    {
        public static void BorderExample()
        {
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();

            // Lägga till ett nytt kalkylblad i Workbook-objektet
            workbook.Worksheets.Add();

            // Hämtar referensen till det nyligen tillagda kalkylbladet genom att ange dess bladindex
            Worksheet worksheet = workbook.Worksheets[0];

            // Åtkomst till cellen "A1" från kalkylbladet
            Cell cell = worksheet.Cells["A1"];

            // Lägger till ett värde i cellen "A1"
            cell.PutValue("Hello World");

            // Hämtar cellstilen
            Style style = cell.GetStyle();

            // Anger linjestil för den övre kanten
            Border topBorder = style.Borders[BorderType.TopBorder];
            topBorder.LineStyle = CellBorderType.Medium;
            topBorder.Color = Color.Red;

            // Anger linjestil för den nedre kanten
            Border bottomBorder = style.Borders[BorderType.BottomBorder];
            bottomBorder.LineStyle = CellBorderType.Thick;
            bottomBorder.Color = Color.Blue;

            // Anger linjestil för den vänstra kanten
            Border leftBorder = style.Borders[BorderType.LeftBorder];
            leftBorder.LineStyle = CellBorderType.Dashed;
            leftBorder.Color = Color.Green;

            // Anger linjestil för den högra kanten
            Border rightBorder = style.Borders[BorderType.RightBorder];
            rightBorder.LineStyle = CellBorderType.Dotted;
            rightBorder.Color = Color.Purple;

            // Tillämpar stilen på cellen
            cell.SetStyle(style);

            // Sparar Excel-filen
            workbook.Save("BorderExample.xlsx");
            workbook.Save("BorderExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


