---
title: "JsonLoadOptions.MultipleWorksheets"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà JsonLoadOptions. Indica se importare ogni attributo dell'oggetto JsonObject come un worksheet quando tutti i nodi figli sono nodi array"
type: docs
url: /it/net/aspose.cells/jsonloadoptions/multipleworksheets/
---
## JsonLoadOptions.MultipleWorksheets property

Indica se importare ogni attributo dell'oggetto JsonObject come un foglio di lavoro quando tutti i nodi figlio sono nodi array.

```csharp
public bool MultipleWorksheets { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonLoadOptionsPropertyMultipleWorksheetsDemo
    {
        public static void Run()
        {
            // Crea opzioni di caricamento JSON con MultipleWorksheets abilitato
            JsonLoadOptions options = new JsonLoadOptions { MultipleWorksheets = true };
            
            // Carica il file JSON nel workbook con le opzioni specificate
            Workbook workbook = new Workbook("example.json", options);
            
            // Accedi ai dati dal primo worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Visualizza alcuni valori di esempio dal JSON caricato
            Console.WriteLine("D5 cell value: " + cells["D5"].StringValue);
            Console.WriteLine("E5 cell value: " + cells["E5"].StringValue);
            Console.WriteLine("D7 cell value: " + cells["D7"].StringValue);
            Console.WriteLine("B14 cell value: " + cells["B14"].StringValue);
        }
    }
}
```

### Vedi anche

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


