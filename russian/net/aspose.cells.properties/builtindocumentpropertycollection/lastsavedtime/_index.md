---
title: "BuiltInDocumentPropertyCollection.LastSavedTime"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство BuiltInDocumentPropertyCollection. Получает или задает время последнего сохранения в локальном часовом поясе"
type: docs
url: /ru/net/aspose.cells.properties/builtindocumentpropertycollection/lastsavedtime/
---
## BuiltInDocumentPropertyCollection.LastSavedTime property

Получает или задает время последнего сохранения в локальном часовом поясе.

```csharp
public DateTime LastSavedTime { get; set; }
```

### Примечания

Aspose.Cells не обновляет это свойство при изменении документа.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLastSavedTimeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Установить встроенные свойства документа
            workbook.BuiltInDocumentProperties.CreatedTime = new DateTime(2023, 1, 1);
            workbook.BuiltInDocumentProperties.LastPrinted = DateTime.Now;
            workbook.BuiltInDocumentProperties.LastSavedTime = DateTime.Now;

            // Отобразить свойство LastSavedTime
            Console.WriteLine("Last Saved Time: " + 
                workbook.BuiltInDocumentProperties.LastSavedTime);

            // Сохраните книгу
            workbook.Save("DocumentPropertiesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


