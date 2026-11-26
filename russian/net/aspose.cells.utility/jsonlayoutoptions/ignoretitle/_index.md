---
title: "JsonLayoutOptions.IgnoreTitle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство JsonLayoutOptions. Игнорирует заголовки атрибутов"
type: docs
url: /ru/net/aspose.cells.utility/jsonlayoutoptions/ignoretitle/
---
## JsonLayoutOptions.IgnoreTitle property

Игнорирует заголовки атрибутов

```csharp
public bool IgnoreTitle { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsPropertyIgnoreTitleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Пример JSON-данных
            string jsonInput = @"{
                ""Products"": [
                    {
                        ""Name"": ""Product1"",
                        ""Price"": 100,
                        ""Date"": ""2023-01-15""
                    },
                    {
                        ""Name"": ""Product2"",
                        ""Price"": 200,
                        ""Date"": ""2023-02-20""
                    }
                ]
            }";

            // Установите JsonLayoutOptions с IgnoreTitle = true
            JsonLayoutOptions options = new JsonLayoutOptions();
            options.IgnoreTitle = true;  // This will skip the title row in output
            options.ArrayAsTable = true;
            options.DateFormat = "yyyy/MM/dd";

            // Импортировать данные JSON
            JsonUtility.ImportData(jsonInput, worksheet.Cells, 0, 0, options);

            // Сохраните книгу
            workbook.Save("output_ignore_title.xlsx");
        }
    }
}
```

### См. также

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


