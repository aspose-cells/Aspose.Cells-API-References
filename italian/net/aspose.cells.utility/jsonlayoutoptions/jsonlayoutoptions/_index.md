---
title: "JsonLayoutOptions.JsonLayoutOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore JsonLayoutOptions. Costruttore per il caricamento delle opzioni di layout JSON"
type: docs
url: /it/net/aspose.cells.utility/jsonlayoutoptions/jsonlayoutoptions/
---
## JsonLayoutOptions constructor

Costruttore per il caricamento delle opzioni di layout JSON.

```csharp
public JsonLayoutOptions()
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crea dati JSON di esempio
            string json = @"{
                ""Name"": ""John"",
                ""Age"": 30,
                ""Address"": {
                    ""Street"": ""123 Main St"",
                    ""City"": ""New York""
                }
            }";

            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Inizializza JsonLayoutOptions usando il costruttore
            JsonLayoutOptions options = new JsonLayoutOptions();
            
            // Imposta le opzioni
            options.ArrayAsTable = true;
            options.IgnoreArrayTitle = false;
            options.IgnoreObjectTitle = false;

            // Importa dati JSON nel foglio di lavoro
            JsonUtility.ImportData(json, workbook.Worksheets[0].Cells, 0, 0, options);

            // Salva la cartella di lavoro
            workbook.Save("JsonImportDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


