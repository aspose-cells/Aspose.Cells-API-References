---
title: "JsonLayoutOptions.JsonLayoutOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор JsonLayoutOptions. Конструктор загрузки параметров макета JSON"
type: docs
url: /ru/net/aspose.cells.utility/jsonlayoutoptions/jsonlayoutoptions/
---
## JsonLayoutOptions constructor

Конструктор загрузки параметров макета JSON.

```csharp
public JsonLayoutOptions()
```

### Примеры

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
            // Создать пример данных JSON
            string json = @"{
                ""Name"": ""John"",
                ""Age"": 30,
                ""Address"": {
                    ""Street"": ""123 Main St"",
                    ""City"": ""New York""
                }
            }";

            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Инициализировать JsonLayoutOptions с помощью конструктора
            JsonLayoutOptions options = new JsonLayoutOptions();
            
            // Установите параметры.
            options.ArrayAsTable = true;
            options.IgnoreArrayTitle = false;
            options.IgnoreObjectTitle = false;

            // Импортировать JSON-данные в лист
            JsonUtility.ImportData(json, workbook.Worksheets[0].Cells, 0, 0, options);

            // Сохраните книгу
            workbook.Save("JsonImportDemo.xlsx");
        }
    }
}
```

### См. также

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


