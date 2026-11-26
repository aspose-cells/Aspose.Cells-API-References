---
title: "JsonLoadOptions.KeptSchema"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство JsonLoadOptions. Указывает, сохраняется ли схема этого JSON"
type: docs
url: /ru/net/aspose.cells/jsonloadoptions/keptschema/
---
## JsonLoadOptions.KeptSchema property

Указывает, сохранять ли схему этого JSON.

```csharp
public bool KeptSchema { get; set; }
```

### Примечания

Иногда мы сохраняем файл в JSON после загрузки файла JSON.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class JsonLoadOptionsPropertyKeptSchemaDemo
    {
        public static void Run()
        {
            // Создать параметры загрузки JSON
            JsonLoadOptions options = new JsonLoadOptions();

            // Отобразить значение по умолчанию свойства KeptSchema
            Console.WriteLine("Default KeptSchema value: " + options.KeptSchema);

            // Установить KeptSchema в true
            options.KeptSchema = true;
            Console.WriteLine("KeptSchema set to: " + options.KeptSchema);

            // Создать пример файла JSON
            string jsonData = @"{
                ""Employees"": [
                    { ""ID"": 1, ""Name"": ""John"", ""Department"": ""Sales"" },
                    { ""ID"": 2, ""Name"": ""Jane"", ""Department"": ""Marketing"" }
                ]
            }";

            System.IO.File.WriteAllText("sample.json", jsonData);

            try
            {
                // Загрузить JSON с включённым KeptSchema
                Workbook workbook = new Workbook("sample.json", options);

                // Отобразить информацию о загруженной книге
                Console.WriteLine("Workbook loaded with KeptSchema: " + options.KeptSchema);
                Console.WriteLine("Number of worksheets: " + workbook.Worksheets.Count);

                // Сохраните книгу
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

### См. также

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


