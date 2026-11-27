---
title: "JsonLoadOptions.StartCell"
second_title: "Aspose.Cells för .NET API‑referens"
description: "JsonLoadOptions-egenskap. Hämtar och anger startcellen"
type: docs
url: /sv/net/aspose.cells/jsonloadoptions/startcell/
---
## JsonLoadOptions.StartCell property

Hämtar och anger startcellen.

```csharp
public string StartCell { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonLoadOptionsPropertyStartCellDemo
    {
        public static void Run()
        {
            // Skapa JSON-inläsningsalternativ med StartCell-egenskapen
            JsonLoadOptions options = new JsonLoadOptions
            {
                StartCell = "B3" // JSON data will start from cell B3
            };

            // Skapa en arbetsbok från JSON-fil med alternativ
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("Header");
            
            // Skapa en exempel-JSON-fil
            System.IO.File.WriteAllText("data.json", "{\"Name\":\"John\",\"Age\":30,\"City\":\"New York\"}");
            
            // Läs in JSON-data i arbetsboken
            workbook = new Workbook("data.json", options);

            // Spara arbetsboken
            workbook.Save("JsonStartCellDemo.xlsx");
        }
    }
}
```

### Se även

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


