---
title: "FindOptions.RegexKey"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FindOptions-egenskap. Anger om den sökta nyckeln är regex. Om true kommer den sökta nyckeln att behandlas som regex och tolkas. Annars kommer nyckeln att tolkas enligt reglerna i MS Excel"
type: docs
url: /sv/net/aspose.cells/findoptions/regexkey/
---
## FindOptions.RegexKey property

Anger om den sökta nyckeln är ett regex. Om true kommer den sökta nyckeln att behandlas som regex och tolkas. Annars kommer nyckeln att tolkas enligt reglerna i MS Excel.

```csharp
public bool RegexKey { get; set; }
```

### Anmärkningar

Även om söknyckeln har angetts som regex kan den omformas enligt den specificerade [`LookAtType`](../lookattype/). Till exempel, när typen är Contains (detta är standardvärdet för dessa alternativ) kommer jokertecken att läggas till i början och slutet av söknyckeln automatiskt för att säkerställa att matchningen kontrolleras som \"contains\". I detta fall blir de reguljära uttrycken mer komplexa och prestandan minskar också. Så, med prestanda i åtanke, om användaren har specificerat den exakta regeln för regex, finns det ingen anledning att använda [`LookAtType`](../lookattype/) som ett extra villkor och användaren kan sätta den till EntireContent för att få bättre prestanda.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyRegexKeyDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ställ in testdata med mönstermatchande strängar
            worksheet.Cells["A1"].PutValue("[hello]");
            worksheet.Cells["A2"].PutValue("Regular text");
            worksheet.Cells["A3"].PutValue("[another_example]");

            // Skapa sökalternativ med regex aktiverat
            FindOptions options = new FindOptions();
            options.RegexKey = true;
            options.LookInType = LookInType.Values;
            options.LookAtType = LookAtType.Contains;

            // Sök efter celler som matchar regex-mönstret
            string regEx = "\\[[a-zA-Z0-9_]+\\]";
            Cell foundCell = worksheet.Cells.Find(regEx, null, options);

            // Skriv ut resultatet
            if (foundCell != null)
            {
                Console.WriteLine("Found cell: " + foundCell.Name + " with value: " + foundCell.StringValue);
            }
            else
            {
                Console.WriteLine("No matching cells found");
            }
        }
    }
}
```

### Se även

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


