---
title: "JsonLoadOptions.LayoutOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "JsonLoadOptions-Eigenschaft. Die Optionen für den Import von JSON"
type: docs
url: /de/net/aspose.cells/jsonloadoptions/layoutoptions/
---
## JsonLoadOptions.LayoutOptions property

Die Optionen für den JSON-Import.

```csharp
public JsonLayoutOptions LayoutOptions { get; set; }
```

### Beispiele

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
            // JSON-Ladeoptionen mit LayoutOptions erstellen
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

            // Neue Arbeitsmappe mit JSON-Daten erstellen
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten für JSON
            string json = @"{
                ""Products"": [
                    { ""ID"": 1, ""Name"": ""Product A"", ""Price"": 19.99, ""Date"": ""2023-05-15"" },
                    { ""ID"": 2, ""Name"": ""Product B"", ""Price"": 29.99, ""Date"": ""2023-06-20"" }
                ]
            }";

            // JSON in ein Arbeitsblatt importieren
            JsonUtility.ImportData(json, worksheet.Cells, 0, 0, options.LayoutOptions);

            // Speichere die Arbeitsmappe
            workbook.Save("JsonWithLayoutOptions.xlsx");
        }
    }
}
```

### Siehe auch

* class [JsonLayoutOptions](../../../aspose.cells.utility/jsonlayoutoptions/)
* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


