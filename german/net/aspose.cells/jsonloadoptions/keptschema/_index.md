---
title: "JsonLoadOptions.KeptSchema"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "JsonLoadOptions-Eigenschaft. Gibt an, ob das Schema dieses JSON beibehalten wird"
type: docs
url: /de/net/aspose.cells/jsonloadoptions/keptschema/
---
## JsonLoadOptions.KeptSchema property

Gibt an, ob das Schema dieses JSON beibehalten wird.

```csharp
public bool KeptSchema { get; set; }
```

### Hinweise

Manchmal speichern wir die Datei im JSON-Format, nachdem wir die JSON-Datei geladen haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class JsonLoadOptionsPropertyKeptSchemaDemo
    {
        public static void Run()
        {
            // JSON-Ladeoptionen erstellen
            JsonLoadOptions options = new JsonLoadOptions();

            // Den Standardwert der Eigenschaft KeptSchema anzeigen
            Console.WriteLine("Default KeptSchema value: " + options.KeptSchema);

            // KeptSchema auf true setzen
            options.KeptSchema = true;
            Console.WriteLine("KeptSchema set to: " + options.KeptSchema);

            // Beispiel-JSON-Datei erstellen
            string jsonData = @"{
                ""Employees"": [
                    { ""ID"": 1, ""Name"": ""John"", ""Department"": ""Sales"" },
                    { ""ID"": 2, ""Name"": ""Jane"", ""Department"": ""Marketing"" }
                ]
            }";

            System.IO.File.WriteAllText("sample.json", jsonData);

            try
            {
                // JSON mit aktiviertem KeptSchema laden
                Workbook workbook = new Workbook("sample.json", options);

                // Informationen über die geladene Arbeitsmappe anzeigen
                Console.WriteLine("Workbook loaded with KeptSchema: " + options.KeptSchema);
                Console.WriteLine("Number of worksheets: " + workbook.Worksheets.Count);

                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


