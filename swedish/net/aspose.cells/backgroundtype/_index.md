---
title: "Enum BackgroundType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.BackgroundType enum. Enumererar cellbakgrundsmönsterstyper"
type: docs
url: /sv/net/aspose.cells/backgroundtype/
---
## BackgroundType enumeration

Enumererar typer av cellbakgrundsmönster.

```csharp
public enum BackgroundType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| DiagonalCrosshatch | `9` | Representerar diagonalt korshäftningsmönster. |
| DiagonalStripe | `8` | Representerar diagonalt randmönster. |
| Gray6 | `18` | Representerar 6,25 % grått mönster |
| Gray12 | `17` | Representerar 12,5 % grått mönster |
| Gray25 | `4` | Representerar 25 % grått mönster. |
| Gray50 | `2` | Representerar 50 % grått mönster. |
| Gray75 | `3` | Representerar 75 % grått mönster. |
| HorizontalStripe | `5` | Representerar horisontellt randmönster. |
| None | `0` | Representerar ingen bakgrund. |
| ReverseDiagonalStripe | `7` | Representerar omvänd diagonalt randmönster. |
| Solid | `1` | Representerar solid mönster. |
| ThickDiagonalCrosshatch | `10` | Representerar tjockt diagonalt korshäftningsmönster. |
| ThinDiagonalCrosshatch | `16` | Representerar tunt diagonalt korshäftningsmönster. |
| ThinDiagonalStripe | `14` | Representerar tunt diagonalt randmönster. |
| ThinHorizontalCrosshatch | `15` | Representerar tunt horisontellt korshäftningsmönster. |
| ThinHorizontalStripe | `11` | Representerar tunt horisontellt randmönster. |
| ThinReverseDiagonalStripe | `13` | Representerar tunt omvänt diagonalt randmönster. |
| ThinVerticalStripe | `12` | Representerar ett tunt vertikalt randmönster. |
| VerticalStripe | `6` | Representerar ett vertikalt randmönster. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class BackgroundTypeDemo
    {
        public static void BackgroundTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Åtkomst till en cell från kalkylbladet
            Cell cell = worksheet.Cells["A1"];
            
            // Ange värdet för cellen
            cell.PutValue("Hello, Aspose!");

            // Skapa ett stilobjekt
            Style style = cell.GetStyle();
            
            // Ange bakgrundsmönsterstypen
            style.Pattern = BackgroundType.DiagonalStripe;
            
            // Ange förgrundsfärgen
            style.ForegroundColor = Color.Red;
            
            // Ange bakgrundsfärgen
            style.BackgroundColor = Color.Green;
            
            // Tillämpa stilen på cellen
            cell.SetStyle(style);
            
            // Spara arbetsboken
            workbook.Save("BackgroundTypeExample.xlsx");
            workbook.Save("BackgroundTypeExample.pdf");



        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


