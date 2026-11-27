---
title: "ReplaceOptions.RegexKey"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ReplaceOptions-egenskap. Anger om den sökta nyckeln är regex. Om true tas den sökta nyckeln som regex"
type: docs
url: /sv/net/aspose.cells/replaceoptions/regexkey/
---
## ReplaceOptions.RegexKey property

Anger om den sökta nyckeln är regex. Om true så kommer den sökta nyckeln att behandlas som regex.

```csharp
public bool RegexKey { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReplaceOptionsPropertyRegexKeyDemo
    {
        public static void Run()
        {
            // Skapa arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("apple");
            worksheet.Cells["A2"].PutValue("banana");
            worksheet.Cells["A3"].PutValue("orange");
            worksheet.Cells["A4"].PutValue("pear");
            worksheet.Cells["A5"].PutValue("plum");

            // Skapa ersättningsalternativ med regex
            ReplaceOptions options = new ReplaceOptions();
            options.RegexKey = true; // Enable regex matching
            
            // Ersätt alla ord som börjar med 'p' eller 'b' följt av en vokal
            string pattern = "^[pb][aeiou]";
            string replacement = "FRUIT";
            
            // Utför ersättningen
            workbook.Replace(pattern, replacement, options);

            // Spara resultatet
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


