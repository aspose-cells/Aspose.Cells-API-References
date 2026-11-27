---
title: "Enum TextStrikeType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.TextStrikeType‑enum. Denna typ specificerar genomstrykningstypen"
type: docs
url: /sv/net/aspose.cells/textstriketype/
---
## TextStrikeType enumeration

Denna typ specificerar genomstrykningstypen.

```csharp
public enum TextStrikeType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Single | `0` | En enkel genomstrykning som tillämpas på texten. |
| Double | `1` | En dubbel genomstrykning som tillämpas på texten. Fungerar endast för text i former eller diagram. |
| None | `2` | Ingen genomstrykning tillämpas på texten. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TextStrikeTypeDemo
    {
        public static void TextStrikeTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            // Hämta referensen till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            // Åtkomst till cellen "A1" från kalkylbladet
            Cell cell = worksheet.Cells["A1"];
            // Lägger till ett värde i cellen "A1"
            cell.PutValue("Hello Aspose!");

            // Åtkomst till cellens teckensnitt
            Style style = cell.GetStyle();
            Font font = style.Font;

            // Ställer in genomstrykningstypen till Enkel
            font.StrikeType = TextStrikeType.Single;

            // Tillämpa stilen på cellen
            cell.SetStyle(style);

            // Spara arbetsboken
            workbook.Save("TextStrikeTypeExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


