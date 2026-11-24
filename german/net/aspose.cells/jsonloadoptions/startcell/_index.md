---
title: "JsonLoadOptions.StartCell"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "JsonLoadOptions-Eigenschaft. Liest und setzt die Startzelle"
type: docs
url: /de/net/aspose.cells/jsonloadoptions/startcell/
---
## JsonLoadOptions.StartCell property

Liest und setzt die Startzelle.

```csharp
public string StartCell { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonLoadOptionsPropertyStartCellDemo
    {
        public static void Run()
        {
            // JSON-Ladeoptionen mit der StartCell-Eigenschaft erstellen
            JsonLoadOptions options = new JsonLoadOptions
            {
                StartCell = "B3" // JSON data will start from cell B3
            };

            // Arbeitsmappe aus JSON-Datei mit Optionen erstellen
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("Header");
            
            // Beispiel-JSON-Datei erstellen
            System.IO.File.WriteAllText("data.json", "{\"Name\":\"John\",\"Age\":30,\"City\":\"New York\"}");
            
            // JSON-Daten in Arbeitsmappe laden
            workbook = new Workbook("data.json", options);

            // Speichere die Arbeitsmappe
            workbook.Save("JsonStartCellDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


