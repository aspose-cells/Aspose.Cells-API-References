---
title: "Enum FontUnderlineType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.FontUnderlineType enum. Uppräkning av teckensnittets understrykningstyper"
type: docs
url: /sv/net/aspose.cells/fontunderlinetype/
---
## FontUnderlineType enumeration

Enumererar typsnittets understrykningsstilar.

```csharp
public enum FontUnderlineType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `0` | Representerar ingen understrykning. |
| Single | `1` | Representerar enkel understrykning. |
| Double | `2` | Representerar dubbel understrykning. |
| Accounting | `3` | Representerar enkel bokföringsunderstrykning. |
| DoubleAccounting | `4` | Representerar dubbel bokföringsunderstrykning. |
| Dash | `5` | Representerar streckad understrykning. |
| DashDotDotHeavy | `6` | Representerar tjock streck-punkt-punkt-understrykning. |
| DashDotHeavy | `7` | Representerar tjock streck-punkt-understrykning. |
| DashedHeavy | `8` | Representerar tjock streckad understrykning. |
| DashLong | `9` | Representerar lång streckad understrykning. |
| DashLongHeavy | `10` | Representerar tjock lång streckad understrykning. |
| DotDash | `11` | Representerar streck-punkt-understrykning. |
| DotDotDash | `12` | Representerar streck-punkt-punkt-understrykning. |
| Dotted | `13` | Representerar prickad understrykning |
| DottedHeavy | `14` | Representerar tjock prickad understrykning |
| Heavy | `15` | Representerar tjock understrykning |
| Wave | `16` | Representerar vågunderstrykning |
| WavyDouble | `17` | Representerar dubbel vågunderstrykning |
| WavyHeavy | `18` | Representerar kraftig vågunderstrykning |
| Words | `19` | Representerar understrykning av icke-mellanslagstecken. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontUnderlineTypeDemo
    {
        public static void FontUnderlineTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Hämta referensen till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Åtkomst till cellen "A1" från kalkylbladet
            Cell cell = worksheet.Cells["A1"];
            
            // Lägger till ett värde i cellen "A1"
            cell.PutValue("Hello Aspose!");

            // Hämta stil för cellen
            Style style = cell.GetStyle();
            
            // Ställ in teckensnittets understrykningstyp till enkel understrykning
            style.Font.Underline = FontUnderlineType.Single;
            
            // Tillämpa stilen på cellen
            cell.SetStyle(style);

            // Spara arbetsboken
            workbook.Save("FontUnderlineTypeExample.xlsx");
            workbook.Save("FontUnderlineTypeExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


