---
title: "JsonLoadOptions.LayoutOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà JsonLoadOptions. Le opzioni di importazione JSON"
type: docs
url: /it/net/aspose.cells/jsonloadoptions/layoutoptions/
---
## JsonLoadOptions.LayoutOptions property

Le opzioni di importazione JSON.

```csharp
public JsonLayoutOptions LayoutOptions { get; set; }
```

### Esempi

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
            // Crea opzioni di caricamento JSON con LayoutOptions
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

            // Crea un nuovo workbook con dati JSON
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Dati JSON di esempio
            string json = @"{
                ""Products"": [
                    { ""ID"": 1, ""Name"": ""Product A"", ""Price"": 19.99, ""Date"": ""2023-05-15"" },
                    { ""ID"": 2, ""Name"": ""Product B"", ""Price"": 29.99, ""Date"": ""2023-06-20"" }
                ]
            }";

            // Importa JSON nel worksheet
            JsonUtility.ImportData(json, worksheet.Cells, 0, 0, options.LayoutOptions);

            // Salva la cartella di lavoro
            workbook.Save("JsonWithLayoutOptions.xlsx");
        }
    }
}
```

### Vedi anche

* class [JsonLayoutOptions](../../../aspose.cells.utility/jsonlayoutoptions/)
* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


