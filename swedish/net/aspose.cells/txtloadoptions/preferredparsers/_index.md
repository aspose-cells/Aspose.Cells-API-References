---
title: "TxtLoadOptions.PreferredParsers"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TxtLoadOptions-egenskap. Hämtar och sätter föredragna värdetolkar för inläsning av textfil"
type: docs
url: /sv/net/aspose.cells/txtloadoptions/preferredparsers/
---
## TxtLoadOptions.PreferredParsers property

Hämtar och anger föredragna värde‑tolkare för att läsa in textfil.

```csharp
public ICustomParser[] PreferredParsers { get; set; }
```

### Anmärkningar

parsers[0] är den parser som kommer att användas för den första kolumnen i textmallfilen, parsers[1] är den parser som kommer att användas för den andra kolumnen, ...etc. Den sista (parsers[parsers.length-1]) kommer att användas för alla andra kolumner med start från parsers.length-1. Om ett objekt är null kommer motsvarande kolumn att tolkas av standard‑parsern för Aspose.Cells.

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyPreferredParsersDemo
    {
        private class StringParser : ICustomParser
        {
            public bool Parse(string value, out object result)
            {
                result = value; // Always return as string
                return true;
            }

            public object ParseObject(string value)
            {
                return value; // Always return as string
            }

            public string GetFormat()
            {
                return "String"; // Return format description
            }
        }

        public static void Run()
        {
            // Skapa CSV-läsalternativ
            TxtLoadOptions options = new TxtLoadOptions(LoadFormat.Csv);
            
            // Ange föredragna parserar – prova först anpassad strängparser, sedan standardparserar
            options.PreferredParsers = new ICustomParser[] { new StringParser(), null };

            // Exempel på CSV-data med datum
            string csvData = "\"2018-10-08\",2018-10-08\n\"2018-10-08\",2018-10-08";
            
            // Läs in arbetsbok med alternativ
            Workbook workbook = new Workbook(new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData)), options);
            Cells cells = workbook.Worksheets[0].Cells;

            // Verifiera parsresultat
            Console.WriteLine("A1 Type: " + cells[0, 0].Type); // Should be string
            Console.WriteLine("A1 Value: " + cells[0, 0].StringValue); // "2018-10-08"
            Console.WriteLine("B1 Type: " + cells[0, 1].Type); // Should be DateTime
            Console.WriteLine("B1 Value: " + cells[0, 1].DateTimeValue); // 10/8/2018
        }
    }
}
```

### Se även

* interface [ICustomParser](../../icustomparser/)
* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


