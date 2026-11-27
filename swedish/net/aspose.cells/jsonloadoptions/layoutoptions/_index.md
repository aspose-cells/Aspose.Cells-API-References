---
title: "JsonLoadOptions.LayoutOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "JsonLoadOptions-egenskap. Alternativen för att importera JSON"
type: docs
url: /sv/net/aspose.cells/jsonloadoptions/layoutoptions/
---
## JsonLoadOptions.LayoutOptions property

Alternativen för import av JSON.

```csharp
public JsonLayoutOptions LayoutOptions { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLoadOptionsPropertyLayoutOptionsDemo
    {
        public static void Run()
        {
            // Skapa JSON-inläsningsalternativ med LayoutOptions
            JsonLoadOptions options = new JsonLoadOptions
            {
                LayoutOptions = new JsonLayoutOptions
                {
                    ArrayAsTable = true,
                    IgnoreNull = false,
                    ConvertNumericOrDate = true,
                    NumberFormat = "0.00",
                    DateFormat = "yyyy-MM-dd"
                }
            };

            // Skapa en ny arbetsbok med JSON-data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Exempel på JSON‑data
            string json = @"{
                ""Products"": [
                    { ""ID"": 1, ""Name"": ""Product A"", ""Price"": 19.99, ""Date"": ""2023-05-15"" },
                    { ""ID"": 2, ""Name"": ""Product B"", ""Price"": 29.99, ""Date"": ""2023-06-20"" }
                ]
            }";

            // Importera JSON till kalkylbladet
            JsonUtility.ImportData(json, worksheet.Cells, 0, 0, options.LayoutOptions);

            // Spara arbetsboken
            workbook.Save("JsonWithLayoutOptions.xlsx");
        }
    }
}
```

### Se även

* class [JsonLayoutOptions](../../../aspose.cells.utility/jsonlayoutoptions/)
* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


