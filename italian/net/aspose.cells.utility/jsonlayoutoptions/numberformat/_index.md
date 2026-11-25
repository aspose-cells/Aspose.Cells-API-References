---
title: "JsonLayoutOptions.NumberFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà JsonLayoutOptions. Ottiene e imposta il formato del valore numerico"
type: docs
url: /it/net/aspose.cells.utility/jsonlayoutoptions/numberformat/
---
## JsonLayoutOptions.NumberFormat property

Ottiene e imposta il formato del valore numerico.

```csharp
public string NumberFormat { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsPropertyNumberFormatDemo
    {
        public static void Run()
        {
            // Crea stringa di dati JSON
            string jsonData = @"{
                ""Products"": [
                    { ""ID"": 101, ""Price"": 19.95, ""Date"": ""2023-05-15"" },
                    { ""ID"": 102, ""Price"": 29.99, ""Date"": ""2023-06-20"" }
                ]
            }";

            // Crea JsonLayoutOptions con NumberFormat
            JsonLayoutOptions layoutOptions = new JsonLayoutOptions
            {
                ArrayAsTable = true,
                NumberFormat = "0.00",
                DateFormat = "yyyy-MM-dd"
            };

            // Crea cartella di lavoro da JSON
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue(jsonData);
            JsonUtility.ImportData(jsonData, workbook.Worksheets[0].Cells, 0, 0, layoutOptions);

            // Salva in Excel
            workbook.Save("JsonNumberFormatDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


