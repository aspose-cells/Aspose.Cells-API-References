---
title: "JsonLoadOptions.StartCell"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà JsonLoadOptions. Ottiene e imposta la cella di partenza"
type: docs
url: /it/net/aspose.cells/jsonloadoptions/startcell/
---
## JsonLoadOptions.StartCell property

Ottiene e imposta la cella iniziale.

```csharp
public string StartCell { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonLoadOptionsPropertyStartCellDemo
    {
        public static void Run()
        {
            // Crea opzioni di caricamento JSON con la proprietà StartCell
            JsonLoadOptions options = new JsonLoadOptions
            {
                StartCell = "B3" // JSON data will start from cell B3
            };

            // Crea un workbook da un file JSON con opzioni
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("Header");
            
            // Crea un file JSON di esempio
            System.IO.File.WriteAllText("data.json", "{\"Name\":\"John\",\"Age\":30,\"City\":\"New York\"}");
            
            // Carica dati JSON nel workbook
            workbook = new Workbook("data.json", options);

            // Salva la cartella di lavoro
            workbook.Save("JsonStartCellDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


