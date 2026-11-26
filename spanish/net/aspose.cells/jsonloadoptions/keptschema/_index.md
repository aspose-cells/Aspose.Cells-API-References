---
title: "JsonLoadOptions.KeptSchema"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad JsonLoadOptions. Indica si se mantiene el esquema de este json"
type: docs
url: /es/net/aspose.cells/jsonloadoptions/keptschema/
---
## JsonLoadOptions.KeptSchema property

Indica si se mantiene el esquema de este JSON.

```csharp
public bool KeptSchema { get; set; }
```

### Observaciones

A veces guardaremos el archivo en JSON después de cargar el archivo JSON.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class JsonLoadOptionsPropertyKeptSchemaDemo
    {
        public static void Run()
        {
            // Crear opciones de carga JSON
            JsonLoadOptions options = new JsonLoadOptions();

            // Mostrar el valor predeterminado de la propiedad KeptSchema
            Console.WriteLine("Default KeptSchema value: " + options.KeptSchema);

            // Establecer KeptSchema a true
            options.KeptSchema = true;
            Console.WriteLine("KeptSchema set to: " + options.KeptSchema);

            // Crear un archivo JSON de ejemplo
            string jsonData = @"{
                ""Employees"": [
                    { ""ID"": 1, ""Name"": ""John"", ""Department"": ""Sales"" },
                    { ""ID"": 2, ""Name"": ""Jane"", ""Department"": ""Marketing"" }
                ]
            }";

            System.IO.File.WriteAllText("sample.json", jsonData);

            try
            {
                // Cargar JSON con KeptSchema habilitado
                Workbook workbook = new Workbook("sample.json", options);

                // Mostrar información sobre el libro de trabajo cargado
                Console.WriteLine("Workbook loaded with KeptSchema: " + options.KeptSchema);
                Console.WriteLine("Number of worksheets: " + workbook.Worksheets.Count);

                // Guarda el libro de trabajo
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

### Ver también

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


