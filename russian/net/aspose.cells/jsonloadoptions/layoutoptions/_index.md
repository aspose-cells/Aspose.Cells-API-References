---
title: "JsonLoadOptions.LayoutOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство JsonLoadOptions. Параметры импорта JSON"
type: docs
url: /ru/net/aspose.cells/jsonloadoptions/layoutoptions/
---
## JsonLoadOptions.LayoutOptions property

Параметры импорта JSON.

```csharp
public JsonLayoutOptions LayoutOptions { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLoadOptionsPropertyLayoutOptionsDemo
    {
        public static void Run()
        {
            // Создать параметры загрузки JSON с LayoutOptions
            JsonLoadOptions options = new JsonLoadOptions
            {
                LayoutOptions = new JsonLayoutOptions
                {
                    ArrayAsTable = true,
                    IgnoreNull = false,
                    ConvertNumericOrDate = true,
                    NumberFormat = "0.00",
                    DateFormat = "yyyy-MM-dd"
                }
            };

            // Создать новую книгу с данными JSON
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Пример JSON-данных
            string json = @"{
                ""Products"": [
                    { ""ID"": 1, ""Name"": ""Product A"", ""Price"": 19.99, ""Date"": ""2023-05-15"" },
                    { ""ID"": 2, ""Name"": ""Product B"", ""Price"": 29.99, ""Date"": ""2023-06-20"" }
                ]
            }";

            // Импортировать JSON в лист
            JsonUtility.ImportData(json, worksheet.Cells, 0, 0, options.LayoutOptions);

            // Сохраните книгу
            workbook.Save("JsonWithLayoutOptions.xlsx");
        }
    }
}
```

### См. также

* class [JsonLayoutOptions](../../../aspose.cells.utility/jsonlayoutoptions/)
* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


