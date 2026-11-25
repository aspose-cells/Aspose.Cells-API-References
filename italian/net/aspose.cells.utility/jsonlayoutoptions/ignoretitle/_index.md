---
title: "JsonLayoutOptions.IgnoreTitle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà JsonLayoutOptions. Ignora i titoli degli attributi"
type: docs
url: /it/net/aspose.cells.utility/jsonlayoutoptions/ignoretitle/
---
## JsonLayoutOptions.IgnoreTitle property

Ignora i titoli degli attributi

```csharp
public bool IgnoreTitle { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsPropertyIgnoreTitleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Dati JSON di esempio
            string jsonInput = @"{
                ""Products"": [
                    {
                        ""Name"": ""Product1"",
                        ""Price"": 100,
                        ""Date"": ""2023-01-15""
                    },
                    {
                        ""Name"": ""Product2"",
                        ""Price"": 200,
                        ""Date"": ""2023-02-20""
                    }
                ]
            }";

            // Imposta JsonLayoutOptions con IgnoreTitle = true
            JsonLayoutOptions options = new JsonLayoutOptions();
            options.IgnoreTitle = true;  // This will skip the title row in output
            options.ArrayAsTable = true;
            options.DateFormat = "yyyy/MM/dd";

            // Importa dati JSON
            JsonUtility.ImportData(jsonInput, worksheet.Cells, 0, 0, options);

            // Salva la cartella di lavoro
            workbook.Save("output_ignore_title.xlsx");
        }
    }
}
```

### Vedi anche

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


