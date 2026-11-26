---
title: "JsonLoadOptions.MultipleWorksheets"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство JsonLoadOptions. Указывает, импортировать ли каждый атрибут объекта JsonObject как отдельный лист, когда все дочерние узлы являются массивами"
type: docs
url: /ru/net/aspose.cells/jsonloadoptions/multipleworksheets/
---
## JsonLoadOptions.MultipleWorksheets property

Указывает, импортировать ли каждый атрибут объекта JsonObject как отдельный лист, когда все дочерние узлы являются массивами.

```csharp
public bool MultipleWorksheets { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonLoadOptionsPropertyMultipleWorksheetsDemo
    {
        public static void Run()
        {
            // Создать параметры загрузки JSON с включённым MultipleWorksheets
            JsonLoadOptions options = new JsonLoadOptions { MultipleWorksheets = true };
            
            // Загрузить файл JSON в книгу с указанными параметрами
            Workbook workbook = new Workbook("example.json", options);
            
            // Получить доступ к данным первого листа
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Отобразить некоторые примерные значения из загруженного JSON
            Console.WriteLine("D5 cell value: " + cells["D5"].StringValue);
            Console.WriteLine("E5 cell value: " + cells["E5"].StringValue);
            Console.WriteLine("D7 cell value: " + cells["D7"].StringValue);
            Console.WriteLine("B14 cell value: " + cells["B14"].StringValue);
        }
    }
}
```

### См. также

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


