---
title: "BuiltInDocumentPropertyCollection.CreatedTime"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство BuiltInDocumentPropertyCollection. Получает или задает дату создания документа в локальном часовом поясе"
type: docs
url: /ru/net/aspose.cells.properties/builtindocumentpropertycollection/createdtime/
---
## BuiltInDocumentPropertyCollection.CreatedTime property

Получает или задает дату создания документа в локальном часовом поясе.

```csharp
public DateTime CreatedTime { get; set; }
```

### Примечания

Aspose.Cells не обновляет это свойство при изменении документа.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyCreatedTimeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Установите свойство CreatedTime в текущее время
            DateTime currentTime = DateTime.Now;
            workbook.BuiltInDocumentProperties.CreatedTime = currentTime;
            
            // Сохраните книгу
            string outputPath = "output_CreatedTimeDemo.xlsx";
            workbook.Save(outputPath);
            
            // Загрузить сохранённую книгу, чтобы проверить свойство
            Workbook loadedWorkbook = new Workbook(outputPath);
            DateTime loadedTime = loadedWorkbook.BuiltInDocumentProperties.CreatedTime;
            
            Console.WriteLine("Original CreatedTime: " + currentTime);
            Console.WriteLine("Loaded CreatedTime: " + loadedTime);
        }
    }
}
```

### См. также

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


