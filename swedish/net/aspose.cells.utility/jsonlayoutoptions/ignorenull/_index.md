---
title: "JsonLayoutOptions.IgnoreNull"
second_title: "Aspose.Cells för .NET API‑referens"
description: "JsonLayoutOptions‑egenskap. Anger om null‑värden ska ignoreras"
type: docs
url: /sv/net/aspose.cells.utility/jsonlayoutoptions/ignorenull/
---
## JsonLayoutOptions.IgnoreNull property

Anger om null‑värde ska ignoreras.

```csharp
public bool IgnoreNull { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsPropertyIgnoreNullDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Exempel‑JSON med null‑värden
            string json = @"{
                ""Name"": ""John"",
                ""Age"": 30,
                ""Address"": null,
                ""Salary"": 500.00
            }";

            // Konfigurera JSON‑importalternativ med IgnoreNull satt till true
            JsonLayoutOptions options = new JsonLayoutOptions();
            options.IgnoreNull = true;
            options.NumberFormat = "$0.00";

            // Importera JSON‑data till kalkylblad
            JsonUtility.ImportData(json, cells, 0, 0, options);

            // Verifiera den importerade datan (null‑Adress bör ignoreras)
            Console.WriteLine("Name: " + cells["A2"].StringValue);    // John
            Console.WriteLine("Age: " + cells["B2"].IntValue);        // 30
            Console.WriteLine("Address exists: " + (cells["C2"].Value != null)); // False
            Console.WriteLine("Salary: " + cells["D2"].StringValue);  // $500.00

            // Spara arbetsboken
            workbook.Save("JsonIgnoreNullDemo.xlsx");
        }
    }
}
```

### Se även

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


