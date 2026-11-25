---
title: "JsonLoadOptions.KeptSchema"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà JsonLoadOptions. Indica se mantenere lo schema di questo JSON"
type: docs
url: /it/net/aspose.cells/jsonloadoptions/keptschema/
---
## JsonLoadOptions.KeptSchema property

Indica se mantenere lo schema di questo JSON.

```csharp
public bool KeptSchema { get; set; }
```

### Osservazioni

A volte salveremo il file in JSON dopo aver caricato il file JSON.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class JsonLoadOptionsPropertyKeptSchemaDemo
    {
        public static void Run()
        {
            // Crea opzioni di caricamento JSON
            JsonLoadOptions options = new JsonLoadOptions();

            // Mostra il valore predefinito della proprietà KeptSchema
            Console.WriteLine("Default KeptSchema value: " + options.KeptSchema);

            // Imposta KeptSchema su true
            options.KeptSchema = true;
            Console.WriteLine("KeptSchema set to: " + options.KeptSchema);

            // Crea un file JSON di esempio
            string jsonData = @"{
                ""Employees"": [
                    { ""ID"": 1, ""Name"": ""John"", ""Department"": ""Sales"" },
                    { ""ID"": 2, ""Name"": ""Jane"", ""Department"": ""Marketing"" }
                ]
            }";

            System.IO.File.WriteAllText("sample.json", jsonData);

            try
            {
                // Carica JSON con KeptSchema abilitato
                Workbook workbook = new Workbook("sample.json", options);

                // Mostra informazioni sul workbook caricato
                Console.WriteLine("Workbook loaded with KeptSchema: " + options.KeptSchema);
                Console.WriteLine("Number of worksheets: " + workbook.Worksheets.Count);

                // Salva la cartella di lavoro
                workbook.Save("KeptSchemaOutput.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


