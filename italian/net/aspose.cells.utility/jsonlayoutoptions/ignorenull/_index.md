---
title: "JsonLayoutOptions.IgnoreNull"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà JsonLayoutOptions. Indica se ignorare i valori null"
type: docs
url: /it/net/aspose.cells.utility/jsonlayoutoptions/ignorenull/
---
## JsonLayoutOptions.IgnoreNull property

Indica se ignorare i valori null.

```csharp
public bool IgnoreNull { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsPropertyIgnoreNullDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Esempio di JSON con valori null
            string json = @"{
                ""Name"": ""John"",
                ""Age"": 30,
                ""Address"": null,
                ""Salary"": 500.00
            }";

            // Configura le opzioni di importazione JSON con IgnoreNull impostato su true
            JsonLayoutOptions options = new JsonLayoutOptions();
            options.IgnoreNull = true;
            options.NumberFormat = "$0.00";

            // Importa dati JSON nel foglio di lavoro
            JsonUtility.ImportData(json, cells, 0, 0, options);

            // Verifica i dati importati (l'indirizzo null dovrebbe essere ignorato)
            Console.WriteLine("Name: " + cells["A2"].StringValue);    // John
            Console.WriteLine("Age: " + cells["B2"].IntValue);        // 30
            Console.WriteLine("Address exists: " + (cells["C2"].Value != null)); // False
            Console.WriteLine("Salary: " + cells["D2"].StringValue);  // $500.00

            // Salva la cartella di lavoro
            workbook.Save("JsonIgnoreNullDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


