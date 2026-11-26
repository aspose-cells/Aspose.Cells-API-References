---
title: "JsonLayoutOptions.ArrayAsTable"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство JsonLayoutOptions. Обрабатывает массив как таблицу"
type: docs
url: /ru/net/aspose.cells.utility/jsonlayoutoptions/arrayastable/
---
## JsonLayoutOptions.ArrayAsTable property

Обрабатывает массив как таблицу.

```csharp
public bool ArrayAsTable { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsPropertyArrayAsTableDemo
    {
        public static void Run()
        {
            // Создайте книгу и откройте первый лист
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Создайте параметры макета JSON и установите ArrayAsTable в true
            JsonLayoutOptions options = new JsonLayoutOptions();
            options.ArrayAsTable = true;
            options.IgnoreTitle = true;

            // Пример данных JSON (упрощённый для демонстрации)
            string jsonData = @"{
                ""products"": [
                    {""id"":1, ""name"":""Laptop"", ""price"":999.99},
                    {""id"":2, ""name"":""Phone"", ""price"":599.99}
                ]
            }";

            // Импортировать JSON-данные в лист
            JsonUtility.ImportData(jsonData, sheet.Cells, 0, 0, options);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


