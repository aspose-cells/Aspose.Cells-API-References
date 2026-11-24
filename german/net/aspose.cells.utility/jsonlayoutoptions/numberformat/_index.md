---
title: "JsonLayoutOptions.NumberFormat"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "JsonLayoutOptions-Eigenschaft. Liest und setzt das Format des numerischen Werts."
type: docs
url: /de/net/aspose.cells.utility/jsonlayoutoptions/numberformat/
---
## JsonLayoutOptions.NumberFormat property

Liest und setzt das Format des numerischen Werts.

```csharp
public string NumberFormat { get; set; }
```

### Beispiele

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
            // JSON-Datenzeichenfolge erstellen
            string jsonData = @"{
                ""Products"": [
                    { ""ID"": 101, ""Price"": 19.95, ""Date"": ""2023-05-15"" },
                    { ""ID"": 102, ""Price"": 29.99, ""Date"": ""2023-06-20"" }
                ]
            }";

            // JsonLayoutOptions mit NumberFormat erstellen
            JsonLayoutOptions layoutOptions = new JsonLayoutOptions
            {
                ArrayAsTable = true,
                NumberFormat = "0.00",
                DateFormat = "yyyy-MM-dd"
            };

            // Arbeitsmappe aus JSON erstellen
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue(jsonData);
            JsonUtility.ImportData(jsonData, workbook.Worksheets[0].Cells, 0, 0, layoutOptions);

            // In Excel speichern
            workbook.Save("JsonNumberFormatDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


