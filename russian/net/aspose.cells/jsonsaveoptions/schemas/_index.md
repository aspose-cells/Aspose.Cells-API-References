---
title: "JsonSaveOptions.Schemas"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство JsonSaveOptions. Исходная json-схема каждого листа"
type: docs
url: /ru/net/aspose.cells/jsonsaveoptions/schemas/
---
## JsonSaveOptions.Schemas property

Исходная схема JSON каждой таблицы.

```csharp
public string[] Schemas { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertySchemasDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Пример JSON-данных для импорта
            string jsonData = @"{
                ""Products"": [
                    {
                        ""ID"": 101,
                        ""Name"": ""Product A"",
                        ""Price"": 99.99
                    }
                ]
            }";

            // Импортировать JSON-данные в лист
            JsonUtility.ImportData(jsonData, workbook.Worksheets[0].Cells, 0, 0, new JsonLayoutOptions());

            // Пример схемы для проверки
            string schema = @"{
                ""$schema"": ""http://json-schema.org/draft-07/schema#"",
                ""type"": ""object"",
                ""properties"": {
                    ""Products"": {
                        ""type"": ""array"",
                        ""items"": {
                            ""type"": ""object"",
                            ""properties"": {
                                ""ID"": { ""type"": ""integer"" },
                                ""Name"": { ""type"": ""string"" },
                                ""Price"": { ""type"": ""number"" }
                            },
                            ""required"": [""ID"", ""Name"", ""Price""]
                        }
                    }
                },
                ""required"": [""Products""]
            }";

            // Настройте параметры сохранения JSON со схемой
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.Schemas = new string[] { schema };
            saveOptions.ExportNestedStructure = true;
            saveOptions.SkipEmptyRows = true;

            // Сохраните книгу с параметрами JSON
            string outputPath = "output_with_schema.json";
            workbook.Save(outputPath, saveOptions);

            Console.WriteLine("Workbook saved with JSON schema validation.");
        }
    }
}
```

### См. также

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


