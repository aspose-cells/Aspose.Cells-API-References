---
title: JsonLoadOptions.KeptSchema
second_title: Aspose.Cells for .NET API Reference
description: JsonLoadOptions property. Indicates whether keeping schema of this json
type: docs
url: /net/aspose.cells/jsonloadoptions/keptschema/
---
## JsonLoadOptions.KeptSchema property

Indicates whether keeping schema of this json.

```csharp
public bool KeptSchema { get; set; }
```

### Remarks

Sometimes we will save the file to JSON after loading JSON file.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class JsonLoadOptionsPropertyKeptSchemaDemo
    {
        public static void Run()
        {
            // Create JSON load options
            JsonLoadOptions options = new JsonLoadOptions();

            // Display the default value of KeptSchema property
            Console.WriteLine("Default KeptSchema value: " + options.KeptSchema);

            // Set KeptSchema to true
            options.KeptSchema = true;
            Console.WriteLine("KeptSchema set to: " + options.KeptSchema);

            // Create a sample JSON file
            string jsonData = @"{
                ""Employees"": [
                    { ""ID"": 1, ""Name"": ""John"", ""Department"": ""Sales"" },
                    { ""ID"": 2, ""Name"": ""Jane"", ""Department"": ""Marketing"" }
                ]
            }";

            System.IO.File.WriteAllText("sample.json", jsonData);

            try
            {
                // Load JSON with KeptSchema enabled
                Workbook workbook = new Workbook("sample.json", options);

                // Display information about the loaded workbook
                Console.WriteLine("Workbook loaded with KeptSchema: " + options.KeptSchema);
                Console.WriteLine("Number of worksheets: " + workbook.Worksheets.Count);

                // Save the workbook
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

### See Also

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


