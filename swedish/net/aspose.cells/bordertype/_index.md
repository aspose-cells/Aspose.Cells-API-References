---
title: "Enum BorderType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.BorderType enum. Enumererar gränslinje- och diagonallinjetyper"
type: docs
url: /sv/net/aspose.cells/bordertype/
---
## BorderType enumeration

Enumererar typer av kantlinjer och diagonala linjer.

```csharp
[Flags]
public enum BorderType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| LeftBorder | `1` | Representerar vänster gränslinje. |
| RightBorder | `2` | Representerar att högra gränslinjen finns. |
| TopBorder | `4` | Representerar övre gränslinje. |
| BottomBorder | `8` | Representerar nedre gränslinje. |
| DiagonalDown | `10` | Representerar den diagonala linjen från övre vänster till nedre höger. |
| DiagonalUp | `20` | Representerar den diagonala linjen från nedre vänster till övre höger. |
| Vertical | `40` | Endast för dynamisk stil, såsom villkorsstyrd formatering, pivottabell. |
| Horizontal | `80` | Endast för dynamisk stil, såsom villkorsstyrd formatering, pivottabell. |
| SideBorders | `F` | Indikerar de fyra sidogränserna: LeftBorder, RightBorder, TopBorder och BottomBorder. |
| Diagonal | `30` | Speciell kombination av flera gränser för användarens bekvämlighet i vissa API:er. Indikerar diagonala gränser för DiagonalUp och DiagonalDown. |
| DynamicStyleBorders | `C0` | Indikerar vertikal och horisontell för dynamisk stil. |
| None | `0` | Ingen gräns har specificerats. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class BorderTypeDemo
    {
        public static void BorderTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            // Skapa ett cellområde
            var range = worksheet.Cells.CreateRange("A1:D4");

            // Skapa ett stilobjekt
            Style style = workbook.CreateStyle();
            // Ställ in gränserna för området
            style.SetBorder(BorderType.LeftBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.RightBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.TopBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.DiagonalDown, CellBorderType.Thin, Color.Red);
            style.SetBorder(BorderType.DiagonalUp, CellBorderType.Thin, Color.Blue);

            // Applicera stilen på området
            StyleFlag flag = new StyleFlag { Borders = true };
            range.ApplyStyle(style, flag);

            // Spara arbetsboken
            workbook.Save("BorderTypeExample.xlsx");
            workbook.Save("BorderTypeExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


