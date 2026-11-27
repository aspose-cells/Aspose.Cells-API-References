---
title: "JsonLayoutOptions.NumberFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "JsonLayoutOptions‑egenskap. Hämtar och anger formatet för numeriska värden"
type: docs
url: /sv/net/aspose.cells.utility/jsonlayoutoptions/numberformat/
---
## JsonLayoutOptions.NumberFormat property

Hämtar och anger formatet för numeriskt värde.

```csharp
public string NumberFormat { get; set; }
```

### Exempel

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
            // Skapa JSON‑datasträng
            string jsonData = @"{
                ""Products"": [
                    { ""ID"": 101, ""Price"": 19.95, ""Date"": ""2023-05-15"" },
                    { ""ID"": 102, ""Price"": 29.99, ""Date"": ""2023-06-20"" }
                ]
            }";

            // Skapa JsonLayoutOptions med NumberFormat
            JsonLayoutOptions layoutOptions = new JsonLayoutOptions
            {
                ArrayAsTable = true,
                NumberFormat = "0.00",
                DateFormat = "yyyy-MM-dd"
            };

            // Skapa arbetsbok från JSON
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue(jsonData);
            JsonUtility.ImportData(jsonData, workbook.Worksheets[0].Cells, 0, 0, layoutOptions);

            // Spara till Excel
            workbook.Save("JsonNumberFormatDemo.xlsx");
        }
    }
}
```

### Se även

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


