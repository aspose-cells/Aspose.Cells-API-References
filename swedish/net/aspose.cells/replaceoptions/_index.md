---
title: "Klass ReplaceOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ReplaceOptions klass. Representerar ersättningsalternativen"
type: docs
url: /sv/net/aspose.cells/replaceoptions/
---
## ReplaceOptions class

Representerar ersättningsalternativen.

```csharp
public class ReplaceOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [ReplaceOptions](replaceoptions/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [CaseSensitive](../../aspose.cells/replaceoptions/casesensitive/) { get; set; } | Indikerar om den sökta strängen är skiftlägeskänslig. |
| [FontSettings](../../aspose.cells/replaceoptions/fontsettings/) { get; set; } | De rikligt formaterade inställningarna för den ersatta texten. |
| [MatchEntireCellContents](../../aspose.cells/replaceoptions/matchentirecellcontents/) { get; set; } | Anger om hela cellinnehållet ska matchas |
| [RegexKey](../../aspose.cells/replaceoptions/regexkey/) { get; set; } | Anger om den sökta nyckeln är regex. Om true så kommer den sökta nyckeln att behandlas som regex. |
| [StyleFlags](../../aspose.cells/replaceoptions/styleflags/) { get; set; } | Hämtar och anger flaggor för att tillämpa teckensnittsinställningar. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ReplaceOptionsDemo
    {
        public static void ReplaceOptionsExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata i kalkylbladet
            sheet.Cells["A1"].PutValue("Hello World");
            sheet.Cells["A2"].PutValue("Hello Aspose");
            sheet.Cells["A3"].PutValue("Goodbye World");

            // Skapa ReplaceOptions
            ReplaceOptions options = new ReplaceOptions
            {
                CaseSensitive = false,
                MatchEntireCellContents = false,
                RegexKey = false
            };

            // Ersätt "Hello" med "Hi" i kalkylbladet
            int replacedCount = workbook.Replace("Hello", "Hi", options);

            // Skriv ut antalet utförda ersättningar
            Console.WriteLine($"Number of replacements made: {replacedCount}");

            // Spara arbetsboken
            workbook.Save("ReplaceOptionsExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


