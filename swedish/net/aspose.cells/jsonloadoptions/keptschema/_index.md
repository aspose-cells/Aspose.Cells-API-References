---
title: "JsonLoadOptions.KeptSchema"
second_title: "Aspose.Cells för .NET API‑referens"
description: "JsonLoadOptions-egenskap. Anger om schemat för denna JSON ska behållas"
type: docs
url: /sv/net/aspose.cells/jsonloadoptions/keptschema/
---
## JsonLoadOptions.KeptSchema property

Anger om schemat för denna JSON ska behållas.

```csharp
public bool KeptSchema { get; set; }
```

### Anmärkningar

Ibland sparar vi filen till JSON efter att ha läst in JSON-filen.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class JsonLoadOptionsPropertyKeptSchemaDemo
    {
        public static void Run()
        {
            // Skapa JSON-inläsningsalternativ
            JsonLoadOptions options = new JsonLoadOptions();

            // Visa standardvärdet för KeptSchema-egenskapen
            Console.WriteLine("Default KeptSchema value: " + options.KeptSchema);

            // Ställ in KeptSchema till true
            options.KeptSchema = true;
            Console.WriteLine("KeptSchema set to: " + options.KeptSchema);

            // Skapa en exempel-JSON-fil
            string jsonData = @"{
                ""Employees"": [
                    { ""ID"": 1, ""Name"": ""John"", ""Department"": ""Sales"" },
                    { ""ID"": 2, ""Name"": ""Jane"", ""Department"": ""Marketing"" }
                ]
            }";

            System.IO.File.WriteAllText("sample.json", jsonData);

            try
            {
                // Läs in JSON med KeptSchema aktiverat
                Workbook workbook = new Workbook("sample.json", options);

                // Visa information om den inlästa arbetsboken
                Console.WriteLine("Workbook loaded with KeptSchema: " + options.KeptSchema);
                Console.WriteLine("Number of worksheets: " + workbook.Worksheets.Count);

                // Spara arbetsboken
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

### Se även

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


