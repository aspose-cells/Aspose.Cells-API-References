---
title: "ReplaceOptions.MatchEntireCellContents"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ReplaceOptions egenskap. Anger om hela cellinnehållet ska matchas"
type: docs
url: /sv/net/aspose.cells/replaceoptions/matchentirecellcontents/
---
## ReplaceOptions.MatchEntireCellContents property

Anger om hela cellinnehållet ska matchas

```csharp
public bool MatchEntireCellContents { get; set; }
```

### Anmärkningar

Standardvärdet är sant.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReplaceOptionsPropertyMatchEntireCellContentsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ange exempelcellvärden
            worksheet.Cells["A1"].PutValue("apple");
            worksheet.Cells["A2"].PutValue("apple pie");
            worksheet.Cells["A3"].PutValue("an apple");
            worksheet.Cells["A4"].PutValue("apples");

            // Ersätt med MatchEntireCellContents = true (endast exakt matchning)
            ReplaceOptions options1 = new ReplaceOptions();
            options1.MatchEntireCellContents = true;
            workbook.Replace("apple", "orange", options1);

            // Ersätt med MatchEntireCellContents = false (delvis matchning)
            ReplaceOptions options2 = new ReplaceOptions();
            options2.MatchEntireCellContents = false;
            workbook.Replace("apple", "banana", options2);

            // Skriv ut resultat
            Console.WriteLine("A1: " + worksheet.Cells["A1"].StringValue); // orange (exact match)
            Console.WriteLine("A2: " + worksheet.Cells["A2"].StringValue); // banana pie (partial match)
            Console.WriteLine("A3: " + worksheet.Cells["A3"].StringValue); // an banana (partial match)
            Console.WriteLine("A4: " + worksheet.Cells["A4"].StringValue); // bananas (partial match)
        }
    }
}
```

### Se även

* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


