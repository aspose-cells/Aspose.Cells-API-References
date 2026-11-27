---
title: "Enum AutoFillType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.AutoFillType‑enum. Representerar autofyll‑typen"
type: docs
url: /sv/net/aspose.cells/autofilltype/
---
## AutoFillType enumeration

Representerar autofyll-typen.

```csharp
public enum AutoFillType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Copy | `1` | Kopierar värdet och formatet från källområdet till målområdet |
| Default | `0` | Fyller automatiskt målområdet med värdet och formatet. |
| Formats | `3` | Kopierar endast formatet från källområdet till målområdet. |
| Series | `2` | Utöka värdet i källområdet till målområdet i form av en serie och kopiera formatet till målområdet. |
| Values | `4` | Kopierar endast värdet från källområdet till målområdet. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFillTypeDemo
    {
        public static void AutoFillTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa ett område (A1:A10) och fyll det med några värden
            Aspose.Cells.Range sourceRange = worksheet.Cells.CreateRange("A1:A10");
            for (int i = 0; i < 10; i++)
            {
                sourceRange[i, 0].PutValue(i + 1);
            }

            // Skapa ett målområde (B1:B10)
            Aspose.Cells.Range targetRange = worksheet.Cells.CreateRange("B1:B10");

            //Serietypfel, ärendet har skapats
            // Använd AutoFill-metoden med AutoFillType.Series för att fylla målområdet
            //sourceRange.AutoFill(targetRange, AutoFillType.Series);

            // Använd AutoFill-metoden med AutoFillType.Copy för att fylla målområdet
            sourceRange.AutoFill(targetRange, AutoFillType.Copy);
            // Spara arbetsboken
            workbook.Save("AutoFillTypeExample.xlsx");
            workbook.Save("AutoFillTypeExample.pdf");
        }
    }

}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


