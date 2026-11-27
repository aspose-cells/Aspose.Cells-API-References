---
title: "Cell.Replace"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell metod. Ersätt texten i cellen med alternativ"
type: docs
url: /sv/net/aspose.cells/cell/replace/
---
## Cell.Replace method

Ersätt cellens text med alternativ.

```csharp
public void Replace(string placeHolder, string newValue, ReplaceOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| platshållare | String | Cellplatshållare |
| nyttVärde | String | Strängvärde att ersätta |
| alternativ | ReplaceOptions | Ersättningsalternativen |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodReplaceWithStringStringReplaceOptionsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Hello World");
            worksheet.Cells["A2"].PutValue("hello world");
            worksheet.Cells["A3"].PutValue("HELLO WORLD");
            worksheet.Cells["B1"].PutValue("Replaced");

            // Skapa ersättningsalternativ
            ReplaceOptions options = new ReplaceOptions();
            options.CaseSensitive = false;
            options.MatchEntireCellContents = false;

            // Hämta teckensnittinställningar från cell B1 för att tillämpa på ersättningar
            options.FontSettings = worksheet.Cells["B1"].GetCharacters();

            // Ersätt alla varianter av "hello" med "Hi" med hjälp av alternativen
            foreach (Cell cell in worksheet.Cells)
            {
                cell.Replace("Hello", "Hi", options);
            }

            // Spara arbetsboken
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [ReplaceOptions](../../replaceoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


