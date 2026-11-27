---
title: "JsonLayoutOptions.ArrayAsTable"
second_title: "Aspose.Cells för .NET API‑referens"
description: "JsonLayoutOptions-egenskap. Behandlar array som tabell"
type: docs
url: /sv/net/aspose.cells.utility/jsonlayoutoptions/arrayastable/
---
## JsonLayoutOptions.ArrayAsTable property

Bearbetar array som tabell.

```csharp
public bool ArrayAsTable { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsPropertyArrayAsTableDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok och öppna det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Skapa JSON-layoutalternativ och sätt ArrayAsTable till true
            JsonLayoutOptions options = new JsonLayoutOptions();
            options.ArrayAsTable = true;
            options.IgnoreTitle = true;

            // Exempel på JSON-data (förenklad för demonstration)
            string jsonData = @"{
                ""products"": [
                    {""id"":1, ""name"":""Laptop"", ""price"":999.99},
                    {""id"":2, ""name"":""Phone"", ""price"":599.99}
                ]
            }";

            // Importera JSON‑data till kalkylblad
            JsonUtility.ImportData(jsonData, sheet.Cells, 0, 0, options);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


