---
title: "Enum TextCapsType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.TextCapsType-enum. Denna typ specificerar versaltyperna för texten"
type: docs
url: /sv/net/aspose.cells/textcapstype/
---
## TextCapsType enumeration

Denna typ specificerar versaltyper för texten.

```csharp
public enum TextCapsType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `0` | Ingen versal |
| All | `1` | Applicera versaler på texten. |
| Small | `2` | Applicera små versaler på texten. |

### Anmärkningar

Kan endast tillämpas på diagram och form.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TextCapsTypeDemo
    {
        public static void TextCapsTypeExample()
        {
            // Ytterligare kod för att demonstrera hur instansen kan användas
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ange ett cellvärde
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Hello Aspose!");

            // Hämta cellens stil
            Style style = cell.GetStyle();

            // Ange teckensnittets versaltyp till Alla versaler
            style.Font.CapsType = Aspose.Cells.TextCapsType.All;

            // Tillämpa stilen på cellen
            cell.SetStyle(style);

            // Spara arbetsboken
            workbook.Save("TextCapsTypeExample.xlsx");

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


