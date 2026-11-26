---
title: "JsonLoadOptions.StartCell"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство JsonLoadOptions. Получает и задает начальную ячейку"
type: docs
url: /ru/net/aspose.cells/jsonloadoptions/startcell/
---
## JsonLoadOptions.StartCell property

Получает и задает начальную ячейку.

```csharp
public string StartCell { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonLoadOptionsPropertyStartCellDemo
    {
        public static void Run()
        {
            // Создать параметры загрузки JSON с свойством StartCell
            JsonLoadOptions options = new JsonLoadOptions
            {
                StartCell = "B3" // JSON data will start from cell B3
            };

            // Создать книгу из файла JSON с параметрами
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("Header");
            
            // Создать пример файла JSON
            System.IO.File.WriteAllText("data.json", "{\"Name\":\"John\",\"Age\":30,\"City\":\"New York\"}");
            
            // Загрузить данные JSON в книгу
            workbook = new Workbook("data.json", options);

            // Сохраните книгу
            workbook.Save("JsonStartCellDemo.xlsx");
        }
    }
}
```

### См. также

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


