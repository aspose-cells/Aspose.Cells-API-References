---
title: "JsonLoadOptions.MultipleWorksheets"
second_title: "Aspose.Cells för .NET API‑referens"
description: "JsonLoadOptions-egenskap. Anger om varje attribut i JsonObject-objektet ska importeras som ett kalkylblad när alla barnnoder är arraynoder"
type: docs
url: /sv/net/aspose.cells/jsonloadoptions/multipleworksheets/
---
## JsonLoadOptions.MultipleWorksheets property

Anger om varje attribut i JsonObject‑objektet ska importeras som ett kalkylblad när alla undernoder är arraynoder.

```csharp
public bool MultipleWorksheets { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonLoadOptionsPropertyMultipleWorksheetsDemo
    {
        public static void Run()
        {
            // Skapa JSON-inläsningsalternativ med MultipleWorksheets aktiverat
            JsonLoadOptions options = new JsonLoadOptions { MultipleWorksheets = true };
            
            // Läs in JSON-fil i arbetsboken med de angivna alternativen
            Workbook workbook = new Workbook("example.json", options);
            
            // Åtkomst till data från det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Visa några exempelvärden från den inlästa JSON
            Console.WriteLine("D5 cell value: " + cells["D5"].StringValue);
            Console.WriteLine("E5 cell value: " + cells["E5"].StringValue);
            Console.WriteLine("D7 cell value: " + cells["D7"].StringValue);
            Console.WriteLine("B14 cell value: " + cells["B14"].StringValue);
        }
    }
}
```

### Se även

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


