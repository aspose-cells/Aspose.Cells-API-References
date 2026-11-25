---
title: "JsonLayoutOptions.ArrayAsTable"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà JsonLayoutOptions. Elabora l'Array come tabella"
type: docs
url: /it/net/aspose.cells.utility/jsonlayoutoptions/arrayastable/
---
## JsonLayoutOptions.ArrayAsTable property

Elabora l'Array come tabella.

```csharp
public bool ArrayAsTable { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsPropertyArrayAsTableDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro e accedi al primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Crea opzioni di layout JSON e imposta ArrayAsTable su true
            JsonLayoutOptions options = new JsonLayoutOptions();
            options.ArrayAsTable = true;
            options.IgnoreTitle = true;

            // Esempio di dati JSON (semplificato per dimostrazione)
            string jsonData = @"{
                ""products"": [
                    {""id"":1, ""name"":""Laptop"", ""price"":999.99},
                    {""id"":2, ""name"":""Phone"", ""price"":599.99}
                ]
            }";

            // Importa dati JSON nel foglio di lavoro
            JsonUtility.ImportData(jsonData, sheet.Cells, 0, 0, options);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


